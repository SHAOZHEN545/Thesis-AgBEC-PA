# Breit–Wigner Event Rate for Photoassociation

## Motivation

This note derives the Breit–Wigner event-rate coefficient for photoassociation from a laser-coupled Fano model. The main goal is to keep the laser frequency explicit all the way through the derivation, so that the final rate coefficient carries the light-shifted photoassociation detuning

$$
\Delta_{\rm PA}(E)
=
E+h\nu-h\nu_0-S_b(E).
\tag{1}
$$

The final result is

$$
\boxed{
K_d(E)
=
v_{\rm rel}
\frac{\pi}{k^2}
\sum_{\ell}
(2\ell+1)
\frac{
\hbar\Gamma_d\;\hbar\Gamma_b(E,\ell)
}{
\left[
E+h\nu-h\nu_0-S_b(E)
\right]^2
+
\left(
\hbar\Gamma_{\rm tot}/2
\right)^2
}.
}
\tag{2}
$$

Here $d$ is the detected exit channel. In a trap-loss measurement, $d$ can represent spontaneous-emission channels that remove atom pairs from the trapped entrance channel.

---

## 1. Conventions and physical setup

Take the zero of energy to be the ground electronic dissociation threshold. The entrance-channel scattering states are

$$
|g;E,\ell m\rangle,
\tag{3}
$$

with

$$
H_g |g;E,\ell m\rangle
=
E |g;E,\ell m\rangle.
\tag{4}
$$

Here $E$ is the relative collision energy, $\ell$ is the partial wave, and $m$ is the magnetic quantum number.

The relative wave number and relative velocity are

$$
k
=
\frac{\sqrt{2\mu E}}{\hbar},
\qquad
v_{\rm rel}
=
\frac{\hbar k}{\mu}
=
\sqrt{\frac{2E}{\mu}},
\tag{5}
$$

where $\mu$ is the reduced mass.

The excited molecular bound state is

$$
|e;b\rangle
\equiv
|b\rangle.
\tag{6}
$$

In the lab frame, let the bare energy of this excited bound state above the ground-state dissociation threshold be

$$
E_b^{\rm lab}
=
h\nu_0.
\tag{7}
$$

Thus $h\nu_0$ is the photon energy that would connect a zero-energy ground-state atom pair to the bare excited bound state, before including the laser-induced shift.

Throughout the final photoassociation formula, the symbols $\Gamma_j$ denote rates in units of s$^{-1}$. Therefore $\hbar\Gamma_j$ is the corresponding energy width. It is useful to define

$$
\gamma_j
\equiv
\hbar\Gamma_j,
\tag{8}
$$

so that $\gamma_j$ has units of energy. In the derivation below, the algebra is cleaner in terms of $\gamma_j$. At the end we return to the usual photoassociation notation $\hbar\Gamma_j$.

---

## 2. Lab-frame laser coupling

The bare molecular Hamiltonian is

$$
H_{\rm mol}
=
\sum_{\ell m}\int_0^\infty dE\;
E\,|g;E,\ell m\rangle\langle g;E,\ell m|
+
h\nu_0\,|b\rangle\langle b|.
\tag{9}
$$

Without the laser, the entrance scattering state $|g;E,\ell m\rangle$ is not coupled to $|b\rangle$. The laser supplies the missing photon energy.

Let the applied laser have angular frequency

$$
\omega_L
=
2\pi\nu,
\qquad
\hbar\omega_L
=
h\nu.
\tag{10}
$$

Treat the laser as a classical monochromatic electric field,

$$
\mathbf{E}_L(t)
=
\frac{1}{2}\mathcal{E}_L\hat{\epsilon}e^{-i\omega_L t}
+
\frac{1}{2}\mathcal{E}_L^*\hat{\epsilon}^*e^{+i\omega_L t}.
\tag{11}
$$

The molecule-field interaction is

$$
V_L(t)
=
-\mathbf{d}\cdot \mathbf{E}_L(t),
\tag{12}
$$

where $\mathbf{d}$ is the molecular electric dipole operator.

Define the near-resonant free-bound laser matrix element

$$
W_{E\ell m}
=
-\frac{1}{2}\mathcal{E}_L
\langle b|\mathbf{d}\cdot\hat{\epsilon}|g;E,\ell m\rangle.
\tag{13}
$$

Then the lab-frame laser interaction contains terms of the form

$$
\begin{aligned}
V_L(t)
=
\sum_{\ell m}\int dE\;
\bigg[
&
W_{E\ell m}e^{-i\omega_L t}
|b\rangle\langle g;E,\ell m|
\\
&
+
\widetilde{W}_{E\ell m}e^{+i\omega_L t}
|b\rangle\langle g;E,\ell m|
+
{\rm h.c.}
\bigg].
\end{aligned}
\tag{14}
$$

The first term oscillates as $e^{-i\omega_L t}$ and corresponds to near-resonant photon absorption: the ground-channel atom pair absorbs one laser photon and is promoted to the excited bound molecular state. The second term is the counter-rotating term.

The full lab-frame Hamiltonian is therefore

$$
H_{\rm lab}(t)
=
H_{\rm mol}
+
V_L(t).
\tag{15}
$$

Because $H_{\rm lab}(t)$ is explicitly time dependent, the molecular subsystem alone does not conserve energy. The laser can exchange energy $h\nu$ with the atom pair. The useful conserved quantity after the rotating-frame transformation is the quasienergy.

---

## 3. Rotating frame and rotating wave approximation

Define the projector onto the excited bound state,

