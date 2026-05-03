# Angular factors for homonuclear $^{107}$Ag photoassociation to D2 $0_g^-$ and $1_u$ states

This note applies the angular-factor framework from the cesium worked example to the proposed homonuclear silver-107 photoassociation experiment.  I do **not** repeat the full body-frame theory; instead I keep the same normalization and factorization as the tutorial and redo the channel-specific algebra for

$$
^{107}\mathrm{Ag}+{}^{107}\mathrm{Ag},
\qquad
I=\frac12,
\qquad
5s\,{}^2S_{1/2}+5p\,{}^2P_{3/2},
\qquad
f_1=f_2=1,
\qquad
\ell=0.
$$

The main result for the requested D2 $0_g^-$ channel is

$$
\boxed{
A\bigl(0_g^-;D2;f+f=1+1;s\text{-wave}\bigr)
=
\frac{7}{162}
\approx 0.04321.
}
$$

Under the convention described below for the D2 $1_u$ state, the unpolarized $f=1+1$, $s$-wave factor is also

$$
\boxed{
A\bigl(1_u;D2;f+f=1+1;s\text{-wave}\bigr)
=
\frac{7}{162}.
}
$$

For Zeeman-polarized samples, the result depends strongly on the prepared $m_f$ state.  For the D2 $0_g^-$ channel,

$$
\boxed{
A_{m_f=\pm1}(0_g^-)=\frac19,
\qquad
A_{m_f=0}(0_g^-)=\frac1{18}.
}
$$

Thus, in this angular-factor model, spin-polarizing into the stretched $|f=1,m_f=\pm1\rangle$ states increases the $0_g^-$ angular factor by

$$
\frac{1/9}{7/162}=\frac{18}{7}\approx2.57
$$

relative to the unpolarized statistical mixture.

---

## 1. Framework and normalization

The PA coupling is written in the same separated form as in the tutorial:

$$
V_{b,\nu}
=
\frac{\mathcal E_0 d_{\rm at}}{2}
\langle \psi_v|\chi_{E\ell}\rangle
\,a_\nu,
$$

where the dimensionless amplitude $a_\nu$ contains the rotational, polarization, electronic, hyperfine, exchange-symmetry, and molecular body-frame algebra.

The angular factor is the line strength

$$
A
=
\sum_{\rm final}\overline{|a_\nu|^2}_{\rm initial}.
$$

For the table-style unresolved angular factor, I use the same factorization as in the Cs example:

$$
\boxed{
A
=
\left(\frac13\right)
\times
\left(\text{exchange/statistical entrance weight}\right)
\times
\left(\text{body-fixed internal line strength}\right).
}
$$

The first factor, $1/3$, is the rotational/orientation/polarization average.  The nontrivial work is therefore to compute

1. which entrance hyperfine sectors survive Bose exchange symmetry for $s$-wave collisions, and  
2. the body-fixed electronic/hyperfine Clebsch--Gordan line strength after the correct molecular symmetry filter is applied.

---

## 2. Silver-107 input data

Silver is alkali-like in the relevant sense:

$$
\mathrm{Ag}:\ [\mathrm{Kr}]4d^{10}5s^1,
$$

so the ground valence electron has

$$
j_g=\frac12.
$$

For the D2 asymptote,

$$
j_e=\frac32.
$$

Both stable silver isotopes have nuclear spin

$$
I=\frac12.
$$

For the requested entrance channel,

$$
f=1=I+j_g.
$$

Because $^{107}$Ag has integer atomic hyperfine angular momentum in the $f=1$ state, the atom behaves as a boson for the exchange-symmetry counting relevant here.  The proposed experiment is homonuclear, so both atoms are $^{107}$Ag and the identical-particle exchange constraint must be imposed.

---

## 3. Entrance-channel exchange symmetry for $f+f=1+1$, $s$ wave

The two-atom hyperfine product basis has

$$
(2f+1)^2=3^2=9
$$

states.

Couple the two atomic hyperfine angular momenta:

$$
|f,f;F_tM_F\rangle.
$$

For two equal $f$ values, exchange gives

$$
P_{12}|f,f;F_tM_F\rangle
=
(-1)^{2f-F_t}|f,f;F_tM_F\rangle.
$$

