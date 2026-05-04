## The physical picture

Two ultracold alkali atoms approach each other on a ground-state molecular potential $V_g(R)$, where $R$ is the internuclear separation. A laser, red-detuned by $\Delta$ from the atomic resonance line (D1 or D2), illuminates the pair. At a specific internuclear distance — the **Condon point** $R_C$ — the energy gap between $V_g(R)$ and an excited molecular potential $V_e(R)$ exactly matches the laser photon energy:

$$
V_e(R_C) - V_g(R_C) = \hbar\omega_L.
$$

The laser can then drive a **free-to-bound** transition: the scattering atom pair is photoassociated into a bound vibrational level $|v\rangle$ of $V_e$, forming a transient excited molecule.

The goal: derive the rate of this process, express it in terms of quantities an experimentalist controls (laser intensity, detuning, temperature), and understand when this rate saturates.

---

## Step 1. The coupling matrix element — where the Franck–Condon factor is born

### 1.1 Born–Oppenheimer factorization

In the Born–Oppenheimer picture, both the initial and final states factor into an electronic part and a nuclear (vibrational/scattering) part:

$$
|i\rangle = |\text{elec}_g\rangle \otimes |\chi_{E,\ell}(R)\rangle, \qquad
|f\rangle = |\text{elec}_e\rangle \otimes |\psi_v(R)\rangle.
$$

Here $|\chi_{E,\ell}\rangle$ is the radial scattering wave function on $V_g$ at collision energy $E$ and partial wave $\ell$ (energy-normalized: $\langle \chi_{E'}|\chi_E\rangle = \delta(E-E')$), and $|\psi_v\rangle$ is the unit-normalized bound vibrational wave function on $V_e$.

The electric-dipole interaction with the laser field is:

$$
\hat{H}_{\text{int}} = -\hat{\vec{d}} \cdot \vec{E}(t),
$$

where $\hat{\vec{d}}$ is the molecular electric dipole operator and $\vec{E}(t) = \vec{\epsilon}\,\mathcal{E}_0\cos(\omega_L t)$ is the laser field with polarization $\vec{\epsilon}$ and amplitude $\mathcal{E}_0$. In the rotating-wave approximation, the coupling matrix element is:

$$
V_b(E,\ell) = \frac{\mathcal{E}_0}{2}\langle f|\hat{\vec{d}}\cdot\vec{\epsilon}|i\rangle.
$$

### 1.2 Separating electronic and nuclear degrees of freedom

Inserting the BO factorization:

$$
V_b(E,\ell) = \frac{\mathcal{E}_0}{2} \int_0^\infty \psi_v^*(R)\;\underbrace{\langle\text{elec}_e|\hat{\vec{d}}\cdot\vec{\epsilon}|\text{elec}_g\rangle}_{d_{eg}(R)}\;\chi_{E,\ell}(R)\;dR.
$$

The function $d_{eg}(R)$ is the **$R$-dependent electronic transition dipole moment**. At large $R$ (where PA typically occurs, $R \gtrsim 40\,a_0$), $d_{eg}(R)$ approaches the **atomic** transition dipole moment $d_{\text{at}}$, because the two atoms are far enough apart that the molecular transition is essentially an atomic one. This motivates the:

> **Condon approximation.** Pull $d_{eg}(R) \approx d_{\text{at}}$ out of the integral.

This gives the key factorization:

$$
\boxed{V_{b,\nu}(E,\ell) = \frac{\mathcal{E}_0\,d_{\text{at}}}{2}\;\underbrace{\langle \psi_v | \chi_{E,\ell}\rangle}_{S(E,v)\;\text{(Franck--Condon overlap)}}\;\times\;a_\nu,}
\tag{1}
$$

where $\nu$ labels a specific angular/hyperfine/rotational channel, and $a_\nu$ is the **amplitude-level angular factor** for that channel. It contains all the Clebsch–Gordan and Wigner coefficients from projecting the laser polarization onto the body-frame electronic transition dipole, coupling two specific hyperfine states to a specific molecular Hund's-case-(c) state, and enforcing exchange symmetry for identical nuclei. For a single channel, $a_\nu$ is a product of CG coefficients and is typically a modest fraction of unity. When the experiment does not resolve individual channels, one squares, sums over final quantum numbers, and averages over initial ones; the result is the **line-strength angular factor** $A(g,e,\vec{\epsilon})$ discussed in Step 2.3 and Appendix B.

**Why this differs from the two-level Rabi model**: the coupling matrix element is the *atomic Rabi frequency* (which is $\Omega_{\text{at}} = d_{\text{at}}\mathcal{E}_0/\hbar$) times the *nuclear wave function overlap* (the Franck–Condon overlap), times the angular factor $a_\nu$. In the familiar two-level Rabi problem, the two states have perfect spatial overlap — both are the same atom in the same place — and there is one angular channel. Here, the initial and final *nuclear* wave functions live on different potentials and have very different spatial structure, so you pick up a penalty factor: the FC overlap. And there are many angular/hyperfine channels, each with its own coupling strength $a_\nu$.

### 1.3 Connecting $\mathcal{E}_0$ to laser intensity

The field amplitude relates to the laser intensity $I$ via $I = \tfrac{1}{2}\epsilon_0 c\,\mathcal{E}_0^2$, so:

$$
\mathcal{E}_0 = \sqrt{\frac{2I}{\epsilon_0 c}}.
$$

The **atomic Rabi frequency** is therefore:

$$
\Omega_{\text{at}} = \frac{d_{\text{at}}\mathcal{E}_0}{\hbar} = \frac{d_{\text{at}}}{\hbar}\sqrt{\frac{2I}{\epsilon_0 c}}.
$$

We can also express this through the **atomic saturation intensity** $I_{\text{sat}}$, defined for a two-level atom with natural linewidth $\Gamma$ as:

$$
I_{\text{sat}} = \frac{\pi h c \Gamma}{3\lambda^3},
$$

which gives the useful relation:

$$
\frac{\Omega_{\text{at}}^2}{2} = \frac{\Gamma^2}{4}\frac{I}{I_{\text{sat}}}.
\tag{$\star$}
$$

