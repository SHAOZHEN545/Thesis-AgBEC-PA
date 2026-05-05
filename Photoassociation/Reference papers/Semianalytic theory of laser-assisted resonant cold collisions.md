---
title: "Semianalytic theory of laser-assisted resonant cold collisions"
authors:
  - John L. Bohn
  - P. S. Julienne
journal: "Physical Review A"
volume: 60
issue: 1
pages: "414-425"
year: 1999
doi: "10.1103/PhysRevA.60.414"
tags:
  - physics
  - cold-collisions
  - photoassociation
  - scattering-theory
  - quantum-defect-theory
---

# Semianalytic theory of laser-assisted resonant cold collisions

**John L. Bohn**  
JILA and Department of Physics, University of Colorado, Boulder, Colorado

**P. S. Julienne**  
Atomic Physics Division, NIST, Gaithersburg, Maryland

Received 1 February 1999

## Abstract

A general formalism is derived for analytically representing the scattering properties of ultracold atoms subject to one or more resonant photoassociation lasers. The resulting formulas cleanly separate laser intensities and detunings from overlap integrals of molecular wave functions. As a consequence, laser-induced energy shifts and line broadenings are given in an explicit form. In the case of the initial photoassociation step, these quantities are given more simply in terms of the relevant molecular potential curves and wave functions near the Condon point.

**PACS number(s):** 34.50.Rk

---

# I. Introduction

The interaction of lasers with atoms is a cornerstone in modern atomic physics. In particular, the laser cooling experiments begun over a decade ago opened up a new energy regime in atomic collisions [1]. At the sub-millikelvin temperatures encountered in cold atom traps, collisions are greatly simplified by their nearly purely $s$-wave character, yet are complicated by tiny energy scales, such as fine and hyperfine energies and optical line widths, that are of little concern at higher collision energies. In addition, effects of the Wigner threshold law become particularly prominent at these energies. These considerations have led to a rich physics of ultracold atoms [2]. More recent advances have yielded optical techniques that can produce even microkelvin temperatures [3], though they have yet to achieve densities sufficiently high to produce Bose-Einstein condensation.

Lasers also make effective probes of cold atoms, as well as tools for their manipulation. Thus a number of spectroscopic studies have been performed in cold atoms, namely, atomic spectroscopy of very narrow lines [4], as well as molecular spectroscopy of very delicate vibrational levels that would not exist outside the cold trap environment [5]. The latter, photoassociation (PA) spectroscopy [6], yields asymmetric line shapes whose understanding requires accounting for the near-threshold behavior of atomic scattering in the presence of the laser field. Line-shape formulas have been suggested previously for one- [7] and two-color [8] PA spectra.

In addition, laser light has been variously suggested as an implement for catalyzing the production of cold molecules [9-12] or for cooling the molecules directly [13]. In these scenarios multiple lasers must be considered, either to make more favorable Franck-Condon overlaps [9,10] or to serve as repumping light [13]. Other proposals have suggested laser-light manipulation of the effective interatomic interactions, embodied in $s$-wave scattering lengths [14,15]. These approaches should make an even richer array of Bose-Einstein condensates than occur naturally.