For $f=1$,

$$
(-1)^{2f-F_t}=(-1)^{2-F_t}=(-1)^{F_t}.
$$

For homonuclear bosons in an $s$ wave,

$$
\ell=0
$$

is even, so the spatial wavefunction is symmetric.  Therefore the allowed hyperfine states are the symmetric, even-$F_t$ sectors:

$$
F_t=0,2.
$$

Their total degeneracy is

$$
(2\cdot0+1)+(2\cdot2+1)=1+5=6.
$$

Thus the statistical exchange factor for an unpolarized $f=1+1$ sample is

$$
\boxed{
W_{\rm ex}
=
\frac{6}{9}
=
\frac23.
}
$$

This replaces the Cs factor $45/81$ in the original worked example.

---

## 4. D2 $0_g^-$ channel

### 4.1 Target molecular state

For the D2 asymptote,

$$
j_g=\frac12,
\qquad
j_e=\frac32.
$$

For an $\Omega=0$ excited molecular state, the relevant projection pairs are

$$
\omega_e=+\frac12,
\quad
\omega_g=-\frac12,
$$

and

$$
\omega_e=-\frac12,
\quad
\omega_g=+\frac12.
$$

The $0_g^-$ state used in the Cs tutorial corresponds to the $J_{12}=2$, $\Omega=0$ combination, symmetrized with gerade inversion:

$$
|\Phi_{0_g^-}\rangle
=
\frac1{\sqrt2}
\left(
|eg;J_{12}=2,\Omega=0\rangle
+
|ge;J_{12}=2,\Omega=0\rangle
\right).
$$

The plus sign is the same convention used in the Cs $0_g^-$ derivation.

### 4.2 Molecular symmetry filter: why $q=\pm1$

For a final $0_g^-$ state, electric-dipole inversion symmetry requires the lower continuum component to be ungerade.  In the table-style calculation, this is the lower

$$
a^3\Sigma_u^+
$$

sector.

The lower continuum has reflection label $+$, while the final state has reflection label $-$.  Therefore this is a reflection-changing transition,

$$
\Sigma^+\to0^-.
$$

As in the Cs calculation, the body-frame line strength must keep the perpendicular body-frame dipole components

$$
q=\pm1,
$$

and must not include the parallel component $q=0$ in the same reflection-adapted line strength.

### 4.3 Body-fixed amplitude

The entrance hyperfine state is expanded as

$$
|(ff)F_tM_F\rangle
=
\sum_{m_{I1},\omega_1,m_{I2},\omega_2}
C^{F_tM_F}_{m_{I1}\omega_1m_{I2}\omega_2}
|m_{I1},\omega_1;m_{I2},\omega_2\rangle,
$$

where now

$$
I=\frac12,
\qquad
f=1,
\qquad
\omega_1,\omega_2=\pm\frac12.
$$

The coefficient is

$$
\begin{aligned}
C^{F_tM_F}_{m_{I1}\omega_1m_{I2}\omega_2}
&=
\langle f m_{f1};f m_{f2}|F_tM_F\rangle
\langle I m_{I1};\tfrac12\omega_1|f m_{f1}\rangle
\langle I m_{I2};\tfrac12\omega_2|f m_{f2}\rangle,
\end{aligned}
$$

with

$$
m_{f1}=m_{I1}+\omega_1,
\qquad
m_{f2}=m_{I2}+\omega_2.
$$

The one-atom body-frame dipole coefficient is

$$
\frac{
\langle 5p_{3/2},\omega_e|d_q|5s_{1/2},\omega_g\rangle
}{d_{\rm at}}
=
\langle 1q;\tfrac12\omega_g|\tfrac32\omega_e\rangle.
$$

The two coherent excitation pathways give