$$
P_b
=
|b\rangle\langle b|.
\tag{16}
$$

Use the unitary transformation

$$
R(t)
=
e^{-i\omega_L t P_b}.
\tag{17}
$$

Write the lab-frame wavefunction as

$$
|\psi_{\rm lab}(t)\rangle
=
R(t)|\psi_{\rm rot}(t)\rangle.
\tag{18}
$$

The rotating-frame Schrödinger equation is

$$
i\hbar\frac{\partial}{\partial t}|\psi_{\rm rot}(t)\rangle
=
H_{\rm rot}(t)|\psi_{\rm rot}(t)\rangle,
\tag{19}
$$

with

$$
H_{\rm rot}(t)
=
R^\dagger(t)H_{\rm lab}(t)R(t)
-
i\hbar R^\dagger(t)\dot{R}(t).
\tag{20}
$$

First evaluate the derivative term. Since

$$
\dot{R}(t)
=
-i\omega_L P_b R(t),
\tag{21}
$$

we get

$$
-i\hbar R^\dagger(t)\dot{R}(t)
=
-\hbar\omega_L P_b
=
-h\nu\,|b\rangle\langle b|.
\tag{22}
$$

Therefore the excited bound-state energy is shifted downward by one photon energy:

$$
h\nu_0\,|b\rangle\langle b|
\longrightarrow
(h\nu_0-h\nu)|b\rangle\langle b|.
\tag{23}
$$

Thus, in the rotating frame, the excited bound state has quasienergy

$$
E_b^{\rm rot}
=
h\nu_0-h\nu.
\tag{24}
$$

The ground-channel scattering states are not rotated, so their energies remain $E$.

Next transform the coupling term. Since

$$
R^\dagger(t)|b\rangle\langle g;E,\ell m|R(t)
=
e^{+i\omega_L t}|b\rangle\langle g;E,\ell m|,
\tag{25}
$$

the near-resonant absorption term becomes time independent:

$$
R^\dagger(t)
\left[
W_{E\ell m}e^{-i\omega_L t}
|b\rangle\langle g;E,\ell m|
\right]
R(t)
=
W_{E\ell m}
|b\rangle\langle g;E,\ell m|.
\tag{26}
$$

The counter-rotating term becomes

$$
R^\dagger(t)
\left[
\widetilde{W}_{E\ell m}e^{+i\omega_L t}
|b\rangle\langle g;E,\ell m|
\right]
R(t)
=
\widetilde{W}_{E\ell m}e^{+2i\omega_L t}
|b\rangle\langle g;E,\ell m|.
\tag{27}
$$

Therefore

$$
\begin{aligned}
H_{\rm rot}(t)
=
&
\sum_{\ell m}\int dE\;
E\,|g;E,\ell m\rangle\langle g;E,\ell m|
+
(h\nu_0-h\nu)|b\rangle\langle b|
\\
&
+
\sum_{\ell m}\int dE\;
\left[
W_{E\ell m}|b\rangle\langle g;E,\ell m|
+
W_{E\ell m}^*|g;E,\ell m\rangle\langle b|
\right]
\\
&
+
\sum_{\ell m}\int dE\;
\left[
\widetilde{W}_{E\ell m}e^{+2i\omega_L t}|b\rangle\langle g;E,\ell m|
+
\widetilde{W}_{E\ell m}^*e^{-2i\omega_L t}|g;E,\ell m\rangle\langle b|
\right].
\end{aligned}
\tag{28}
$$

The last line oscillates at approximately $2\omega_L$. When the laser is near resonance and the relevant coupling strengths, detunings, and decay rates are much smaller than $\omega_L$, these terms average to zero on the timescale of the photoassociation dynamics.

The rotating wave approximation drops the $e^{\pm 2i\omega_L t}$ terms. Thus

$$
\boxed{
H_{\rm RWA}
=
\sum_{\ell m}\int dE\;
E\,|g;E,\ell m\rangle\langle g;E,\ell m|
+
(h\nu_0-h\nu)|b\rangle\langle b|
+
\sum_{\ell m}\int dE\;
\left[
W_{E\ell m}|b\rangle\langle g;E,\ell m|
+
W_{E\ell m}^*|g;E,\ell m\rangle\langle b|
\right].
}
\tag{29}
$$

This is the time-independent Fano model used for the scattering derivation, with the identifications

$$
E_b
\longrightarrow
E_b^{\rm rot}
=
h\nu_0-h\nu,
\tag{30}
$$

and

$$
V_b(E,\ell m)
\longrightarrow
W_{E\ell m}.
\tag{31}
$$

Therefore the discrete state in the Fano model is not the lab-frame excited molecular state at energy $h\nu_0$. It is the laser-dressed, rotating-frame bound state at quasienergy $h\nu_0-h\nu$.

The bare resonance condition is

$$
E
=
h\nu_0-h\nu,
\tag{32}
$$

or equivalently

$$
E+h\nu
=
h\nu_0.
\tag{33}
$$

The incoming atom pair contributes collision energy $E$, the laser contributes photon energy $h\nu$, and the sum must match the excited molecular bound-state energy $h\nu_0$.

---

## 4. Equivalent dressed-state interpretation

The same result can be obtained by quantizing the laser mode.

In the quantized picture, the entrance state is

$$
|g;E,\ell m;N\rangle,
\tag{34}
$$

with total energy

$$
E+Nh\nu.
\tag{35}
$$

After absorbing one photon, the excited molecular state is

$$
|b;N-1\rangle,
\tag{36}
$$

with total energy

$$
h\nu_0+(N-1)h\nu.
\tag{37}
$$

