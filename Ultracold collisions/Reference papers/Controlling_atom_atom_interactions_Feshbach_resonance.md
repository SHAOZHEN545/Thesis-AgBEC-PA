# Chapter 16 — Controlling atom-atom interactions

## 16.1 Introduction

In the previous chapter, we saw that collisions between ultracold atoms can be described in good approximation by a single parameter, the scattering length $a$. Depending on the sign of $a$, the effective interactions can be repulsive ($a>0$) or attractive ($a<0$). When they vanish ($a=0$) the gas behaves as an ideal gas. A very important breakthrough occurred in this field when it was realized that $a$ can be changed using a static magnetic field. The physical mechanism responsible for this variation of $a$ is the so-called Feshbach resonance that appears when, during a collision process, the two colliding atoms pass through a resonant intermediate state where they are bound. There is a certain analogy between this effect and the resonant scattering of a photon by an atom when the frequency $\omega_i$ of the incident photon is close to the frequency $\omega_A$ of an atomic transition connecting the initial state of the atom (which is generally the ground state $g$) to an excited state $e$.

It is well known[^1] that the scattering amplitude then exhibits a resonant behavior associated with an energy denominator $\omega_i-\omega_A+i(\Gamma/2)$, where $\Gamma$ is the natural width of the excited state. The Feshbach resonance is similarly associated with an energy denominator $E_{\mathrm{coll}}-E_{\mathrm{bound}}+i(\Gamma_{\mathrm{bound}}/2)$, where $E_{\mathrm{coll}}$ is the energy of the initial state of the two atoms in the collision channel and $E_{\mathrm{bound}}$ and $\Gamma_{\mathrm{bound}}$ are the energy and the width of the intermediate bound state appearing in the collision process.[^2] At very low temperatures, the scattering amplitude is proportional to the scattering length $a$. Since the magnetic moments of the two-atom system are generally not the same in the initial collision state and the intermediate bound state, $E_{\mathrm{coll}}-E_{\mathrm{bound}}$ can be tuned by varying a static magnetic field $B$. As a result, the scattering length $a$ exhibits resonant variations when $B$ is swept around values corresponding to the vanishing of $E_{\mathrm{coll}}-E_{\mathrm{bound}}$.

This chapter is devoted to a description of Feshbach resonances and of some of their applications. We first introduce the notion of collision channel in the simple case of two colliding alkali atoms (Sec. 16.2). We also describe the microscopic atom-atom interactions that give rise to the potential curves in the various channels as well as the couplings between different channels. The most rigorous way of calculating the scattering lengths is then to solve a set of coupled differential equations derived from the Schrödinger equation called coupled channel equations. The remaining part of the chapter deals with the simple case in which only two channels are involved: the “open” channel containing the initial collision state and the “closed” channel containing the intermediate resonant bound state. In Sec. 16.3, we develop the analogy with the resonant scattering of a photon by an atom in more detail by using a simple diagrammatic approach. A more precise calculation is then presented in the case of the two-channel model. In Sec. 16.4, we first calculate the scattering states of the two-channel Hamiltonian and we show that the scattering length contains a term varying as $(B-B_0)^{-1}$, where $B_0$ is the resonant value of the magnetic field.[^3] We analyze the various features of the corresponding Feshbach resonance.

Feshbach resonances are not only useful for manipulating the scattering length and for controlling atom-atom interactions, but also for producing bound states with remarkable properties. When the scattering length is positive, the two-channel Hamiltonian has a bound state whose wave function and binding energy are calculated in Sec. 16.5. In particular, we show that in the vicinity of the Feshbach resonance, this bound state has universal properties that depend only on the scattering length and not on the microscopic details of the interaction potential. By varying the static field from a region where $a$ is negative to a region where $a$ is positive one can transform a pair of two ultracold colliding atoms into an ultracold molecule. In Sec. 16.6, we briefly review various methods for converting atom pairs into molecules including optical Feshbach resonances and photoassociation.[^4]

## 16.2 Collision channels

### 16.2.1 Microscopic interactions

Let us consider two alkali atoms, ignoring in a first step the nuclear spin degrees of freedom. Figure 16.1 gives the variations with $r$ of the Born-Oppenheimer potentials that give the interaction energy of the two atoms separated by a distance $r$. There are two potential curves depending on the quantum number $S=1$ (triplet state) or $S=0$ (singlet state) of the total spin $\mathbf{S}=\mathbf{S}_1+\mathbf{S}_2$, where $\mathbf{S}_1$ and $\mathbf{S}_2$ are the spins of the valence electrons of the two atoms.

> [!figure]
> ![[Fig. 16.1.png|center|500]]
> **Figure 16.1.** Born Oppenheimer potentials of two alkali atoms versus the distance $r$ between the two atoms. The potential is not the same in the triplet state ($S=1$) and in the singlet state ($S=0$).

The antisymmetry of the wave function of the two electrons requires that for $S=1$ (symmetric spin state) the orbital wave function must be antisymmetric, and vice versa for $S=0$. It follows that, at short distances, the electrostatic repulsion is not the same in the triplet and in the singlet state. This explains the splitting of the two Born-Oppenheimer potentials. At large distance, the splitting between the two curves tends to zero since both potentials are dominated by the attractive van der Waals interaction that varies as $-1/r^6$, where $r$ is the relative distance between the two atoms. Let $P_S$ and $P_T$ be the projection operators onto the singlet and triplet manifolds. The electrostatic interaction between the two atoms can be written as

$$
V_{\mathrm{el}}(r)=V_S(r)P_S+V_T(r)P_T. \tag{16.1}
$$

Using the expressions of $P_S$ and $P_T$ in terms of $\mathbf{S}_1$ and $\mathbf{S}_2$, one gets

$$
V_{\mathrm{el}}(r)=\frac{1}{4}V_S(r)+\frac{3}{4}V_T(r)+\frac{\mathbf{S}_1\cdot\mathbf{S}_2}{2\hbar^2}\left[V_T(r)-V_S(r)\right]. \tag{16.2}
$$

This interaction depends only on the distance $r$ between the two atoms and remains invariant under a rotation of the molecular axis. It thus commutes with the relative angular momentum $\mathbf{L}$ of the two atoms and cannot connect two states with different quantum numbers $\ell$ of this angular momentum.

There are also magnetic interactions $V_{ss}$ between the two atoms that result from the dipole-dipole interactions between the two spin magnetic moments which are much smaller than $V_{\mathrm{el}}$. Contrary to $V_{\mathrm{el}}$, $V_{ss}$ depends on the relative orientation of the molecular axis and the spin direction and can connect two states with different values of $\ell$.

Finally, the total interaction Hamiltonian is equal to

$$
V^{\mathrm{int}}=V_{\mathrm{el}}+V_{ss}. \tag{16.3}
$$

### 16.2.2 Quantum numbers of the initial collision state. Collision channels

We now take into account the nuclear spins $\mathbf{I}_1$ and $\mathbf{I}_2$ of the two atoms. The interaction of these nuclear spins with the valence electrons gives rise to two hyperfine states for each atom characterized (in low magnetic fields) by quantum numbers $f_1$ and $f_2$ with magnetic sublevels $m_{f1}$ and $m_{f2}$. Consider two atoms in the states $f_1,m_{f1}$ and $f_2,m_{f2}$, respectively, undergoing a collision at very low temperature, so that one can consider only the $\ell=0$ partial wave. The initial collision state of the two ultracold atoms is thus characterized by the set of quantum numbers

$$
\alpha:\{f_1,m_{f1},f_2,m_{f2},\ell=0\} \tag{16.4}
$$

summarized by the simplified notation $\alpha$. This set of quantum numbers defines a collision channel, here the entrance channel. There are of course other channels defined by other sets $\beta$ of quantum numbers. The diagonal element of $V^{\mathrm{int}}$ in each channel provides a potential energy for each channel. But $V^{\mathrm{int}}$ also has off diagonal elements between different channels that give rise to coupled channel equations.

### 16.2.3 Coupled channel equations

The eigenstates of the total Hamiltonian with eigenvalues $E$ can be written:

$$
|\psi\rangle=\sum_{\alpha}\psi_{\alpha}(\mathbf{r})|\alpha\rangle \tag{16.5}
$$

where $\psi_{\alpha}(\mathbf{r})$ is the wave function in channel $\alpha$ whose radial part is of the form

$$
\frac{F_{\alpha}(r,E)}{r}. \tag{16.6}
$$

The coupled equations of motion of the $F_{\alpha}$’s deduced from Schrödinger equation have the following form:

$$
\frac{\partial^2}{\partial r^2}F_{\alpha}(r,E)+\frac{2\mu}{\hbar^2}\sum_{\beta}\left[E\delta_{\alpha\beta}-V_{\alpha\beta}(r)\right]F_{\beta}(r,E)=0, \tag{16.7}
$$