$$
\begin{aligned}
\mathcal M_q(F_t,M_F;m_{I1},m_{I2})
&=
\sum_{\omega_1,\omega_2}
C^{F_tM_F}_{m_{I1}\omega_1m_{I2}\omega_2}
\frac1{\sqrt2}
\Bigg[
\sum_{\omega_e,\omega_g}
\langle \tfrac32\omega_e;\tfrac12\omega_g|2,0\rangle
\delta_{\omega_g,\omega_2}
\langle 1q;\tfrac12\omega_1|\tfrac32\omega_e\rangle
\\
&\qquad\qquad+
\sum_{\omega_g,\omega_e}
\langle \tfrac12\omega_g;\tfrac32\omega_e|2,0\rangle
\delta_{\omega_g,\omega_1}
\langle 1q;\tfrac12\omega_2|\tfrac32\omega_e\rangle
\Bigg].
\end{aligned}
$$

This is the same expression as in the Cs note, but with

$$
I=\frac12,
\qquad
f=1,
\qquad
F_t=0,2.
$$

### 4.4 Body-fixed line strength

The body-fixed internal line strength is

$$
\boxed{
B(0_g^-)
=
\frac1{6}
\sum_{F_t=0,2}
\sum_{M_F=-F_t}^{F_t}
\sum_{q=\pm1}
\sum_{m_{I1},m_{I2}}
\left|
\mathcal M_q(F_t,M_F;m_{I1},m_{I2})
\right|^2.
}
$$

The denominator $6$ is the number of allowed symmetric entrance hyperfine states.

The partial sums are

$$
F_t=0:\quad \frac1{18},
$$

and

$$
F_t=2:\quad \frac{10}{9}.
$$

Therefore

$$
\sum_{F_t=0,2}\cdots
=
\frac1{18}+\frac{10}{9}
=
\frac76,
$$

and

$$
\boxed{
B(0_g^-)
=
\frac16\frac76
=
\frac7{36}.
}
$$

As a diagnostic, if one incorrectly includes $q=0$ together with $q=\pm1$, the body-fixed value becomes

$$
B_{q=-1,0,+1}=\frac7{12},
$$

while the $q=0$ contribution alone is

$$
B_{q=0}=\frac7{18}.
$$

Thus, just as in the Cs $0_g^-$ example, the exclusion of $q=0$ is not because the atomic Clebsch--Gordan coefficient vanishes.  It is because $q=0$ belongs to the wrong molecular reflection-sector line strength for the $a^3\Sigma_u^+\to0_g^-$ transition.

### 4.5 Final $0_g^-$ angular factor

Putting the pieces together,

$$
A(0_g^-)
=
\frac13
\times
\frac69
\times
\frac7{36}.
$$

Therefore

$$
\boxed{
A(0_g^-)
=
\frac7{162}
\approx0.04321.
}
$$

---

## 5. D2 $1_u$ channel

### 5.1 Convention for the $1_u$ state

The label $1_u$ specifies

$$
|\Omega|=1
$$

and ungerade inversion symmetry.  For the calculation below, I take the D2 $1_u$ state to be the $J_{12}=1$, $|\Omega|=1$ ungerade Hund-case-(c) state,

$$
|\Phi_{1_u,\Omega}\rangle
=
\frac1{\sqrt2}
\left(
|eg;J_{12}=1,\Omega\rangle
-
|ge;J_{12}=1,\Omega\rangle
\right),
\qquad
\Omega=\pm1.
$$

The minus sign is the ungerade counterpart of the gerade plus sign used above.  The standard molecular label $1_u$ usually denotes $|\Omega|=1$, so the final line strength below sums over both $\Omega=+1$ and $\Omega=-1$ components.

If instead one is working with a single signed $\Omega$ component only, the body-fixed result should be divided by two.

### 5.2 Molecular symmetry filter

Since the final state is ungerade, electric-dipole inversion symmetry requires the lower continuum component to be gerade.  The corresponding table-style lower sector is

$$
X^1\Sigma_g^+.
$$

The transition from a $\Sigma^+$ lower state to a $|\Omega|=1$ upper state is a perpendicular transition, so the body-frame components counted are again

$$
q=\pm1.
$$

### 5.3 Body-fixed line strength

The amplitude is the same coherent two-pathway expression as above, but with

$$
J_{12}=1,
\qquad
\Omega=\pm1,
\qquad
\text{ungerade sign }(-).
$$

The body-fixed line strength is

