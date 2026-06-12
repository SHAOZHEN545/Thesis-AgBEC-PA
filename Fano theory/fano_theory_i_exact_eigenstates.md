# Fano Theory I — Hilbert-Space Decomposition, Discrete-Continuum Coupling, and Exact Eigenstates

This note introduces Fano theory as a diagonalization problem. The basic situation is that a Hamiltonian contains extended continuum sectors and localized sectors, and the exact eigenstates are neither purely continuum states nor purely discrete states. They are dressed superpositions.

The viewpoint is close to scattering theory, but the emphasis is different. In ordinary scattering theory one often begins with an incoming asymptotic channel and asks how the interaction maps it into outgoing channels. In Fano theory one instead asks how the Hamiltonian itself is diagonalized when a localized state is embedded in, or coupled to, a continuum. The familiar asymmetric Fano line shape is then not a separate phenomenological rule. It is the observable trace of this exact diagonalization.

The guiding picture is

$$
\text{bare continuum} \; + \; \text{bare localized state}
\quad \longrightarrow \quad
\text{exact continuum eigenstates with localized admixture}.
$$

This is why the same formalism appears in photoionization, autoionization, predissociation, nuclear reactions, waveguides, quantum dots, and cold-atom Feshbach resonances.

---

## 1. Why discrete-continuum coupling is natural

A localized state and a continuum state sound like different kinds of objects, but they can have the same total energy. Once that happens, nothing in quantum mechanics forbids them from mixing.

In atomic photoionization, a photon may eject an electron directly into an ionization continuum. It may also excite a localized doubly excited state which later autoionizes into the same continuum. The detector sees the same final ionized fragments, so the two histories interfere.

In molecular predissociation, a vibrational or electronic bound state may lie above a dissociation threshold. It is localized in one approximate potential curve, but it can decay into a continuum of separated fragments in another.

In cold-atom Feshbach resonances, an open scattering channel is coupled to a closed-channel bound state. Tuning a magnetic field moves the closed-channel level relative to the open-channel threshold. When the dressed level approaches threshold, the open-channel scattering changes dramatically.

The common structure is not the detailed microscopic system. It is the Hilbert-space decomposition

$$
\mathcal H
=
\mathcal H_P\oplus \mathcal H_Q,
$$

where $\mathcal H_P$ contains continuum channel states and $\mathcal H_Q$ contains localized states. The symbols $P$ and $Q$ are chosen deliberately: they are the same projectors that later appear in Feshbach projection theory.

---

## 2. Continuum and localized sectors

Let $P$ project onto a continuum sector and $Q$ project onto a localized sector:

$$
P+Q=1,
\qquad
P^2=P,
\qquad
Q^2=Q,
\qquad
PQ=0.
$$

The continuum sector may contain several channels. We write an energy-normalized continuum basis as

$$
|E,a\rangle,
$$

where $E$ is the continuum energy and $a$ is a channel label. The label $a$ may include arrangement, spin, angular-momentum, hyperfine, electronic, vibrational, rotational, or threshold data. Sums over $a$ should be read as including whatever discrete sums and continuous degeneracy integrals are needed.

The continuum resolution of identity is written schematically as

$$
P
=
\sum_a\int dE\,|E,a\rangle\langle E,a|,
$$

with