where

$$
V_{\alpha\beta}(r)=\left[E_{f_1,m_{f1}}+E_{f_2,m_{f2}}+\frac{\ell(\ell+1)\hbar^2}{2\mu r^2}\right]\delta_{\alpha\beta}+V^{\mathrm{int}}_{\alpha\beta}(r). \tag{16.8}
$$

Solving these coupled differential equations numerically gives the asymptotic behavior of $F_{\alpha}$ for large $r$, from which one can determine the phase shift $\delta_0$ and, consequently, the scattering length $a$ in the entrance channel.

To get more insight into Feshbach resonances, we now consider a simplified model that takes only two modes into account: that containing the entering collision state and that containing the intermediate resonant bound state.

### 16.2.4 Two-channel model

Figure 16.2 represents the two channels that are kept in the model. The colliding ultracold atoms, with a very small energy $E$, belong to the entrance collision channel, called the open channel. The other channel contains the resonant bound state $\varphi_{\mathrm{res}}$ whose energy $E_{\mathrm{res}}$ is very close to $E$. This channel is called closed because its dissociation threshold is above $E$, so that the two colliding atoms cannot belong to the continuum of this channel. By sweeping a static magnetic field, the open and the closed channel potentials move with respect to each other so that the difference between $E_{\mathrm{res}}$ and $E$ is varied.

> [!figure]
> ![[Fig. 16.2.png|center|500]]
> **Figure 16.2.** Two-channel model: open channel containing the entering collision state with a very small energy $E$; closed channel, whose threshold is larger than $E$, containing a bound state whose energy $E_{\mathrm{res}}$ is very close to $E$.

The state of the system can be written as a vector whose components refer to each channel:

$$
\begin{pmatrix}|\varphi_{\mathrm{op}}\rangle\\|\varphi_{\mathrm{cl}}\rangle\end{pmatrix} \tag{16.9}
$$

where the indices op and cl refer to the spin state in each channel. In this two-state basis, the two-channel Hamiltonian $H_2$ is represented by

$$
H_2=\begin{pmatrix}H_{\mathrm{op}} & W\\ W & H_{\mathrm{cl}}\end{pmatrix} \tag{16.10}
$$

where

$$
H_{\mathrm{op}}=T+V_{\mathrm{op}}\quad\text{and}\quad H_{\mathrm{cl}}=T+V_{\mathrm{cl}} \tag{16.11}
$$

with $T=-\hbar^2\Delta/(2\mu)$ the kinetic energy operator. In Eq. (16.11), $V_{\mathrm{op}}$ and $V_{\mathrm{cl}}$ are the interaction potential operators in the open and closed channels, respectively. $W$ describes the coupling between the two channels.

We will also neglect all eigenstates of $H_{\mathrm{cl}}$ other than $\varphi_{\mathrm{res}}$ since near the resonance ($E_{\mathrm{res}}\simeq0$), they are far from resonance and, compared to $\varphi_{\mathrm{res}}$, their contribution is negligible. In this single resonance approximation, we can thus use the following simple expression for the closed channel Hamiltonian:

$$
H_{\mathrm{cl}}=E_{\mathrm{res}}|\varphi_{\mathrm{res}}\rangle\langle\varphi_{\mathrm{res}}|. \tag{16.12}
$$

In Secs. 16.4 and 16.5, we will show that this model is sufficiently simple to allow one to diagonalize the Hamiltonian $H_2$ and to get analytical expressions for the main physical quantities of interest:

- scattering length,
- energy and wave function of the bound state of the two-channel Hamiltonian when this bound state exists.

Before doing these calculations, we first present, in the next section, a simple physical interpretation of Feshbach resonances.

## 16.3 Qualitative discussion. Analogy between Feshbach resonances and resonant light scattering

Let us first recall the elementary processes involved in the calculation of the resonant light scattering amplitude.[^5] The first diagram of Fig. 16.3 describes the lowest order scattering process. The impinging photon with wave vector $\mathbf{k}_i$ and energy $\hbar\omega_i=\hbar c k_i$ is absorbed by the atom which goes from the ground state $g$ to an excited state $e$ located at an energy $\hbar\omega_A$ above $g$. The atom then falls back to $g$ by spontaneously emitting the scattered photon $(\mathbf{k}_f,\omega_f)$. The energy mismatch in the intermediate state is $\delta E=\hbar(\omega_i-\omega_A)$, so that the corresponding virtual transition lasts a time on the order of $\hbar/|\delta E|=1/|\omega_i-\omega_A|$, that becomes longer and longer when $\omega_i$ tends to $\omega_A$. The propagator of the intermediate state of the scattering process is proportional to $1/(\omega_i-\omega_A)$. This is the origin of the resonant enhancement of the scattering amplitude.

> [!figure]
> ![[Fig. 16.3.png|center|500]]
> **Figure 16.3.** Feynman diagrams representing the resonant scattering of a photon by an atom.

The other Feynman diagrams represent higher order processes where the atom virtually emits and reabsorbs one or more photons before emitting the scattered photon $(\mathbf{k}_f,\omega_f)$. Summing the amplitudes corresponding to all these processes leads to a renormalized propagator for the excited state that is obtained by replacing its energy $\hbar\omega_A$ by $\hbar[\omega_A+\Delta_0-i(\Gamma_0/2)]$, where $\hbar\Delta_0$ and $\hbar\Gamma_0$ are the energy shift and the energy width of $e$, respectively, due to the coupling of the discrete state $e$ with the continuum of states where the atom is in $g$ in the presence of a photon. The scattering process can also take place with intermediate states $e'$ other than $e$, that are far from resonance when $\omega_i$ is close to $\omega_A$. These give rise to a non-resonant background amplitude that is nearly constant when $\omega_i$ is scanned around $\omega_A$. Finally, this analysis predicts a photon scattering amplitude of the form

$$
A(\mathbf{k}_i\to\mathbf{k}_f)=A_{\mathrm{non-resonant}}+A_{\mathrm{resonant}} \tag{16.13}
$$

where

$$
A_{\mathrm{resonant}}\propto\frac{1}{\omega_i-\omega_A-\Delta_0+i(\Gamma_0/2)}. \tag{16.14}
$$

A similar analysis can be applied to the scattering of two ultracold atoms with an intermediate bound resonant state in a closed channel (see Fig. 16.4). The first diagram at the left of this figure represents a process where the two ultracold atoms in the entrance collision state $\varphi_{\mathrm{coll}}$ combine into the bound state $\varphi_{\mathrm{res}}$ of the closed channel with energy $E_{\mathrm{res}}$ before dissociating into the final collision state. The propagator of this state varies as $1/(E-E_{\mathrm{res}})$ and is very large when $E_{\mathrm{res}}$ is close to $E$. The other diagrams of Fig. 16.4 represent higher order processes where the intermediate bound state virtually dissociates and recombines a certain number of times before undergoing the final dissociation into the final collision state.

> [!figure]
> ![[Fig. 16.4.png|center|500]]
> **Figure 16.4.** Feynman diagrams representing the resonant scattering of two ultracold atoms.

As in the previous example, one expects that the resonant scattering amplitude varies as:

$$
A_{\mathrm{resonant}}\propto\frac{1}{E-E_{\mathrm{res}}-\hbar\Delta_0+i\hbar(\Gamma_0/2)} \tag{16.15}
$$

where $\hbar\Delta_0$ and $\hbar\Gamma_0$ are the energy shift and the energy width of the bound state $\varphi_{\mathrm{res}}$, respectively, that result from the coupling of this discrete state in the closed channel to the continuum of collision states in the open channel. The new feature here is that the density of states in the continuum of collision states is very small for the energy $E$ of the initial state because the two colliding atoms are ultracold. It follows that the decay rate $\Gamma_0$ of $\varphi_{\mathrm{res}}$, which according to the Fermi golden rule, is proportional to the density of states of the continuum at an energy equal to $E_{\mathrm{res}}$, is negligible when $E_{\mathrm{res}}$ is close to $E\simeq0$. One can thus replace $\Gamma_0$ by 0 in Eq. (16.15). Finally, one expects that the scattering length $a$, which is proportional to the scattering amplitude when $E\to0$, has the form

$$
a=a_{\mathrm{non-resonant}}+a_{\mathrm{resonant}} \tag{16.16}
$$

where $a_{\mathrm{non-resonant}}$ is a background non-resonant scattering length corresponding to scattering processes without intermediate association into a bound intermediate state, and where

$$
a_{\mathrm{resonant}}\propto\frac{1}{B-B_0} \tag{16.17}
$$

where $B_0$ is the value of the static field for which $E_{\mathrm{res}}+\hbar\Delta_0=E\simeq0$. Such a prediction is confirmed by the quantitative calculations presented in the next section.