$$
\boxed{
B(1_u)
=
\frac1{6}
\sum_{F_t=0,2}
\sum_{M_F=-F_t}^{F_t}
\sum_{q=\pm1}
\sum_{\Omega=\pm1}
\sum_{m_{I1},m_{I2}}
\left|
\mathcal M_q^{(1_u)}(F_t,M_F;m_{I1},m_{I2};\Omega)
\right|^2.
}
$$

The partial sums are again

$$
F_t=0:\quad \frac1{18},
$$

and

$$
F_t=2:\quad \frac{10}{9}.
$$

Therefore

$$
\boxed{
B(1_u)=\frac7{36}.
}
$$

The final unpolarized $1_u$ angular factor is therefore

$$
A(1_u)
=
\frac13
\times
\frac69
\times
\frac7{36}
=
\boxed{\frac7{162}}.
$$

A useful caveat: in this pure $J_{12}$ model, the ungerade $J_{12}=2$, $|\Omega|=1$ component has zero coupling from the symmetric $f=1+1$, $s$-wave entrance manifold.  If the physical molecular level has appreciable mixing between ideal $J_{12}=1$ and $J_{12}=2$ characters, the observed line strength should be weighted by that mixing.

---

## 6. Zeeman-polarized entrance states

Now replace the unpolarized statistical mixture by a prepared entrance state

$$
|f=1,m_f=m\rangle_1
|f=1,m_f=m\rangle_2,
\qquad
m=-1,0,+1.
$$

Because both atoms are in the same internal state and the collision is $s$ wave, this product state is already symmetric under particle exchange.  Therefore the unpolarized factor

$$
\frac69
$$

should not be applied.  Instead we compute a fixed-state internal strength

$$
S_m
=
\sum_{\rm final}\left|\mathcal M_m\right|^2,
$$

and then use

$$
\boxed{
A_m=\frac13 S_m.
}
$$

This comparison assumes the same unresolved rotational/orientation/polarization average used above.  If a real experiment fixes a quantization axis and uses a definite lab-frame laser polarization, the lab-frame polarization selection rules should be applied explicitly on top of this body-frame estimate.

### 6.1 D2 $0_g^-$, Zeeman-polarized result

For the $0_g^-$ channel, with the same reflection-adapted $q=\pm1$ filter as above, the fixed-state strengths are

| prepared state | nonzero body-frame pieces | $S_m$ | $A_m=\frac13S_m$ |
|---:|---:|---:|---:|
| $m_f=-1$ | $q=+1$ | $\frac13$ | $\frac19$ |
| $m_f=0$ | $q=-1,+1$ | $\frac16$ | $\frac1{18}$ |
| $m_f=+1$ | $q=-1$ | $\frac13$ | $\frac19$ |

Thus

$$
\boxed{
A_{m_f=\pm1}(0_g^-)=\frac19,
\qquad
A_{m_f=0}(0_g^-)=\frac1{18}.
}
$$

Relative to the unpolarized result,

$$
A_{\rm unpol}(0_g^-)=\frac7{162},
$$

these are enhancement factors

$$
\frac{A_{m_f=\pm1}}{A_{\rm unpol}}
=
\frac{18}{7}
\approx2.57,
$$

and

$$
\frac{A_{m_f=0}}{A_{\rm unpol}}
=
\frac97
\approx1.29.
$$

So, for the D2 $0_g^-$ state, spin-polarizing helps in this angular-factor model, and the stretched states $m_f=\pm1$ are better than $m_f=0$ by a factor of two.

### 6.2 D2 $1_u$, Zeeman-polarized result

For the $J_{12}=1$, $|\Omega|=1$, ungerade $1_u$ convention used above, the fixed-state strengths are

| prepared state | $S_m$ | $A_m=\frac13S_m$ |
|---:|---:|---:|
| $m_f=-1$ | $0$ | $0$ |
| $m_f=0$ | $\frac16$ | $\frac1{18}$ |
| $m_f=+1$ | $0$ | $0$ |

Thus, for this idealized pure $1_u$ state,

$$
\boxed{
A_{m_f=0}(1_u)=\frac1{18},
\qquad
A_{m_f=\pm1}(1_u)=0.
}
$$