Most of these phenomena have one thing in common, namely, the resonant excitation of a pair of free atoms into one or more quasibound molecular states. For the above applications, and for others yet unseen, we derive in this paper a general formalism for resonant scattering of cold atoms in a light field. Our approach will yield analytic formulas for resonance line shapes that clearly separate their dependence on laser intensities and detunings from those on Franck-Condon factors (FCF's) and related quantities. In this way the results will be transparent and easily evaluated even when considering the many parameters involved in a multiple-laser experiment. In addition, the influence of the Wigner laws will be manifest in these formulas.

Our approach will exploit the ideas of a quantum-defect approach to atomic scattering theory [16]. Namely, we will first waive the requirement that wave functions in bound state channels be finite in the limit of large interatomic separation $R$. Then the same perturbative expressions for scattering amplitudes will apply to all channel couplings, i.e., free-bound and bound-bound transitions, as well as spontaneous emission, are handled on an equal footing. Then, in a second step, we will "close" the bound-state channels, by requiring that their wave functions vanish at infinite atomic separation. There will then emerge simple algebraic procedures for constructing the relevant scattering probabilities from Franck-Condon factors and the laser parameters. These probabilities will incorporate laser-induced broadenings and energy shifts, the latter being approximated in our theory by a type of "second-order" Franck-Condon factor.

A notable recent paper by Napolitano [17] takes up similar resonant line-shape issues, with particular emphasis on intense laser fields. It thus treats one-color photoassociation in great detail, including the resulting mixtures of many scattering partial waves. The present treatment is complementary, in that the laser fields are assumed weak (though they may be strong enough to broaden the line shapes). Our focus has been rather on the application of multiple lasers of different colors, to emphasize the rich resonant structure of multiple resonant states.

After describing the basic process in Sec. II A, we produce in Sec. II the mathematical derivation of our main results, namely, Eqs. (2.20), (2.21), and Eqs. (2.34)-(2.36). The reader more interested in applications than in formalism can thus skip most of Sec. II and begin constructing scattering matrices and line-shape formulas according to the recipes of Secs. III and IV. Of particular interest are Eqs. (3.6) and (3.7), which provide useful approximate formulas for line widths and laser-induced shifts of resonance positions for the initial PA step.

*Electronic address: bohn@murphy.colorado.edu*

---

# II. General Theory

## A. The process

> [!figure] Figure 1
> Schematic potentials for cold collisions in the presence of two near-resonant laser fields, illustrating the notation developed in the text for $N=2$.

> [!figure] Figure 2
> Schematic potentials for cold collisions in the presence of one near-resonant laser field, demonstrating the way the formalism handles the PA process. Potential $V_{b1}$ has been shifted down in energy by $\hbar\omega_1$, so that the resonance lies at $E \simeq \Delta_1$, the laser's detuning. The artificial channel $V_{a1}$ models the spontaneous emission rate $\gamma_1$.

Figure 1 sketches the general process that we aim to describe. A pair of cold atoms approaches one another with relative kinetic energy $E$ (typically $<1\ \mathrm{mK}$), guided by their interaction potential $V_0$. Here we envision for simplicity a single incident channel, for instance, a pure triplet channel in the case of collisions between stretched-state alkali atoms. We will ignore fine and hyperfine structure in this paper, focusing instead on individual resonances well separated from their neighbors, in order to emphasize the structure of the line shapes. Nevertheless, the conclusions we come to are quite general, and carry over to more advanced scattering problems, by replacing Franck-Condon factors and the like with their multichannel counterparts.

The atom pair is promoted by the first laser to a bound state of energy $E_{b1}$ in a potential $V_{b1}(R)$. This laser is tuned to an angular frequency $\omega_1$, which is detuned by an amount $\Delta_{1b}=E_{b1}-\hbar\omega_1$ from the bound state. In addition, the laser's intensity $I_1$ gives rise to a radiative coupling

$$
V_{01}^{\mathrm{rad}}=\left(\frac{2\pi I_1}{c}\right)^{1/2}d_1(R),
$$

where $d_1(R)$ is an $R$-dependent molecular dipole matrix element. $d_1(R)$ can be estimated, for our purposes, from the atomic dipole matrix element; details are given in [18]. This radiative coupling, together with the free-bound Franck-Condon factor for this transition, generates a stimulated rate

$$
\Gamma_1 = 2\pi\left[V_{01}^{\mathrm{rad}}(R_C)\right]^2\left|\langle \phi_{b1}\mid f_0\rangle\right|^2,
$$

by Fermi's golden rule. Here $\phi_{b1}(R)$ denotes the unit-normalized bound state wave function of energy $E_b$ in potential $V_{b1}$, and $f_0(R)$ denotes the energy-normalized scattering wave function in the incident channel, to be defined in Sec. II C. The radiative coupling $V_{01}^{\mathrm{rad}}$ is evaluated at the Condon radius $R_C$, where the photon's energy just makes up the difference between the ground- and excited-state potentials.

From level $b_1$, additional lasers can drive the atom pair between any of a number of other bound states, $b_2,\ldots,b_N$, which may generally be either above or below the original scattering energy $E$. These lasers, with angular frequencies $\omega_i$, $i=2,\ldots,N$, have detunings

$$
\Delta_i = E_{bi}-\hbar(\omega_1\pm\omega_2\cdots\pm\omega_i),
\tag{2.1}
$$

where in each case a plus sign denotes absorption of a photon, while a minus sign denotes emission of a photon (for clarity, Fig. 1 depicts absorption only and sets $N=2$). The laser intensities $I_i$ also imply radiative couplings $V_{i,i+1}^{\mathrm{rad}}$, analogous to $V_{01}^{\mathrm{rad}}$. For bound-bound stimulated rates we adopt the Rabi-frequency notation

$$
\hbar\Omega_i=V_{i,i+1}^{\mathrm{rad}}(R_{C i,i+1})\,\langle\phi_{bi}\mid\phi_{b(i+1)}\rangle,
\qquad i=2,\ldots,N-1.
$$

This rate depends on the overlap integral of each bound-state wave function $\phi_{bi}(R)$ with its successor $\phi_{b(i+1)}(R)$, and the radiative coupling is again evaluated at the appropriate Condon point $R_{C i,i+1}$.

From each bound state $i$ there exists the possibility of a spontaneous emission event that occurs with a rate $\gamma_i$, which is usually proportional to the atomic decay rates of the atoms involved. Such events can release enormous amounts of kinetic energy on the scale of the trapped atoms, in which case they lead to trap loss. Indeed, this loss is often the experimental signature of resonances in PA spectroscopy. Alternatively, a probe laser may ionize the state of interest and produce loss [5]. Another possibility is that $\gamma_i$ represents the rate for nonradiating molecular states to fall from the trap region; this process has been suggested as a means for producing ultracold molecules [12].

The full treatment of spontaneous emission during atomic collisions can be quite involved [19]. We will bypass this complexity by coupling each bound state $b_i$ to an "artificial channel," identified by a purely repulsive potential $V_{ia}(R)$. The artificial potentials will account phenomenologically for the flux lost by spontaneous emission or other loss processes [20]. Trap loss will then be determined in our model by the appropriate scattering matrix element $S_{0,ai}$ which gives the probability amplitude for the atom pair to encounter each other with energy $E$ in the incident channel, interact under the influence of the laser light, then be ejected by scattering into artificial channel $a_i$. Our main task in this paper is to relate these scattering matrix elements to the detunings $\Delta_i$, stimulated rates $\Gamma$ and $\Omega_i$, and the spontaneous rates $\gamma_i$.

The observed line shape will be given by the thermally averaged value of the scattering matrix element,

$$
\begin{aligned}
K&(T,\Delta_1,\ldots,\Delta_N,I_1,\ldots,I_N,\gamma_1,\ldots,\gamma_N) \\
&=\left\langle
\frac{\pi v}{k^2}\sum_{l=0}^{\infty}(2l+1)
\left|S_{0,ia}(E,l,\Delta_1,\ldots,\Delta_N,I_1,\ldots,I_N,\gamma_1,\ldots,\gamma_N)\right|^2
\right\rangle.
\end{aligned}
\tag{2.2}
$$

Here the brackets denote the appropriate thermal average over a distribution of relative velocities $v$, at temperature $T$, and $k=\sqrt{2\mu E/\hbar^2}$, i.e., $k$ is the wave number for reduced mass $\mu$.

The diagonal element $S_{00}$ of the scattering matrix will also prove of relevance, for studies aimed at influencing the elastic-scattering properties of cold atoms. These elements will naturally emerge along with the rest of the scattering matrix in the following.

## B. Model

To cast this process as a scattering problem, we find it convenient to let $E$ denote the same total energy in every channel. We thus shift the potential $V_{b1}$ lower in energy by $\hbar\omega_1$, as illustrated in Fig. 2. In this case the detuning $\Delta_1$ represents the energy of the bound-state $b_1$ relative to the incident threshold, whereby the resonance condition becomes $E\simeq\Delta_1$. Likewise, we will regard each potential $V_{bi}$ as shifted by an amount $\hbar(\omega_1\pm\omega_2\cdots\pm\omega_i)$, with the signs chosen in accordance with Eq. (2.1). Figure 2 also illustrates the artificial channel potential $V_{1a}(R)$, designed to be totally repulsive and to converge at large $R$ to a value well below the incident threshold, so that its threshold effects will not become significant.

In the absence of radiative coupling we take the Hamiltonian to be diagonal, with diagonal potential matrix of the form

$$
V(R)=\mathrm{diag}\left[V_0(R),V_{a1}(R),\ldots,V_{aN}(R),V_{b1}(R),\ldots,V_{bN}(R)\right].
\tag{2.3}
$$

In this notation we incorporate a centrifugal potential, $\hbar^2l(l+1)/(2\mu R^2)$, into the incident channel potential $V_0$. The incident channel, together with the artificial channels, identify $N+1$ "open" channels, in which the atoms are energetically able to proceed to infinite separation $R$. The bound channels likewise identify $N$ "closed" channels, in which the atoms do not have sufficient energy to escape from one another. Once the lasers are switched on, these channels become coupled through the appropriate off-diagonal radiative couplings $V_{ij}^{\mathrm{rad}}$ described in Sec. II A [18]. In addition, each closed channel is coupled to its corresponding artificial channel by an $R$-independent coupling $V_{i,i}^{\mathrm{artif}}$, whose strength is adjusted artificially to reproduce the correct spontaneous decay rate, according to the golden rule:

$$
\gamma_i=2\pi\left(V_{i,i}^{\mathrm{artif}}\right)^2\left|\langle \phi_{bi}\mid f_{ai}\rangle\right|^2.
\tag{2.4}
$$

Just as above for the stimulated rate, $f_{ai}$ denotes an energy normalized scattering wave function, while $\phi_{bi}$ stands for a unit-normalized bound-state wave function. Schematically, the full potential $V+V'\equiv V+V^{\mathrm{rad}}+V^{\mathrm{artif}}$ takes the form

$$
V+V'=\begin{pmatrix}
V_0 & 0 & \cdots & 0 & V_{01}^{\mathrm{rad}} & 0 & \cdots & 0 \\
0 & V_{1a} & 0 & \cdots & 0 & V_{11}^{\mathrm{artif}} & 0 & \cdots & 0 \\
\vdots & 0 & V_{2a} & & & 0 & V_{22}^{\mathrm{artif}} & & \vdots \\
0 & 0 & & V_{Na} & 0 & 0 & \cdots & V_{NN}^{\mathrm{artif}} \\
V_{10}^{\mathrm{rad}} & V_{11}^{\mathrm{artif}} & 0 & \cdots & 0 & V_{1b} & V_{12}^{\mathrm{rad}} & \cdots & 0 \\
0 & 0 & V_{22}^{\mathrm{artif}} & & 0 & V_{12}^{\mathrm{rad}} & V_{2b} & & \vdots \\
\vdots & \vdots & & \ddots & \vdots & \vdots & & \ddots & V_{N-1,N}^{\mathrm{rad}} \\
0 & 0 & \cdots & V_{NN}^{\mathrm{artif}} & 0 & 0 & \cdots & V_{N-1,N}^{\mathrm{rad}} & V_{Nb}
\end{pmatrix}.
\tag{2.5}
$$

The resulting coupled-channel Schrodinger equation, in matrix form, is

$$
\left[-\frac{\hbar^2}{2\mu}\frac{d^2}{dR^2}+V(R)+V'(R)\right]F(R)=EF(R).
\tag{2.6}
$$

Here the off-diagonal potential matrix elements are denoted $V'$, to be used as a perturbation Hamiltonian in the following. In Eq. (2.6), $F=\{F_{ii'}\}$ is a matrix of solutions, whose second index $i'$ labels the linearly independent solutions. The wave-function components must be regular at the origin $[F_{i,i'}(0)=0]$ and must satisfy scattering boundary conditions in the open channels:

$$
F_{i,i'}(R)\sim \sqrt{\frac{2\mu}{\pi\hbar^2 k_i}}
\left[\exp(-ik_iR)\delta_{ii'}-\exp(ik_iR)S_{ii'}\right],
\qquad R\to\infty.
\tag{2.7}
$$

Here $k_i$ denotes the wave number in channel $i$, namely, $k_i^2=2\mu(E-E_i)/\hbar^2$, where $E_i$ denotes the threshold energy of channel $i$. The normalization coefficient in Eq. (2.7) is appropriate to energy normalization; we will see below that a different factor is obtained for the unit-normalized wave functions in closed channels. These boundary conditions define the scattering matrix $S_{ii'}$ in terms of energy-normalized incoming and outgoing plane waves in the various open channels. Eqs. (2.5)-(2.7) pose a well-defined coupled-channels model for laser-assisted scattering [18]. Indeed, we will in Sec. III compare our simple line-shape formulas with direct numerical solutions to this problem.

As an alternative to the complex-valued scattering matrix, we find it convenient to work with the real-valued reaction matrix $K^{\mathrm{red}}$, defined by relating the long-range behavior of $F$ in the open channels to standing waves at large $R$:

$$
F_{ii'}(R)\sim \sqrt{\frac{2\mu}{\pi\hbar^2 k_i}}
\left[\sin k_iR\,\delta_{ii'}+\cos k_iR\,K^{\mathrm{red}}_{ii'}\right],
\qquad R\to\infty.
\tag{2.8}
$$

The superscript "red" on $K$ stands for "reduced," a notation that will become evident in the following subsection. The reaction and scattering matrices are related through

$$
S=\frac{1+iK^{\mathrm{red}}}{1-iK^{\mathrm{red}}},
\tag{2.9}
$$

i.e., they bear the same relation as $\exp(2i\delta)$ and $\tan(\delta)$ for a scattering phase shift $\delta$.

## C. Quantum defect treatment

A full discussion of quantum-defect methods as applied to molecular physics can be found elsewhere [16]; here we will merely summarize the results we need. We note also that this viewpoint has seen a recent revival in its application to atomic collisions near threshold [21-23]. The spirit of quantum defect theory (QDT) consists of separating the physics of channel coupling from the physics of resonances. Namely, it initially treats all channels, both open and closed, on an equal footing, generating a "short-range" $K$ matrix that tends to depend smoothly on energy. In our case, this $K$ matrix will also vary smoothly and predictably with the laser parameters. In a second step, QDT "eliminates" the closed channels, i.e., requires that their wave functions vanish at asymptotically large $R$. In this second step, the sharp energy dependences that characterize resonant scattering will appear. In the context of laser-assisted cold collisions, this two-step treatment will emphasize formally the role of laser intensities and detunings in determining line shapes, while separating the role of molecular physics embodied in the Franck-Condon factors.

We first generate, for each channel, a pair of reference functions $f_i(R)$ and $g_i(R)$, that satisfy the single-channel Schrodinger equations,

$$
\left[-\frac{\hbar^2}{2\mu}\frac{d^2}{dR^2}+V_i(R)\right]
\begin{Bmatrix} f_i(R) \\ g_i(R) \end{Bmatrix}
=E\begin{Bmatrix} f_i(R) \\ g_i(R) \end{Bmatrix}.
\tag{2.10}
$$

In the open channels, $f_i$ and $g_i$ are defined by the following boundary conditions:

$$
\begin{aligned}
f_i(R)&\sim R^{l_i}, && R\to 0,\\
f_i(R)&\sim \sqrt{\frac{2\mu}{\pi\hbar^2 k_i}}\sin(k_iR-l_i\pi/2+\eta_i), && R\to\infty,\\
g_i(R)&\sim R^{-l_i-1}, && R\to 0,\\
g_i(R)&\sim -\sqrt{\frac{2\mu}{\pi\hbar^2 k_i}}\cos(k_iR-l_i\pi/2+\eta_i), && R\to\infty,
\end{aligned}
\tag{2.11}
$$

where $l_i=0$ in all artificial channels, and $l_0$ corresponds to the partial wave of interest in the incident channel. These solutions already include the elastic-scattering phase shifts $\eta_i$ for scattering in the potentials $V_i$. These functions are said to be "energy normalized," as a consequence of which their Wronskian becomes

$$
W(f_i,g_i)=f_i\frac{dg_i}{dR}-\frac{df_i}{dR}g_i=\frac{2\mu}{\pi\hbar^2}.
\tag{2.12}
$$

We note here that the artificial channel potentials (hence wave functions) are fairly arbitrary, because: (i) their elastic phase shifts are unobservable, (ii) loss rates to these channels will ultimately be replaced by phenomenological rates, and (iii) energy shifts arising from these channels are unphysical, and should be disregarded in applications of the semianalytic formulas (see Sec. III).

In the closed channels, $f_i$ and $g_i$ are defined by a WKB-like boundary condition at each channel's potential minimum $R=R_{0i}$, as related in [16]. These functions are likewise energy normalized, so that they are treated on an equal footing with the open-channel functions. Namely, $f_i$ satisfies $f_i\sim R^{l_i}$ as $R\to0$, while the WKB-like condition

$$
f_i^2\left[k_i^2+\left(\frac{df_i/dR}{f_i}\right)^2\right]\sim k_i
\qquad \text{at } R=R_{0i}
\tag{2.13}
$$

determines an energy-like normalization in these channels. The irregular function $g_i$ is defined to be "out of phase" with $f_i$ at $V_i$'s minimum, in analogy with the definitions in (2.11):

$$
g_i\sim -\frac{1}{k_i}\frac{df_i}{dR}\qquad \text{at } R=R_{0i}.
\tag{2.14}
$$

$f_i$ and $g_i$ are generally both divergent as $R\to\infty$; however, when the total energy $E$ coincides with the energy of a bound state of $V_i$, $f_i$ vanishes at large $R$ and becomes proportional to a bound-state wave function $\phi_i$, related to $f_i$ by

$$
f_i=\left(\frac{1}{\pi}\frac{\partial\nu_i}{\partial E}\right)^{1/2}\phi_i,
\tag{2.15}
$$

and "space" normalized in the usual way,

$$
\int_0^\infty dR\,\phi_i^2(R)=1.
\tag{2.16}
$$

Here $\nu_i/\pi=\nu_i(E)/\pi$ stands for a quantum defect, a quantity that takes integer values whenever $E=E_n$ coincides with a bound state of energy $E_n$, and interpolates smoothly between these values [16].

In terms of these reference functions the $K$ matrix satisfies a relation analogous to Eq. (2.8):

$$
F_{ii'}(R)\sim f_i(R)\delta_{ii'}-g_i(R)K_{ii'},
\tag{2.17}
$$

or in matrices,

$$
F(R)\sim f(R)-g(R)K.
\tag{2.18}
$$

In this last form, $f$ and $g$ stand for diagonal matrices, whose diagonal elements are the regular and irregular channel functions. This relation will define $K$ for open and closed channels alike. $K$ generally has a weak energy dependence, because physical boundary conditions have yet to be imposed on the closed channels. Imposing these conditions is conventionally done by partitioning $K$ into open and closed blocks:

$$
K=\begin{pmatrix}
K^{oo} & K^{oc} \\
K^{co} & K^{cc}
\end{pmatrix}.
\tag{2.19}
$$

Rearranging the solutions (2.18) so that closed-channel wave functions vanish at large $R$ amounts to defining a reduced $K$ matrix [24],

$$
K^{\mathrm{red}}=K^{oo}-K^{oc}\left(\tan\nu+K^{cc}\right)^{-1}K^{co},
\tag{2.20}
$$

whose dimension is the number of open channels. The physical scattering matrix is then obtained from

$$
S=\exp(i\eta)\frac{1+iK^{\mathrm{red}}}{1-iK^{\mathrm{red}}}\exp(i\eta),
\tag{2.21}
$$

where $\exp(i\eta)$ denotes a diagonal matrix whose diagonal elements are $\exp(i\eta_i)$ for the elastic phase shifts $\eta_i$.

## D. Perturbative evaluation of $K$

Often in scattering calculations the $K$ matrix is evaluated numerically, by directly integrating the coupled-channel Schrodinger equation for the scattering process. In this subsection, we instead evaluate $K$ perturbatively, in order to determine final results in an analytic way. Our treatment recasts $K$ as an explicitly $R$-dependent quantity $K(R)$, which accounts for the "running value" of $K$ as $R$ progresses from zero to $\infty$. That is, we write the coupled-channel wave function in a form analogous to Eq. (2.18),

$$
F(R)=[f(R)-g(R)K(R)]Z(R),
\tag{2.22}
$$

for all values of $R$. Here $f$ and $g$ stand for diagonal matrices consisting of the regular and irregular channel reference functions, while $Z$ stands for a normalization matrix. (Note that $Z$ is often denoted $I$ in the QDT literature; here we use $Z$ to avoid confusion with our notation for laser intensity.) $K$ then satisfies a first-order differential equation in $R$, with initial boundary condition $K(0)=0$, and $K$ will tend at asymptotically large $R$ to the correct scattering $K$ matrix [25-27]. This viewpoint is often valuable in mapping the range of $R$ where the scattering phase shifts accumulate. It can thereby shed light on the processes involved in channel coupling [26,27], although we will not address this issue here.

To derive the differential equation for $K(R)$, we find it convenient to reparametrize Eq. (2.22) as

$$
F(R)=f(R)Z(R)-g(R)J(R).
\tag{2.23}
$$

This decomposition factors $K$ into $Z$ and $J$, in analogy to factoring a tangent into a sine and cosine, so that $K=JZ^{-1}$. The gradient of $F$ is then

$$
\frac{dF}{dR}=\frac{df}{dR}Z-\frac{dg}{dR}J+f\frac{dZ}{dR}-g\frac{dJ}{dR}.
\tag{2.24}
$$

The matrices $Z$ and $J$ are not of individual interest, since it is their ratio that determines observable scattering properties. We are, therefore, free to impose an additional constraint between these matrices, which we choose to be

$$
f\frac{dZ}{dR}-g\frac{dJ}{dR}\equiv 0.
\tag{2.25}
$$

This procedure is well known in the theory of ordinary differential equations as the "technique of variational parameters" [28]. With this definition, the Schrodinger equation (2.6) for $F$ becomes, after substituting the definition (2.10) of the reference functions,

$$
-\frac{\hbar^2}{2\mu}\left(\frac{df}{dR}\frac{dZ}{dR}-\frac{dg}{dR}\frac{dJ}{dR}\right)+V'(R)F(R)=0.
\tag{2.26}
$$

We then invert the linear system (2.25) and (2.26) to determine expressions for the derivatives of $Z$ and $J$:

$$
\frac{dZ}{dR}=-\pi g(R)V'(R)F(R),
\qquad
\frac{dJ}{dR}=-\pi f(R)V'(R)F(R),
\tag{2.27}
$$

where we have exploited the Wronskian (2.12) of the channel functions. We finally insert the relations (2.23) and (2.27) into $dK/dR$ to obtain the equation for $K$:

$$
\begin{aligned}
\frac{dK}{dR}
&=\frac{dJ}{dR}Z^{-1}-JZ^{-1}\frac{dZ}{dR}Z^{-1} \\
&=-\pi fV'f+\pi fV'gK+\pi KgV'f-\pi KgV'gK.
\end{aligned}
\tag{2.28}
$$

Such expressions are already familiar in the distorted-wave theory of scattering [29].

In the limit where the radiative coupling is weak, $K$ is expected to remain small, since the fully coupled scattering wave functions differ little from those in the absence of the radiation. In this case we neglect all but the first term on the right-hand-side of Eq. (2.28), yielding an expression for the first-order $K$ matrix:

$$
K^{(1)}=-\pi\int_0^\infty dR\, f(R)V'(R)f(R).
\tag{2.29}
$$

We will further assert that each element $V'_{ij}(R)$ can be well approximated by its value near the Condon point $R_{Cij}$ of the transition, whereby the off-diagonal elements of $K$ become

$$
K_{ij}=-\pi V'_{ij}(R_{Cij})\int_0^\infty dR\,f_i(R)f_j(R).
\tag{2.30}
$$

The second-order contribution to $K$ is evaluated by inserting the integrand of Eq. (2.29) into Eq. (2.28), and including terms on the right-hand-side of Eq. (2.28) that are linear in $K$. Again taking $V'$ constant, we find

$$
\begin{aligned}
K_{ij}^{(2)}={}&-\pi^2\sum_k V'_{ik}(R_{Cik})V'_{kj}(R_{Ckj}) \\
&\times\left(
\int_0^\infty dR\,f_i(R)g_k(R)\int_0^R dR'\,f_k(R')f_j(R')
+\int_0^\infty dR\,g_k(R)f_j(R)\int_0^R dR'\,f_i(R')f_k(R')
\right).
\end{aligned}
\tag{2.31}
$$

This expression describes the influence of channel $i$ on channel $j$, via their mutual interaction with intermediate channel $k$. As a particularly important case, we note the diagonal elements of $K$ that reflect phase shifts in channel $i$ due to its interaction with other channels $k$:

$$
K_{ii}^{(2)}=-2\pi^2\sum_k\left[V'_{ik}(R_{Cik})\right]^2
\int_0^\infty dR\,f_i(R)g_k(R)
\int_0^R dR'\,f_k(R')f_i(R').
\tag{2.32}
$$

As we will see below, this shift is responsible for the apparent energy shift of the resonances in closed channels $i$ due to their interaction with the open channels $k$. Note that this energy shift is proportional to laser intensity.

To turn these results into a useful formula we exploit the fact that we are describing resonant scattering to make a few further approximations. First, in any closed-channel $k$ we note that the phase shift $\nu_k\sim n\pi$ near resonance, so that the tangent in Eq. (2.20) can be approximated as

$$
\tan\nu_k\sim \frac{\partial\nu_k}{\partial E}(E-\Delta_k).
\tag{2.33}
$$

The second approximation involves the closed-channel wave function. Namely, near the resonance condition $E\sim\Delta_k$ this wave function is very well described by the regular channel function $f_k$, with essentially no admixture of the irregular function $g_k$. Moreover, the regular function can in this circumstance be represented by the space-normalized wave function $\phi_k$ defined in Eq. (2.15).

Based on these approximations, the contributions to $K$ arising from the first-order term $K^{(1)}$ are as follows. Matrix elements between one open and one closed channel become

$$
K_{ik}=-\pi V'_{ik}(R_{Cik})\left(\frac{1}{\pi}\frac{\partial\nu_k}{\partial E}\right)^{1/2}
\int_0^\infty dR\,f_i(R)\phi_k(R),
\tag{2.34}
$$

where $V'_{ik}$ stands for either radiative or artificial coupling, depending on whether $i=0$ or $i>0$. If both channels are closed, $V'=V^{\mathrm{rad}}$, and the matrix elements become instead

$$
K_{kk'}=-\pi V_{kk'}^{\mathrm{rad}}(R_{Ckk'})\frac{1}{\pi}\left(\frac{\partial\nu_k}{\partial E}\frac{\partial\nu_{k'}}{\partial E}\right)^{1/2}
\int_0^\infty dR\,\phi_k(R)\phi_{k'}(R).
\tag{2.35}
$$

Thus the only nonvanishing off-diagonal components of $K$ are $K_{0,b1}$, $K_{ai,bi}$, and $K_{bi,b(i+1)}$, following the pattern of off-diagonal elements of the potential matrix (2.5).

Similarly, we note that elements of the second-order contribution $K^{(2)}$ vanish whenever the intermediate state $k$ in Eq. (2.31) refers to a closed channel, since we disregard contributions due to $g_k$. Comparison with the potential matrix (2.5) then demonstrates that $K_{ij}$ vanishes between any two open channels $i$ and $j$, as well as between channel 0 and channel $b_2$ (interacting via $b_1$), between artificial channel $a_i$ and bound channel $b(i+1)$ (interacting via $b_i$), and between $b_i$ and $b(i+2)$ [interacting via $b(i+1)$]. This leaves only the diagonal elements of $K$ in closed channels, which take the form

$$
K_{kk}=-2\pi^2\sum_i\left[V'_{ik}(R_{Cik})\right]^2
\left(\frac{1}{\pi}\frac{\partial\nu_k}{\partial E}\right)
\int_0^\infty dR\,\phi_k(R)g_i(R)
\int_0^R dR'\,f_i(R')\phi_k(R').
\tag{2.36}
$$

The structure of $K$ will emerge more clearly in the examples in the next two sections.

---

# III. Single-Laser Line-Shape Formulas

In this section and the next we will present examples of the formalism of the last section, showing explicitly how to transform the approximate $K$-matrix formulas (2.34)-(2.36) into useful expressions for the relevant scattering matrix elements. In this section we describe the action of a single laser, emphasizing the role of laser intensity in broadening and shifting the resonance features.

Within our model, this analysis entails a three-channel scattering problem, requiring a single bound-state channel $V_b(R)$ and a single artificial channel potential $V_a(R)$, along with the incident channel potential $V_0(R)$. With this notation the $K$ matrix reads

$$
K=\begin{pmatrix}
0 & 0 & K_{0b} \\
0 & 0 & K_{ab} \\
K_{b0} & K_{ba} & K_{bb}
\end{pmatrix}.
\tag{3.1}
$$

We reiterate that this expression follows from our second-order (in $V'$) approximation; in general, all elements of $K$ will be nonzero. In this context, the zero elements of $K$ reflect the fact that the open channels are not directly coupled, but interact only through their mutual couplings to the intermediate bound state. $K$ is thus already partitioned into open and closed portions as in Eq. (2.19). Carrying out the reduction (2.20) then yields the reduced $K$ matrix,

$$
K^{\mathrm{red}}=\frac{-1}{\tan\nu_b+K_{bb}}
\begin{pmatrix}
K_{0b}K_{b0} & K_{0b}K_{ba} \\
K_{ab}K_{b0} & K_{ab}K_{ba}
\end{pmatrix}.
\tag{3.2}
$$

When the expressions for $K$, Eqs. (2.34) and (2.36), are inserted here, the final expression for $K^{\mathrm{red}}$ ensues:

$$
K^{\mathrm{red}}=\frac{-1}{2[E-(\Delta+E_1)]}
\begin{pmatrix}
\Gamma & \sqrt{\gamma\Gamma} \\
\sqrt{\gamma\Gamma} & \gamma
\end{pmatrix}.
\tag{3.3}
$$

Here $\gamma$ [see Eq. (2.4)] stands for the spontaneous emission loss rate, which can be determined empirically from the molecular radiative lifetime. Moreover,

$$
\Gamma=2\pi\left(V_{0b}^{\mathrm{rad}}\right)^2
\left|\int_0^\infty dR\,f_0(R)\phi_b(R)\right|^2
\tag{3.4}
$$

denotes the intensity-dependent stimulated absorption/emission rate generated by the laser. (Here and in the following we will suppress the explicit notation $R_C$, evaluation at the Condon point being assumed.) The energy shift of the effective resonance position due to the laser is

$$
E_1=-2\pi\left(V_{0b}^{\mathrm{rad}}\right)^2
\int_0^\infty dR\,\phi_b(R)g_0(R)
\int_0^R dR'\,f_0(R')\phi_b(R').
\tag{3.5}
$$

Evaluating the Franck-Condon factor in Eq. (3.4) is familiar, but evaluating the "second-order" FCF in Eq. (3.5) is less so. To compute it, it is generally necessary to tabulate the values of the inner integrand while computing the first-order FCF. Alternatively, in some cases we can apply a stationary phase approximation to estimate these integrals. This procedure is particularly useful for describing the initial photoassociation step; it is detailed in the Appendix, yielding the approximations,

$$
\Gamma=2\pi\left(V_{0b}^{\mathrm{rad}}\right)^2
\left(\frac{\partial E}{\partial n}\right)
\frac{|f_0(R_C)|^2}{D_C},
\tag{3.6}
$$

$$
E_1=\pi\left(V_{0b}^{\mathrm{rad}}\right)^2
\left(\frac{\partial E}{\partial n}\right)
\frac{f_0(R_C)g_0(R_C)}{D_C},
\tag{3.7}
$$

where the open-channel wave functions $f_0$ and $g_0$ are evaluated at the Condon point $R_C$, and

$$
D_C\equiv \left.\frac{\partial V_b}{\partial R}\right|_{R_C}.
\tag{3.8}
$$

The reflection approximation expressions (3.6) and (3.7) thus depend on properties of wave functions and potential curves, along with the level density of vibrational levels in potential $V_b$, which can be approximated as

$$
\frac{\partial E}{\partial n}\simeq \frac{E_{n+1}-E_{n-1}}{2}.
\tag{3.9}
$$

Moreover, this approximation makes the threshold behavior of these quantities manifestly apparent. In the $k\to0$ limit, the definitions (2.11) imply $\Gamma\sim k$ and $E_1\sim\mathrm{const}$.

> [!figure] Figure 3
> The laser-induced width ($\Gamma$) and energy shift ($E_1$) parameters for PA in lithium, as described in the text, for a PA laser intensity of $500\ \mathrm{W/cm^2}$ and detuning $\Delta=20\ \mathrm{MHz}$. Variations with collision energy give the line-shape (3.11) non-Lorentzian features. Dots show the reflection approximation results.

In general, within the close-coupled theory presented here there are additional apparent shifts arising from coupling to the open artificial channels. These shifts are unphysical artifacts of treating spontaneous emission channels in exactly the same way as open scattering channels, and should be neglected in applications of our semianalytic formulas. Equation (3.5), since it is applied to the physical scattering channel, yields the physical, laser-induced line shift.

Equation (3.3) represents in a compact way all the relevant scattering information. From it, we can extract the scattering matrix using Eq. (2.21). The inelastic part is

$$
S_{0a}=-i\exp[i(\eta_0+\eta_a)]\frac{\sqrt{\gamma\Gamma}}{E-(\Delta_b+E_1)+i(\gamma+\Gamma)/2},
\tag{3.10}
$$

whereby the trap loss probability becomes

$$
|S_{0a}|^2=\frac{\gamma\Gamma}{[E-(\Delta+E_1)]^2+\left(\frac{\gamma+\Gamma}{2}\right)^2}.
\tag{3.11}
$$

We have thus reproduced the line shape in [7], and extended it by accounting for the energy shift $E_1$ and broadened width $\gamma+\Gamma$.

The inelastic-scattering probability in Eq. (3.11) is formally a Lorentzian, but in the low-energy regime both the width $\Gamma$ and the energy shift $E_1$ have explicit threshold variations. Figure 3 illustrates this dependence, using as an example PA to the $v=64$ vibrational level of the $b^3\Sigma_g$ excited state of lithium. This level has been observed in PA spectroscopy at Rice University [30]; for reference purposes, we note that it is detuned $\sim56\ \mathrm{cm}^{-1}$ from the atomic resonance, and has a Condon point at $R_C=35\ \mathrm{a.u.}$ The detuning from the molecular bound state is here taken as $\Delta=20\ \mathrm{MHz}$. The upper curve of Fig. 3 shows the laser-induced line width $\Gamma$, computed from Eq. (3.4), for laser intensity $I=500\ \mathrm{W/cm^2}$. At this intensity $\Gamma$ becomes comparable to the spontaneous emission linewidth of $12\ \mathrm{MHz}$ [31], at which point the transition begins to saturate. Also, $\Gamma$ drops to zero in proportion to $E^{1/2}$, owing to the energy dependence of the Franck-Condon factor in Eq. (3.4). As this dropoff occurs on an energy scale comparable to $\gamma$, it must be included in any PA line-shape analysis, as has been emphasized [7,32].

The lower curve in Fig. 3 shows the energy shift parameter $E_1$ computed from Eq. (3.5), for the same intensity $500\ \mathrm{W/cm^2}$. This shift is also comparable to $\gamma$, implying that laser-induced shifts become significant for laser fields near and beyond saturation. Note also that $E_1$ is negative, implying that the shift is always in the direction of red detuning.

This negative shift will be generic in near-threshold resonant scattering, for the following reason. In the Fano theory of a bound state coupled to a continuum, the energy shift is given formally by a principal part integral [33],

$$
E_1^{\mathrm{Fano}}=P\int dE'\frac{V(E')^2}{E-E'}.
\tag{3.12}
$$

Here $V(E')$ represents essentially the density of continuum states at energy $E'$. For $E$ near the unperturbed resonance position, the integrand in Eq. (3.12) is positive when $E'<E$ and negative when $E'>E$. The positive slope of $V(E')$ versus $E'$ near threshold ensures that the negative part of the integrand will contribute more strongly, and Eq. (3.12) will be negative. Another way of saying this is that the continuum levels will try to "repel" the unperturbed bound state, but since there is "more continuum" on the high-energy side, the net shift must be to lower energy, i.e., toward threshold. (In passing, we remark that Eq. (3.5) is a convenient way of computing $E_1$ on the energy shell, instead of performing the difficult energy integral (3.12) [20].)

The results of the reflection approximation, Eqs. (3.6) and (3.7), are also plotted, as points, in Fig. 3. The agreement for the width $\Gamma$ is excellent, as has been noted in [34]. The approximation also works quite well for the energy shift, reproducing its value to within a few percent. We have thus generated a simple approximate means for determining the laser-induced shifts, which should be of use in saturation studies of the PA process. Moreover, as noted above, the reflection approximation explains the threshold dependencies $\Gamma\sim E^{1/2}$ and $E_1\sim\mathrm{const}$.

> [!figure] Figure 4
> Scattering probabilities $|S_{0a}|^2$ for PA in lithium, for various laser intensities and a fixed detuning of $\Delta=20\ \mathrm{MHz}$. Points denote numerical solutions to a quantum close-coupling problem; continuous curves were calculated from the line-shape formula (3.11).

> [!figure] Figure 5
> Thermally averaged trap loss rates, according to Eq. (2.2), versus laser detuning, assuming a temperature of $1\ \mathrm{mK}$. The plotted abscissa is $-\Delta$ rather than $\Delta$, to place red detuning to the left. Broadening and laser-induced redshifts are visible.

The action of laser intensities on the actual scattering probabilities $|S_{0a}|^2$ is shown in Fig. 4. As the transition saturates, we see the characteristic broadening and red shift of the line shape. In this figure the points represent a full numerical solution to the coupled-channels problem set up in Sec. II B, while the continuous lines were computed using our simple line-shape formula (3.11) [35]. The simplified formulas are quite adequate, showing slight deviation from the close-coupling solution only at the highest intensity, $1000\ \mathrm{W/cm^2}$, well above saturation. Figure 5 translates these scattering probabilities into observable line shapes, by thermally averaging $|S_{0a}|^2$ according to Eq. (2.2), and assuming a temperature of $1\ \mathrm{mK}$. We have plotted these rates versus $-\Delta$, rather than versus $\Delta$, to place red detuning to the left. Note the asymmetric line shape, with a long tail toward red detuning, as has been previously noted [7]. For fixed detuning, scattering probability diminishes at high enough intensity (Fig. 4), as the apparent resonance position moves effectively below threshold. Varying the detuning, however, can restore the resonance to positive scattering energies, whereby the thermally averaged signal gets larger at greater intensity (Fig. 5). The laser must be detuned farther to the red to do so at higher intensities.

We can also derive from our reduced $K$ matrix the elastic scattering matrix element,

$$
S_{00}=\exp(2i\eta_0)\frac{E-(\Delta+E_1)-i\left(\frac{\Gamma-\gamma}{2}\right)}{E-(\Delta+E_1)+i\left(\frac{\Gamma+\gamma}{2}\right)}.
\tag{3.13}
$$

From this scattering matrix element we can extract a complex-valued phase shift via $S_{00}=\exp(2i\delta)$, with $\delta=\lambda+i\mu$, whose imaginary part accounts for the flux lost into the artificial channel. This, in turn, gives us a complex-valued scattering length,

$$
a_{\mathrm{sc}}=-\frac{1}{k}(\lambda+i\mu),
\tag{3.14}
$$

where $k=\sqrt{2\mu E/\hbar^2}$ stands for the incident wave number, evaluated in the limit of small $E$. In the present model, and assuming $\tan\delta\simeq\delta$, we arrive at an expression for the laser-dependent scattering length,

$$
\operatorname{Re}(a_{\mathrm{sc}})\simeq a_{\mathrm{sc}}(\mathrm{nat})-rac{1}{k}\frac{\frac{1}{2}\Gamma[E-(\Delta+E_1)]}{[E-(\Delta+E_1)]^2-\frac{\Gamma^2-\gamma^2}{4}},
\tag{3.15}
$$

$$
\operatorname{Im}(a_{\mathrm{sc}})=\frac{1}{k}\frac{\frac{1}{4}\Gamma\gamma}{[E-(\Delta+E_1)]^2-\frac{\Gamma^2+\gamma^2}{4}},
\tag{3.16}
$$

where $a_{\mathrm{sc}}(\mathrm{nat})$ is the unperturbed scattering length. Note that $\Gamma\sim k$, so that $a_{\mathrm{sc}}$ is well defined in the limit of vanishing $k$. These expressions have already been discussed in [15], where they are used to express the feasibility of altering scattering lengths in this way. Similar expressions, including the shift, have also appeared in [14].

---

# IV. Two-Laser Line Shapes

In this section we derive the scattering matrix for a collision in the presence of two independently tunable lasers. This example is a little more complicated than the single-laser case, and should provide suitable instruction for constructing similar scattering matrices in more elaborate contexts. In this case we will have five channels: 0, as usual, stands for the incident channel, and $a_1$ and $a_2$ are the artificial channels into which bound-state channels $b_1$ and $b_2$ decay, respectively. The pattern of off-diagonal coupling due to radiative and artificial couplings is given, analogously to Eq. (3.1), by

$$
K=\begin{pmatrix}
0 & 0 & 0 & K_{0,b1} & 0 \\
0 & 0 & 0 & K_{a1,b1} & 0 \\
0 & 0 & 0 & 0 & K_{a2,b2} \\
K_{0,b1} & K_{a1,b1} & 0 & K_{b1,b1} & K_{b1,b2} \\
0 & 0 & K_{a2,b2} & K_{b1,b2} & K_{b2,b2}
\end{pmatrix}.
\tag{4.1}
$$

We proceed, as before, to construct from this matrix the reduced $K$ matrix,

$$
\begin{aligned}
K^{\mathrm{red}}={}&\frac{-1}{(K_{b1,b1}+\tan\nu_{b1})(K_{b2,b2}+\tan\nu_{b2})-K_{b1,b2}^2} \\
&\times
\begin{pmatrix}
K_{0,b1}(K_{b2,b2}+\tan\nu_{b2})K_{0,b1} & K_{0,b1}(K_{b2,b2}+\tan\nu_{b2})K_{a1,b1} & -K_{0,b1}K_{b1,b2}K_{a2,b2} \\
K_{a1,b1}(K_{b2,b2}+\tan\nu_{b2})K_{0,b1} & K_{a1,b1}(K_{b2,b2}+\tan\nu_{b2})K_{a1,b1} & -K_{a1,b1}K_{b1,b2}K_{a2,b2} \\
-K_{a2,b2}K_{b1,b2}K_{0,b1} & -K_{a2,b2}K_{b2,b1}K_{b1,a1} & K_{a2,b2}(K_{b1,b1}+\tan\nu_{b1})K_{a2,b2}
\end{pmatrix}.
\end{aligned}
\tag{4.2}
$$

Again, in complete analogy with what we did in the single-laser case, we identify free-bound couplings with the following rates:

$$
\Gamma=2\pi\left(V_{0,b1}^{\mathrm{rad}}\right)^2
\left|\int_0^\infty dR\,f_0(R)\phi_{b1}(R)\right|^2
\tag{4.3}
$$

for the initial stimulated process to bound level $b_1$, and

$$
\gamma_i=2\pi\left(V_{bi,ai}^{\mathrm{artif}}\right)^2
\left|\int_0^\infty dR\,f_{ai}(R)\phi_{bi}(R)\right|^2
\tag{4.4}
$$

for spontaneous emission from either bound-state $i$. In addition, we have this time to identify the Rabi frequency for transitions between the two bound states, through

$$
\hbar\Omega=\left|V_{b1,b2}^{\mathrm{rad}}\int_0^\infty dR\,\phi_{b1}(R)\phi_{b2}(R)\right|.
\tag{4.5}
$$

Then, making the approximation (2.33) for the energy dependence of the quantum defects, we write the reduced $K$ matrix in terms of observables through

$$
K^{\mathrm{red}}=\frac{-1/2}{[E-(\Delta_1+E_1)][E-(\Delta_2+E_2)]-(\hbar\Omega)^2}
\begin{pmatrix}
\Gamma[E-(\Delta_2+E_2)] & \sqrt{\gamma_1\Gamma}[E-(\Delta_2+E_2)] & -\sqrt{\gamma_2\Gamma}\hbar\Omega \\
\sqrt{\gamma_1\Gamma}[E-(\Delta_2+E_2)] & \gamma_1[E-(\Delta_2+E_2)] & -\sqrt{\gamma_1\gamma_2}\hbar\Omega \\
-\sqrt{\gamma_2\Gamma}\hbar\Omega & -\sqrt{\gamma_1\gamma_2}\hbar\Omega & \gamma_2[E-(\Delta_1+E_1)]
\end{pmatrix}.
\tag{4.6}
$$

Here again there are energy shifts that arise from the interaction of closed channels with open ones. The relevant shift for us is $E_1$, which is generated by the connection of bound state $b_1$ with the incident continuum:

$$
E_1=-2\pi\left(V_{0,b1}^{\mathrm{rad}}\right)^2
\int_0^\infty dR\,\phi_{b1}(R)g_0(R)
\int_0^R dR'\,f_0(R')\phi_{b1}(R').
\tag{4.7}
$$

As above, this expression deliberately neglects the influence of the continuum channel $a_1$, which we regard as unphysical. The expression for $E_2$, which arises from the coupling of bound state $b_2$ with the artificial channel $a_2$, is likewise artificial, and should be neglected in applications of the two-color results in this section.

The physical scattering results are summarized in the scattering amplitudes $S_{0,0}$, $S_{0,a1}$, and $S_{0,a2}$. After some algebra, the recipe (2.21) yields

$$
S_{0,a1}=\frac{-i\sqrt{\gamma_1\Gamma}(E-\Delta_2+i\gamma_2/2)}{d(E,\Gamma,\gamma_1,\gamma_2,\Delta_1,\Delta_2,E_1)},
\tag{4.8}
$$

$$
S_{0,a2}=\frac{i\sqrt{\gamma_2\Gamma}\hbar\Omega}{d(E,\Gamma,\gamma_1,\gamma_2,\Delta_1,\Delta_2,E_1)},
\tag{4.9}
$$

$$
\begin{aligned}
S_{0,0}&=\frac{n(E,\Gamma,\gamma_1,\gamma_2,\Delta_1,\Delta_2,E_1)}{d(E,\Gamma,\gamma_1,\gamma_2,\Delta_1,\Delta_2,E_1)},\\[4pt]
n(E,\Gamma,\gamma_1,\gamma_2,\Delta_1,\Delta_2,E_1)
&=\left\{[E-(\Delta_1+E_1)](E-\Delta_2)-(\hbar\Omega)^2-\frac{\gamma_2(\gamma_1-\Gamma)}{4}\right\} \\
&\quad+i\left\{\frac{(\gamma_1-\Gamma)(E-\Delta_2)}{2}+\frac{\gamma_2[E-(\Delta_1+E_1)]}{2}\right\}.
\end{aligned}
\tag{4.10}
$$

The resonance denominator is

$$
\begin{aligned}
d(E,\Gamma,\gamma_1,\gamma_2,\Delta_1,\Delta_2,E_1)
={}&\left\{[E-(\Delta_1+E_1)](E-\Delta_2)-(\hbar\Omega)^2-\frac{\gamma_2(\gamma_1+\Gamma)}{4}\right\} \\
&+i\left\{\frac{(\gamma_1+\Gamma)(E-\Delta_2)}{2}+\frac{\gamma_2[E-(\Delta_1+E_1)]}{2}\right\}.
\end{aligned}
\tag{4.11}
$$

Squaring the amplitudes (4.8)-(4.10) yields the probabilities for various outcomes of the laser-assisted scattering process. The relatively simple algebraic forms of the resulting expressions prove convenient for designing experiments aimed at producing a desired outcome. These issues have been described in [8] and extended in [12].

---

# V. Conclusions

We have derived a straightforward algebraic procedure for deriving line-shape formulas in the context of laser-assisted cold collisions. These formulas are specialized to the case of near-resonant laser transitions. The basic inputs consist of Franck-Condon factors between the states involved, as well as "second-order" Franck-Condon factors, e.g., Eqs. (2.36) that give explicit formulas for the energy shifts associated with high laser power. These quantities, together with the detunings and intensities of the lasers, fit into simple manipulations of small matrices to yield scattering probabilities, leading to thermally averaged line shapes. Moreover, for the initial PA step, these quantities can be estimated using the simple reflection formula results (3.6) and (3.7), without explicitly performing a Franck-Condon integral at all. The one- and two-color examples presented here are illustrative of the general procedure, which should prove useful in contexts yet to be envisioned.

## Acknowledgments

This work was supported in part by the National Science Foundation, and in part by the U.S. Office of Naval Research.

---

# Appendix: Reflection Formula

The reflection approximation, as developed in Ref. [36] and extended to cold atoms in [34], can in some cases circumvent the need to evaluate Franck-Condon-type integrals such as in Eqs. (3.4) and (3.5). In this appendix we reproduce Ref. [34]'s derivation for photoassociation linewidths, and extend it to describe also intensity-dependent line shifts. We will focus on the special case of the initial photoassociation step, from the incident continuum channel to the vibrational bound state in potential $V_b$.

We begin by casting the incident-channel wave function $f_0$ and its irregular counterpart, into a phase-amplitude form, after Milne [37],

$$
f_0(R)=\sqrt{\frac{2\mu}{\pi\hbar^2}}\alpha_0(R)\sin\beta_0(R),
$$

$$
g_0(R)=-\sqrt{\frac{2\mu}{\pi\hbar^2}}\alpha_0(R)\cos\beta_0(R).
\tag{A1}
$$

Note the minus sign in the definition of $g_0$, which is purely a convention, but which formally affects the result (A24) below. This is an exact representation of these wave functions, provided $\alpha_0$ and $\beta_0$ satisfy

$$
\left(\frac{d^2}{dR^2}+k_0^2(R)\right)\alpha_0=\frac{1}{\alpha_0^3},
\qquad
\alpha_0^2\frac{d\beta_0}{dR}=1,
\tag{A2}
$$

with local wave number

$$
k_0(R)=\sqrt{\frac{2\mu}{\hbar^2}[E-V_0(R)]}.
\tag{A3}
$$

The bound-state wave function $\phi_b$ is likewise described as

$$
\phi_b(R)=\sqrt{\frac{\partial E}{\partial\nu}}\,f_b(R),
\tag{A4}
$$

$$
f_b(R)=\sqrt{\frac{2\mu}{\pi\hbar^2}}\alpha_b(R)\sin\beta_b(R),
\tag{A5}
$$

with $\alpha_b$ and $\beta_b$ satisfying equations similar to Eq. (A2). In terms of these Milne functions, the expression for the linewidth becomes

$$
\Gamma=2\pi\left(V_{0b}^{\mathrm{rad}}\right)^2
\left(\frac{\partial E}{\partial n}\right)
\left(\frac{2\mu}{\pi\hbar^2}\right)|I_{0b}|^2,
\tag{A6}
$$

in terms of the integral

$$
I_{0b}\equiv\int_0^\infty dR\,\alpha_0(R)\alpha_b(R)\sin\beta_0(R)\sin\beta_b(R)
\tag{A7}
$$

$$
\simeq\frac{1}{2}\int_0^\infty dR\,\alpha_0(R)\alpha_b(R)\cos(\beta_0-\beta_b),
\tag{A8}
$$

where we have neglected rapidly oscillating $\cos(\beta_0+\beta_b)$ terms in comparison to $\cos(\beta_0-\beta_b)$ terms. Note that Eq. (2.15)'s factor $\partial E/\partial(\nu/\pi)$ is replaced here by $\partial E/\partial n$, the actual density of vibrational levels.

The basic idea of the reflection approximation is that rapid oscillations of the integrand in Eq. (A7) keep contributions to the integral near zero except when $R$ is near the Condon point, $R_C$, which is the point of stationary phase. In the field-dressed picture described in Sec. II B, $R_C$ is the radius at which the potentials $V_0$ and $V_b$ cross. We, therefore, expand the phase difference $\beta_0-\beta_b$ near $R\simeq R_C$:

$$
\beta_0-\beta_b\simeq b_0+b_1(R-R_C)+\frac{b_2}{2}(R-R_C)^2+\cdots.
\tag{A9}
$$

To evaluate the expansion coefficients, it helps to think in terms of WKB approximations to the phases, namely,

$$
\beta_b\simeq\int_{R_C}^{R}dR'\,k_b(R')-\frac{\pi}{4}.
\tag{A10}
$$

We then find [34]

$$
b_0\simeq \beta_0(R_C)+\frac{\pi}{4},
\tag{A11}
$$

$$
b_1\simeq \left.\frac{1}{\alpha_0^2}\right|_{R_C}-\left.k_b\right|_{R_C}\simeq0,
\tag{A12}
$$

$$
b_2\simeq\left.\frac{\partial k_0}{\partial R}\right|_{R_C}
-\left.\frac{\partial k_b}{\partial R}\right|_{R_C}
\simeq \left.\frac{\mu}{\hbar^2 k_b}\frac{\partial V_b}{\partial R}\right|_{R_C}.
\tag{A13}
$$

Approximation (A12) asserts that the radial kinetic energy in each channel is nearly the same at $R=R_C$, while approximation (A13) notes that $\partial V_0/\partial R$ is vanishingly small compared to $\partial V_b/\partial R$ near the Condon point. We further define

$$
b_2\simeq\frac{\mu D_C}{\hbar^2 k_b},
\qquad
D_C\equiv\left.\frac{\partial V_b}{\partial R}\right|_{R_C}.
\tag{A14}
$$

Our integral (A8) then becomes

$$
I_{0b}\simeq\frac{1}{2}\int_0^\infty dR\,\alpha_0(R)\alpha_b(R)
\cos\left[b_0+\frac{b_2}{2}(R-R_C)^2\right].
\tag{A15}
$$

This integrand is strongly peaked around $R=R_C$, meaning we can further approximate

$$
I_{0b}\simeq\frac{1}{2}\alpha_0(R_C)\alpha_b(R_C)\sqrt{\frac{2\pi}{b_2}}\cos(b_0+\pi/4),
\tag{A16}
$$

where we have used

$$
\int_0^\infty dx\,\cos(x^2)=\int_0^\infty dx\,\sin(x^2)=\frac{1}{2}\sqrt{\frac{\pi}{2}}.
\tag{A17}
$$

Inserting Eqs. (A11) and (A13) for $b_0$ and $b_2$, and using the WKB expression $\alpha_b=1/\sqrt{k_b}$, Eq. (A16) yields for the linewidth,

$$
\Gamma=2\pi\left(V_{0b}^{\mathrm{rad}}\right)^2
\left(\frac{\partial E}{\partial n}\right)
\frac{|f_0(R_C)|^2}{D_C}.
\tag{A18}
$$

As has been noted before, photoassociation line strengths are a direct probe of the ground-state wave function's magnitude near the Condon point, and can thus be used to estimate scattering lengths [38].

There remains only to estimate the energy shift (3.5). In the language developed above, this quantity reads

$$
E_1=-2\pi\left(V_{0b}^{\mathrm{rad}}\right)^2
\left(\frac{\partial E}{\partial n}\right)
\left(\frac{2\mu}{\pi\hbar^2}\right)^2I_{0b}^{(2)},
\tag{A19}
$$

in terms of the "second-order" integral,

$$
\begin{aligned}
I_{0b}^{(2)}={}&\int_0^\infty dR\,\alpha_b(R)\sin\beta_b(R)(-1)\alpha_0(R)\cos\beta_0(R) \\
&\times\int_0^R dR'\,\alpha_0(R')\sin\beta_0(R')\alpha_b(R')\sin\beta_b(R').
\end{aligned}
\tag{A20}
$$

Again neglecting rapidly oscillating phases, this integral becomes

$$
\begin{aligned}
I_{0b}^{(2)}\simeq{}&\frac{1}{4}\int_0^\infty dR\,\alpha_b(R)\alpha_0(R)
\sin\left[b_0+\frac{b_2}{2}(R-R_C)^2\right] \\
&\times\int_0^R dR'\,\alpha_0(R')\alpha_b(R')
\cos\left[b_0+\frac{b_2}{2}(R'-R_C)^2\right],
\end{aligned}
\tag{A21}
$$

in terms of the phase expansions defined above.

Now, the "inner" integrand in Eq. (A21) represents essentially a delta function in $R$, whereby the $R'$ integration yields a step function. The integral then simplifies to

$$
\begin{aligned}
I_{0b}^{(2)}\simeq{}&\frac{1}{4}\alpha_0(R_C)\alpha_b(R_C)\sqrt{\frac{2\pi}{b_2}}\cos(b_0+\pi/4) \\
&\times\int_{R_C}^{\infty}\alpha_b(R)\alpha_0(R)
\sin\left[b_0+\frac{b_2}{2}(R-R_C)^2\right]dR.
\end{aligned}
\tag{A22}
$$

Performing the integration a second time (note the different lower limit), the integral simplifies to

$$
I_{0b}^{(2)}\simeq\frac{1}{8}\left(\frac{2\pi}{b_2}\right)\alpha_b(R_C)^2\alpha_0(R_C)^2\cos(b_0+\pi/4)\sin(b_0+\pi/4).
\tag{A23}
$$

Again making the appropriate substitutions produces the final result:

$$
E_1\simeq\pi\left(V_{0b}^{\mathrm{rad}}\right)^2
\left(\frac{\partial E}{\partial n}\right)
\frac{f_0(R_C)g_0(R_C)}{D_C}.
\tag{A24}
$$

---

# References

[1] S. Chu, Rev. Mod. Phys. **70**, 685 (1998); C. N. Cohen-Tannoudji, ibid. **70**, 707 (1998); W. D. Phillips, ibid. **70**, 721 (1998).

[2] J. Weiner, V. S. Bagnato, S. Zilio, and P. S. Julienne, Rev. Mod. Phys. **71**, 1 (1999).

[3] B. Saubamea et al., Phys. Rev. Lett. **79**, 3146 (1997).

[4] C. L. Cesar et al., Phys. Rev. Lett. **77**, 255 (1996).

[5] K. M. Jones et al., Europhys. Lett. **33**, 85 (1996).

[6] H. R. Thorsheim, J. Weiner, and P. S. Julienne, Phys. Rev. Lett. **58**, 2420 (1987).

[7] R. Napolitano, J. Weiner, C. J. Williams, and P. S. Julienne, Phys. Rev. Lett. **73**, 1352 (1994).

[8] J. L. Bohn and P. S. Julienne, Phys. Rev. A **54**, R4637 (1996).

[9] Y. B. Band and P. S. Julienne, Phys. Rev. A **51**, R4317 (1995).

[10] R. Cote and A. Dalgarno, Chem. Phys. Lett. **279**, 50 (1997).

[11] A. Vardi et al., J. Chem. Phys. **107**, 6166 (1997).

[12] P. S. Julienne, K. Burnett, Y. B. Band, and W. C. Stwalley, Phys. Rev. A **58**, R797 (1988).

[13] J. T. Bahns, W. C. Stwalley, and P. L. Gould, J. Chem. Phys. **104**, 9689 (1996).

[14] P. O. Fedichev, Yu. Kagan, G. V. Shlyapnikov, and J. T. M. Walraven, Phys. Rev. Lett. **77**, 2913 (1996).

[15] J. L. Bohn and P. S. Julienne, Phys. Rev. A **56**, 1486 (1997).

[16] F. H. Mies, J. Chem. Phys. **80**, 2514 (1983).

[17] R. Napolitano, Phys. Rev. A **57**, 1164 (1998).

[18] F. H. Mies, in *Theoretical Chemistry: Advances and Perspectives*, edited by D. Henderson (Academic, New York, 1981), Vol. 6B.

[19] M. Trippenbach, B. Gao, J. Cooper, and K. Burnett, Phys. Rev. A **45**, 6539 (1992); **45**, 6555 (1992).

[20] M. L. Du and A. Dalgarno, Phys. Rev. A **43**, 3474 (1991).

[21] J. P. Burke, J. L. Bohn, and C. H. Greene, Phys. Rev. Lett. **81**, 3355 (1998).

[22] M. Cavagnero, Phys. Rev. A **50**, 2841 (1994).

[23] B. Gao, Phys. Rev. A **54**, 2022 (1996).

[24] M. Aymar, C. H. Greene, and E. Luc-Koenig, Rev. Mod. Phys. **68**, 1015 (1996).

[25] F. Calogero, *Variable Phase Approach to Potential Scattering* (Academic, New York, 1967), Chap. 9.

[26] V. K. Babamov, J. Chem. Phys. **69**, 3414 (1978).

[27] J. L. Bohn, Phys. Rev. A **49**, 3761 (1994).

[28] E. L. Ince, *Ordinary Differential Equations* (Dover, New York, 1956).

[29] P. S. Julienne and F. H. Mies, J. Phys. B **14**, 4335 (1981).

[30] E. R. I. Abraham, W. I. McAlexander, C. A. Sackett, and R. G. Hulet, Phys. Rev. Lett. **74**, 1315 (1995).

[31] W. I. McAlexander, E. R. I. Abraham, and R. G. Hulet, Phys. Rev. A **54**, R5 (1996).

[32] E. Tiesinga et al., J. Res. Natl. Inst. Stand. Technol. **101**, 505 (1997).

[33] U. Fano, Phys. Rev. **124**, 1866 (1961).

[34] P. S. Julienne, J. Res. Natl. Inst. Stand. Technol. **101**, 487 (1996).

[35] To ensure agreement with the full coupled-channels model, we have also included the energy shift due to artificial channel coupling. This shift is computed in exactly the same way as the physical shift, but by replacing $f_0$ and $g_0$ in Eq. (3.5) by the artificial channel wave functions $f_a$ and $g_a$, and by replacing the laser coupling $V_{0b}^{\mathrm{rad}}$ by the spontaneous emission coupling $V_{ab}^{\mathrm{artif}}$.

[36] A. Jablonski, Phys. Rev. **68**, 78 (1945).

[37] W. E. Milne, Phys. Rev. **35**, 863 (1930); F. Robicheaux, U. Fano, M. Cavagnero, and D. A. Harmin, Phys. Rev. A **35**, 3619 (1987).

[38] R. Cote, A. Dalgarno, Y. Sun, and R. G. Hulet, Phys. Rev. Lett. **74**, 3581 (1995).