Subtract the common photon energy $Nh\nu$ from both states. The entrance state has relative energy $E$, while the excited dressed state has relative energy

$$
h\nu_0-h\nu.
\tag{38}
$$

This is exactly the rotating-frame bound-state energy $E_b^{\rm rot}$. Therefore the rotating-frame derivation and the dressed-state derivation are the same physical statement.

---

## 5. The Fano scattering model after RWA

For a fixed entrance partial wave $\ell m$, suppress the labels temporarily and write

$$
|E\rangle
\equiv
|g;E,\ell m\rangle,
\qquad
V_b(E)
\equiv
W_{E\ell m}.
\tag{39}
$$

The energy-normalized continuum satisfies

$$
\langle E'|E\rangle
=
\delta(E'-E).
\tag{40}
$$

The RWA Fano Hamiltonian for this partial wave is

$$
H
=
H_0+V,
\tag{41}
$$

where

$$
H_0|E\rangle
=
E|E\rangle,
\qquad
H_0|b\rangle
=
E_b^{\rm rot}|b\rangle,
\tag{42}
$$

and

$$
\langle E|V|b\rangle
=
V_b(E),
\qquad
\langle b|V|E\rangle
=
V_b^*(E).
\tag{43}
$$

We take

$$
\langle b|V|b\rangle
=
0,
\qquad
\langle E'|V|E\rangle
=
0.
\tag{44}
$$

These assumptions mean that there is no direct continuum-continuum coupling and no diagonal bound-state shift already included in $V$. Any such diagonal shift can be absorbed into the definition of the bare energy or into the self-energy shift introduced below.

---

## 6. Scattering eigenstate and the origin of the $+i\epsilon$

We want the exact scattering eigenstate with incoming energy $E$ and outgoing-wave boundary condition. Write it as

$$
|\Psi_E^+\rangle
=
|E\rangle
+
a(E)|b\rangle
+
\int dE'\;c(E',E)|E'\rangle.
\tag{45}
$$

The superscript $+$ means outgoing boundary condition. The first term is the incident energy-normalized scattering state. The $a(E)|b\rangle$ term is the resonant bound-state amplitude. The integral term is the continuum part of the scattered wave.

Applying

$$
H|\Psi_E^+\rangle
=
E|\Psi_E^+\rangle
\tag{46}
$$

and projecting onto $\langle b|$ gives