This is a qualitatively different conclusion from the $0_g^-$ channel.  If the goal is specifically the $1_u$ state under this model, preparing $m_f=0$ is favored, while the stretched states are symmetry-suppressed.

---

## 7. Summary table

### Unpolarized homonuclear $^{107}$Ag, $f+f=1+1$, $s$ wave

| target state | molecular model | $q$ components counted | $W_{\rm ex}$ | $B$ | $A=\frac13 W_{\rm ex}B$ |
|---|---|---:|---:|---:|---:|
| D2 $0_g^-$ | $J_{12}=2$, $\Omega=0$, gerade | $q=\pm1$ | $\frac69$ | $\frac7{36}$ | $\frac7{162}$ |
| D2 $1_u$ | $J_{12}=1$, $|\Omega|=1$, ungerade | $q=\pm1$, $\Omega=\pm1$ | $\frac69$ | $\frac7{36}$ | $\frac7{162}$ |

### Zeeman-polarized entrance-state comparison

| target state | $A_{m_f=-1}$ | $A_{m_f=0}$ | $A_{m_f=+1}$ | best choice in this model |
|---|---:|---:|---:|---|
| D2 $0_g^-$ | $\frac19$ | $\frac1{18}$ | $\frac19$ | $m_f=\pm1$ |
| D2 $1_u$ | $0$ | $\frac1{18}$ | $0$ | $m_f=0$ |

---

## 8. Minimal exact-code verification

The following symbolic Python/SymPy code reproduces the exact rational values above.  It follows the same Clebsch--Gordan structure as the Mathematica check in the tutorial.

```python
from sympy import S, sqrt, simplify
from sympy.physics.wigner import clebsch_gordan

I = S(1)/2
jg = S(1)/2
je = S(3)/2
f = S(1)
allowed_F = [S(0), S(2)]

def mlist(j):
    return [-j + i for i in range(int(2*j) + 1)]

def cg(j1, m1, j2, m2, J, M):
    if m1 + m2 != M:
        return S(0)
    return clebsch_gordan(j1, j2, J, m1, m2, M)

def amp_F(F, M, q, mI1, mI2, J12, Omega, parity_sign):
    total = S(0)
    for mj1 in mlist(jg):
        for mj2 in mlist(jg):
            mf1 = mI1 + mj1
            mf2 = mI2 + mj2
            ci = (
                cg(f, mf1, f, mf2, F, M)
                * cg(I, mI1, jg, mj1, f, mf1)
                * cg(I, mI2, jg, mj2, f, mf2)
            )

            me1 = mj1 + q
            term1 = (
                cg(S(1), q, jg, mj1, je, me1)
                * cg(je, me1, jg, mj2, J12, Omega)
                / sqrt(2)
            )

            me2 = mj2 + q
            term2 = (
                cg(S(1), q, jg, mj2, je, me2)
                * cg(jg, mj1, je, me2, J12, Omega)
                / sqrt(2)
            )

            total += ci * (term1 + parity_sign * term2)
    return simplify(total)

def B_unpolarized(J12, Omegas, parity_sign):
    total = S(0)
    partial = {}
    for F in allowed_F:
        subtotal = S(0)
        for M in mlist(F):
            for q in [S(-1), S(1)]:
                for Omega in Omegas:
                    for mI1 in mlist(I):
                        for mI2 in mlist(I):
                            a = amp_F(F, M, q, mI1, mI2, J12, Omega, parity_sign)
                            subtotal += a*a
        partial[F] = simplify(subtotal)
        total += subtotal
    return simplify(total / S(6)), partial

# D2 0g-: J12=2, Omega=0, gerade sign +
B_0g, partial_0g = B_unpolarized(S(2), [S(0)], +1)
print(B_0g, partial_0g)
# 7/36, {0: 1/18, 2: 10/9}

# D2 1u: J12=1, Omega=+/-1, ungerade sign -
B_1u, partial_1u = B_unpolarized(S(1), [S(1), S(-1)], -1)
print(B_1u, partial_1u)
# 7/36, {0: 1/18, 2: 10/9}
```

For the polarized calculation, replace the coupled entrance state by the product state $|f=1,m\rangle_1|f=1,m\rangle_2$ and remove the average over the six allowed $F_t$ states.