$$
\langle E',b|E,a\rangle
=
\delta_{ba}\delta(E'-E).
$$

The localized sector is spanned by states

$$
|\phi_\nu\rangle,
\qquad
Q=\sum_\nu |\phi_\nu\rangle\langle\phi_\nu|.
$$

The index $\nu$ labels the bare localized levels. These may be atomic autoionizing states, molecular bound states, cavity modes, quantum-dot levels, or closed-channel bound states.

The word bare is important. The vectors $|E,a\rangle$ and $|\phi_\nu\rangle$ are not usually exact eigenstates of the full Hamiltonian. They are eigenstates of the separated continuum and localized blocks before the two sectors are coupled.

---

## 3. The general Hamiltonian in block form

The exact Hamiltonian may be decomposed as

$$
H
=
PHP+QHQ+PHQ+QHP.
$$

In a completely general continuum basis, the matrix elements are

$$
\langle E',b|PHP|E,a\rangle
=H^{(P)}_{ba}(E',E),
$$

$$
\langle\phi_\mu|QHQ|\phi_\nu\rangle
=H^{(Q)}_{\mu\nu},
$$

and

$$
\langle E,a|PHQ|\phi_\nu\rangle
=V_{a\nu}(E).
$$

Thus $PHP$ contains continuum-continuum dynamics, $QHQ$ contains localized-state dynamics, and $PHQ+QHP$ converts localized amplitude into continuum amplitude and conversely.

For Fano theory it is useful to take one preliminary step: diagonalize the continuum block and the localized block separately. That is, choose the continuum states so that

$$
PHP|E,a\rangle=E|E,a\rangle,
$$

and choose the localized states so that

$$
QHQ|\phi_\nu\rangle=E_\nu|\phi_\nu\rangle.
$$

This does not mean continuum-continuum interactions have been ignored. It means they have been absorbed into the background continuum basis. Later, in scattering language, this background may already contain potential scattering phases. Fano theory then studies the additional effect of coupling this background continuum to localized states.

With this choice, the Hamiltonian has the form

$$
H
=
\sum_a\int dE\,E|E,a\rangle\langle E,a|
+
\sum_\nu E_\nu|\phi_\nu\rangle\langle\phi_\nu|
+
\sum_{a\nu}\int dE\,
\left[
V_{a\nu}(E)|E,a\rangle\langle\phi_\nu|
+V_{\nu a}(E)|\phi_\nu\rangle\langle E,a|
\right],
$$

where Hermiticity gives $V_{\nu a}(E)=V_{a\nu}(E)^*$.

Single-channel reduction: if there is one continuum and one localized state, this becomes

$$
H
=
\int dE\,E|E\rangle\langle E|
+E_0|\phi\rangle\langle\phi|
+
\int dE\,
\left[
V(E)|E\rangle\langle\phi|
+V(E)^*|\phi\rangle\langle E|
\right].
$$

This is the elementary Fano model.

---

## 4. Exact eigenstate ansatz

An exact stationary eigenstate of the full Hamiltonian satisfies

$$
H|\Psi_E\rangle=E|\Psi_E\rangle.
$$

Since $P+Q=1$, it can be expanded as

$$
|\Psi_E\rangle
=
\sum_a\int dE'\,A_a(E';E)|E',a\rangle
+
\sum_\nu C_\nu(E)|\phi_\nu\rangle.
$$

The coefficients $A_a(E';E)$ are continuum amplitudes, while $C_\nu(E)$ are localized amplitudes. This is not a perturbation expansion. It is simply the expansion of an exact eigenvector in the uncoupled sector basis.

Projecting the Schrödinger equation with $\langle E',a|$ gives

$$
(E-E')A_a(E';E)=\sum_\nu V_{a\nu}(E')C_\nu(E).
$$

Projecting with $\langle\phi_\mu|$ gives

$$
(E-E_\mu)C_\mu(E)
=
\sum_a\int dE'\,V_{\mu a}(E')A_a(E';E).
$$

These two equations are the algebraic core of Fano theory. The continuum equation says that localized amplitude acts as a source for continuum amplitude. The discrete equation says that the localized state is shifted and broadened by the continuum amplitude it emits and reabsorbs.

---

## 5. Principal-value solution and self-energy

The equation

$$
(E-E')A_a(E';E)
=
\sum_\nu V_{a\nu}(E')C_\nu(E)
$$

has to be interpreted as a distribution, because the denominator vanishes at $E'=E$. A scattering boundary condition would use

$$
\frac{1}{E-E'+i0}
=
\operatorname{P}\frac{1}{E-E'}-i\pi\delta(E-E').
$$

Fano's original diagonalization is often presented in a standing-wave form, where the singular part is written as a principal value plus an explicit on-shell term:

$$
A_a(E';E)
=
Z_a(E)\delta(E'-E)
+
\sum_\nu
\operatorname{P}\frac{V_{a\nu}(E')C_\nu(E)}{E-E'}.
$$

The coefficients $Z_a(E)$ represent the freedom to add a homogeneous continuum solution at the same energy. They are fixed by the remaining discrete-sector equations and by normalization.

Substituting this expression into the localized-sector equation gives

$$
(E-E_\mu)C_\mu(E)
=
\sum_a V_{\mu a}(E)Z_a(E)
+
\sum_\nu \Delta_{\mu\nu}(E)C_\nu(E),
$$

where

$$
\Delta_{\mu\nu}(E)
=
\sum_a\operatorname{P}\int dE'\,
\frac{V_{\mu a}(E')V_{a\nu}(E')}{E-E'}.
$$

The matrix $\Delta(E)$ is the continuum-induced energy shift. It is a real principal-value effect. Physically, the localized sector virtually emits into the continuum and reabsorbs from it. Even if real decay is not allowed in a given channel, virtual propagation can shift the location of a level.

If instead we impose the outgoing $+i0$ boundary prescription, the same substitution gives the complex self-energy

$$
\Sigma^{(+)}_{\mu\nu}(E)
=
\sum_a\int dE'\,
\frac{V_{\mu a}(E')V_{a\nu}(E')}{E-E'+i0}.
$$

Using the distribution identity,

$$
\Sigma^{(+)}_{\mu\nu}(E)
=
\Delta_{\mu\nu}(E)-\frac{i}{2}\Gamma_{\mu\nu}(E),
$$

with

$$
\Gamma_{\mu\nu}(E)
=
2\pi\sum_a V_{\mu a}(E)V_{a\nu}(E).
$$

The imaginary part appears only from continuum states exactly on shell. It is the continuum-induced width matrix.

For one localized state coupled to several open continua,

$$
\Delta(E)=\sum_a\operatorname{P}\int dE'\,
\frac{|V_a(E')|^2}{E-E'},
$$

and

$$
\Gamma(E)=\sum_a\Gamma_a(E),
\qquad
\Gamma_a(E)=2\pi |V_a(E)|^2.
$$

Thus a multichannel resonance has a total width $\Gamma$ and partial widths $\Gamma_a$. In the two-channel case, $\Gamma=\Gamma_1+\Gamma_2$, and the branching ratio into channel $a$ is controlled by $\Gamma_a/\Gamma$.

Single-channel reduction: for one continuum and one localized state,

$$
\Delta(E)=\operatorname{P}\int dE'\,\frac{|V(E')|^2}{E-E'},
\qquad
\Gamma(E)=2\pi |V(E)|^2.
$$

The dressed resonance energy is near the solution of

$$
E_r=E_0+\Delta(E_r),
$$

and its decay width is approximately $\Gamma(E_r)$ when the coupling varies slowly on the scale of the resonance.

---

## 6. The elementary one-discrete-state/one-continuum model

Now specialize to one continuum $|E\rangle$ and one localized state $|\phi\rangle$. Write

$$
|\Psi_E\rangle
=a(E)|\phi\rangle+
\int dE'\,b_E(E')|E'\rangle.
$$

The projected equations are

$$
(E-E_0)a(E)
=
\int dE'\,V(E')^*b_E(E'),
$$

and

$$
(E-E')b_E(E')=V(E')a(E).
$$

The standing-wave solution of the second equation is

$$
b_E(E')
=z(E)\delta(E'-E)
+a(E)\operatorname{P}\frac{V(E')}{E-E'}.
$$

Substitution into the first equation gives

$$
[E-E_0-\Delta(E)]a(E)=V(E)^*z(E).
$$

Choose the phase of $|E\rangle$ so that $V(E)$ is real near the resonance. Then

$$
z(E)=\frac{E-E_0-\Delta(E)}{V(E)}a(E).
$$

It is conventional to introduce the reduced detuning

$$
\varepsilon_F(E)
=
\frac{E-E_0-\Delta(E)}{\Gamma(E)/2}.
$$

Since $\Gamma(E)=2\pi V(E)^2$, the on-shell continuum coefficient may be written as

$$
z(E)=\pi V(E)\varepsilon_F(E)a(E).
$$

Thus, up to continuum normalization, the exact eigenstate has the form

$$
|\Psi_E\rangle
=a(E)
\left[
|\phi\rangle
+
\operatorname{P}\int dE'\,\frac{V(E')}{E-E'}|E'\rangle
+
\pi V(E)\varepsilon_F(E)|E\rangle
\right].
$$

This expression is the heart of the Fano construction. The exact state is not a bare localized state plus a small correction. It is a continuum eigenstate whose localized component becomes large near $E_0+\Delta(E)$.

The localized spectral weight has the Breit-Wigner form

$$
|a(E)|^2
\propto
\frac{\Gamma(E)}{[E-E_0-\Delta(E)]^2+[\Gamma(E)/2]^2},
$$

with the proportionality fixed by the energy normalization of $|\Psi_E\rangle$. The Lorentzian here describes the amount of localized character inside an exact continuum eigenstate. The observed line shape need not be Lorentzian, because a detector may also couple directly to the continuum part.

---

## 7. Bare states versus dressed states

The bare localized state $|\phi\rangle$ is an eigenstate of $QHQ$, not of $H$. The bare continuum state $|E,a\rangle$ is an eigenstate of $PHP$, not of $H$. Once $PHQ$ is present, neither sector is independently invariant.

A dressed state is what remains after the coupling is included. In the continuum, the dressed objects are exact energy-normalized eigenstates $|\Psi_E\rangle$. Near a resonance, each exact eigenstate contains a localized component, and the localized spectral weight is concentrated near the shifted energy $E_r$.

There is a useful but potentially misleading phrase: the discrete state decays into the continuum. Strictly speaking, after coupling to an open continuum, the bare discrete state is no longer a normalizable stationary eigenstate. Time-dependent decay is the evolution of an initially prepared bare or mostly localized packet when expanded in the exact continuum eigenstates. The width $\Gamma$ is the energy-domain imprint of that time-domain decay.

In multichannel language, the dressed localized propagator is governed by the effective $Q$-space operator

$$
H_{\mathrm{eff}}^{(+)}(E)
=
QHQ+QHP\frac{1}{E-PHP+i0}PHQ.
$$

In the localized basis,

$$
H_{\mathrm{eff}}^{(+)}(E)
=
E_\nu\delta_{\mu\nu}+\Delta_{\mu\nu}(E)-\frac{i}{2}\Gamma_{\mu\nu}(E).
$$

The resonance position and width are therefore not properties of $QHQ$ alone. They are properties of the localized sector dressed by virtual and real excursions into the continuum.

---

## 8. The origin of Fano interference

The exact eigenstate contains both a continuum component and a localized component. Therefore an external probe can reach the same final exact state in two coherent ways.

For example, let $D$ be a photon-induced transition operator from an initial bound state $|i\rangle$. Define

$$
D_a(E)=\langle E,a|D|i\rangle,
\qquad
D_\nu=\langle\phi_\nu|D|i\rangle.
$$

The transition amplitude into an exact eigenstate is

$$
M(E)=\langle\Psi_E|D|i\rangle.
$$

Using the exact eigenstate expansion, this amplitude contains a direct continuum contribution and a localized contribution. These are not probabilities to be added. They are amplitudes to the same final state, so they interfere.

In the one-continuum/one-discrete-state model, assume $D_E=\langle E|D|i\rangle$ and $V(E)$ vary slowly across the resonance. The amplitude can be written in the standard Fano form

$$
M(E)=M_{\mathrm{bg}}(E)\frac{q+\varepsilon_F}{\varepsilon_F+i},
$$

where $M_{\mathrm{bg}}(E)$ is the smooth background continuum amplitude and

$$
q
=
\frac{
D_\phi+
\operatorname{P}\int dE'\,\frac{V(E')^*D_{E'}}{E-E'}
}{
\pi V(E)^*D_E
}
$$

up to the phase convention used for continuum states.

Therefore the transition probability or cross section has the profile

$$
\frac{\sigma(E)}{\sigma_{\mathrm{bg}}(E)}
=
\frac{(q+\varepsilon_F)^2}{1+\varepsilon_F^2}.
$$

This is the familiar Fano resonance formula. Its asymmetry is not caused merely by an energy-dependent decay rate. It is caused by interference between a smooth continuum path and a resonant localized path.

Several limits are useful. If $|q|$ is large, the resonant path dominates and the profile looks almost Lorentzian. If $q=0$, the resonance appears as a dip, because the direct and resonant amplitudes cancel at $\varepsilon_F=0$. For finite $q$, the zero occurs at

$$
\varepsilon_F=-q.
$$

The line shape is therefore a phase-sensitive object. It remembers how the localized and continuum excitation amplitudes are combined in the exact eigenstate.

---

## 9. Multichannel and two-channel reductions

In a multichannel problem, the same localized state may couple to many continua. The resonance denominator is still controlled by

$$
E-E_0-\Delta(E)+\frac{i}{2}\Gamma(E),
$$

but now

$$
\Gamma(E)=\sum_a 2\pi |V_a(E)|^2.
$$

The numerator depends on how the state is prepared and which outgoing channel is observed. Thus the total resonance position and width may be common, while the observed Fano parameter can be channel dependent.

The simplest two-channel Feshbach version has one open channel $o$ and one closed sector containing a localized state $|\phi_c\rangle$. The open channel supplies asymptotic scattering states, while the closed-channel state supplies the localized level. Eliminating the closed state gives an energy-dependent open-channel interaction

$$
H_{\mathrm{eff},P}(E)
=
PHP+PHQ\frac{1}{E-QHQ}QHP.
$$

For a single closed-channel level, this produces a resonant open-channel term of the schematic form

$$
T_{\mathrm{res}}(E)
\propto
\frac{|V_o(E)|^2}{E-E_c-\Delta(E)+i\Gamma(E)/2}.
$$

This is the Feshbach resonance mechanism in its simplest form. A state that is closed-channel-like in its bare description becomes visible in the open channel because coupling dresses it with open-channel amplitude.

If there are two open continua, say $a=1,2$, then

$$
\Gamma(E)=\Gamma_1(E)+\Gamma_2(E),
\qquad
\Gamma_a(E)=2\pi |V_a(E)|^2.
$$

The resonance may be formed through channel $1$ and decay into channel $2$, or conversely. In scattering language this gives resonant contributions to both elastic and inelastic transition amplitudes. In Fano language it is the same exact eigenstate viewed through different channel projections.

---

## 10. Relation to scattering states and Lippmann--Schwinger theory

The Fano ansatz and the Lippmann--Schwinger equation are two ways of organizing the same physics.

In Lippmann--Schwinger theory, an exact scattering state is written as

$$
|\psi_\alpha^{(+)}\rangle
=
|\alpha\rangle+\frac{1}{E_\alpha-H_0+i0}V|\psi_\alpha^{(+)}\rangle.
$$

The free channel $|\alpha\rangle$ supplies the asymptotic boundary condition. The resolvent supplies the outgoing prescription.

In Fano theory, the continuum part of the exact eigenstate obeys

$$
A_a^{(+)}(E';E)
=
\chi_a\delta(E'-E)
+
\frac{1}{E-E'+i0}
\sum_\nu V_{a\nu}(E')C_\nu^{(+)}(E),
$$

where $\chi_a$ specifies the incoming or background continuum combination. This is the same structure in energy representation: a homogeneous on-shell continuum term plus a resolvent-generated response to the localized-sector source.

Feshbach projection theory makes the bridge explicit. Projecting the exact equation gives

$$
(E-PHP)P|\Psi_E\rangle=PHQ Q|\Psi_E\rangle,
$$

and

$$
(E-QHQ)Q|\Psi_E\rangle=QHP P|\Psi_E\rangle.
$$

Eliminating $P|\Psi_E\rangle$ gives an effective localized-sector equation with

$$
QHP\frac{1}{E-PHP+i0}PHQ,
$$

which is precisely the self-energy responsible for $\Delta(E)$ and $\Gamma(E)$. Eliminating $Q|\Psi_E\rangle$ instead gives an effective open-channel interaction, the natural starting point for Feshbach resonant scattering.

Thus this note prepares for scattering theory in two directions. First, it explains why an exact scattering state can contain strong closed or localized admixture. Second, it explains why resonant scattering amplitudes acquire shifted energies, widths, and interference zeros.

---

## 11. Logical summary

The Hilbert space is decomposed into continuum and localized sectors,

$$
\mathcal H=\mathcal H_P\oplus\mathcal H_Q,
\qquad
P+Q=1.
$$

After diagonalizing the uncoupled sector Hamiltonians,

$$
PHP|E,a\rangle=E|E,a\rangle,
\qquad
QHQ|\phi_\nu\rangle=E_\nu|\phi_\nu\rangle.
$$

The full Hamiltonian contains continuum-localized couplings

$$
V_{a\nu}(E)=\langle E,a|H|\phi_\nu\rangle.
$$

An exact eigenstate is expanded as

$$
|\Psi_E\rangle
=
\sum_a\int dE'\,A_a(E';E)|E',a\rangle
+
\sum_\nu C_\nu(E)|\phi_\nu\rangle.
$$

The continuum equation gives a principal-value response plus an on-shell homogeneous term,

$$
A_a(E';E)
=
Z_a(E)\delta(E'-E)
+
\sum_\nu
\operatorname{P}\frac{V_{a\nu}(E')C_\nu(E)}{E-E'}.
$$

Substitution into the localized equation produces the real energy shift

$$
\Delta_{\mu\nu}(E)
=
\sum_a\operatorname{P}\int dE'\,
\frac{V_{\mu a}(E')V_{a\nu}(E')}{E-E'},
$$

and the outgoing boundary value produces the width matrix

$$
\Gamma_{\mu\nu}(E)=2\pi\sum_a V_{\mu a}(E)V_{a\nu}(E).
$$

For one localized state and one continuum,

$$
\Delta(E)=\operatorname{P}\int dE'\,\frac{|V(E')|^2}{E-E'},
\qquad
\Gamma(E)=2\pi|V(E)|^2,
$$

and the reduced detuning is

$$
\varepsilon_F(E)=\frac{E-E_0-\Delta(E)}{\Gamma(E)/2}.
$$

A probe that can reach both the smooth continuum and the localized component observes the Fano profile

$$
\frac{\sigma(E)}{\sigma_{\mathrm{bg}}(E)}
=
\frac{(q+\varepsilon_F)^2}{1+\varepsilon_F^2}.
$$

The profile is asymmetric because it is an interference pattern between two amplitudes leading to the same exact continuum eigenstate.

This is the Fano route into resonant scattering. The next natural step is to connect these exact eigenstates to channel-resolved Lippmann--Schwinger states, transition matrices, and Feshbach projection operators.