## 16.4 Scattering states of the two-channel Hamiltonian

In this section, we first calculate the eigenstates of the Hamiltonian $H_2$ with a positive energy $E$. These form a continuum of scattering states of the two atoms, taking into account the effect of the coupling $W$ between the two channels. From their asymptotic behavior when $E\to0$, we deduce the scattering length $a$ and analyze its variations with the static field.

### 16.4.1 Calculation of the dressed scattering states

Supposing that the state given by Eq. (16.9) is an eigenstate of the Hamiltonian (16.10) with an eigenvalue $E$ that leads to a system of two coupled equations:

$$
H_{\mathrm{op}}|\varphi_{\mathrm{op}}\rangle+W|\varphi_{\mathrm{cl}}\rangle=E|\varphi_{\mathrm{op}}\rangle, \tag{16.18}
$$

$$
W|\varphi_{\mathrm{op}}\rangle+H_{\mathrm{cl}}|\varphi_{\mathrm{cl}}\rangle=E|\varphi_{\mathrm{cl}}\rangle. \tag{16.19}
$$

The two components of the scattering state corresponding to an incoming state with wave vector $\mathbf{k}$ will be denoted $\varphi_{\mathrm{op}}^{\mathbf{k}}$ and $\varphi_{\mathrm{cl}}^{\mathbf{k}}$. The first equation of (16.19) can then be written:

$$
(E-H_{\mathrm{op}})|\varphi_{\mathrm{op}}^{\mathbf{k}}\rangle=W|\varphi_{\mathrm{cl}}^{\mathbf{k}}\rangle. \tag{16.20}
$$

Its solution is the sum of a solution of the equation with the right-hand side set to zero and a solution of the full equation with the right-hand side considered as a source term:

$$
|\varphi_{\mathrm{op}}^{\mathbf{k}}\rangle=|\varphi_{\mathbf{k}}^+\rangle+G_{\mathrm{op}}^+(E)W|\varphi_{\mathrm{cl}}^{\mathbf{k}}\rangle\quad\text{where}\quad G_{\mathrm{op}}^+(E)=\frac{1}{E-H_{\mathrm{op}}+i\varepsilon}. \tag{16.21}
$$

In Eq. (16.21), $G_{\mathrm{op}}^+(E)$ is a Green function of $H_{\mathrm{op}}$. The term $+i\varepsilon$, where $\varepsilon$ is a positive number that tends to zero, insures that the second term of Eq. (16.21) has the asymptotic behavior of an outgoing scattering state for $r\to\infty$. The first term of Eq. (16.21) involves only $H_{\mathrm{op}}$, and is chosen as an outgoing scattering state of $H_{\mathrm{op}}$ in order to get the good behavior for $r\to\infty$.[^6]

$$
\varphi_{\mathbf{k}}^+(\mathbf{r})=\frac{1}{(2\pi)^{3/2}}\left[e^{i\mathbf{k}\cdot\mathbf{r}}+\frac{1}{E-T+i\varepsilon}V_{\mathrm{op}}\varphi_{\mathbf{k}}^+(\mathbf{r})\right]. \tag{16.22}
$$

The second equation of (16.19) can then be written:

$$
(E-H_{\mathrm{cl}})|\varphi_{\mathrm{cl}}^{\mathbf{k}}\rangle=W|\varphi_{\mathrm{op}}^{\mathbf{k}}\rangle. \tag{16.23}
$$

Its solution can be expressed in terms of the Green function of $H_{\mathrm{cl}}$:

$$
|\varphi_{\mathrm{cl}}^{\mathbf{k}}\rangle=G_{\mathrm{cl}}(E)W|\varphi_{\mathrm{op}}^{\mathbf{k}}\rangle\quad\text{where}\quad G_{\mathrm{cl}}(E)=(E-H_{\mathrm{cl}})^{-1}. \tag{16.24}
$$

Using the single resonance approximation (16.12), one gets

$$
|\varphi_{\mathrm{cl}}^{\mathbf{k}}\rangle=|\varphi_{\mathrm{res}}\rangle\frac{\langle\varphi_{\mathrm{res}}|W|\varphi_{\mathrm{op}}^{\mathbf{k}}\rangle}{E-E_{\mathrm{res}}}. \tag{16.25}
$$

The two components $|\varphi_{\mathrm{op}}^{\mathbf{k}}\rangle$ and $|\varphi_{\mathrm{cl}}^{\mathbf{k}}\rangle$ of the scattering states of $H_2$ are sometimes called dressed states because they include the effect of the coupling $W$ between the two channels. The eigenstates $|\varphi_{\mathbf{k}}^+\rangle$ and $|\varphi_{\mathrm{res}}\rangle$ of $H_{\mathrm{op}}$ and $H_{\mathrm{cl}}$ are called bare states.

Inserting Eq. (16.25) into Eq. (16.21) gives

$$
|\varphi_{\mathrm{op}}^{\mathbf{k}}\rangle=|\varphi_{\mathbf{k}}^+\rangle+G_{\mathrm{op}}^+(E)W|\varphi_{\mathrm{res}}\rangle\frac{\langle\varphi_{\mathrm{res}}|W|\varphi_{\mathrm{op}}^{\mathbf{k}}\rangle}{E-E_{\mathrm{res}}}. \tag{16.26}
$$

In order to eliminate $|\varphi_{\mathrm{op}}^{\mathbf{k}}\rangle$ in the right-hand side, we multiply both sides of Eq. (16.21) by $\langle\varphi_{\mathrm{res}}|W$, which gives

$$
\frac{\langle\varphi_{\mathrm{res}}|W|\varphi_{\mathrm{op}}^{\mathbf{k}}\rangle}{E-E_{\mathrm{res}}}=\frac{\langle\varphi_{\mathrm{res}}|W|\varphi_{\mathbf{k}}^+\rangle}{E-E_{\mathrm{res}}-\langle\varphi_{\mathrm{res}}|WG_{\mathrm{op}}^+(E)W|\varphi_{\mathrm{res}}\rangle}. \tag{16.27}
$$

Inserting Eq. (16.27) into Eq. (16.26), we finally get

$$
|\varphi_{\mathrm{op}}^{\mathbf{k}}\rangle=|\varphi_{\mathbf{k}}^+\rangle+G_{\mathrm{op}}^+(E)\frac{W|\varphi_{\mathrm{res}}\rangle\langle\varphi_{\mathrm{res}}|W}{E-E_{\mathrm{res}}-\langle\varphi_{\mathrm{res}}|WG_{\mathrm{op}}^+(E)W|\varphi_{\mathrm{res}}\rangle}|\varphi_{\mathbf{k}}^+\rangle. \tag{16.28}
$$

Only bare states appear in the right-hand side of Eq. (16.28).

#### Connection with the two-potential scattering

Equation (16.28) can be rewritten in a more suggestive way. If we introduce the effective coupling $V_{\mathrm{eff}}$ defined by

$$
V_{\mathrm{eff}}=W\frac{|\varphi_{\mathrm{res}}\rangle\langle\varphi_{\mathrm{res}}|}{E-E_{\mathrm{res}}-\langle\varphi_{\mathrm{res}}|WG_{\mathrm{op}}^+(E)W|\varphi_{\mathrm{res}}\rangle}W \tag{16.29}
$$

we get, by inserting Eq. (16.29) into Eq. (16.28):

$$
|\varphi_{\mathrm{op}}^{\mathbf{k}}\rangle=|\varphi_{\mathbf{k}}^+\rangle+\frac{1}{E-H_{\mathrm{op}}+i\varepsilon}V_{\mathrm{eff}}|\varphi_{\mathbf{k}}^+\rangle. \tag{16.30}
$$

Like $V_{\mathrm{op}}$, $V_{\mathrm{eff}}$ acts only inside the open channel space. It describes the effect of virtual transitions to the closed channel subspace. The two-channel scattering problem can thus be reformulated in terms of a single-channel scattering problem (in the open channel) which describes the scattering produced by $V_{\mathrm{eff}}$ of waves distorted by $V_{\mathrm{op}}$ through a generalized Lippmann-Schwinger equation used in two-potential scattering problems.[^7]

In other words, the two incident particles interact with two potentials: $V_{\mathrm{op}}$ which acts in the entering channel and $V_{\mathrm{eff}}$ which accounts for the virtual transition and that corresponds to the scattering of waves distorted by the potential $V_{\mathrm{op}}$.

### 16.4.2 Existence of a resonance in the scattering amplitude

#### 16.4.2.1 Position and width of the resonance

The second term of Eq. (16.28) is the most interesting since it gives the effects that arise from the coupling $W$. Its contribution to the scattering amplitude becomes large if its denominator vanishes, i.e. if

