Approximation framework for estimating line positions, Franck--Condon factors, saturation intensities, and loss rates for ultracold homonuclear alkali-like photo-association.

**Target use case:** one PA laser, one excited molecular symmetry/state at a time, near an atomic D-line asymptote. The code should take the long-range coefficient of the selected excited curve, a user-chosen ground-state scattering length, and experimental conditions, then output expected PA line positions and approximate rates.

**Working philosophy:** this is not a replacement for a coupled-channel or quantum-chemistry calculation. It is a controlled, code-friendly approximation pipeline whose value is that every uncertain physical ingredient is explicit and tunable.

---

## 0. Minimal pipeline summary

For a single chosen excited potential, the calculation chain is:

1. **Choose excited potential**
   $$
   V_e(R) \simeq D - \frac{C_n'}{R^n}.
   $$
   For homonuclear alkali-like PA near an S+P asymptote, the relevant near-asymptotic tail is usually resonant dipole--dipole, so $n=3$.

2. **Use LeRoy--Bernstein (LB) to generate near-threshold bound states**
   $$
   E_b(v) \equiv D-E_v,
   \qquad
   R_v = \left(\frac{C_n'}{E_b(v)}\right)^{1/n}.
   $$

3. **Generate the ground-state threshold scattering wavefunction**
   $$
   V_g(R) \simeq -\frac{C_6}{R^6},
   \qquad
   \chi_E(R) = \chi_E(R;C_6,\mu,T,a).
   $$
   The free parameter is the scattering length $a$. For Ag, this should be treated as a scan/tuning parameter.

4. **Use reflection approximation for the free-bound Franck--Condon factor**
   $$
   F_{v;E} \equiv |S(E,v)|^2 \approx \text{prefactor}(\mu,C_n',R_v)\,|\chi_E(R_v)|^2.
   $$

5. **Apply angular factor**
   $$
   A = \sum_{\rm final}\overline{|a_\nu|^2}_{\rm initial}.
   $$
   This is a separate multiplicative line-strength factor, typically $\sim 10^{-2}$ to $10^{-1}$.

6. **Compute stimulated width, PA saturation intensity, and rate**
   $$
   \Gamma_b \propto I\,A\,F_{v;E},
   \qquad
   I_{\rm sat}^{\rm PA} \propto \frac{1}{A F_{v;E}},
   \qquad
   R_{\rm PA} \propto n I A F_{v;E}.
   $$

7. **Convert rate to observable trap loss**
   In an ODT, compare laser-on and laser-off holds. The useful object is the additional PA loss rate above the one-body background lifetime.

---

## 1. Notation and unit conventions

| Symbol | Meaning | Typical code unit |
|---|---|---|
| $R$ | internuclear separation | $a_0$ |
| $D$ | selected atomic dissociation limit | often set to 0 |
| $E_v$ | excited bound-state energy | Hartree or cm$^{-1}$ |
| $E_b=D-E_v$ | binding energy / red detuning from asymptote | Hartree, cm$^{-1}$, Hz |
| $\mu$ | reduced mass in the radial Hamiltonian | electron masses in a.u. |
| $C_6$ | ground-state vdW coefficient | a.u. |
| $C_n'$ | excited-state long-range coefficient | a.u.; for S+P often $C_3'$ |
| $a$ | s-wave scattering length | $a_0$; user-tunable |
| $T$ | collision temperature | K or $\mu$K |
| $k$ | relative wave number | $a_0^{-1}$ |
| $\Gamma$ | natural decay rate | s$^{-1}$, use $\Gamma=2\pi\times$linewidth in Hz |
| $I$ | PA intensity | W/cm$^2$ or W/m$^2$ |
| $I_{\rm sat}$ | atomic saturation intensity | W/cm$^2$ |
| $I_{\rm sat}^{\rm PA}$ | PA saturation intensity | W/cm$^2$ |
| $A$ | angular line-strength factor | dimensionless |
| $F_{v;E}=|S|^2$ | energy-normalized free-bound FCF | J$^{-1}$ or Hartree$^{-1}$ |
| $\beta_{\rm PA}=K(T)$ | two-body PA rate coefficient | cm$^3$/s |
| $R_{\rm PA}=n\beta_{\rm PA}$ | local per-atom PA loss rate | s$^{-1}$ |

Use one unit system internally. The cleanest for the wavefunction and reflection calculation is **atomic units** with $\hbar=1$, then convert $F_{v;E}$ from Hartree$^{-1}$ to J$^{-1}$ before SI rate formulas.

Useful constants:

$$
1\ E_h = 219474.63137\ \mathrm{cm^{-1}},
\qquad
1\ \mathrm{\AA}=1.8897261246\ a_0.
$$

---

## 2. Pure long-range excited potentials

For homonuclear alkali-like systems near the D2 asymptote, the analytic pure-long-range model uses the dimensionless variables

$$
X=\frac{C}{9R^3\Delta},
\qquad
Y=\frac{E-E_{1/2}^0}{\Delta}
=\frac{E-E_{3/2}^0}{\Delta}+1,
$$

where $\Delta=E_{3/2}^0-E_{1/2}^0$ is the atomic fine-structure splitting and

$$
C=e^2 |\langle n0|r|nl\rangle|^2.
$$

The radial dipole matrix element can be inferred from D-line data by

$$
\langle r\rangle
=3\sqrt{\frac{\pi\epsilon_0\hbar c^3}{e^2\omega_{D2}^3}\Gamma_{D2}}
=3\sqrt{\frac{\pi\epsilon_0\hbar c^3}{e^2\omega_{D1}^3}\Gamma_{D1}}.
$$

Taking the D2 asymptote as zero energy, the dimensional potential is

$$
V(R)=E-E_{3/2}^0=\Delta(Y-1).
$$

The analytic branches used in the notes are

$$
Y_{0_g^-}
=\frac12\left[(1-3X)+\sqrt{1-6X+81X^2}\right],
$$

and

$$
Y_{1_u}
=\frac13(2+6X)
+\omega\left(\frac12q+\sqrt{s}\right)^{1/3}
+\omega^2\left(\frac12q-\sqrt{s}\right)^{1/3},
$$

with

$$
\omega=\frac{-1-i\sqrt3}{2},
\qquad
q=-\frac{2}{27}-20X^3,
$$

$$
s=-\frac{7}{27}X^2+\frac{20}{27}X^3-\frac{49}{3}X^4-243X^6.
$$

Near dissociation, both approach

$$
V_e(R)\to -\frac{C_3'}{R^3}.
$$

For the two D2 pure-long-range branches:

$$
C_3'(0_g^-)=\frac13 C,
\qquad
C_3'(1_u)=\frac{\sqrt7-2}{9}C.
$$

**Pipeline choice:** for the first rate-estimation code, use only the asymptotic form $D-C_3'/R^3$. The full analytic PLR curve is useful for checking the expected well depth and where the pure-long-range approximation breaks down, but the LB + reflection pipeline only needs the near-asymptotic $C_3'$.

---

## 3. LeRoy--Bernstein near-dissociation formula

For an excited long-range potential

$$
V_e(R)=D-\frac{C_n'}{R^n},
$$

the LB formula gives

$$
v_D-v
=\frac{2n}{n-2}\sqrt{\frac{\mu}{2\pi\hbar^2}}
\frac{\Gamma(1/2+1/n)}{\Gamma(1+1/n)}
\frac{(C_n')^{1/n}}{n}
\left[D-E(v)\right]^{\frac{n-2}{2n}}.
$$

Equivalently,

$$
D-E(v)=\left[(v_D-v)H_n\right]^{\frac{2n}{n-2}},
$$

where

$$
H_n=\frac{n-2}{2n}
\sqrt{\frac{2\pi\hbar^2}{\mu}}
\frac{\Gamma(1+1/n)}{\Gamma(1/2+1/n)}
\frac{n}{(C_n')^{1/n}}.
$$

The outer classical turning point is

$$
R_v=\left(\frac{C_n'}{D-E(v)}\right)^{1/n}
=\frac{(C_n')^{1/n}}{\left[(v_D-v)H_n\right]^{2/(n-2)}}.
$$

### Special case: resonant dipole tail, $n=3$

For $n=3$,

$$
H_3=\frac12\sqrt{\frac{2\pi\hbar^2}{\mu}}
\frac{\Gamma(4/3)}{\Gamma(5/6)}
\frac{1}{(C_3')^{1/3}},
$$

$$
E_b(v)=D-E(v)=\left[(v_D-v)H_3\right]^6,
$$

$$
R_v=\left(\frac{C_3'}{E_b(v)}\right)^{1/3}.
$$

### Near-threshold indexing

For a top-down index, use

$$
v_{\rm top}=-1,-2,-3,\ldots
$$

with the least-bound state at $-1$. Then $v_D-v_{\rm top}$ is the effective quantum-number distance from the dissociation limit. The unknown $v_D$ is a phase/integration constant. For predictions without spectroscopy, choose a convention such as $-1<v_D<0$, scan it, or tune it during Cs benchmarking.

**Code output from this block:** a table with at least

$$
\{v_{\rm top}, E_b, \delta_{\rm Hz}, \delta_{\rm GHz}, \delta_{\rm cm^{-1}}, R_v\}.
$$

---

## 4. Ground-state Wigner-threshold vdW scattering wavefunction

Assume the entrance-channel ground potential is dominated by

$$
V_g(R)=-\frac{C_6}{R^6}.
$$

Define

$$
\beta_6=\left(\frac{2\mu C_6}{\hbar^2}\right)^{1/4},
\qquad
\mathcal E_6=\frac{\hbar^2}{2\mu\beta_6^2},
\qquad
x=\frac{R}{\beta_6}.
$$

At threshold, with $E=\hbar^2k^2/(2\mu)\ll\mathcal E_6$, the energy-normalized s-wave solution is

$$
\boxed{
\chi_E(R)
=\frac{1}{\sqrt{2\pi}}
\frac{1}{\sqrt{\mathcal E_6\beta_6}}
\sqrt{k\beta_6}\sqrt{x}
\left[
\Gamma\!\left(\frac34\right)J_{-1/4}\!\left(\frac{1}{2x^2}\right)
-\frac{2a}{\beta_6}\Gamma\!\left(\frac54\right)J_{1/4}\!\left(\frac{1}{2x^2}\right)
\right].
}
$$

The scattering length $a$ is the only short-range parameter in this approximation. This is the knob to tune in Ag.

In atomic units, a convenient implementation used in the existing code is equivalent to

$$
\chi_E(R) = \beta_6\sqrt{\frac{\mu k}{\pi}}\;\chi_{\rm shape}(R),
$$

with

$$
\chi_{\rm shape}(R)
=\sqrt{x}
\left[
\Gamma\!\left(\frac34\right)J_{-1/4}\!\left(\frac{1}{2x^2}\right)
-\frac{2a}{\beta_6}\Gamma\!\left(\frac54\right)J_{1/4}\!\left(\frac{1}{2x^2}\right)
\right].
$$

The large-$R$, small-$kR$ matching is

$$
\chi_E(R)\to \sqrt{\frac{2\mu k}{\pi\hbar^2}}(R-a),
$$

which is the energy-normalized threshold asymptote.

### Energy scaling

At fixed Condon point/turning point $R_v$, the Bessel part is independent of collision energy. The prefactor gives

$$
|\chi_E(R_v)|^2\propto k\propto\sqrt{E}\propto\sqrt{T}.
$$

This scaling is important when comparing Cs MOT temperatures to colder Ag ODT temperatures.

---

## 5. Reflection approximation for the free-bound FCF

The exact free-bound Franck--Condon overlap is

$$
S(E,v)=\langle\psi_v|\chi_E\rangle
=\int_0^\infty \psi_v(R)\chi_E(R)\,dR,
\qquad
F_{v;E}=|S(E,v)|^2.
$$

Because $\chi_E$ is energy-normalized and $\psi_v$ is unit-normalized, $F_{v;E}$ has units of inverse energy.

The reflection approximation collapses the integral to the Condon/outer-turning point:

$$
F_{v;E}\approx \frac{dE_v/dv}{D_C}\,|\chi_E(R_C)|^2,
$$

where

$$
R_C\approx R_v,
\qquad
D_C=\left|\frac{d}{dR}[V_e(R)-V_g(R)]\right|_{R_C}.
$$

For $V_e(R)=D-C_n'/R^n$, neglecting the much weaker ground-state slope at the Condon point,

$$
D_C\approx \left|\frac{dV_e}{dR}\right|_{R_v}
=\frac{nC_n'}{R_v^{n+1}}.
$$

### Homonuclear resonant-dipole case, $n=3$

For $V_e=D-C_3'/R^3$, the Wang--Stwalley reflection result is

$$
\boxed{
F_{v;E}
=(2\pi\hbar^2)^{1/2}
\frac{\Gamma(4/3)}{\Gamma(5/6)}
\mu^{-1/2}
\left(\frac{C_3'}{R_v^3}\right)^{-1/2}
|\chi_E(R_v)|^2.
}
$$

Since $C_3'/R_v^3=E_b(v)$, this can be coded as

$$
F_{v;E}
=(2\pi\hbar^2)^{1/2}
\frac{\Gamma(4/3)}{\Gamma(5/6)}
\mu^{-1/2}
E_b(v)^{-1/2}
|\chi_E(R_v)|^2.
$$

In atomic units $(\hbar=1)$:

$$
F_{v;E}^{\rm (a.u.)}
=\sqrt{2\pi}\frac{\Gamma(4/3)}{\Gamma(5/6)}
\mu^{-1/2}
E_b^{-1/2}
|\chi_E(R_v)|^2.
$$

Convert to SI by

$$
F_{v;E}^{\rm (J^{-1})}=\frac{F_{v;E}^{\rm (Hartree^{-1})}}{E_h\ [{\rm J}]}.
$$

---

## 6. Angular factor

The laser coupling can be factored as

$$
V_{b,\nu}
=\frac{\mathcal E_0 d_{\rm at}}{2}
\langle\psi_v|\chi_E\rangle\,a_\nu,
$$

where $a_\nu$ contains all polarization, rotational, electronic, hyperfine, and exchange-symmetry algebra. The unresolved line-strength angular factor is

$$
A=\sum_{\rm final}\overline{|a_\nu|^2}_{\rm initial}.
$$

For $^{107}\mathrm{Ag}+{}^{107}\mathrm{Ag}$, D2, $f_1=f_2=1$, s-wave entrance:

$$
A(0_g^-)=\frac{7}{162}\approx0.04321,
$$

and under the convention in the angular-factor note,

$$
A(1_u)=\frac{7}{162}\approx0.04321.
$$

For a Zeeman-polarized $0_g^-$ calculation:

$$
A_{m_f=\pm1}=\frac19,
\qquad
A_{m_f=0}=\frac1{18}.
$$

**Do not hide this factor inside the FCF.** Keep $F_{v;E}$ as a radial/nuclear quantity and $A$ as a separate angular line strength. This makes it easy to compare unpolarized, spin-polarized, $0_g^-$, and $1_u$ cases.

---

## 7. Coupling, stimulated width, and saturation intensity

The laser field amplitude obeys

$$
I=\frac12\epsilon_0c\mathcal E_0^2,
\qquad
\mathcal E_0=\sqrt{\frac{2I}{\epsilon_0c}}.
$$

The atomic Rabi frequency is

$$
\Omega_{\rm at}=\frac{d_{\rm at}\mathcal E_0}{\hbar}.
$$

Using the standard D-line saturation intensity

$$
I_{\rm sat}=\frac{\pi hc\Gamma}{3\lambda^3},
$$

one has

$$
\frac{\Omega_{\rm at}^2}{2}=\frac{\Gamma^2}{4}\frac{I}{I_{\rm sat}}.
$$

If Drag/Pillet notation uses $K=\Omega_{\rm at}/2$, then

$$
\boxed{K^2=\frac{\Gamma^2}{8}\frac{I}{I_{\rm sat}}.}
$$

The single-channel Fermi-golden-rule width is

$$
\Gamma_b(E)=\frac{2\pi}{\hbar}|V_b(E)|^2.
$$

After averaging/summing unresolved angular channels,

$$
\boxed{
\Gamma_b(E)
=\frac{\pi\hbar\Gamma^2}{4}\frac{I}{I_{\rm sat}}
F_{v;E}\,A.
}
$$

Define the PA saturation intensity by $\Gamma_b=\Gamma_{\rm nat}\simeq\Gamma$. Then

$$
\boxed{
I_{\rm sat}^{\rm PA}
=\frac{4}{\pi\hbar\Gamma F_{v;E}A}\,I_{\rm sat}.
}
$$

If $A$ is not included in this formula, the result is the radial-only saturation intensity and must be divided by $A$ to get the physical unresolved-line saturation scale.

---

## 8. Weak-field PA rate formula

In the perturbative, unsaturated limit $\Gamma_b\ll\Gamma$, the Drag/Pillet-style local per-atom PA loss rate can be coded as

$$
\boxed{
R_{\rm PA}
=A\left(\frac{3}{2\pi}\right)^{3/2}
\frac{h}{2}
\;n\lambda_{\rm th}^3
\;e^{-E_r/k_BT}
\;K^2
\;F_{v;E}.
}
$$

Use the convention

$$
\lambda_{\rm th}=\frac{h}{\sqrt{3\mu k_BT}},
\qquad
K^2=\frac{\Gamma^2}{8}\frac{I}{I_{\rm sat}}.
$$

Here $n$ is the local density or effective density, and $E_r/k_BT$ is often set to 1 for the benchmark convention used in the Cs paper-style estimate.

This rate has the scaling

$$
R_{\rm PA}\propto n I A F_{v;E}\lambda_{\rm th}^3.
$$

Since the threshold FCF itself scales as $F_{v;E}\propto |\chi_E(R_v)|^2\propto \sqrt{T}$, the total weak-field temperature scaling at fixed $R_v$ is approximately

$$
R_{\rm PA}\propto T^{-3/2}\times T^{1/2}=T^{-1},
$$

assuming the same selected collision-energy convention and no thermal averaging over a broad resonance.

The associated two-body coefficient is

$$
\beta_{\rm PA}=K(T),
\qquad
R_{\rm PA}=n_{\rm eff}\beta_{\rm PA},
$$

up to the common factor-of-two convention for whether one PA event is counted as one event or two atoms lost.

---

## 9. Saturated/on-resonance rate formula

The perturbative formula is only valid for $s\ll1$, where

$$
s\equiv\frac{I}{I_{\rm sat}^{\rm PA}}
=\frac{\Gamma_b}{\Gamma}.
$$

For a single s-wave resonance, on resonance, trap-loss detection, and no other decay channels,

$$
\boxed{
K_{\rm on-res}(E)
=\frac{4\pi v_{\rm rel}}{k^2}\frac{s}{(1+s)^2}.
}
$$

Limiting cases:

$$
s\ll1:\ K\propto I,
\qquad
s=1:\ K_{\rm max}=\frac{\pi v_{\rm rel}}{k^2},
\qquad
s\gg1:\ K\propto I^{-1}.
$$

This is the saturation correction that can suppress the rate by a factor $\sim1/4$ relative to naively extrapolating the weak-field formula to $s=1$.

For the first pipeline code, compute both:

1. the weak-field Drag/Pillet rate; and
2. a saturation-corrected rate using $s/(1+s)^2$, normalized so it agrees with the weak-field result at $s\ll1$.

---

## 10. ODT observable: laser-on versus laser-off hold

In a continuously loaded MOT, the usual rate equation is

$$
\frac{dN}{dt}=L-\gamma N-(\beta+\beta_{\rm PA})\int n^2(\mathbf r)\,d^3r.
$$

In a loaded-once ODT, set $L=0$. The clean experimental comparison is:

- hold for time $t_h$ with PA laser off;
- hold for the same $t_h$ with PA laser on;
- compare atom number, temperature, and possibly density-normalized loss.

Define the effective density

$$
n_{\rm eff}=\frac{\int n^2(\mathbf r)\,d^3r}{\int n(\mathbf r)\,d^3r}.
$$

Then the per-atom PA loss rate is approximately

$$
R_{\rm PA}=\beta_{\rm PA}n_{\rm eff}.
$$

If the density does not change too much during the hold, a simple signal estimate is

$$
\frac{N_{\rm on}(t_h)}{N_{\rm off}(t_h)}
\approx \exp[-R_{\rm PA}t_h],
$$

so the fractional PA signal is

$$
\mathcal S
=1-\frac{N_{\rm on}}{N_{\rm off}}
\approx 1-e^{-R_{\rm PA}t_h}
\approx R_{\rm PA}t_h
\quad (R_{\rm PA}t_h\ll1).
$$

For stronger two-body loss or large density evolution, solve

$$
\frac{dN}{dt}=-\gamma N-\beta_{\rm PA}\frac{N^2}{V_{\rm eff}},
$$

where $V_{\rm eff}=N^2/\int n^2d^3r$. With constant $V_{\rm eff}$, the solution is

$$
N(t)=\frac{N_0e^{-\gamma t}}{1+\frac{\beta_{\rm PA}N_0}{\gamma V_{\rm eff}}(1-e^{-\gamma t})}.
$$

This is the better ODT observable model if PA loss is not a small perturbation.

---

## 11. Cs benchmark checklist

Before applying the pipeline to Ag, reproduce the Cs benchmark at the order-of-magnitude level.

Use a Cs $0_g^-(6s+6p_{3/2})$ line close to the Drag/Pillet example and check:

- $A=125/3888\approx0.03215$ for the relevant Cs unresolved angular factor.
- Correct linewidth convention: $\Gamma=2\pi\times5.22\ \mathrm{MHz}$, not $5.22\times10^6\ \mathrm{s^{-1}}$.
- Correct coupling convention:
  $$
  K^2=\frac{\Gamma^2}{8}\frac{I}{I_0}.
  $$
- Atomic saturation intensity:
  $$
  I_0=\frac{\pi hc\Gamma}{3\lambda_{\rm PA}^3}.
  $$
- Reflection FCF in Hartree$^{-1}$, converted to J$^{-1}$.
- Weak-field rate at the selected line.
- Saturation intensity scale; the Cs note gives a benchmark inferred value
  $$
  F_{v;E}\approx1.28\times10^{24}\ \mathrm{J^{-1}},
  \qquad
  I_{\rm sat}^{\rm PA}\approx29.8\ \mathrm{W/cm^2}
  $$
  for the specific benchmark convention.

The goal is not exact agreement. The useful validation is whether the pipeline lands within the same scale after a plausible scattering-length tuning and the same linewidth/angular conventions.

---

## 12. Ag implementation inputs

For $^{107}\mathrm{Ag}$, D2 photoassociation into $0_g^-$ or $1_u$, a minimal input block should contain:

```python
species = "Ag107"
state = "0g-"              # or "1u"
n_long_range = 3
mass_amu = ...              # isotope mass
mu_au = ...                 # reduced mass in electron masses
lambda_D2_nm = 328.163
Gamma_over_2pi_MHz = 23.4
Delta_fs_cm = 920.61
C_radial_a0_squared = 7.69  # C = e^2 <r>^2 in atomic units/convention used by notes
C3_prime_au = C_radial_a0_squared / 3              # 0g-
# C3_prime_au = ((sqrt(7)-2)/9) * C_radial_a0_squared  # 1u
C6_ground_au = ...          # best available Ag-Ag ground C6
a_scattering_a0 = user_tuned
T_uK = 25.0
n_density_cm3 = 1e12
I_PA_Wcm2 = ...
A_angular = 7/162
vD = user_or_scan
v_top_min, v_top_max = -1, -N
accessible_detuning_GHz = 150.0
```

The code should expose $a$ and $v_D$ as top-level knobs. The scattering length changes the wavefunction amplitude and node positions; $v_D$ shifts the LB ladder relative to the dissociation limit.

---

## 13. Recommended code architecture

For the next step, use **one standalone pipeline script first**, but write it internally as modular functions. This is the best compromise: it is easy to run, easy to give to an AI/code reviewer, and avoids the overhead of a premature package.

Recommended single-file structure:

```text
pa_single_state_pipeline.py

1. imports and constants
2. dataclasses / dictionaries for SpeciesInput, PotentialInput, ExperimentInput
3. unit conversions
4. pure-long-range C3 helpers
5. LeRoy--Bernstein ladder generator
6. vdW threshold scattering wavefunction
7. reflection FCF calculator
8. saturation/rate calculators
9. ODT signal estimator
10. plotting/export helpers
11. main():
    - load inputs at top
    - generate LB table
    - compute chi(Rv), FCF, Isat_PA, R_PA
    - filter by accessible detuning
    - write CSV + plots + markdown summary
```

Later, once the Cs benchmark and Ag scan stabilize, split into a small package:

```text
pa_rate/
  constants.py
  units.py
  potentials.py
  leroy_bernstein.py
  scattering_vdw.py
  reflection.py
  rates.py
  odt_loss.py
scripts/
  run_cs_benchmark.py
  run_ag_0gm_scan.py
  run_ag_1u_scan.py
```

**Do not start with many files.** The physics is already complicated; the first deliverable should be one readable, inspectable script whose numerical assumptions are all visible at the top.

---

## 14. Known limitations and warning labels

1. **Pure-long-range potential limitation**
   The Ag $0_g^-$ and $1_u$ wells are predicted to be compact compared with textbook pure-long-range alkalis. Short-range exchange, correlation, and multichannel effects can shift well depths and level positions. Trust the $-C_3/R^3$ tail closest to dissociation more than the inner well.

2. **LB validity**
   LB is an asymptotic near-dissociation formula. It should not be trusted deep in the well. For Ag, focus first on levels accessible within the red-detuning window and with large enough $R_v$.

3. **Reflection approximation**
   It replaces a real overlap integral by a local value $|\chi_E(R_v)|^2$. It is useful for trends and scale estimates but can miss line-by-line structure, especially when the excited wavefunction is not well described by a simple outer-turning-point Airy peak.

4. **Scattering length uncertainty**
   For Ag, $a$ is unknown and physically important. Treat it as a scan parameter. Do not report one rate without showing sensitivity to $a/\beta_6$.

5. **Threshold wavefunction limitation**
   The Bessel form assumes a pure $-C_6/R^6$ ground potential, s-wave collisions, and $E\ll\mathcal E_6$. It may break down for large $|a|$, near resonant scattering, higher partial waves, or Condon points too far into the short-range region.

6. **Angular factor separability**
   The angular factor is assumed independent of $R$ and separated from the radial FCF. This is the right first approximation but can be modified by channel mixing.

7. **Rate formula regime**
   The Drag/Pillet expression is a weak-field perturbative result. Near saturation, use the $s/(1+s)^2$ correction or a full optical-Breit--Wigner treatment.

8. **Experimental signal model**
   ODT loss depends on density distribution, heating, finite PA beam overlap, background lifetime, and possible secondary collisions. Use $n_{\rm eff}$, not just peak density, when comparing to atom-number data.

---

## 15. Final “one-line” computational recipe

For each candidate vibrational level $v$:

$$
E_b(v)=[(v_D-v)H_3]^6,
\qquad
R_v=\left(\frac{C_3'}{E_b}\right)^{1/3},
$$

$$
\chi_E(R_v)=\chi_E(R_v;\mu,C_6,T,a),
$$

$$
F_{v;E}=\sqrt{2\pi}\frac{\Gamma(4/3)}{\Gamma(5/6)}
\mu^{-1/2}E_b^{-1/2}|\chi_E(R_v)|^2
\quad\text{(a.u.)},
$$

$$
I_{\rm sat}^{\rm PA}=\frac{4I_{\rm sat}}{\pi\hbar\Gamma A F_{v;E}},
$$

$$
R_{\rm PA}=A\left(\frac{3}{2\pi}\right)^{3/2}\frac{h}{2}
\,n_{\rm eff}\lambda_{\rm th}^3e^{-E_r/k_BT}
\left(\frac{\Gamma^2}{8}\frac{I}{I_{\rm sat}}\right)F_{v;E}.
$$

Then filter by the experimental accessible detuning window, e.g.

$$
0<E_b/h<150\ \mathrm{GHz}
$$

for the current Ag laser window.