C. Drag et al.[^1] (Eq. 8) define the "half Rabi frequency" $K = \Omega_{\text{at}}/2$, so $K^2 = \Omega_{\text{at}}^2/4$. From ($\star$), this gives $K^2 = \tfrac{\Gamma^2}{8}\tfrac{I}{I_0}$ with their $I_0 = I_{\text{sat}}$. (Note: the printed formula in C. Drag et al.[^1] Eq. (8) reads $K^2 = (\Gamma/8)(I/I_0)$ with a single power of $\Gamma$, but this is a typographical error in the source article — the correct expression must have $\Gamma^2$ for dimensional consistency, since $K$ has dimensions of frequency.)

### 1.4 Dimensions of the Franck–Condon overlap

Since these dimensions propagate through every formula below, let us nail them down once and for all.

The energy-normalized scattering wave function satisfies $\langle\chi_{E'}|\chi_E\rangle = \delta(E-E')$. Since $\delta(E)$ has dimensions of $1/\text{energy}$, and the integral $\int |\chi_E|^2\,dR$ has dimensions of $[\chi]^2 \times \text{length}$, we need $[\chi]^2\times\text{length} = 1/\text{energy}$, giving:

$$
[\chi_{E,\ell}(R)] = \frac{1}{\sqrt{\text{energy}\times\text{length}}}.
$$

The unit-normalized bound state has $[\psi_v(R)] = 1/\sqrt{\text{length}}$.

Therefore the Franck–Condon overlap has dimensions:

$$
[S] = [\langle\psi_v|\chi_E\rangle] = \frac{1}{\sqrt{\text{length}}}\times\frac{1}{\sqrt{\text{energy}\times\text{length}}}\times\text{length} = \frac{1}{\sqrt{\text{energy}}},
$$

and the **FC factor** $|S|^2$ has dimensions of $1/\text{energy}$.

This means $V_b = (\hbar\Omega_{\text{at}}/2)\times S$ has dimensions of $\text{energy}/\sqrt{\text{energy}} = \sqrt{\text{energy}}$. This will be important in Step 2.

---

## Step 2. The stimulated width $\Gamma_b$ — a careful derivation from Fermi's golden rule

### 2.1 Why Fermi's golden rule, not Rabi oscillations?

In a standard two-level system with discrete states, you get coherent Rabi oscillations. But here the initial state is a **continuum** of scattering states at all energies $E$. This is exactly the Fano problem (Fano, 1961): a discrete state $|b\rangle$ embedded in (and coupled to) a continuum. The coupling to many continuum modes causes the discrete state to decay irreversibly — the recurrence time for Rabi-like revival diverges to infinity. The result is exponential decay of $|b\rangle$, characterized by a width $\Gamma_b$.

### 2.2 Deriving $\Gamma_b$ from Fermi's golden rule — properly

Fermi's golden rule in its textbook form uses **box-normalized** states $|n\rangle$ (satisfying $\langle n|m\rangle = \delta_{nm}$) and gives the transition rate from a discrete state $|b\rangle$ into a group of final states:

$$
\Gamma = \frac{2\pi}{\hbar}\,|{\langle n|V|b\rangle}|^2\;\rho(E),
\tag{FGR-box}
$$

where $\rho(E) = dn/dE$ is the **density of states** — the number of box-normalized states per unit energy.

Now, the energy-normalized states $|E\rangle$ are related to the box-normalized states by:

$$
|E\rangle = \sqrt{\rho(E)}\;|n(E)\rangle.
$$

This is just the statement that $\langle E'|E\rangle = \rho(E)\langle n'|n\rangle = \rho(E)\delta_{nn'} \to \delta(E-E')$ in the continuum limit. Therefore the matrix elements are related by:

$$
\langle E|V|b\rangle = \sqrt{\rho(E)}\;\langle n(E)|V|b\rangle
\qquad\Longrightarrow\qquad
|\langle n|V|b\rangle|^2 = \frac{|\langle E|V|b\rangle|^2}{\rho(E)}.
$$

Substituting into (FGR-box):

$$
\Gamma = \frac{2\pi}{\hbar}\;\frac{|\langle E|V|b\rangle|^2}{\rho(E)}\;\rho(E) = \frac{2\pi}{\hbar}\;|\langle E|V|b\rangle|^2.
$$

The density of states cancels exactly. This is the enormous convenience of energy-normalized states: Fermi's golden rule becomes simply

$$
\boxed{\Gamma_b(E,\ell) = \frac{2\pi}{\hbar}\;|V_b(E,\ell)|^2,}
\tag{2}
$$

with no explicit density-of-states factor. The density of states is already **built into** the normalization of $\chi_{E,\ell}$.

Let us verify the dimensions. From Step 1, $[V_b] = \sqrt{\text{energy}}$, so $|V_b|^2$ has dimensions of energy. Then $\Gamma_b = (2\pi/\hbar)\times\text{energy} = 1/\text{time}$. Correct: $\Gamma_b$ is a rate.

### 2.3 Explicit expression for $\Gamma_b$ in terms of laser intensity

Substituting Eq. (1) into Eq. (2), for a single angular channel $\nu$:

$$
\Gamma_{b,\nu}(E,\ell) = \frac{2\pi}{\hbar}\left(\frac{\hbar\Omega_{\text{at}}}{2}\right)^2 |S(E,v)|^2\,|a_\nu|^2 = \frac{\pi\hbar\Omega_{\text{at}}^2}{2}\;|S(E,v)|^2\;|a_\nu|^2.
$$

When the experiment does not resolve individual channels $\nu$, we sum $|a_\nu|^2$ over final quantum numbers ($J, M_J$) and average over the statistical mixture of initial quantum numbers ($F_t, M_F$), weighted by the bosonic symmetry constraints. This produces the **line-strength angular factor**:

$$
A(g,e,\vec{\epsilon}) \;\equiv\; \sum_{\text{final}} \overline{|a_\nu|^2}_{\;\text{initial}},
$$

and the channel-averaged stimulated width becomes:

$$
\Gamma_b(E,\ell) = \frac{\pi\hbar\Omega_{\text{at}}^2}{2}\;|S(E,v)|^2\;A(g,e,\vec{\epsilon}).
$$