$$
E=E_{\mathrm{res}}+\langle\varphi_{\mathrm{res}}|WG_{\mathrm{op}}^+(E)W|\varphi_{\mathrm{res}}\rangle. \tag{16.31}
$$

When $E$ is close to 0, the last term of Eq. (16.31) is equal to

$$
\langle\varphi_{\mathrm{res}}|WG_{\mathrm{op}}^+(0)W|\varphi_{\mathrm{res}}\rangle=\sum_{\mathbf{k}}\frac{|\langle\varphi_{\mathrm{res}}|W|\varphi_{\mathbf{k}}^+\rangle|^2}{-E_{\mathbf{k}}+i\varepsilon}=\hbar\Delta_0. \tag{16.32}
$$

Its interpretation is clear: it gives the shift $\hbar\Delta_0$ of $|\varphi_{\mathrm{res}}\rangle$ due to the second order coupling induced by $W$ between $|\varphi_{\mathrm{res}}\rangle$ and the continuum of $H_{\mathrm{op}}$. We thus predict that the scattering amplitude, and so the scattering length, will be maximum (in absolute value), not when $E_{\mathrm{res}}$ is close to 0, but when the shifted energy of $|\varphi_{\mathrm{res}}\rangle$

$$
\widetilde{E}_{\mathrm{res}}=E_{\mathrm{res}}+\hbar\Delta_0 \tag{16.33}
$$

is close to the energy $E\simeq0$ of the incoming state.

Strictly speaking, the Green function $G_{\mathrm{op}}^+(E)=(E-E_{\mathbf{k}}^{\mathrm{op}}+i\varepsilon)^{-1}$ appearing in Eq. (16.31) is equal to

$$
\frac{1}{E-E_{\mathbf{k}}^{\mathrm{op}}+i\varepsilon}=\mathcal{P}\left(\frac{1}{E-E_{\mathbf{k}}^{\mathrm{op}}}\right)-i\pi\delta(E-E_{\mathbf{k}}^{\mathrm{op}}) \tag{16.34}
$$

where $\mathcal{P}$ means principal part. Because of the last term of Eq. (16.34), Eq. (16.32) should also contain an imaginary term that describes the damping of $|\varphi_{\mathrm{res}}\rangle$ due to its coupling with the continuum of $H_{\mathrm{op}}$ induced by $W$. However, we are considering here the limit of ultracold collisions ($E\to0$) where the density of states of the continuum of $H_{\mathrm{op}}$ vanishes, which means that the damping of $|\varphi_{\mathrm{res}}\rangle$ can be ignored in the limit $E\to0$.

All the qualitative predictions of the previous section concerning the position and the width of the resonance of the scattering amplitude are thus confirmed.

#### 16.4.2.2 Resonant value $B_0$ of the magnetic field

Assuming that the spin configurations of the two channels have different magnetic moments, the energies of the states in these channels vary differently when a static magnetic field $B$ is applied and scanned. If $\xi$ is the difference of the magnetic moments in the two channels, the difference between the energies of two states belonging to the channels varies linearly with $B$, with a slope $\xi$. If we take the energy of the dissociation threshold of the open channel as the zero of energy, the energy $E_{\mathrm{res}}$ of $\varphi_{\mathrm{res}}$ is equal to

$$
E_{\mathrm{res}}=\xi(B-B_{\mathrm{res}}) \tag{16.35}
$$

where $B_{\mathrm{res}}$ is the magnetic field for which $E_{\mathrm{res}}$ is degenerate with the energy $E\simeq0$ of the ultracold collision state. In fact, the position of the resonance is given, not by the zero of $E_{\mathrm{res}}$, but by the zero of $\widetilde{E}_{\mathrm{res}}$:

$$
\widetilde{E}_{\mathrm{res}}=E_{\mathrm{res}}+\hbar\Delta_0=\xi(B-B_0). \tag{16.36}
$$

This equation gives the correct value of the field, $B_0$, at which one expects a divergence of the scattering amplitude. Figure 16.5 gives the variations of $E_{\mathrm{res}}$ and $\widetilde{E}_{\mathrm{res}}$ with the static magnetic field $B$. We suppose here that $\xi<0$. Since, according to Eq. (16.32), $\Delta_0$ is also negative, $B_0$ is smaller than $B_{\mathrm{res}}$.

> [!figure]
> ![[Fig. 16.5.png|center|500]]
> **Figure 16.5.** Variations of $E_{\mathrm{res}}$ and $\widetilde{E}_{\mathrm{res}}$ with the static magnetic field $B$.

### 16.4.3 Asymptotic behavior of the dressed scattering states

Only the asymptotic behavior of the open channel component of the dressed scattering state (16.28) is relevant because the closed channel component, proportional to $|\varphi_{\mathrm{res}}\rangle$, tends to zero much more rapidly. We expect the asymptotic behavior of $|\varphi_{\mathrm{op}}^{\mathbf{k}}\rangle$ to be of the form

$$
\varphi_{\mathrm{op}}^{\mathbf{k}}(\mathbf{r})\simeq_{r\to\infty}\frac{1}{(2\pi)^{3/2}}\left[e^{i\mathbf{k}\cdot\mathbf{r}}+f(k,\mathbf{n})\frac{e^{ikr}}{r}\right]\quad\text{where}\quad \mathbf{n}=\frac{\mathbf{r}}{r}. \tag{16.37}
$$

In the limit $\mathbf{k}\to0$, the scattering amplitude becomes spherically symmetric and gives the scattering length that we want to calculate:

$$
f(k,\mathbf{n})\to_{k\to0}-a. \tag{16.38}
$$

#### 16.4.3.1 Background scattering length

The first term of Eq. (16.28) describes the scattering in the open channel without coupling to the closed channel. Its asymptotic behavior gives the scattering length $a_{\mathrm{op}}$ in the open channel with $W=0$. This scattering length is often called the background scattering length:

$$
a_{\mathrm{op}}=a_{\mathrm{bg}}. \tag{16.39}
$$

#### 16.4.3.2 Effect of the inter-channel coupling on the asymptotic behavior

The second term of Eq. (16.28) describes the effect of the coupling to the closed channel. Using Eqs. (16.31) and (16.33), we can rewrite (when $E\simeq0$) Eq. (16.26) in the following way:

$$
|\varphi_{\mathrm{op}}^{\mathbf{k}}\rangle=|\varphi_{\mathbf{k}}^+\rangle+G_{\mathrm{op}}^+(E)\frac{W|\varphi_{\mathrm{res}}\rangle\langle\varphi_{\mathrm{res}}|W}{E-\widetilde{E}_{\mathrm{res}}}|\varphi_{\mathbf{k}}^+\rangle. \tag{16.40}
$$

The contribution of the inter-channel coupling to the asymptotic behavior of the dressed scattering state is given by the large $r$ dependence of the last term of this equation:

$$
\langle\mathbf{r}|G_{\mathrm{op}}^+(E)\frac{W|\varphi_{\mathrm{res}}\rangle\langle\varphi_{\mathrm{res}}|W}{E-\widetilde{E}_{\mathrm{res}}}|\varphi_{\mathbf{k}}^+\rangle=\int d^3r'\,\langle\mathbf{r}|G_{\mathrm{op}}^+(E)|\mathbf{r}'\rangle\langle\mathbf{r}'|\frac{W|\varphi_{\mathrm{res}}\rangle\langle\varphi_{\mathrm{res}}|W}{E-\widetilde{E}_{\mathrm{res}}}|\varphi_{\mathbf{k}}^+\rangle. \tag{16.41}
$$

We thus need to know the asymptotic behavior of the Green’s function of $H_{\mathrm{op}}$ for large $r$:

$$
G_{\mathrm{op}}^+(E,\mathbf{r},\mathbf{r}')=\langle\mathbf{r}|\frac{1}{E-H_{\mathrm{op}}+i\varepsilon}|\mathbf{r}'\rangle. \tag{16.42}
$$

One can show that this Green function can be expressed in terms of the incoming scattering states of $H_{\mathrm{op}}$:[^8]

$$
G_{\mathrm{op}}^+(E,\mathbf{r},\mathbf{r}')\simeq_{r\to\infty}-\frac{e^{ikr}}{r}\frac{2\mu}{\hbar^2}\sqrt{\frac{\pi}{2}}\left(\varphi_{k\mathbf{n}}^-(\mathbf{r}')\right)^*,\quad \mathbf{n}=\mathbf{r}/r \tag{16.43}
$$