$$
E_b^{\rm rot}a(E)
+
\int dE'\;V_b^*(E')c(E',E)
+
V_b^*(E)
=
Ea(E).
\tag{47}
$$

Projecting onto $\langle E'|$ gives

$$
E'c(E',E)
+
V_b(E')a(E)
=
Ec(E',E).
\tag{48}
$$

Rearranging Eq. (48),

$$
(E-E')c(E',E)
=
V_b(E')a(E).
\tag{49}
$$

Naively, one would write $c(E',E)=V_b(E')a(E)/(E-E')$. But this expression is singular at $E'=E$. More importantly, the inverse of $E-H_0$ is not unique on the continuum. The homogeneous equation has solutions proportional to $\delta(E-E')$, so one must specify how the scattered wave behaves asymptotically.

The Lippmann-Schwinger equation supplies this missing information:

$$
|\Psi_E^\pm\rangle
=
|E\rangle
+
\frac{1}{E-H_0\pm i0}V|\Psi_E^\pm\rangle.
\tag{50}
$$

The choice $+i0$ defines the outgoing scattering state. The choice $-i0$ defines the incoming scattering state.

Therefore Eq. (49) is solved as

$$
\boxed{
c(E',E)
=
\frac{V_b(E')a(E)}{E-E'+i0}.
}
\tag{51}
$$

This is the precise meaning of the $+i\epsilon$ prescription:

$$
\frac{1}{E-E'+i0}
\equiv
\lim_{\epsilon\to 0^+}
\frac{1}{E-E'+i\epsilon}.
\tag{52}
$$

### 6.1 Distribution identity

The denominator in Eq. (51) is interpreted as a distribution. The Sokhotski-Plemelj identity gives

$$
\frac{1}{x+i0}
=
\mathcal{P}\frac{1}{x}
-
i\pi\delta(x).
\tag{53}
$$

With $x=E-E'$,

$$
\frac{1}{E-E'+i0}
=
\mathcal{P}\frac{1}{E-E'}
-
i\pi\delta(E-E').
\tag{54}
$$

Thus $c(E',E)$ contains two pieces:

$$
c(E',E)
=
V_b(E')a(E)
\mathcal{P}\frac{1}{E-E'}
-
i\pi V_b(E)a(E)\delta(E-E').
\tag{55}
$$

The principal-value part produces a real energy shift of the bound level. The delta-function part puts amplitude exactly on shell, $E'=E$, and gives the imaginary part of the self-energy. This imaginary part is the width. Physically, it is the irreversible loss of probability from the discrete state into open continuum states.

If we used only the principal value, the state would be a standing-wave solution. There would be a level shift but no net outgoing flux. The $-i\pi\delta(E-E')$ term is the mathematical signature of outgoing scattering flux.

### 6.2 Time-domain meaning: retarded propagation

The $+i0$ prescription can also be understood from time evolution. For $\epsilon>0$,

$$
\frac{1}{E-H_0+i\epsilon}
=
-\frac{i}{\hbar}
\int_0^\infty dt\;
e^{i(E-H_0+i\epsilon)t/\hbar}.
\tag{56}
$$

The factor $e^{-\epsilon t/\hbar}$ makes the integral converge at large positive time. The integral only runs over $t>0$, so the scattered wave is produced after the incoming wave interacts with the potential. This is the retarded, causal choice.

The opposite prescription gives

$$
\frac{1}{E-H_0-i\epsilon}
=
\frac{i}{\hbar}
\int_{-\infty}^0 dt\;
e^{i(E-H_0-i\epsilon)t/\hbar},
\tag{57}
$$

which is advanced in the scattering sense and corresponds to incoming-wave boundary conditions for the scattered part.

### 6.3 Coordinate-space meaning: outgoing spherical waves

For a free relative-motion Hamiltonian

$$
H_0
=
-\frac{\hbar^2}{2\mu}\nabla^2,
\tag{58}
$$

define $E=\hbar^2k^2/(2\mu)$. The coordinate-space Green function is

$$
G_0^+(\mathbf{r},\mathbf{r}')
=
\left\langle \mathbf{r}\left|
\frac{1}{E-H_0+i0}
\right|\mathbf{r}'\right\rangle.
\tag{59}
$$

It evaluates to

$$
G_0^+(\mathbf{r},\mathbf{r}')
=
-\frac{\mu}{2\pi\hbar^2}
\frac{e^{+ik|\mathbf{r}-\mathbf{r}'|}}{|\mathbf{r}-\mathbf{r}'|}.
\tag{60}
$$

The corresponding $-i0$ Green function is

$$
G_0^-(\mathbf{r},\mathbf{r}')
=
-\frac{\mu}{2\pi\hbar^2}
\frac{e^{-ik|\mathbf{r}-\mathbf{r}'|}}{|\mathbf{r}-\mathbf{r}'|}.
\tag{61}
$$

The full stationary wave has time dependence $e^{-iEt/\hbar}$. Therefore the outgoing Green function has phase

$$
e^{ikR}e^{-iEt/\hbar}
=
e^{i(kR-\omega t)},
\qquad
R=|\mathbf{r}-\mathbf{r}'|,
\qquad
\omega=\frac{E}{\hbar}.
\tag{62}
$$

A surface of constant phase satisfies

$$
kR-\omega t
=
{\rm constant},
\tag{63}
$$

so

$$
\frac{dR}{dt}
=
\frac{\omega}{k}
>
0.
\tag{64}
$$

Thus the wavefront moves outward as time increases. This is why $+i0$ means outgoing boundary condition. By contrast, $e^{-ikR}e^{-iEt/\hbar}$ has constant phase $-kR-\omega t={\rm constant}$, giving $dR/dt=-\omega/k<0$, which is an incoming spherical wave.

---

## 7. Self-energy and the resonant bound-state amplitude

Substitute Eq. (51) into Eq. (47):

$$
E_b^{\rm rot}a(E)
+
a(E)\int dE'\;
\frac{|V_b(E')|^2}{E-E'+i0}
+
V_b^*(E)
=
Ea(E).
\tag{65}
$$

Move the first two terms to the right form:

$$
\left[
E-E_b^{\rm rot}
-
\int dE'\;
\frac{|V_b(E')|^2}{E-E'+i0}
\right]a(E)
=
V_b^*(E).
\tag{66}
$$

Define the entrance-continuum self-energy

$$
\Sigma_b(E)
=
\int dE'\;
\frac{|V_b(E')|^2}{E-E'+i0}.
\tag{67}
$$

Using Eq. (54),

$$
\Sigma_b(E)
=
\mathcal{P}\int dE'\;
\frac{|V_b(E')|^2}{E-E'}
-
i\pi |V_b(E)|^2.
\tag{68}
$$

Define the real light shift

$$
S_b(E)
=
\mathcal{P}\int dE'\;
\frac{|V_b(E')|^2}{E-E'},
\tag{69}
$$

and the entrance stimulated energy width

$$
\gamma_b(E)
=
2\pi |V_b(E)|^2.
\tag{70}
$$

Then

$$
\Sigma_b(E)
=
S_b(E)
-
i\frac{\gamma_b(E)}{2}.
\tag{71}
$$

Since $\gamma_b=\hbar\Gamma_b$,

$$
\hbar\Gamma_b(E)
=
2\pi |V_b(E)|^2.
\tag{72}
$$

For the specific photoassociation partial wave $\ell$, we write

$$
\hbar\Gamma_b(E,\ell)
=
2\pi |W_{E\ell}|^2,
\tag{73}
$$

with any magnetic sublevel and polarization factors either included in $W_{E\ell}$ or averaged/summed separately.

Now Eq. (66) gives

$$
a(E)
=
\frac{
V_b^*(E)
}{
E-E_b^{\rm rot}-S_b(E)+i\gamma_b(E)/2
}.
\tag{74}
$$

Using the RWA energy $E_b^{\rm rot}=h\nu_0-h\nu$,

$$
E-E_b^{\rm rot}-S_b(E)
=
E-(h\nu_0-h\nu)-S_b(E)
=
E+h\nu-h\nu_0-S_b(E).
\tag{75}
$$

Therefore the resonant bound-state amplitude is

$$
a(E)
=
\frac{
V_b^*(E)
}{
E+h\nu-h\nu_0-S_b(E)+i\gamma_b(E)/2
}.
\tag{76}
$$

If the entrance continuum were the only open channel, this would be the whole result. In photoassociation, however, the excited molecular state can also decay by spontaneous emission or other loss mechanisms, so the denominator must include the total width.

---

## 8. Adding additional decay channels

Let the excited bound state also couple to other open continua, labeled by $j$. These may include spontaneous-emission channels, predissociation channels, optical pumping channels, or any other channel that removes flux from the entrance channel.

For each channel $j$, introduce a coupling matrix element $V_j(E_j)$. The self-energy contribution from channel $j$ is

$$
\Sigma_j(E)
=
\int dE_j\;
\frac{|V_j(E_j)|^2}{E-E_j+i0}.
\tag{77}
$$

As before,

$$
\Sigma_j(E)
=
S_j(E)
-
i\frac{\gamma_j(E)}{2},
\tag{78}
$$

where

$$
S_j(E)
=
\mathcal{P}\int dE_j\;
\frac{|V_j(E_j)|^2}{E-E_j},
\tag{79}
$$

and

$$
\gamma_j(E)
=
2\pi |V_j(E)|^2
=
\hbar\Gamma_j(E).
\tag{80}
$$

The total self-energy is

$$
\Sigma_{\rm tot}(E)
=
\sum_j \Sigma_j(E).
\tag{81}
$$

In photoassociation notation, it is common to keep the laser-induced entrance-channel shift explicitly as $S_b(E)$ and absorb small additional real shifts into the definition of $h\nu_0$. With that convention,

$$
\Sigma_{\rm tot}(E)
=
S_b(E)
-
i\frac{\gamma_{\rm tot}(E)}{2},
\tag{82}
$$

where

$$
\gamma_{\rm tot}
=
\gamma_b
+
\gamma_{\rm nat}
+
\gamma_o.
\tag{83}
$$

Equivalently,

$$
\Gamma_{\rm tot}
=
\Gamma_b
+
\Gamma_{\rm nat}
+
\Gamma_o.
\tag{84}
$$

The resonant propagator of the bound state is therefore

$$
\boxed{
G_b(E)
=
\frac{1}{
E+h\nu-h\nu_0-S_b(E)+i\hbar\Gamma_{\rm tot}/2
}.
}
\tag{85}
$$

This is the central place where the RWA laser detuning enters the Breit–Wigner formula.

---

## 9. Why the $S$ matrix is the object we need

The $S$ matrix is the object that connects asymptotic incoming scattering channels to asymptotic outgoing scattering channels. In a collision experiment, the interaction happens only in a finite region, but the incoming and outgoing particles are prepared and detected far away from that region. Therefore the measurable quantities are not the short-range wavefunction amplitudes by themselves, but the outgoing fluxes in each channel for a given incoming flux.

For an incoming channel $i$, the asymptotic scattering relation is schematically

$$
|{\rm out}\rangle
=
S|{\rm in}\rangle.
\tag{86}
$$

The matrix element

$$
S_{fi}(E)
=
\langle f;{\rm out}|S|i;{\rm in}\rangle
\tag{87}
$$

is the probability amplitude for an incoming wave in channel $i$ to emerge in channel $f$ at the same conserved total energy.

For $f\neq i$, there is no identity contribution. The transition probability for that partial wave is simply

$$
P_{f\leftarrow i}^{(\ell)}(E)
=
|S_{fi}^{(\ell)}(E)|^2.
\tag{88}
$$

This is why the detection cross-section is proportional to $|S_d(E)|^2$: photoassociation detection is an inelastic, state-changing event. The $S$ matrix tells us the outgoing flux in the detected channel per incoming flux in the entrance channel.

The $T$ matrix is related to the $S$ matrix by

$$
S_{fi}(E)
=
\delta_{fi}
-
2\pi i\,T_{fi}(E),
\tag{89}
$$

for energy-normalized continuum states. In the Fano model, the transition from the entrance channel to any exit channel happens by entering the resonant bound state, propagating on the bound-state resonance, and exiting into the final channel.

---

## 10. Multi-channel resonant $S$ matrix and the origin of $\sqrt{\Gamma_b\Gamma_d}$

Let $i$ denote the entrance channel and $d$ denote the detected exit channel. In the present problem,

$$
i
=
(g;E,\ell m),
\tag{90}
$$

and $d$ is some detected decay or loss channel.

From the Fano solution, the bound-state amplitude generated by the incoming channel $i$ is

$$
a_i(E)
=
V_i^*(E)G_b(E),
\tag{91}
$$

where

$$
V_i(E)
=
V_b(E)
=
W_{E\ell m}.
\tag{92}
$$

The $T$-matrix element into the detected channel is

$$
T_{di}(E)
=
\langle d|V|\Psi_i^+\rangle.
\tag{93}
$$

Since there is no direct continuum-continuum coupling in the Fano model, the only contribution is through the resonant bound-state amplitude:

$$
T_{di}(E)
=
V_d(E)a_i(E)
=
V_d(E)V_i^*(E)G_b(E).
\tag{94}
$$

Substitute the resonant propagator:

$$
T_{di}(E)
=
\frac{
V_d(E)V_i^*(E)
}{
E+h\nu-h\nu_0-S_b(E)+i\gamma_{\rm tot}/2
}.
\tag{95}
$$

For $d\neq i$, the $S$ matrix has no identity term, so

$$
S_{di}(E)
=
-2\pi i\,T_{di}(E).
\tag{96}
$$

Therefore

$$
S_{di}(E)
=
\frac{
-2\pi i\,V_d(E)V_i^*(E)
}{
E+h\nu-h\nu_0-S_b(E)+i\gamma_{\rm tot}/2
}.
\tag{97}
$$

Now use the definition of the partial width:

$$
\gamma_i(E)
=
2\pi |V_i(E)|^2,
\qquad
\gamma_d(E)
=
2\pi |V_d(E)|^2.
\tag{98}
$$

The product of couplings can be written as

$$
2\pi V_d(E)V_i^*(E)
=
\sqrt{\gamma_d(E)\gamma_i(E)}\;e^{i\phi_{di}},
\tag{99}
$$

where $\phi_{di}$ is a phase determined by the arbitrary phase convention of the channel states. That phase can be absorbed into the definition of the channel basis, and it drops out of $|S_{di}|^2$ anyway. Choosing the simple phase convention $e^{i\phi_{di}}=1$ gives

$$
\boxed{
S_{di}(E)
=
\frac{
-i\sqrt{\gamma_i(E)\gamma_d(E)}
}{
E+h\nu-h\nu_0-S_b(E)+i\gamma_{\rm tot}/2
}.
}
\tag{100}
$$

For photoassociation, $\gamma_i(E)=\gamma_b(E,\ell)=\hbar\Gamma_b(E,\ell)$ and $\gamma_d=\hbar\Gamma_d$. Thus

$$
\boxed{
S_{d\leftarrow E\ell}(E)
=
\frac{
-i\sqrt{\hbar\Gamma_b(E,\ell)}\sqrt{\hbar\Gamma_d}
}{
E+h\nu-h\nu_0-S_b(E)+i\hbar\Gamma_{\rm tot}/2
}.
}
\tag{101}
$$

This equation explains the numerator. The entrance width $\Gamma_b$ is proportional to the probability per unit time for the entrance scattering continuum to feed the bound state. Since probability is amplitude squared, the entrance amplitude is proportional to $\sqrt{\Gamma_b}$. Likewise, the exit amplitude into channel $d$ is proportional to $\sqrt{\Gamma_d}$. The resonant transition amplitude must contain one factor for entering the resonance and one factor for leaving it, so the numerator is proportional to $\sqrt{\Gamma_b\Gamma_d}$.

Equivalently,

$$
{\rm entrance\ amplitude}
\propto
V_i^*
\propto
\sqrt{\gamma_i},
\qquad
{\rm exit\ amplitude}
\propto
V_d
\propto
\sqrt{\gamma_d}.
\tag{102}
$$

Therefore

$$
{\rm resonant\ transition\ amplitude}
\propto
V_dV_i^*G_b(E)
\propto
\sqrt{\gamma_d\gamma_i}\,G_b(E).
\tag{103}
$$

This is the mathematical content of the informal statement: enter the resonance with amplitude $\sqrt{\Gamma_b}$, propagate on the resonance, and exit with amplitude $\sqrt{\Gamma_d}$.

---

## 11. Elastic channel and loss of flux

For the entrance channel itself, the $S$ matrix includes the identity contribution:

$$
S_{ii}(E)
=
1
-
2\pi i\,T_{ii}(E).
\tag{104}
$$

Here

$$
T_{ii}(E)
=
\frac{|V_i(E)|^2}{
E+h\nu-h\nu_0-S_b(E)+i\gamma_{\rm tot}/2
}.
\tag{105}
$$

Using $\gamma_i=\gamma_b=2\pi|V_i|^2$,

$$
S_{ii}(E)
=
1
-
\frac{i\gamma_b}{
E+h\nu-h\nu_0-S_b(E)+i\gamma_{\rm tot}/2
}.
\tag{106}
$$

Define

$$
\Delta_{\rm PA}(E)
=
E+h\nu-h\nu_0-S_b(E).
\tag{107}
$$

Then

$$
S_{ii}(E)
=
1
-
\frac{i\gamma_b}{
\Delta_{\rm PA}(E)+i\gamma_{\rm tot}/2
}.
\tag{108}
$$

If the entrance channel is the only open channel, then $\gamma_{\rm tot}=\gamma_b$ and

$$
S_{ii}(E)
=
\frac{
\Delta_{\rm PA}(E)-i\gamma_b/2
}{
\Delta_{\rm PA}(E)+i\gamma_b/2
}.
\tag{109}
$$

Therefore

$$
|S_{ii}(E)|^2
=
1.
\tag{110}
$$

This is elastic unitarity: when no other channels exist, the resonance changes only the phase of the outgoing entrance-channel wave, not the total flux.

If additional decay channels exist, define

$$
\gamma_{\rm loss}
=
\gamma_{\rm tot}-\gamma_b
=
\sum_{d\neq i}\gamma_d.
\tag{111}
$$

Then

$$
S_{ii}(E)
=
\frac{
\Delta_{\rm PA}(E)+i(\gamma_{\rm loss}-\gamma_b)/2
}{
\Delta_{\rm PA}(E)+i(\gamma_{\rm loss}+\gamma_b)/2
}.
\tag{112}
$$

The surviving elastic probability is

$$
|S_{ii}(E)|^2
=
\frac{
\Delta_{\rm PA}^2(E)+(\gamma_{\rm loss}-\gamma_b)^2/4
}{
\Delta_{\rm PA}^2(E)+(\gamma_{\rm loss}+\gamma_b)^2/4
}.
\tag{113}
$$

Therefore the flux missing from the entrance channel is

$$
1-|S_{ii}(E)|^2
=
\frac{
\gamma_b\gamma_{\rm loss}
}{
\Delta_{\rm PA}^2(E)+\gamma_{\rm tot}^2/4
}.
\tag{114}
$$

On the other hand, summing the inelastic transition probabilities from Eq. (100) gives

$$
\sum_{d\neq i}|S_{di}(E)|^2
=
\sum_{d\neq i}
\frac{
\gamma_b\gamma_d
}{
\Delta_{\rm PA}^2(E)+\gamma_{\rm tot}^2/4
}
=
\frac{
\gamma_b\gamma_{\rm loss}
}{
\Delta_{\rm PA}^2(E)+\gamma_{\rm tot}^2/4
}.
\tag{115}
$$

Thus

$$
1-|S_{ii}(E)|^2
=
\sum_{d\neq i}|S_{di}(E)|^2.
\tag{116}
$$

This verifies flux conservation. The resonance does not destroy probability; it redistributes outgoing flux among elastic and inelastic channels.

---

## 12. Why the cross-section is $\sigma_d(E,\ell)=\frac{\pi}{k^2}(2\ell+1)|S_d(E)|^2$

For an inelastic transition from entrance channel $i$ to a different channel $d$, the outgoing asymptotic wave in channel $d$ has scattering amplitude

$$
f_{d\leftarrow i}(\theta)
=
\frac{1}{2ik}
\sum_{\ell=0}^{\infty}
(2\ell+1)
S_{d\leftarrow i}^{(\ell)}(E)
P_\ell(\cos\theta).
\tag{117}
$$

There is no $-1$ term here because the incident wave is in channel $i$, not in channel $d$. The $-1$ term appears in elastic scattering, where the outgoing wave in the same channel must be compared with the incident plane wave.

The differential cross-section is

$$
\frac{d\sigma_d}{d\Omega}
=
|f_{d\leftarrow i}(\theta)|^2.
\tag{118}
$$

To get the integrated cross-section, use the orthogonality relation

$$
\int d\Omega\;
P_\ell(\cos\theta)P_{\ell'}(\cos\theta)
=
\frac{4\pi}{2\ell+1}\delta_{\ell\ell'}.
\tag{119}
$$

Substituting Eq. (117) into Eq. (118) and integrating gives

$$
\begin{aligned}
\sigma_d(E)
&=
\int d\Omega\;
\left|
\frac{1}{2ik}
\sum_{\ell}
(2\ell+1)
S_d^{(\ell)}(E)
P_\ell(\cos\theta)
\right|^2
\\
&=
\frac{1}{4k^2}
\sum_{\ell,\ell'}
(2\ell+1)(2\ell'+1)
S_d^{(\ell)}(E)
S_d^{(\ell')*}(E)
\int d\Omega\;
P_\ell(\cos\theta)P_{\ell'}(\cos\theta)
\\
&=
\frac{1}{4k^2}
\sum_{\ell}
(2\ell+1)^2
|S_d^{(\ell)}(E)|^2
\frac{4\pi}{2\ell+1}.
\end{aligned}
\tag{120}
$$

Therefore

$$
\sigma_d(E)
=
\frac{\pi}{k^2}
\sum_{\ell}
(2\ell+1)|S_d^{(\ell)}(E)|^2.
\tag{121}
$$

For a single partial wave,

$$
\boxed{
\sigma_d(E,\ell)
=
\frac{\pi}{k^2}
(2\ell+1)
|S_d^{(\ell)}(E)|^2.
}
\tag{122}
$$

This is the desired relation.

The factor $(2\ell+1)$ counts the magnetic substates $m=-\ell,\ldots,\ell$ when the collision is unpolarized or when the result has been averaged over incident directions. The factor $\pi/k^2$ is the natural partial-wave area scale. The quantity $|S_d^{(\ell)}|^2$ is the probability that incoming flux in partial wave $\ell$ exits in the detected channel.

---

## 13. Breit–Wigner detection cross-section

From Eq. (101),

$$
|S_{d\leftarrow E\ell}(E)|^2
=
\frac{
\hbar\Gamma_b(E,\ell)\;\hbar\Gamma_d
}{
\left[
E+h\nu-h\nu_0-S_b(E)
\right]^2
+
\left(
\hbar\Gamma_{\rm tot}/2
\right)^2
}.
\tag{123}
$$

Insert Eq. (123) into Eq. (122):

$$
\boxed{
\sigma_d(E,\ell)
=
\frac{\pi}{k^2}
(2\ell+1)
\frac{
\hbar\Gamma_d\;\hbar\Gamma_b(E,\ell)
}{
\left[
E+h\nu-h\nu_0-S_b(E)
\right]^2
+
\left(
\hbar\Gamma_{\rm tot}/2
\right)^2
}.
}
\tag{124}
$$

This is the Breit–Wigner cross-section for photoassociation into detected channel $d$.

---

## 14. Event-rate coefficient

The two-body event-rate coefficient at collision energy $E$ is the relative velocity times the event cross-section:

$$
K_d(E)
=
v_{\rm rel}\sigma_d(E).
\tag{125}
$$

Summing over partial waves gives

$$
K_d(E)
=
v_{\rm rel}
\sum_{\ell}\sigma_d(E,\ell).
\tag{126}
$$

Using Eq. (124),

$$
\boxed{
K_d(E)
=
v_{\rm rel}
\frac{\pi}{k^2}
\sum_{\ell}
(2\ell+1)
\frac{
\hbar\Gamma_d\;\hbar\Gamma_b(E,\ell)
}{
\left[
E+h\nu-h\nu_0-S_b(E)
\right]^2
+
\left(
\hbar\Gamma_{\rm tot}/2
\right)^2
}.
}
\tag{127}
$$

This is the desired Breit–Wigner photoassociation event-rate coefficient with the laser detuning explicit.

It is often useful to write it compactly in terms of the light-shifted PA detuning,

$$
\Delta_{\rm PA}(E)
=
E+h\nu-h\nu_0-S_b(E).
\tag{128}
$$

Then

$$
\boxed{
K_d(E)
=
v_{\rm rel}
\frac{\pi}{k^2}
\sum_{\ell}
(2\ell+1)
\frac{
\hbar\Gamma_d\;\hbar\Gamma_b(E,\ell)
}{
\Delta_{\rm PA}^2(E)
+
\left(
\hbar\Gamma_{\rm tot}/2
\right)^2
}.
}
\tag{129}
$$

The resonance occurs when

$$
\Delta_{\rm PA}(E)
=
0,
\tag{130}
$$

or

$$
E+h\nu
=
h\nu_0+S_b(E).
\tag{131}
$$

In the weak-field limit where the light shift is negligible, this reduces to

$$
E+h\nu
=
h\nu_0.
\tag{132}
$$

---

## 15. Unit conventions

There are two common conventions.

### Convention A: energy widths

If $\Gamma_j$ is used to mean an energy width, then

$$
\Gamma_j^{({\rm energy})}
=
2\pi |V_j(E)|^2.
\tag{133}
$$

The Breit–Wigner denominator is

$$
\left[
E+h\nu-h\nu_0-S_b(E)
\right]^2
+
\left(
\Gamma_{\rm tot}^{({\rm energy})}/2
\right)^2.
\tag{134}
$$

### Convention B: rate widths

If $\Gamma_j$ is used to mean a rate in s$^{-1}$, then

$$
\hbar\Gamma_j
=
2\pi |V_j(E)|^2.
\tag{135}
$$

The Breit–Wigner denominator is

$$
\left[
E+h\nu-h\nu_0-S_b(E)
\right]^2
+
\left(
\hbar\Gamma_{\rm tot}/2
\right)^2.
\tag{136}
$$

This note uses Convention B in the final formula, because that is the standard photoassociation form:

$$
\boxed{
K_d(E)
=
v_{\rm rel}
\frac{\pi}{k^2}
\sum_{\ell}
(2\ell+1)
\frac{
\hbar\Gamma_d\;\hbar\Gamma_b(E,\ell)
}{
\left[
E+h\nu-h\nu_0-S_b(E)
\right]^2
+
\left(
\hbar\Gamma_{\rm tot}/2
\right)^2
}.
}
\tag{137}
$$

---

## 16. Optional thermal average

For a gas at temperature $T$, the experimentally observed two-body rate coefficient is often the thermal average over collision energies:

$$
K_d(T)
=
\int_0^\infty dE\;
P_T(E)K_d(E),
\tag{138}
$$

where the Maxwell-Boltzmann relative collision-energy distribution is

$$
P_T(E)
=
\frac{2}{\sqrt{\pi}}
\frac{\sqrt{E}}{(k_B T)^{3/2}}
e^{-E/k_B T}.
\tag{139}
$$

This thermal averaging is separate from the Breit–Wigner derivation itself. The central microscopic result is still the energy-resolved coefficient in Eq. (137).

---

## 17. Summary of the logic

The derivation has four essential steps.

First, the lab-frame laser coupling is time dependent. Transforming to a frame rotating at the laser frequency shifts the excited bound-state energy from $h\nu_0$ to $h\nu_0-h\nu$. After the rotating wave approximation, the problem becomes a time-independent Fano resonance problem.

Second, the outgoing scattering eigenstate is selected by the Lippmann-Schwinger prescription

$$
\frac{1}{E-H_0+i0}.
\tag{140}
$$

This is why

$$
c(E',E)
=
\frac{V_b(E')a(E)}{E-E'+i0}.
\tag{141}
$$

The $+i0$ gives the retarded Green function, which becomes an outgoing spherical wave $e^{+ikr}/r$ in coordinate space. It also produces the imaginary part of the self-energy, hence the resonance width.

Third, the resonant transition amplitude from the entrance channel to a detected channel is

$$
S_{d\leftarrow E\ell}(E)
=
\frac{
-i\sqrt{\hbar\Gamma_b(E,\ell)}\sqrt{\hbar\Gamma_d}
}{
E+h\nu-h\nu_0-S_b(E)+i\hbar\Gamma_{\rm tot}/2
}.
\tag{142}
$$

The square roots appear because widths are probabilities per unit time, while the $S$ matrix is an amplitude. Entering the resonance contributes an amplitude proportional to $\sqrt{\Gamma_b}$, and exiting into the detected channel contributes an amplitude proportional to $\sqrt{\Gamma_d}$.

Fourth, the inelastic partial-wave cross-section is

$$
\sigma_d(E,\ell)
=
\frac{\pi}{k^2}
(2\ell+1)
|S_d^{(\ell)}(E)|^2.
\tag{143}
$$

Multiplying by $v_{\rm rel}$ and summing over $\ell$ gives the photoassociation event-rate coefficient Eq. (137).

---

## References

- U. Fano, "Effects of Configuration Interaction on Intensities and Phase Shifts," *Physical Review* **124**, 1866 (1961).
- J. L. Bohn and P. S. Julienne, "Prospects for Influencing Scattering Lengths with Far-Off-Resonant Light," *Physical Review A* **56**, 1486 (1997).
- J. L. Bohn and P. S. Julienne, "Semianalytic theory of laser-assisted resonant cold collisions," *Physical Review A* **60**, 414 (1999).
- K. M. Jones, E. Tiesinga, P. D. Lett, and P. S. Julienne, "Ultracold photoassociation spectroscopy: Long-range molecules and atomic scattering," *Reviews of Modern Physics* **78**, 483 (2006).