Using $\Omega_{\text{at}}^2/2 = (\Gamma^2/4)(I/I_{\text{sat}})$:

$$
\boxed{\Gamma_b(E,\ell) = \frac{\pi\hbar\Gamma^2}{4}\;\frac{I}{I_{\text{sat}}}\;|S(E,v)|^2\;A(g,e,\vec{\epsilon}).}
\tag{3}
$$

For the cesium $0_g^-(6s+6p_{3/2})$ state with both atoms in $f=4$ and even partial waves, C. Drag et al.[^1] tabulate $A = 125/3888 \approx 0.032$ (see Appendix B for a detailed derivation of this value). The smallness of $A$ reflects the fact that only a fraction of the full atomic dipole coupling survives the angular momentum algebra: the molecular $\Omega = 0$ projection, exchange symmetry, and hyperfine structure all reduce the effective coupling.

### 2.4 Physical meaning of $\Gamma_b$

$\Gamma_b$ is the rate at which the **laser-driven** coupling causes the bound excited state $|b\rangle$ to decay back into the ground-state scattering continuum. It is the **stimulated** emission rate for the specific process $|b\rangle \xrightarrow{\text{laser}} |E,\ell\rangle$.

Think of it this way: the laser drives population both *up* (free $\to$ bound, creating the molecule) and *down* (bound $\to$ free, destroying it). In the Fano/scattering picture, both processes are captured by the single width $\Gamma_b$. The laser that creates the PA molecule is the same laser that can break it apart.

---

## Step 3. The three widths of the excited bound state

The excited bound state $|b\rangle$ can decay through several **independent channels**. Each channel contributes additively to the total decay rate:

$$
\Gamma_{\text{tot}} = \Gamma_{\text{nat}} + \Gamma_b(E,\ell) + \Gamma_o.
$$

Here is what each term is and why they are distinct:

**$\Gamma_{\text{nat}}$ — spontaneous emission (natural linewidth):**
The molecule in $|b\rangle$ has an electronically excited atom (it is on the $V_e$ potential, which correlates to one ground + one excited atom at large $R$). This excited atom can spontaneously emit a photon in any direction, at any frequency within the natural line profile, decaying to some state on the ground potential. At long range, the rate of this process approaches the bare atomic spontaneous emission rate $\Gamma$. Crucially, this happens **with or without the PA laser** — it is a property of the excited state itself. The final states after spontaneous decay can be either free (the pair flies apart) or bound (a ground-state molecule is formed — this is how cold molecules are made via PA).

**$\Gamma_b$ — stimulated emission back to the entrance channel:**
This is the rate at which the PA laser drives the molecule back into the specific scattering state it came from. It requires the laser to be present and is proportional to the laser intensity. Unlike $\Gamma_{\text{nat}}$, which scatters into $4\pi$ steradians and all allowed final states, $\Gamma_b$ is the rate for one specific final state: the entrance-channel scattering state at energy $E$ and partial wave $\ell$.

The reason $\Gamma_{\text{nat}}$ and $\Gamma_b$ are counted separately is that they describe **completely different physical processes**. $\Gamma_{\text{nat}}$ is spontaneous (no laser needed, all directions, many final states). $\Gamma_b$ is stimulated (requires the laser, one specific final state). In the language of quantum optics, $\Gamma_{\text{nat}}$ comes from coupling to the vacuum modes of the radiation field; $\Gamma_b$ comes from coupling to the laser mode.

**$\Gamma_o$ — other decay channels:**
Anything else that causes $|b\rangle$ to decay: predissociation (non-adiabatic coupling to a repulsive potential), spin-orbit mixing to other states, collisional quenching, ionization by a probe laser, etc.

**Analogy:** Consider a two-level atom in a laser field inside a leaky cavity. The atom decays by (i) stimulated emission into the laser mode ($\sim\Gamma_b$), (ii) spontaneous emission into free space ($\sim\Gamma_{\text{nat}}$), and (iii) non-radiative quenching ($\sim\Gamma_o$). The total decay rate is the sum. The PA problem has exactly this structure.

---

## Step 4. The Franck–Condon overlap — and the reflection approximation

### 4.1 The free-bound FC factor

The overlap integral is:

$$
S(E,v) = \langle\psi_v|\chi_{E,\ell}\rangle = \int_0^\infty \psi_v(R)\,\chi_{E,\ell}(R)\,dR,
$$

and the FC factor is $|S|^2$ (with dimensions $1/\text{energy}$). Computing $S$ requires knowing both wave functions. The bound state $\psi_v(R)$ comes from solving the Schrödinger equation on $V_e(R)$. The scattering state $\chi_{E,\ell}(R)$ comes from solving on $V_g(R)$ with scattering boundary conditions.

For quantitative work, you compute these numerically. But the **reflection approximation** gives a closed-form result that captures the essential physics.

### 4.2 The reflection approximation: general form and explicit long-range results

The reflection approximation is summarized by P. S. Julienne's light-field collision treatment[^2] and is written explicitly for long-range photoassociation by H. Wang and W. C. Stwalley.[^4] The generic result is:

$$
|S(E,v)|^2 = \frac{dE_v}{dv}\;\frac{1}{D_C}\;|\chi_{E,\ell}(R_C)|^2,
\tag{4}
$$

where:
- $R_C \approx R_{v+}$ is the Condon point, approximately the outer classical turning point of $|v\rangle$,
- $D_C = |d[V_e(R)-V_g(R)]/dR|_{R_C}$ is the difference in slopes of the excited and ground potentials at $R_C$,
- $dE_v/dv$ is the vibrational level spacing of the excited state.

The physics behind this is simple: the overlap integral is dominated by a narrow region around the outer turning point of the excited vibrational state, where the bound wave function has an Airy-function-like peak. The reflection approximation collapses the full integral into the value of the ground-state scattering wave function at this one point, multiplied by the local vibrational level spacing and divided by the local slope difference.

For long-range excited potentials of the form