where $\varphi_{k\mathbf{n}}^-$ is the incoming scattering state of $H_{\mathrm{op}}$ leading to an outgoing state $k\mathbf{n}$. Using $(\varphi_{k\mathbf{n}}^-(\mathbf{r}'))^*=\langle\varphi_{k\mathbf{n}}^-|\mathbf{r}'\rangle$ and the closure relation for $\mathbf{r}'$, we get for the asymptotic behavior of the right-hand side of Eq. (16.41):

$$
-\frac{e^{ikr}}{r}\frac{2\mu}{\hbar^2}\sqrt{\frac{\pi}{2}}\frac{\langle\varphi_{k\mathbf{n}}^-|W|\varphi_{\mathrm{res}}\rangle\langle\varphi_{\mathrm{res}}|W|\varphi_{\mathbf{k}}^+\rangle}{E-\widetilde{E}_{\mathrm{res}}}. \tag{16.44}
$$

In the limit $k\to0$, this expression can be written:

$$
-\frac{1}{r}\frac{2\mu}{\hbar^2}\sqrt{\frac{\pi}{2}}\frac{|\langle\varphi_0^+|W|\varphi_{\mathrm{res}}\rangle|^2}{0-\widetilde{E}_{\mathrm{res}}}=+\frac{1}{r}\frac{2\mu}{\hbar^2}2\pi^2\frac{|\langle\varphi_0^+|W|\varphi_{\mathrm{res}}\rangle|^2}{\xi(B-B_0)}. \tag{16.45}
$$

### 16.4.4 Scattering length. Feshbach resonance

The asymptotic behavior of the first term of Eq. (16.28) gives the background scattering length. We must now add the contribution of the second term we have just calculated in Eq. (16.45). To get the asymptotic behavior of the scattering amplitude $f(k,\mathbf{n})$ appearing in Eq. (16.37), we have to multiply (16.45) by $(2\pi)^{3/2}$ because of the normalization coefficient $(2\pi)^{-3/2}$ in Eq. (16.37). We thus get for the total scattering length:

$$
a=a_{\mathrm{bg}}-\frac{2\mu}{\hbar^2}2\pi^2\frac{|\langle\varphi_{\mathbf{0}}^+|W|\varphi_{\mathrm{res}}\rangle|^2}{\xi(B-B_0)}=a_{\mathrm{bg}}\left(1-\frac{\Delta B}{B-B_0}\right) \tag{16.46}
$$

where

$$
\Delta B=\frac{2\mu}{\hbar^2}2\pi^2\frac{|\langle\varphi_{\mathbf{0}}^+|W|\varphi_{\mathrm{res}}\rangle|^2}{\xi a_{\mathrm{bg}}}. \tag{16.47}
$$

The simple expression (16.46) of the variation of $a$ with $B$ was given in [Moerdijk et al. (1995)].

As predicted from the simple discussion of Sec. 16.3, we find that in the two-channel model the scattering length is a sum of two terms: one background term which does not vary around $B_0$, and another term that varies as $1/(B-B_0)$. The variations of the scattering length with the static field are represented in Fig. 16.6. They clearly exhibit the main results derived in this chapter:

- The scattering length diverges when $B=B_0$.
- Its sign changes when $B$ is scanned around $B_0$.
- It vanishes when $B-B_0=\Delta B$.

> [!figure]
> ![[Fig. 16.6.png|center|500]]
> **Figure 16.6.** Variations of the scattering length $a$ with the magnetic field $B$. The figure corresponds to two colliding rubidium-85 atoms each in the state $f=2$, $m_f=-2$. In this case, we have $a_{\mathrm{bg}}<0$ and $\xi<0$.

It is also evident in Fig. 16.6 that the width of the Feshbach resonance is related to the quantity $\Delta B$. The larger $\Delta B$, the broader the resonance. According to Eq. (16.47), $\Delta B$ is proportional to the square of the modulus of the matrix element of the coupling $W$ between the discrete state and the continuum and inversely proportional to the background scattering length.

The first experiment reporting the observation of Feshbach resonances with clouds of cold atoms was done at MIT in the group of Wolfgang Ketterle [Inouye et al. (1998)]. The experiment was performed on a Bose-Einstein condensate of sodium atoms confined in a dipole trap. A uniform external magnetic field was varied in the range where the theoretical prediction of the resonance position was made. The dispersive variation of the scattering length, by a factor over ten, was observed by measuring the interaction energy of the condensate through a time-of-flight experiment. In addition, enhanced inelastic processes that resulted in trap loss were observed in the vicinity of the resonance.[^9] Soon after, a Feshbach resonance of rubidium-85 atoms was observed by Zeeman-resolved photoassociation spectroscopy [Courteille et al. (1998)], and by a dramatic increase of the collision rate in the vicinity of the resonance [Roberts et al. (1998)].

## 16.5 Bound states of the two-channel Hamiltonian

In this section, we show that the two-channel Hamiltonian has a single bound state when the static magnetic field $B$ has a value corresponding to a positive scattering length. We study the $B$-dependence of the energy and wave function of this bound state. In the following, we denote such a bound state as

$$
\begin{pmatrix}|\varphi_{\mathrm{op}}^b\rangle\\|\varphi_{\mathrm{cl}}^b\rangle\end{pmatrix}, \tag{16.48}
$$

where $|\varphi_{\mathrm{op}}^b\rangle$ and $|\varphi_{\mathrm{cl}}^b\rangle$ are the components of the bound state in the open and closed channels, respectively. Expressing that the state (16.48) is an eigenstate of the Hamiltonian (16.10) with eigenvalue $E_b$, we get the following two equations:

$$
H_{\mathrm{op}}|\varphi_{\mathrm{op}}^b\rangle+W|\varphi_{\mathrm{cl}}^b\rangle=E_b|\varphi_{\mathrm{op}}^b\rangle, \tag{16.49}
$$

$$
W|\varphi_{\mathrm{op}}^b\rangle+H_{\mathrm{cl}}|\varphi_{\mathrm{cl}}^b\rangle=E_b|\varphi_{\mathrm{cl}}^b\rangle. \tag{16.50}
$$

### 16.5.1 Calculation of the energy of the bound state

To solve the set of Eqs. (16.50), we can use the Green’s function of $H_{\mathrm{op}}$ and $H_{\mathrm{cl}}$ without the $i\varepsilon$ term, since $E_b$ is negative (below the threshold of $V_{\mathrm{op}}$). This gives:

$$
|\varphi_{\mathrm{op}}^b\rangle=G_{\mathrm{op}}(E_b)W|\varphi_{\mathrm{cl}}^b\rangle\quad\text{and}\quad |\varphi_{\mathrm{cl}}^b\rangle=G_{\mathrm{cl}}(E_b)W|\varphi_{\mathrm{op}}^b\rangle. \tag{16.51}
$$

Using the single resonance approximation for $G_{\mathrm{cl}}$

$$
G_{\mathrm{cl}}(E_b)=\frac{|\varphi_{\mathrm{res}}\rangle\langle\varphi_{\mathrm{res}}|}{E_b-E_{\mathrm{res}}} \tag{16.52}
$$

in the second equation of (16.51) shows that $|\varphi_{\mathrm{cl}}^b\rangle$ is proportional to $|\varphi_{\mathrm{res}}\rangle$, so that

$$
\begin{pmatrix}|\varphi_{\mathrm{op}}^b\rangle\\|\varphi_{\mathrm{cl}}^b\rangle\end{pmatrix}=\frac{1}{N_b}\begin{pmatrix}G_{\mathrm{op}}(E_b)W|\varphi_{\mathrm{res}}\rangle\\|\varphi_{\mathrm{res}}\rangle\end{pmatrix} \tag{16.53}
$$

where $N_b$ is a normalization factor given by

$$
N_b=\sqrt{1+\langle\varphi_{\mathrm{res}}|WG_{\mathrm{op}}^2(E_b)W|\varphi_{\mathrm{res}}\rangle}. \tag{16.54}
$$

From Eqs. (16.51) and (16.52) and the results of the previous section, one can derive an implicit equation for $E_b$:

$$
E_b=\widetilde{E}_{\mathrm{res}}-(2\mu)^2E_b\int d^3k\,\frac{|\langle\varphi_{\mathrm{res}}|W|\varphi_{\mathbf{k}}^+\rangle|^2}{\hbar^2k^2(\hbar^2k^2+2\mu|E_b|)}. \tag{16.55}
$$

#### Demonstration of Eq. (16.55)

Inserting Eq. (16.52) into the second equation of (16.51) gives

$$
|\varphi_{\mathrm{cl}}^b\rangle=\frac{1}{E_b-E_{\mathrm{res}}}|\varphi_{\mathrm{res}}\rangle\langle\varphi_{\mathrm{res}}|W|\varphi_{\mathrm{op}}^b\rangle, \tag{16.56}
$$

which, inserted into Eq. (16.49) leads to

$$
|\varphi_{\mathrm{op}}^b\rangle=\frac{1}{E_b-E_{\mathrm{res}}}G_{\mathrm{op}}(E_b)W|\varphi_{\mathrm{res}}\rangle\langle\varphi_{\mathrm{res}}|W|\varphi_{\mathrm{op}}^b\rangle. \tag{16.57}
$$

As for Eq. (16.26), we can eliminate the dressed state $|\varphi_{\mathrm{op}}^b\rangle$ by multiplying both sides of Eq. (16.57) by $\langle\varphi_{\mathrm{res}}|W$. This gives

$$
E_b-E_{\mathrm{res}}=\langle\varphi_{\mathrm{res}}|WG_{\mathrm{op}}(E_b)W|\varphi_{\mathrm{res}}\rangle. \tag{16.58}
$$

Using the identity

$$
G_{\mathrm{op}}(E_b)=G_{\mathrm{op}}(0)-E_bG_{\mathrm{op}}(0)G_{\mathrm{op}}(E_b). \tag{16.59}
$$

we can rewrite (16.58) as

$$
E_b=E_{\mathrm{res}}+\langle\varphi_{\mathrm{res}}|WG_{\mathrm{op}}(0)W|\varphi_{\mathrm{res}}\rangle-E_b\langle\varphi_{\mathrm{res}}|WG_{\mathrm{op}}(0)G_{\mathrm{op}}(E_b)W|\varphi_{\mathrm{res}}\rangle. \tag{16.60}
$$

The second term of the right-hand side of Eq. (16.60) is the shift $\hbar\Delta_0$ of $\varphi_{\mathrm{res}}$. Adding it to $E_{\mathrm{res}}$, we get $\widetilde{E}_{\mathrm{res}}$, so that Eq. (16.60) can be rewritten:

$$
E_b=\widetilde{E}_{\mathrm{res}}-E_b\langle\varphi_{\mathrm{res}}|WG_{\mathrm{op}}(0)G_{\mathrm{op}}(E_b)W|\varphi_{\mathrm{res}}\rangle. \tag{16.61}
$$

To go further, we introduce the spectral decomposition of $G_{\mathrm{op}}(z)$:

$$
G_{\mathrm{op}}(z)=\int d^3k\,\frac{|\varphi_{\mathbf{k}}^+\rangle\langle\varphi_{\mathbf{k}}^+|}{z-\hbar^2k^2/(2\mu)}+G_{\mathrm{op}}^b(z). \tag{16.62}
$$

The last term of Eq. (16.62) gives the contribution of the bound states of $H_{\mathrm{op}}$. We suppose here that their energy is far below $E=0$, so that we can ignore this term. Inserting Eq. (16.62) into Eq. (16.61) finally leads to Eq. (16.55).

We now try to solve the implicit Eq. (16.55). We first note that $E_b$ is negative, so that the right-hand side of Eq. (16.55) is larger than $\widetilde{E}_{\mathrm{res}}$. Therefore, a negative solution of (16.55) for $E_b$ only exists if $\widetilde{E}_{\mathrm{res}}<0$. According to Fig. 16.5, this is possible only if $B>B_0$, which corresponds to a positive scattering length. There is no bound state for the two-channel Hamiltonian when $a<0$.

To calculate the integral of Eq. (16.55), we introduce the new variable:

$$
u=\frac{\hbar k}{\sqrt{2\mu|E_b|}} \tag{16.63}
$$

which allows one to rewrite, after angular integration, the integral of Eq. (16.55) as

$$
\frac{1}{\hbar^3}\frac{4\pi}{\sqrt{2\mu|E_b|}}\int_0^\infty du\,\frac{|\langle\varphi_{\mathrm{res}}|W|\varphi_{\mathbf{k}}^+\rangle|^2}{u^2+1}. \tag{16.64}
$$

Let $k_0$ be the width of $|\langle\varphi_{\mathrm{res}}|W|\varphi_{\mathbf{k}}^+\rangle|^2$ considered as a function of $k$. This defines a value $u_0$ of $u$,

$$
u_0=\frac{\hbar k_0}{\sqrt{2\mu|E_b|}} \tag{16.65}
$$

that characterizes the width in $u$ of the numerator of the integrand of Eq. (16.64). Two different limits can then be considered depending on whether $u_0$ is much larger or much smaller than 1.

#### First limit: $u_0\gg1\Leftrightarrow |E_b|\ll\hbar^2k_0^2/2\mu$

The denominator of the integral of Eq. (16.64) varies more rapidly with $u$ than the numerator which can be replaced by its value for $\mathbf{k}=\mathbf{0}$. Equation (16.64) can thus be approximated by

$$
\frac{1}{\hbar^3}\frac{4\pi}{\sqrt{2\mu|E_b|}}|\langle\varphi_{\mathrm{res}}|W|\varphi_{\mathbf{0}}^+\rangle|^2\underbrace{\int_0^\infty\frac{du}{u^2+1}}_{=\pi/2}. \tag{16.66}
$$

Replacing the integral of Eq. (16.55) by Eq. (16.66) yields

$$
E_b=\widetilde{E}_{\mathrm{res}}+\sqrt{|E_b|}\frac{2\pi^2(2\mu)^{3/2}}{\hbar^3}|\langle\varphi_{\mathrm{res}}|W|\varphi_{\mathbf{0}}^+\rangle|^2. \tag{16.67}
$$

We can re-express $|\langle\varphi_{\mathrm{res}}|W|\varphi_0^+\rangle|^2$ in terms of $\Delta B$ thanks to (16.47) and $\widetilde{E}_{\mathrm{res}}<0$ in terms of $\xi(B-B_0)$ thanks to Eq. (16.36). When $B$ is larger but close to $B_0$, one can neglect the left-hand side of Eq. (16.67), and obtain an approximate value for $E_b$:

$$
E_b\simeq-\frac{\hbar^2}{2\mu a^2}\propto(B-B_0)^2. \tag{16.68}
$$

#### Second limit: $u_0\ll1\Leftrightarrow |E_b|\gg\hbar^2k_0^2/2\mu$

The numerator of the integral of Eq. (16.64) varies more rapidly with $u$ than the denominator, so that we can neglect the term in $u^2$ in the denominator. In fact, this approximation amounts to neglecting $\hbar^2k^2$ compared to $2\mu|E_b|$ in the denominator of the integral of Eq. (16.55) and allows us to transform Eq. (16.55) into

$$
\begin{aligned}
E_b&=\widetilde{E}_{\mathrm{res}}+(2\mu)^2\int d^3k\,\frac{|\langle\varphi_{\mathrm{res}}|W|\varphi_{\mathbf{k}}^+\rangle|^2}{2\mu\hbar^2k^2}\\
&=\widetilde{E}_{\mathrm{res}}+\int d^3k\,\frac{|\langle\varphi_{\mathrm{res}}|W|\varphi_{\mathbf{k}}^+\rangle|^2}{\hbar^2k^2/(2\mu)}\\
&=\widetilde{E}_{\mathrm{res}}-\hbar\Delta_0=E_{\mathrm{res}}=\xi(B-B_{\mathrm{res}}).
\end{aligned} \tag{16.69}
$$

We have used the expression (16.32) of $\hbar\Delta_0$ and Eq. (16.35).

The results of this calculation are summarized in Fig. 16.7. The two-channel Hamiltonian has no bound state when $\widetilde{E}_{\mathrm{res}}>0$. This is easy to understand. When the bound state of the open channel, shifted by its coupling with the continuum of the open channel, has a shifted energy $\widetilde{E}_{\mathrm{res}}$ which is still positive, it remains resonantly coupled to the continuum and can decay into this continuum, so that it is no longer a discrete state but a metastable one. From Eqs. (16.36), (16.46) and (16.47), it is easy to check that condition $\widetilde{E}_{\mathrm{res}}>0$ is equivalent to $a>0$ and to $B-B_0>0$ ($<0$) when $\xi<0$ ($>0$).

When $B-B_0$ is very small compared to $B_{\mathrm{res}}-B_0$, $|E_b|$ increases quadratically with $B-B_0$. When $E_{\mathrm{res}}\to-\infty$, the coupling of the bound state of the closed channel to the continuum of the open channel becomes negligible and the bound state of the two-channel Hamiltonian coincides with the bound state of the open channel, so that $E_b$ coincides with $E_{\mathrm{res}}$.

> [!figure]
> ![[Fig. 16.7.png|center|500]]
> **Figure 16.7.** Energy $E_b$ of the bound state of the two-channel Hamiltonian versus the magnetic field $B$. As in Fig. 16.5, we suppose here that $\xi<0$. The bound state only exists for $\widetilde{E}_{\mathrm{res}}<0$, which is equivalent to $B>B_0$ when $\xi$ is negative (and also to $a>0$ for all signs of $\xi$). After a quadratic increase of $|E_b|$ with $B-B_0$, $E_b$ tends to the unshifted energy $E_{\mathrm{res}}$ of the bound state of the closed channel.

### 16.5.2 Wave function of the bound state

From Eqs. (16.53) and (16.54), it is possible to calculate the relative weight of the closed channel component $\varphi_{\mathrm{cl}}^b$ in the (normalized) bound state wave function of the Hamiltonian $H_2$. One gets

$$
\langle\varphi_{\mathrm{cl}}^b|\varphi_{\mathrm{cl}}^b\rangle=\frac{1}{N_b^2}\quad\text{with}\quad N_b^2=1+\langle\varphi_{\mathrm{res}}|WG_{\mathrm{op}}^2(E_b)W|\varphi_{\mathrm{res}}\rangle. \tag{16.70}
$$

Using

$$
G_{\mathrm{op}}(E_b)=\frac{1}{E_b-H_{\mathrm{op}}}\Rightarrow \frac{\partial}{\partial E_b}G_{\mathrm{op}}(E_b)=-\frac{1}{(E_b-H_{\mathrm{op}})^2}=-G_{\mathrm{op}}^2(E_b). \tag{16.71}
$$

we can rewrite the second equation of (16.70) as

$$
N_b^2=1-\frac{\partial}{\partial E_b}\langle\varphi_{\mathrm{res}}|WG_{\mathrm{op}}(E_b)W|\varphi_{\mathrm{res}}\rangle. \tag{16.72}
$$

Combining this equation with Eqs. (16.35) and (16.58), we find for the normalization coefficient $N_b$ the simple expression

$$
\frac{1}{N_b^2}=\frac{1}{\xi}\frac{\partial E_b}{\partial B}. \tag{16.73}
$$

This result can be expressed in simple terms. For a given value of $B$, the weight of the closed channel component in the wave function of the dressed bound state is just given by the slope of the curve giving $E_b(B)$ versus $B$, divided by the slope $\xi$ of the asymptote of this curve (see Fig. 16.7). When the bound state of the two-channel Hamiltonian appears near $B=B_0$ in the region $a>0$, the slope of the curve $E_b(B)$ is equal to 0 and the weight of the closed channel component in its wave function is negligible. The dressed bound state is essentially a linear combination of states of the continuum of $H_{\mathrm{op}}$. For larger values of $B$, near the asymptote of $E_b(B)$, this weight tends to 1 and the dressed bound state coincides with the bare one.

The previous conclusion means that, near the Feshbach resonance, the coupling with the closed channel can be neglected for calculating the wave function of the bound state and that we can thus look for the eigenfunction of $H_{\mathrm{op}}$ with an eigenvalue $-\hbar^2/(2\mu a^2)$. The asymptotic behavior of this wave function (at distances larger than the range of $V_{\mathrm{op}}$) can be obtained by solving the one-dimensional radial Schrödinger equation for $u_0(r)$ with $V_{\mathrm{op}}=0$:

$$
-\frac{\hbar^2}{2\mu}\frac{d^2u_0(r)}{dr^2}=-\frac{\hbar^2}{2\mu a^2}u_0(r). \tag{16.74}
$$

The three-dimensional wave function of the dressed bound state thus behaves asymptotically as

$$
\frac{\exp(-r/a)}{r}. \tag{16.75}
$$

Its spatial extent is given by the scattering length $a$.

### 16.5.3 Halo states

Equations (16.68) and (16.75) show that near the Feshbach resonance the properties of the bound state are universal: its wave function and its energy depend only on a single quantity, the scattering length $a$, and not on the details of the interaction potential giving rise to this scattering length. Near the Feshbach resonance, $a$ is much larger than the range of the atom-atom interaction potential, and the wave function of the Feshbach molecule (also referred to as Feshbach dimer) extends far into the classically forbidden region. These giant molecules are also called halo states. Examples of halo states are found in other fields, like the deuteron in nuclear physics and the helium molecules.[^10] Feshbach dimers are particularly interesting because one can change their size by just sweeping a magnetic field.

#### Efimov states

Quantum halo states also exist for three body systems. In 1970, Vitaly Efimov predicted the existence of giant bound states of three identical bosons [Efimov (1970, 1971)]. After this theoretical prediction, a long period of more than three decades elapsed before homonuclear Efimov trimers were experimentally observed in ultracold cesium, potassium and lithium atoms [Kraemer et al. (2006); Zaccanti et al. (2009); Gross et al. (2009); Pollack et al. (2009)]. Figure 16.8 reproduces the energy of these trimers $T$ versus the inverse of the scattering length $1/a$ (green curves of the figure). There are an infinite series of such curves. Two successive Efimov states appear at values of $a$ differing by a universal scaling factor $x$ equal to 22.7 (the figure is not at scale). Their binding energies differ by $x^2$. In the region $a<0$, there are no bound states.

> [!figure]
> ![[Fig. 16.8.png|center|500]]
> **Figure 16.8.** Energy of the Efimov trimer states versus the inverse of the scattering length (green curves). A series of families of states associated with the different green curves is predicted with a scaling factor $x=22.7$ for the relative sizes of two successive trimers and $x^2$ for their binding energies. The heavy black line in the right part of the figure is the energy of the dimer predicted to exist for $a>0$. Figure adapted from [Ferlaino and Grimm (2010)]. Copyright: American Physical Society.

Efimov states were detected as resonances in the three-body decay rates near a Feshbach resonance. Suppose that $|a|$ is slowly decreased in the region $a<0$. When $a$ reaches the value corresponding to the abscissa of the starting point of the lowest green curve of Fig. 16.8, three atoms $A$ can combine and form an Efimov trimer:

$$
A+A+A\to T.
$$

This opens decay channels into deeply bound dimer states and appears as resonant enhancement of the atom loss near the resonant value of $a$. Note that we have already shown that there are no dimers $D$ corresponding to a bound state of two atoms $A$ in the region $a<0$. There are, however, Efimov trimers. This is why these Efimov states are sometimes called Borromean states since they can stay together without any two-body binding.

In the region $a>0$, the heavy black line represents the energy of the dimers discussed in Sec. 16.5. The lowest green curve intersects this heavy black line for a certain value of $a$. If $a$ is decreased in the region $a>0$ and reaches this value, a dimer $D$ can combine with an atom $A$ and form a trimer $T$:

$$
D+A\to T.
$$

This results in resonant atom-dimer relaxation loss rates and can be used to detect the right end of the trimer curve.

More recently, the next family of Efimov states (second green curve of Fig. 16.8) has been detected in ultracold potassium atoms [Zaccanti et al. (2009)]. The sizes of the trimers of the two first families have been found to scale with the expected factor $x=22.7$. Interspecies trimers KRbRb and KKRb formed with potassium and rubidium atoms have also been observed [Barontini et al. (2009)].

## 16.6 Producing ultracold molecules

A great amount of attention is presently being paid to the production of ultracold molecules because important developments are expected in this research field, in fundamental and applied physics as well as in quantum chemistry. In this chapter, we will not review all these developments[^11] though a few of them will be described in subsequent chapters, in connection with the study of quantum degenerate gases. Our main concern in this chapter, devoted to the control of atom-atom interactions, is to show how ultracold molecules can be produced from ultracold atoms by controlling their interactions with a magnetic field (magnetic tuning of a Feshbach resonance) or an optical field (photoassociation).

### 16.6.1 Magnetic tuning of a Feshbach resonance

The principle of this method is shown in Fig. 16.9. If the magnetic field $B$ is slowly swept through the Feshbach resonance from the region $a<0$ to the region $a>0$, the system of the two ultracold atoms, initially in a very low energy state, remains adiabatically in the lowest energy state, which, in the region $a>0$, becomes the molecular bound state studied in the previous section.[^12]

> [!figure]
> ![[Fig. 16.9.png|center|500]]
> **Figure 16.9.** If the magnetic field $B$ is swept slowly through the Feshbach resonance from the region $a<0$ to the region $a>0$, a pair of two ultracold atoms is transformed into an ultracold molecule.

Once they are formed, these Feshbach molecules, with a spatial extent on the order of $a$, can undergo three-body inelastic collisions with the background ultracold gas which transfer them to deep molecular bound states with a spatial extent on the order of the potential range, $b\ll a$. The released energy in this process is shared between the molecules and the remaining atom.

It turns out that Feshbach molecules formed from two fermionic atoms in two different spin states are much less sensitive to these inelastic processes than those formed with bosonic atoms. Such a difference comes from the Pauli principle. In a collision between a Feshbach molecule formed from two fermions in different spin states and a fermionic atom from the background ultracold gas, two of the three fermions are necessarily in the same spin state. The inelastic collision rate is actually determined by the probability to have these three fermions in the volume $b^3$ associated with the deeply bound molecular state. Pauli principle dramatically reduces this probability because it forbids two identical fermions to be close enough to one another. As a result, the inelastic collision rate is reduced by a factor proportional to a power of $b/a\ll1$ [Petrov et al. (2005)].

We will see in Chap. 26 that this method of sweeping the magnetic field from a region where $a<0$ to a region where $a>0$ has been extensively used to produce ultracold molecules from an ultracold sample of a two-component atomic Fermi gas. A sufficiently large number of such molecules can be formed, to reach the threshold for Bose-Einstein condensation of the molecules (that obey the bosonic statistics since they are made of an even number of fermions).

Generally, their binding energy is very weak and they are well above the ground state of the molecular potential curve of the open channel, though STIRAP techniques[^13] can be applied to transfer them with a very high efficiency to this ground state. The JILA group has recently been able to produce a high phase-space density of polar KRb molecules in the rovibrational ground state [Ni et al. (2008)]. Polar molecules are very interesting because their electric dipole-dipole interactions are anisotropic and have a long range [Lahaye et al. (2009)].

#### Other methods for producing Feshbach molecules

These methods consist of starting with cold atoms in the $a>0$ region and inducing transition between the scattering states of two atoms and the weakly bound state. To ensure conservation of energy and momentum a third partner is required. It can be:

- either a photon from a resonant electromagnetic field which stimulates the transition [Thompson et al. (2005); Gaebler et al. (2007); Papp and Wieman (2006); Weber et al. (2008)];
- or another atom participating in the three-body inelastic process which preferentially populates the least bound state [Jochim et al. (2003b); Zwierlein et al. (2003)].

### 16.6.2 Photoassociation of ultracold atoms

The simplest photoassociation process, represented in Fig. 16.10(a), puts the pair of atoms $A+A$ into a bound molecular state of an excited electronic potential $A+A^*$ by absorption of a photon $\omega_1$. The transition considered here connects a state of the continuum of the entrance channel to a discrete state of another excited potential. The energy distribution of the pair of atoms depends on the temperature and has a certain width. Consequently the width of the absorption line when $\omega_1$ is scanned is in general larger than for a transition between two discrete states. With ultracold atoms, however, the width of the energy distribution of the initial collision state is very small and the broadening of the photo-absorption spectrum is negligible.

> [!figure]
> ![[Fig. 16.10.png|center|500]]
> **Figure 16.10.** (a) one-color photoassociation. A pair of two ultracold atoms $A+A$ absorbs a photon $\omega_1$ and is put in a bound molecular state of an excited electronic potential $A+A^*$. (b) two-color photoassociation. A two-photon stimulated Raman transition (absorption of a photon $\omega_1$ and stimulated emission of a photon $\omega_2$ transfers the pair of atoms $A+A$ into a bound molecular state of the same potential $A+A$).

In general, the discrete molecular state reached after the absorption of the photon is not stable radiatively since one of the two atoms, $A^*$, is in an excited electronic state and can decay by spontaneous emission. The ultracold molecules obtained in this way thus have a short lifetime.

Ultracold molecules in the lower electronic potential, with a much longer lifetime, can be obtained in stimulated Raman processes (two-color photoassociation process represented in Fig. 16.10(b)).[^14] If the two lasers $\omega_1$ and $\omega_2$ are coherent, the configuration involved in the two-photon stimulated Raman process is a $\Lambda$-configuration that gives rise to coherent population trapping and dark states.[^15] The two atoms can be trapped in a linear superposition of a collision state and a bound molecular state. The dark resonance obtained when $\omega_1-\omega_2$ is scanned is very narrow. It allows a very precise determination of the binding energies of the molecular states in the lower electronic potential $A+A$, and in particular of the least bound state, from which one can deduce a very precise value of the scattering length. This method has been applied to measure the scattering length of two metastable helium-4 atoms in the $2^3S_1$ state with an accuracy two orders of magnitude better that all previous determinations [Moal et al. (2006)].

#### Optical Feshbach resonances

In Fig. 16.10(a), the collision state $A+A$ is coupled to a discrete state in another channel relative to the system $A+A^*$ by absorption of a photon $\omega_1$. Once put in this state, the system can come back to the initial state $A+A$ by stimulated emission of a photon $\omega_1$. This cycle absorption-stimulated emission can be repeated several times. The situation is thus similar to the one discussed in Sec. 16.3 and a resonant behavior of the scattering amplitude and scattering length is expected when $\omega_1$ is scanned around the frequency of the transition connecting the collision state to the discrete state. The corresponding resonance is called an optical Feshbach resonance and is studied theoretically in [Fedichev et al. (1996a); Bohn and Julienne (1997)].

There are important differences between magnetic and optical Feshbach resonances. First, the transition between the two states is due now, not to atom-atom interactions, but to the interaction of the pair of atoms with an external radiation field. Second, the discrete state is not only coupled to the continuum of collision states, as for magnetic Feshbach resonances, but also to other channels. The excited bound state $A+A^*$, which contains one excited atom $A^*$, can decay either radiatively or by dissociation (it is no longer coupled to a quasi zero energy continuum state where the density of states vanishes). The factor $i\Gamma_0/2$ must now be kept in Eq. (16.15).

Despite the limitations that result from the instability of the discrete state, optical Feshbach resonances have a few advantages: They can be used for diamagnetic atoms for which magnetic tuning is not available. Light fields can be switched on and off and swept more rapidly than magnetic fields. They can be also more tightly focussed, allowing different groups of atoms to be addressed selectively [Yamazaki et al. (2010)]. Optical Feshbach resonances have been experimentally observed with rubidium-87 atoms [Theis et al. (2004)]. The principle of optical coupling between the collision state and a discrete state can be extended to the two-photon Raman coupling of Fig. 16.10(b), and has been also demonstrated with rubidium-87 atoms [Thalhammer et al. (2005)].

## 16.7 Conclusion

With Feshbach resonances, an unprecedented control of ultracold atoms has been reached. Not only can atoms be cooled to very low temperatures, confined in traps with all possible geometries, but now their interactions can be changed at will by simply tuning a magnetic field. These interactions can be cancelled, their sign can be changed, and their strength can reach very high values at the center of the resonance.

In this chapter, the emphasis has been placed on the elementary collision process, though a primary interest of Feshbach resonances is that they open new exciting possibilities for investigating the fundamental behavior of quantum degenerate bosonic and fermionic gases, and for exploring new regimes with strong interactions that require descriptions beyond mean field. This explains why they play a central role in the experiments trying to simulate, with quantum gases, the behavior of more complex systems found in other fields.

Feshbach resonances are also very attractive for preparing ultracold homonuclear and heteronuclear molecules and for exploring the quantum properties of exotic few body systems like Efimov trimers. Several investigations are presently devoted to the formation of tetramers near a Feshbach resonance. These resonances are thus also very interesting for the study of few body quantum systems [Greene (2010)].

## Footnotes

[^1]: See Chap. 5.

[^2]: Feshbach resonances are an example of phenomena that arise from the resonant coupling of a discrete state to a continuum. Resonances of this type appear in nuclear and atomic physics. They have been studied by renowned physicists, like Ugo Fano and Herman Feshbach. This is why they are sometimes called Fano-Feshbach resonances (see for example [Chin et al. (2010)] and the historical remarks of section I.C of this reference).

[^3]: We will see that the width of the intermediate resonant bound state is negligible when the two colliding atoms are ultracold.

[^4]: For the quantitative analysis of Feshbach resonances, we will follow closely the presentation of [Köhler et al. (2006)]. More details can also be found in this reference concerning ultracold molecules formed by sweeping a magnetic field near a Feshbach resonance.

[^5]: For a more detailed discussion see Sec. 5.2.2 of Chap. 5.

[^6]: The factor $(2\pi)^{-3/2}$ is introduced so that the outgoing scattering states are normalized $\langle\varphi_{\mathbf{k}}^+|\varphi_{\mathbf{k}'}^+\rangle=\delta(\mathbf{k}-\mathbf{k}')$.

[^7]: See for example Chap. 17 of [Joachain (1983)].

[^8]: To demonstrate (16.43), one can use the approach detailed in Exercise 4 of Chap. XIX of Ref. [Messiah (2003)].

[^9]: Near the resonance, the duration of the collision process increases which favors inelastic output channels.

[^10]: For a review on quantum halos see [Jensen et al. (2004)] and references therein.

[^11]: We refer the interested reader to recent review papers [Heinzen (1999); Pillet et al. (2003); Carr and Ye (2009); Bell and Softley (2009); Dulieu and Gabbabini (2009)].

[^12]: For a review on ultracold Feshbach molecules, see [Köhler et al. (2006); Chin et al. (2010); Ferlaino et al. (2009)].

[^13]: See page 307 in Chap. 13.

[^14]: For a review of production of ultracold molecules by photoassociation, see Refs. [Heinzen (1999); Pillet et al. (2003)].

[^15]: See Chaps. 4 and 13.