$$
V_e(R)=D-\frac{C_n'}{R^n},
$$

Wang and Stwalley write the free-bound Franck--Condon factor as

$$
F_{v,J;E,J}\equiv |\langle \chi_{v,J}|\chi_{E,J}\rangle|^2
\approx \frac{dE_v}{dv}\,\frac{1}{d_v}\,|\chi_{E,J}(R_{v+})|^2,
$$

with

$$
d_v=\left|\frac{d}{dR}\left[V_e(R)-V_g(R)\right]\right|_{R_{v+}}
\approx \left|\frac{dV_e}{dR}\right|_{R_{v+}}
=\frac{nC_n'}{R_{v+}^{n+1}}.
$$

Here the last approximation uses the fact that the excited long-range potential is much steeper than the ground-state van der Waals potential in the relevant PA region.

For the **homonuclear alkali case**, where the excited long-range potential is dominated by the resonant dipole--dipole interaction $-C_3'/R^3$, Wang and Stwalley's explicit result is:

$$
\boxed{
F_{v;E,J}(n=3) = (2\pi\hbar^2)^{1/2}\frac{\Gamma(4/3)}{\Gamma(5/6)}\;\mu^{-1/2}
\left(\frac{C_3'}{R_v^3}\right)^{-1/2}
|\chi_{E,J}(R_v)|^2.
}
\tag{WS-9}
$$

This is the most relevant form for the homonuclear PA problem considered here. It says that, once the excited-state long-range coefficient and the outer turning point are fixed, the FC factor is essentially a local measurement of the entrance-channel scattering probability density at $R_v$.

For completeness, for the **heteronuclear alkali case**, where the excited long-range potential is usually van der Waals-like, $-C_6'/R^6$, the corresponding expression is:

$$
\boxed{
F_{v;E,J}(n=6) = (2\pi\hbar^2)^{1/2}\frac{\Gamma(7/6)}{\Gamma(2/3)}\;\mu^{-1/2}
\left(\frac{C_6'}{R_{v+}^6}\right)^{-1/2}
|\chi_{E,J}(R_{v+})|^2.
}
\tag{WS-8}
$$

The heteronuclear expression can be larger at very long range because the difference in slopes between ground and excited potentials is smaller than in the homonuclear resonant-dipole case. In both formulas, however, the central message is the same: the PA line strength tracks $|\chi_{E,J}(R_C)|^2$.

>[!NOTE]
> In C. Drag et al.[^1] (Eq. 7), the FC overlap appears as $S(\alpha,v)=\langle\alpha|v\rangle$ and is evaluated numerically using the relevant Cs$_2$ potentials. That numerical treatment is more accurate for the specific cesium levels studied there, while Eqs. (WS-8) and (WS-9) are the analytic long-range reflection-approximation limits.

### 4.3 Wigner threshold law from the FC overlap

At ultracold energies, the $s$-wave scattering wave function at moderate range behaves as $\chi_{E,0}(R) \propto \sqrt{k}(R - a_s)$ where $k = \sqrt{2\mu E/\hbar^2}$ and $a_s$ is the scattering length. Therefore:

$$
|\chi_{E,0}(R_C)|^2 \propto k \propto \sqrt{E}.
$$

Since $|S|^2 \propto |\chi_E(R_C)|^2$ (from the reflection approximation, Eq. 4) and $\Gamma_b \propto |S|^2$ (from Eq. 3), this energy dependence propagates through to give the **Wigner threshold law**:

$$
\Gamma_b(E, \ell=0) \propto E^{1/2} = E^{\ell+1/2}\big|_{\ell=0}.
$$

More generally, for partial wave $\ell$, the threshold behavior is $\Gamma_b \propto E^{\ell+1/2}$. This is the energy dependence that shapes the PA line profiles discussed in the review by K. M. Jones et al.[^3].

---

## Step 5. The Breit--Wigner two-body PA rate coefficient with the laser frequency explicit

The free-bound Franck--Condon factor and stimulated width from the previous sections tell us how strongly the PA laser couples an entrance-channel scattering state to one excited molecular bound state. The next question is: given that coupling, what is the two-body loss coefficient for a pair of atoms colliding at a definite relative collision energy?

The detailed Fano/Breit--Wigner derivation is best kept in the standalone note *Breit--Wigner Event Rate for Photoassociation*. Here we quote the result in the notation most useful for PA spectroscopy.

For one entrance partial wave $\ell$, the rate coefficient for transfer from the entrance channel into a detection/loss channel $d$ is

$$
\boxed{
K_d(E;\nu_L,I)
=
\frac{\pi v_{\rm rel}}{k^2}
\sum_\ell(2\ell+1)
\frac{\hbar\Gamma_b(E,\ell;I)\,\hbar\Gamma_d}
{\left[E+h\nu_L-h\nu_0-S_b(E,I)\right]^2
+\left[\hbar\Gamma_{\rm tot}(E,I)/2\right]^2}.
}
\tag{5}
$$

Here

$$
E=\frac{\hbar^2k^2}{2\mu}
=\frac12\mu v_{\rm rel}^2
$$

is the **relative collision energy** of the atom pair, not the single-atom kinetic energy. The relative velocity is

$$
v_{\rm rel}=\frac{\hbar k}{\mu}.
$$

The laser-frequency-dependent detuning in the Breit--Wigner denominator is

$$
\Delta_E(E;\nu_L,I)
=
E+h\nu_L-h\nu_0-S_b(E,I).
$$

The resonance condition is therefore

$$
\Delta_E(E;\nu_L,I)=0.
$$

In the weak-light-shift limit, $S_b\approx0$, this means that for a fixed PA laser frequency $\nu_L$, the resonant collision energy is

$$
\boxed{
E_r(\nu_L)=h\nu_0-h\nu_L.
}
\tag{5a}
$$

This is the clean meaning of $E_r$: it is the collision-energy class selected by the PA laser frequency. When the PA laser is scanned, $E_r$ is scanned through the thermal distribution of relative collision energies.

The widths are:

- $\Gamma_b(E,\ell;I)$: laser-induced stimulated width back to the entrance continuum;
- $\Gamma_d$: width into the detected/loss channel, often approximated by the natural radiative width $\Gamma_{\rm nat}$ for trap-loss detection;
- $\Gamma_o$: any additional predissociation, quenching, or other loss width;
- $\Gamma_{\rm tot}=\Gamma_b+\Gamma_d+\Gamma_o$.

In Eq. (5), the widths $\Gamma$ are rates in s$^{-1}$, and the factors $\hbar\Gamma$ convert them into energies in the Lorentzian. This is the notation used by the PA review literature.[^3]

The stimulated width is connected to the PA laser intensity by

$$
\Gamma_b(E,\ell;I)
=
\frac{\pi\hbar\Gamma_{\rm at}^2}{4}
\frac{I}{I_{\rm sat}}
A\,|S(E,v)|^2,
\tag{5b}
$$

where $A$ is the angular line-strength factor and $|S(E,v)|^2$ is the energy-normalized free-bound Franck--Condon factor. This is the same object that appears in the C. Drag et al. formula.[^1]

### 5.1 What does $K_d(E;\nu_L,I)$ mean?

$K_d(E;\nu_L,I)$ is a **two-body rate coefficient at one relative collision energy**. Its units are volume/time, e.g. cm$^3$/s. It is not yet a trap-loss rate and not yet a thermal average.

It is the cross section times relative velocity:

$$
K_d(E;\nu_L,I)=v_{\rm rel}\,\sigma_d(E;\nu_L,I).
$$

The prefactor

$$
\frac{\pi v_{\rm rel}}{k^2}
$$

is the single-partial-wave unitarity scale for an inelastic two-body process. The Lorentzian factor tells us what fraction of the incoming pair flux is transferred into the detected/loss channel.

### 5.2 The on-resonance saturation law for a monoenergetic collision

For the simplest case, take:

- one $s$-wave entrance channel;
- exact resonance, $\Delta_E=0$;
- trap-loss detection, $\Gamma_d=\Gamma_{\rm nat}\equiv\gamma$;
- no other decay, $\Gamma_o=0$.

Define the PA saturation parameter

$$
s\equiv\frac{I}{I_{\rm sat}^{\rm PA}}
=\frac{\Gamma_b}{\gamma}.
$$

Then

$$
\Gamma_{\rm tot}=\gamma+\Gamma_b=\gamma(1+s).
$$

The on-resonance coefficient becomes

$$
\boxed{
K_{\rm on-res}(E;I)
=
\frac{\pi v_{\rm rel}}{k^2}
\frac{4\Gamma_b\gamma}{(\gamma+\Gamma_b)^2}
=
\frac{\pi v_{\rm rel}}{k^2}
\frac{4s}{(1+s)^2}.
}
\tag{5c}
$$

This is the same saturation factor written in several PA saturation papers:

$$
\frac{4s}{(1+s)^2}
=\frac{4\gamma\Gamma_b}{(\gamma+\Gamma_b)^2}.
$$

It has three important limits:

$$
s\ll1:\quad K_{\rm on-res}\propto s\propto I,
$$

$$
s=1:\quad K_{\rm on-res}=\frac{\pi v_{\rm rel}}{k^2},
$$

$$
s\gg1:\quad K_{\rm on-res}\propto \frac1s\propto \frac1I.
$$

Thus for a **monoenergetic** collision, or for a line whose observed peak behaves like a monoenergetic resonance, PA can be oversaturated: the peak height can decrease at high intensity because power broadening makes the resonant scattering probability smaller at the exact line center.

---

## Step 6. Relative collision energy and the thermal distribution

A real MOT or ODT is not monoenergetic. The atoms have a thermal velocity distribution, and PA depends on the **relative** collision energy of an atom pair.

For two atoms at the same temperature $T$, the relative velocity is

$$
\mathbf v_{\rm rel}=\mathbf v_1-\mathbf v_2.
$$

The relative motion is described by the reduced mass

$$
\mu=\frac{m_1m_2}{m_1+m_2}.
$$

The relative collision energy is

$$
E=\frac12\mu v_{\rm rel}^2.
$$

For equal masses $m_1=m_2=m$, the reduced mass is $\mu=m/2$. The relative velocity distribution is broader than the one-particle velocity distribution, but the reduced mass is smaller by the corresponding factor. As a result, the relative-motion energy distribution has the **same temperature parameter** $T$:

$$
\boxed{
P_T(E)dE
=
\frac{2}{\sqrt\pi}
\frac{\sqrt E}{(k_BT)^{3/2}}
\exp\left(-\frac{E}{k_BT}\right)dE.
}
\tag{6}
$$

This distribution is normalized:

$$
\int_0^\infty P_T(E)dE=1.
$$

Its mean is

$$
\langle E\rangle=\frac32k_BT,
$$

and its most probable value is

$$
E_{\rm mode}=\frac12k_BT.
$$

Therefore, setting $E_r=k_BT$ in an order-of-magnitude PA estimate can be a **benchmark convention**, but not a law. It means: choose a representative collision energy of order the thermal energy.

---

## Step 7. The thermal PA coefficient at a scanned laser frequency

The physically useful local two-body PA coefficient at laser frequency $\nu_L$, temperature $T$, and intensity $I$ is obtained by thermal averaging the Breit--Wigner coefficient:

$$
\boxed{
\beta_{\rm PA}(\nu_L,T,I)
=
\int_0^\infty P_T(E)\,K_d(E;\nu_L,I)\,dE.
}
\tag{7}
$$

For one $s$-wave entrance channel this is

$$
\boxed{
\beta_{\rm PA}(\nu_L,T,I)
=
\int_0^\infty
P_T(E)
\frac{\pi v_{\rm rel}}{k^2}
\frac{\hbar\Gamma_b(E,I)\,\hbar\Gamma_d}
{\left[E+h\nu_L-h\nu_0-S_b(E,I)\right]^2
+\left[\hbar\Gamma_{\rm tot}(E,I)/2\right]^2}
\,dE.
}
\tag{7a}
$$

This is the master formula for a PA frequency scan. As $\nu_L$ is scanned, the resonant collision energy

$$
E_r(\nu_L)\approx h\nu_0-h\nu_L
$$

moves through the thermal distribution. The measured PA spectrum is a convolution of:

1. the Lorentzian Breit--Wigner resonance;
2. the thermal relative-energy distribution;
3. the Wigner-threshold energy dependence of $\Gamma_b(E)$;
4. the laser-induced light shift $S_b(E,I)$;
5. the intensity-dependent linewidth $\Gamma_{\rm tot}(E,I)$.

This is why a realistic PA scan is more complicated than simply evaluating a single FC factor.

### 7.1 Weak-field, narrow-resonance limit: C. Drag et al. Eq. (7)

Now impose the approximations used in the C. Drag et al. estimate:[^1]

1. $s$-wave only;
2. weak PA laser, $\Gamma_b\ll\Gamma_d$;
3. no important extra decay, $\Gamma_o\approx0$;
4. weak light shift, $S_b\approx0$;
5. the Lorentzian is narrow compared with the energy scale over which $P_T(E)$, $\Gamma_b(E)$, and $v/k^2$ vary.

Then

$$
\Gamma_{\rm tot}\approx\Gamma_d\equiv\gamma,
$$

and the Lorentzian selects

$$
E=E_r=h\nu_0-h\nu_L.
$$

Using

$$
\int_{-\infty}^{+\infty}
\frac{dE}{(E-E_r)^2+(\hbar\gamma/2)^2}
=
\frac{2\pi}{\hbar\gamma},
$$

Eq. (7a) becomes, schematically,

$$
\beta_{\rm PA}^{\rm weak}(\nu_L,T,I)
\propto
P_T(E_r)
\frac{\pi v_r}{k_r^2}
\hbar\Gamma_b(E_r,I).
$$

More explicitly, for $s$-wave,

$$
\frac{\pi v_{\rm rel}}{k^2}
=
\frac{\pi\hbar}{\mu k}
=
\frac{\pi\hbar^2}{\sqrt{2}\,\mu^{3/2}\sqrt E}.
$$

The factor $\sqrt E$ in the thermal distribution cancels the $1/\sqrt E$ in $v/k^2$. This cancellation is the reason the final C. Drag et al. expression has a simple Boltzmann factor.

The stimulated width is

$$
\Gamma_b(E_r,I)
=
2\pi\hbar\,A\,K^2\,S^2(E_r,v),
$$

where $K=\Omega_{\rm at}/2$ is the half atomic Rabi frequency and

$$
K^2=\frac{\Gamma_{\rm at}^2}{8}\frac{I}{I_0}.
$$

With the C. Drag et al. thermal-wavelength convention

$$
\lambda_{\rm th}=\frac{h}{\sqrt{3\mu k_BT}},
$$

the weak-field local per-atom PA rate is written as

$$
\boxed{
R_{\rm PA}^{\rm weak}
=n_{\rm at}\beta_{\rm PA}^{\rm weak}
=
A\left(\frac{3}{2\pi}\right)^{3/2}
\frac{h}{2}
\,n_{\rm at}\lambda_{\rm th}^3
\,e^{-E_r/k_BT}
\,K^2S^2(E_r,v).
}
\tag{7b}
$$

Equivalently, using the same convention in a more explicit prefactor form,

$$
\boxed{
R_{\rm PA}^{\rm weak}
=
n_{\rm at}\;
\frac{8\pi^3\hbar^2}{\sqrt{2\pi\mu}\,(k_BT)^{3/2}}
\;A\,K^2S^2(E_r,v)\;e^{-E_r/k_BT},
}
\tag{7c}
$$

up to the chosen convention for thermal wavelength and identical-pair normalization. The important invariant structure is

$$
\boxed{
R_{\rm PA}^{\rm weak}
\propto
n_{\rm at}\,A\,I\,S^2(E_r,v)\,T^{-3/2}\,e^{-E_r/k_BT}.
}
$$

This is the C. Drag et al. formula. It is a **weak-field thermal approximation**, not a saturated line-shape formula.

### 7.2 Why people sometimes set $E_r=k_BT$

The exact theory keeps $E_r$ as a laser-frequency-dependent variable:

$$
E_r=h\nu_0-h\nu_L.
$$

Setting

$$
E_r=k_BT
$$

is only a benchmark convention. It means the laser is assumed to address a representative collision-energy class of order the thermal energy, giving

$$
e^{-E_r/k_BT}=e^{-1}.
$$

For a full spectrum, do not set $E_r=k_BT$. Instead compute $\beta_{\rm PA}(\nu_L,T,I)$ as a function of $\nu_L$.

### 7.3 Saturation of a PA scan: peak height versus integrated area

The most common confusion is that different saturation factors describe different observables.

At exact resonance for one collision energy,

$$
K_{\rm on-res}(E;I)
=
\frac{\pi v_{\rm rel}}{k^2}\frac{4s}{(1+s)^2}.
$$

This is a **peak-height** statement. It says that a monoenergetic resonant cross section is maximal at $s=1$ and decreases for $s\gg1$.

But the **area** under a Lorentzian behaves differently. The Lorentzian part of Eq. (7a) has area

$$
\int dE\,
\frac{\hbar\Gamma_b\,\hbar\Gamma_d}
{(E-E_r)^2+[\hbar\Gamma_{\rm tot}/2]^2}
\propto
\frac{\Gamma_b\Gamma_d}{\Gamma_{\rm tot}}.
$$

For $\Gamma_d=\gamma$, $\Gamma_b=s\gamma$, and $\Gamma_{\rm tot}=\gamma(1+s)$, this gives

$$
\boxed{
\text{Lorentzian area}\propto\frac{s}{1+s}.
}
\tag{7d}
$$

Therefore:

$$
\boxed{
\text{line-center peak height}\propto\frac{s}{(1+s)^2},
}
$$

but

$$
\boxed{
\text{integrated line area}\propto\frac{s}{1+s}.
}
$$

These are not contradictory. At high intensity, the peak gets lower but the line gets broader. The area can saturate even while the peak height decreases.

### 7.4 Which saturation limit applies to an experiment?

The answer depends on the comparison between the power-broadened linewidth and the thermal energy width.

#### Regime A: monoenergetic or very cold sample

If the thermal distribution is narrow compared with the optical PA linewidth, the sample behaves nearly monoenergetically. The observed line-center signal follows approximately

$$
\frac{4s}{(1+s)^2}.
$$

Oversaturation reduces the peak height.

#### Regime B: broad thermal distribution and narrow Lorentzian

If

$$
\hbar\Gamma_{\rm tot}\ll k_BT,
$$

then the Lorentzian samples only a narrow slice of the thermal distribution. The thermal convolution near the peak is controlled more by the Lorentzian area, giving a saturation trend closer to

$$
\frac{s}{1+s}
$$

relative to a fixed thermal weight.

#### Regime C: power-broadened linewidth comparable to or larger than the thermal width

If

$$
\hbar\Gamma_{\rm tot}\gtrsim k_BT,
$$

then neither simple law is reliable. One must evaluate the full integral Eq. (7a). At very high intensity, the denominator is large over much of the thermal distribution, and the peak signal can again decrease.

Therefore the safe computational rule is:

$$
\boxed{
\text{For a real PA frequency scan, compute }\beta_{\rm PA}(\nu_L,T,I)
\text{ from Eq. (7a).}
}
$$

The simple factors $1/(1+s)^2$ or $1/(1+s)$ are useful diagnostics, not universal saturation corrections.

---

## Step 8. Mapping $\beta_{\rm PA}$ to MOT or ODT atom-number loss

After the thermal average, the output of the PA theory is a local two-body coefficient

$$
\beta_{\rm PA}(\nu_L,T,I),
$$

with units of volume/time. This is the coefficient to use in density or atom-number rate equations.

### 8.1 Uniform-density intuition

For a single-species gas with uniform density $n$, the local atom-number loss equation is usually written

$$
\boxed{
\frac{dn}{dt}=-\beta_{\rm PA}n^2.
}
\tag{8}
$$

The corresponding local per-atom loss rate is

$$
\boxed{
R_{\rm PA}=n\beta_{\rm PA}.
}
\tag{8a}
$$

This is the quantity reported in many PA papers in units of s$^{-1}$.

### 8.2 There is a factor $1/2$ for identical pairs

For identical atoms, the number of **unique unordered pairs** in a sample of $N$ atoms is

$$
\frac{N(N-1)}{2}\approx\frac{N^2}{2}.
$$

In a small volume element with density $n$, the number of unique pairs scales as

$$
\frac12 n^2 dV^2.
$$

Therefore, if $K_{\rm event}$ is defined as the pair-event coefficient from cross section times relative velocity, the molecule-formation event rate density is

$$
\boxed{
\dot n_{\rm event}
=
\frac12K_{\rm event}n^2.
}
\tag{8b}
$$

But each PA event removes two atoms from the trap. Therefore the atom-loss density is

$$
\dot n_{\rm atom}
=
-2\dot n_{\rm event}
=
-2\left(\frac12K_{\rm event}n^2\right)
=
-K_{\rm event}n^2.
$$

Thus the standard one-species atom-loss coefficient is

$$
\boxed{
\beta_{\rm PA}^{\rm atom-loss}=K_{\rm event}.
}
\tag{8c}
$$

This is why one should **not** multiply the homonuclear PA coefficient by 2 again when inserting it into an atom-number equation. The factor of 2 from two atoms lost per molecule is exactly canceled by the factor $1/2$ from counting identical pairs.

If instead one wants to report the number of molecules or PA events formed per unit time, then

$$
\boxed{
\dot N_{\rm mol/event}
=
\frac12\int \beta_{\rm PA}n^2({\bf r})\,d^3r.
}
\tag{8d}
$$

This is a different observable from atom-number loss.

### 8.3 Heteronuclear pairs

For two distinguishable species $a$ and $b$, there is no identical-pair $1/2$ in the number of pairs:

$$
\text{pair density}\sim n_an_b.
$$

If one PA event removes one atom of each species, then

$$
\frac{dn_a}{dt}=-K_{ab}n_an_b,
\qquad
\frac{dn_b}{dt}=-K_{ab}n_an_b.
$$

The total atom number $N_a+N_b$ decreases twice as fast as the molecule-event count, but each individual species decreases at the event rate. Some experimental papers insert factors of $1/2$ depending on whether their quoted coefficient is defined for total atom loss, single-species loss, or molecule-event formation. The coefficient definition must always be checked.

### 8.4 Spatially varying density and PA-beam overlap

In a real MOT or ODT, the density and PA intensity vary in space. The correct atom-number equation is

$$
\boxed{
\dot N_{\rm PA}
=
-\int \beta_{\rm PA}\bigl(\nu_L,T,I({\bf r})\bigr)
\,n^2({\bf r})\,d^3r.
}
\tag{8e}
$$

If the PA beam is much smaller than the atom cloud and the rate is still linear in intensity, one often writes an effective overlap factor

$$
\beta_{\rm PA}^{\rm eff}
=
\eta\,\beta_{\rm PA}^{\rm bare},
$$

where

$$
\eta
=
\frac{\int n^2({\bf r})I({\bf r})/I_0\,d^3r}
{\int n^2({\bf r})\,d^3r}.
$$

For a Gaussian PA beam crossing a Gaussian atom cloud, this can reduce to expressions such as

$$
\eta=\frac{w_0^2}{w_0^2+2\sigma_R^2}.
$$

Then the MOT equation can be written approximately as

$$
\dot N
=
L-\gamma N-
(\beta+\beta_{\rm PA}^{\rm eff})
\int n^2({\bf r})\,d^3r.
\tag{8f}
$$

This is the clean version of the convention used in the C. Drag et al. trap-loss extraction.[^1]

### 8.5 Steady-state MOT loss ratio

If the non-PA loss gives an effective per-atom decay rate

$$
\Gamma_0=\gamma+\beta n_{\rm eff}=\frac1\tau,
$$

and the PA laser adds an overlap-weighted per-atom loss rate

$$
\lambda_{\rm PA}^{\rm obs}=\eta\,n_{\rm at}\beta_{\rm PA}^{\rm bare},
$$

then the steady-state atom-number ratio is approximately

$$
\boxed{
\frac{N_{\rm PA}}{N_0}
\approx
\frac{\Gamma_0}{\Gamma_0+\lambda_{\rm PA}^{\rm obs}}.
}
\tag{8g}
$$

Equivalently, the observed fractional trap loss is

$$
\boxed{
f_{\rm loss}
=1-\frac{N_{\rm PA}}{N_0}
=
\frac{\lambda_{\rm PA}^{\rm obs}}{\Gamma_0+\lambda_{\rm PA}^{\rm obs}}.
}
\tag{8h}
$$

To compare theory to a de-overlapped experimental rate, use

$$
\boxed{
R_{\rm PA}^{\rm bare}=n_{\rm at}\beta_{\rm PA}^{\rm bare}.
}
$$

To compare theory directly to the observed MOT fluorescence loss, use

$$
\boxed{
R_{\rm PA}^{\rm obs}=\eta R_{\rm PA}^{\rm bare}
}
$$

inside Eq. (8g) or Eq. (8h).

### 8.6 ODT loss without loading

In an ODT or other conservative trap without continuous loading, the equation is usually closer to

$$
\boxed{
\dot N=-\gamma N-\int\beta_{\rm PA}(\nu_L,T,I({\bf r}))n^2({\bf r})d^3r.
}
\tag{8i}
$$

For a thermal gas with a fixed density shape, one often writes

$$
\dot N=-\gamma N-K_2^{\rm eff}N^2,
$$

where $K_2^{\rm eff}$ includes the spatial integral over the density distribution and the PA beam profile. In this case, the observable is the difference between laser-on and laser-off decay curves.

---

## Step 9. Practical computational recipe

For a rate-code pipeline, the hierarchy should be:

$$
S^2(E,v)
\rightarrow
\Gamma_b(E,I)
\rightarrow
K_d(E;\nu_L,I)
\rightarrow
\beta_{\rm PA}(\nu_L,T,I)
\rightarrow
\dot N.
$$

A minimal table can still report the C. Drag et al. weak-field value

$$
R_{\rm PA}^{\rm weak}
=n\beta_{\rm PA}^{\rm weak},
$$

but this should be clearly labeled as a perturbative result.

If one wants to discuss saturation without doing the full convolution, report diagnostic quantities separately:

$$
s=\frac{I}{I_{\rm sat}^{\rm PA}}
=\frac{\Gamma_b}{\gamma},
$$

$$
\text{monoenergetic peak-height factor:}\quad
\frac{1}{(1+s)^2}
\quad\text{relative to weak-field peak height},
$$

$$
\text{integrated-area factor:}\quad
\frac{1}{1+s}
\quad\text{relative to weak-field integrated area}.
$$

Neither factor is a universal replacement for the full integral. The full thermal PA scan is Eq. (7a).


---

## Appendix A. Dictionary of equivalent notations

| This note                                              | Julienne (1996)[^2] / reflection approximation | C. Drag et al.[^1]                            | Jones et al. RMP[^3]                      |
| ------------------------------------------------------ | ---------------------------------------------- | --------------------------------------------- | ----------------------------------------- |
| $V_{b,\nu}(E,\ell)$                                    | —                                              | —                                             | $V_b(E,\ell)$                             |
| $a_\nu$ (amplitude angular factor)                     | —                                              | —                                             | contained in $\mathcal{A}$                |
| $A(g,e,\vec{\epsilon})$ (line-strength angular factor) | —                                              | $A(g,e,\vec{\epsilon}_{\text{PA}})$ (Table I) | —                                         |
| $S(E,v) = \langle\psi_v\|\chi_E\rangle$                | $\langle\Psi_e(v)\|\Psi_g^+(E)\rangle$         | $S(\alpha,v)$                                 | $\langle b\|E,\ell\rangle$ (nuclear part) |
| $\Gamma_b$ (energy)                                    | $\gamma_s$ (energy)                            | (implicit in $A\,K^2 S^2$)                    | $\hbar\Gamma_b$ (energy)                  |
| $\Gamma_{\text{nat}}$ (energy)                         | —                                              | $\hbar\Gamma$ (energy)                        | $\hbar\Gamma_{\text{nat}}$ (energy)       |
| $I_{\text{sat}}$                                       | —                                              | $I_0$                                         | —                                         |
| $D_C$ (slope)                                          | $D_C$, $d_v$                                   | —                                             | —                                         |
| $R_C$ (Condon pt.)                                     | $R_C \approx R_{v+}$                           | —                                             | —                                         |
| $K(T) = \beta_{\text{PA}}$                             | —                                              | $\beta_{\text{PA}}$                           | $K_d(T)$                                  |
| $K(E)$                                                 | —                                              | —                                             | $K_d(E)$                                  |
| $\Delta(E)$ (light shift)                              | —                                              | —                                             | $S_b(E)$                                  |


---

## Appendix B. The angular factor $A(g,e,\vec{\epsilon})$ — detailed derivation

To avoid making this note tremendously long, the derivation details of the angular factor are moved to a standalone tutorial: [[Angular factor in photoassociation - a tutorial]].

[^1]: C. Drag _et al._, "Experimental versus theoretical rates for photoassociation and for formation of ultracold molecules," _IEEE J. Quantum Electron._, vol. 36, no. 12, pp. 1378–1388, Dec. 2000, doi: 10.1109/3.892556.
[^2]: P. S. Julienne, "Cold Binary Atomic Collisions in a Light Field," _J. Res. Natl. Inst. Stand. Technol._, vol. 101, no. 4, pp. 487–503, Jul.–Aug. 1996, doi: 10.6028/jres.101.050.
[^3]: K. M. Jones, E. Tiesinga, P. D. Lett, and P. S. Julienne, "Ultracold photoassociation spectroscopy: Long-range molecules and atomic scattering," _Rev. Mod. Phys._, vol. 78, no. 2, pp. 483–535, May 2006, doi: 10.1103/RevModPhys.78.483.
[^4]: H. Wang and W. C. Stwalley, "Ultracold photoassociative spectroscopy of heteronuclear alkali-metal diatomic molecules," _J. Chem. Phys._, vol. 108, no. 14, pp. 5767–5771, Apr. 1998, doi: 10.1063/1.475987.
