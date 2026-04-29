https://pmc.ncbi.nlm.nih.gov/articles/PMC4963139/
## Cold Binary Atomic Collisions in a Light Field

**Paul S. Julienne**

*National Institute of Standards and Technology, Gaithersburg, MD 20899-0001*

The rate coefficients are calculated for trap loss due to excited state formation during s-wave collisions of two atoms in a light field in a cold atomic gas near conditions for formation of a Bose-Einstein condensate. Blue detuning from the allowed atomic resonance transition causes excitation of a repulsive molecular potential, whereas red detuning causes excitation when the light is tuned near a bound vibrational energy level of an attractive molecular potential. In either case, when the light intensity is low and the detuning is large compared to the natural linewidth of the atomic transition, the rate coefficient for the collisional loss rate is proportional to a molecular Franck-Condon factor. A simple reflection approximation formula is derived which permits the rate coefficient to be given analytically in either case. The Franck-Condon factor is equal to $|\Psi_g(R_C)|^2/D_C$, where $\Psi_g(R_C)$ is the ground state scattering wavefunction at the Condon point $R_C$, where the quasimolecule is in resonance with the exciting light, and $D_C$ is the slope difference between ground and excited potentials at $R_C$. The analytic reflection approximation formula, as well as a simple phase-amplitude formula for the intermediate range wavefunction, give excellent agreement with the results of numerical quantum mechanical calculations. The trap loss rates due to binary collisions are comparable to or exceed those due to atomic recoil heating for a wide range of detunings to the blue of atomic resonance and near the peaks of photoassociation resonances for the case of red detuning.

**Key words:** binary atomic collision; Bose-Einstein Condensation; cold trapped atoms; Franck-Condon factor; photoassociation spectrum; spectral line shape.

**Accepted:** May 15, 1996

## 1. Introduction

Atomic collisions play a crucial role in the phenomena of Bose-Einstein condensation (BEC) [1–3]. Elastic momentum-transfer collisions control the rate of evaporative cooling leading to the high phase-space density required for the formation of a condensate. The ground state scattering length, also a property of elastic collisions, controls the nonlinear coupling parameter in the nonlinear Schrodinger equation for the condensate wavefunction [4]. Inelastic collisions among condensate atoms also determine a lower bound to the loss rate of the condensate (other processes may contribute to loss as well) and thereby help determine the condensate lifetime. Therefore, it is crucial to understand these ground state collisions. Calculating their rates requires that we be able to compute the ground state scattering wavefunction. Although these collisions occur in the absence of light, photoassociation spectroscopy offers a powerful probe of the ground state wavefunction [5–8]. Light also has the prospect for being an important probe of condensate properties and for manipulating a condensate or even the collisions within a condensate. Therefore, it is crucially important to understand how light affects the atoms in a cold, dense atomic gas near the BEC regime.

This article will be concerned with understanding the rates of binary collisions in a weak, off-resonant light field in a cold atomic gas. Since only the case of a weak radiation field is treated, the effect of light on the binary collision can be described perturbatively. The case of a strong saturating field will be treated separately [9]. The detuning is assumed to be large enough compared to the natural atomic linewidth $\gamma_A$ and the density $N$ moderate enough that binary events are sufficiently isolated that three-body collisions can be ignored, as well as collective effects [10]. Certainly, considering binary events is the first step in understanding the effect of light on interacting atoms. The object is to provide a simple framework with which to understand these binary events. They would need to be incorporated at a later stage into a more comprehensive understanding of the dynamics and stability of an atomic gas near BEC. Elsewhere, we give a brief account of the possibility of using photoassociation spectroscopy to probe many-body interactions in a condensate [11].

Another important reason for having a simple model for understanding these binary collisions in a light field is to understand how spectroscopic methods can be used as an experimental tool for probing the ground state scattering wavefunction. In particular, we have proposed that high resolution photoassociation spectroscopy would provide an especially sensitive probe of the ground state potential and scattering properties [5]. In fact, this technique has been used to place bounds on scattering lengths for Li [8], Rb [6], and Na [12, 13] ground state collisions. Even tighter bounds should be possible with improved experiments. In particular, we will show below how the spectroscopy of very cold gases might be used to measure properties of the ground state wavefunction.

The primary effect of light on cold trapped atoms is to cause loss processes by giving the atoms enough energy to escape the trap. For example, a single atom scatters light of frequency $\omega$ detuned $\Delta_A = \omega - \omega_A$ from the atomic resonance frequency $\omega_A$ at the rate,

$$
\gamma_{\text{atomic}} = \gamma_A \left( \frac{\Omega_A}{\Delta_A} \right)^2,\tag{1}
$$

where $\Omega_A = \sqrt{2\pi I / c} \, d_A$ is the Rabi frequency at laser intensity $I$ for the atomic transition with transition dipole $d_A$, and we assume $|\Delta_A| \gg \Omega_A$ and $|\Delta_A| \gg \gamma_A$; $\Delta_A$ is defined so as to be positive for blue detuning and negative for red. Since each scattering event gives a recoil momentum kick of $\hbar k_\omega = \hbar \omega / c$ to the atom, and since the thermal momentum of the atom is comparable to, or smaller than, $\hbar k_\omega$, this atomic light scattering heats the atoms, causing their loss from the trap.

Binary events also cause loss of atoms from a trap, but with a rate which is very different for the cases of red and blue detuning. Figure 1 illustrates the two cases schematically, using the molecular potential energy curves for the quasimolecule comprised of the two colliding atoms. Blue detuning excites the ground state atoms to a repulsive molecular state, causing the production of excited atoms with kinetic energy $E_c = E_g + \hbar \Delta_A$. This heating has been discussed in the context of optical shielding [14,15,9]. The probability for this free-free process is a smooth function of detuning. On the other hand, red detuning excites the ground state atoms to a bound eigenstate of the attractive molecular state. This only happens with high probability if the light is tuned close to exact resonance with the energy $E_v$ of the bound vibrational state $v$. Since the decay of the bound state mostly leads to products that are not trapped, this process gives rise to a trap-loss photoassociation spectrum, which is now well studied for the alkali dimers [16–21]. The probability for this free-bound process is a sharply peaked function of detuning. We have every reason to expect that a gas near BEC conditions, or even a condensate itself, will possess a detailed photoassociation spectrum for detuning on the red side of $\omega_A$.

When the laser intensity $I$ is sufficiently low, the probability for both red and blue detuning loss processes can be described by a Franck-Condon factor between the ground and the excited state radial wavefunctions. For both cases, we will give here a very simple analytic expression for the Franck-Condon factor that is in excellent agreement with fully quantal calculations. We will show that the Franck-Condon factor is proportional to $|\Psi_g(R_C, E)|^2$, the square of the ground state wavefunction at the Condon point $R_C$, where the quasimolecule is in exact resonance with the light. At $R_C$ the difference between excited and ground potentials exactly matches $\hbar\omega$. Our expression for the binary collision rate exhibits the proper quantum threshold law behavior as $E \to 0$. It predicts that the binary collisional loss rate per atom, $\gamma_{\text{binary}}$, also varies as $\Delta_A^{-2}$ and at typical BEC densities generally is comparable to or exceeds the atomic scattering rate, Eq. (1), for a wide range of blue detuning and greatly exceeds the atomic scattering rate when $\omega$ is tuned near a photoassociation resonance.

We will first describe the model and the basic properties of the ground state wavefunction. Then we will discuss the binary collision rates for the case of blue detuning and the reflection approximation for the free-free Franck-Condon factors. Then we will describe the modifications needed to describe the case of red detuning and free-bound Franck-Condon factors. Finally, we will consider some of the implications for a cold atomic gas near BEC.

## 2. Model

The binary collision rates for the two cases described in Fig. 1 will be expressed in terms of Franck-Condon factors between the ground and excited state wavefunctions. However, it is very desirable to formulate the problem using the field-dressed molecular picture of a collision in a light field. This procedure is well-documented elsewhere [22–27], even for cold collisions [28–30,5,14], and need not be described in detail here. A two-state model with a single ground state and a single molecular excited state will be assumed. In the weak-field limit it is straightforward to generalize to multichannel ground and excited states for real alkali systems with hyperfine structure. In fact, we have now developed computer codes that let us include both ground and excited state molecular hyperfine structure for alkali species for optical transitions in the weak field limit [12, 13]. The ground state potential is $V_g(R)$ and the excited state potential is $V_e(R) - \hbar \Delta_A$, where both $V_g$ and $V_e \to 0$ as $R \to \infty$. The ground and excited states are coupled optically by the interaction matrix element $\hbar \Omega(R)$, where the molecular Rabi frequency is

$$
\Omega(R) = \sqrt{2\pi I/c} \, d(R) = b(R)\Omega_A,\tag{2}
$$

where $d(R)$ is the molecular transition dipole, and $0 \leq b(R) \leq 2/\sqrt{3}$ relates the molecular and atomic Rabi frequencies. The particular value of $b$ depends on the molecular states involved. The ground and excited dressed potentials cross at the Condon point $R_C$, the point of quasimolecular resonance, where in the undressed picture of Fig. 1, the difference of upper and lower potential curves matches the photon energy $\hbar\omega$:

$$
\hbar\omega_A + V_e(R_C) - V_g(R_C) = \hbar\omega\tag{3}
$$

$$
V_e(R_C) - V_g(R_C) = \hbar\Delta_A.\tag{4}
$$

In this paper we will carry out purely model illustrative calculations. For this purpose it is sufficient to use analytic Lennard-Jones potentials for the ground and excited states,

$$
V_i(R) = 4\epsilon_i \left( \left( \frac{\sigma}{R} \right)^{2n} - \left( \frac{\sigma}{R} \right)^n \right),\tag{5}
$$

$i = g$ or $e$ and $n = 6$ for the ground state van der Waals potential and $n = 3$ for the excited state resonant dipole potential. The long range variation is $C_6/R^6$ and $C_3/R^3$ respectively. We use a reduced mass characteristic of sodium. It is difficult to show on one graph the potentials over the very large range of energy and distance involved in cold collisions. Figure 2 shows on a logarithmic scale the magnitude $|V(R)|/k_B$ (where $k_B$ is the Boltzmann constant) of the long range potentials for the ground and excited states of the Na$_2$ molecule, for which we take $C_6 = 1500$ atomic units ($e^2a_0^5$, where $e =$ electron charge and $a_0 =$ Bohr radius = 0.0529 nm) and $|C_3| = 10$ atomic units ($e^2a_0^2$). Figure 3 shows on a linear scale the ground and attractive and repulsive excited state potentials, as well as illustrative wavefunctions for each. Since the excited potential is orders of magnitude stronger than the ground state at long range, it is an excellent approximation to neglect the ground state contribution in calculating the Condon point:

$$
|\Delta_A| = \frac{|C_3|}{R_C^3} \implies R_C = \left| \frac{C_3}{\Delta_A} \right|^{1/3}.\tag{6}
$$

Figure 2 also indicates the detunings associated with each $R$, taken as a Condon point. Note that the ground state interaction strength is not negligible at intermediate $R$, but is stronger than 1 μK whenever $R$ is less than about 300 $a_0$.

## 3. Ground State Wavefunction

### 3.1 Long Range Form

We need the ground state wavefunction to use in the reflection formula for the Franck-Condon factors we derive below. When the collision energy $E$ is low enough, only collisions with zero relative angular momentum of nuclear motion contribute to scattering cross sections. The $s$-wave ground state wavefunction takes on the following well-known behavior as $R \to \infty$:

$$
\left| \Psi_{\text{g}}^{\dagger}(E) \right\rangle \sim e^{i\eta_{\text{g}}} \left( \frac{2\mu}{\pi\hbar^2} \right)^{1/2} \frac{\sin(k_{\infty}R + \eta_{\text{g}})}{\sqrt{k_{\infty}}},
$$

where the $\sqrt{2\mu / \pi\hbar^2 k_\infty}$ factor ensures energy normalization,
$|\langle \Psi_g^+ (E) | \Psi_g^+ (E') \rangle|^2 = \delta(E - E')$.

The asymptotic kinetic energy is $E = \hbar^2 k_\infty^2 / 2\mu$, where $\mu = m_A / 2$ is the reduced mass, the deBroglie wavelength is $\lambda_\infty = 2\pi / k_\infty$, and the velocity $v_\infty = \hbar \, k / \mu$. It is sometimes more convenient to write the energy normalization factor as

$$
\left( \frac{2\mu}{\pi\hbar^2 k_\infty} \right)^{1/2} = \frac{2}{(hv_\infty)^{1/2}}.
$$

If $E$ is small enough, the asymptotic phase $\eta_g = n\pi - k_g A_s$, where $A_s$ is the scattering length and $n$ is the number of bound states supported by the ground state potential; the $n\pi$ term can be ignored, since it only introduces an inessential phase factor. The scattering length is a property of the whole potential and for real atoms is very sensitive to small uncertainties in the short range, chemical bonding, range of $R$. However, the scattering length provides a good parameter to characterize the effect on the long range wavefunction of the complete potential.

Figure 4a illustrates typical ground state wavefunctions (in their real form without the trivial complex phase factor $e^{i\eta_s}$) with positive, zero, and negative scattering lengths. These were calculated by making slight changes in the model potential parameters. The inner region wavefunction, say for $R < 30 \, a_0$, is characterized by rapid oscillations as the local kinetic energy increases due to the acceleration by the attractive ground state potential. The intermediate range wavefunction, say for $80 \, a_0 < R < \lambda_x/4$, is nearly linear in $R$ and extrapolates to an intercept near $R = A_s$:

$$
\Psi_g^+ (R, E) \approx e^{i\eta_s} \left( \frac{2\mu}{\pi\hbar^2} \right)^{1/2} \frac{k_{\infty}(R - A_s)}{\sqrt{k_{\infty}}}.\tag{9}
$$

A much more accurate representation of the ground state wavefunction in the intermediate range is found by correcting for the variation in phase and amplitude due to the nonzero ground state potential. The details of this derivation, based on an approximate treatment of the rigorous Milne equation for the phase-amplitude form of the wavefunction, are given in Appendix A. The result is that a more correct form of the long range wavefunction is found from Eqs. (60), (69), and (72):

$$
\Psi_g^+ (R, E) = e^{i\eta_s} \left( \frac{2\mu}{\pi\hbar^2 k_{\infty}} \right)^{1/2} \times a(R) \sin(k_{\infty} \rho(R)),\tag{10}
$$

where

$$
a(R) = 1 - \left( \frac{R_B}{R} \right)^4\tag{11}
$$

$$
\rho(R) = R - A_s - \frac{2}{3} \left( \frac{R_B}{R} \right)^4 R.\tag{12}
$$

Equation (10) only applies in the region $R \gg R_B$ so that the correction term $(R_B/R)^4 \ll 1$, where

$$
R_B = \left( \frac{\mu C_6}{10\hbar^2} \right)^{1/4}\tag{13}
$$

is a constant independent of energy with dimensionality of distance. It has a value of 42 $a_0$ for Na and 77 $a_0$ for Rb. Figure 5 compares the exact wavefunction and the result of Eq. (10) in the near linear region between 60 $a_0$ and 120 $a_0$ for a model Na potential with $A_s = +84.3 \, a_0$. Such a magnitude of $A_s$ is near the actual value for doubly spin-polarized Na [31,32,12]. The actual wavefunction node at 87.5 $a_0$ is shifted 3.2 $a_0$ further out than $A_s$, as accurately predicted by Eqs. (10) and (74). A much larger shift of 18 $a_0$ in node position is predicted for $^{87}\text{Rb}$.

### 3.2 Short Range Form

Before leaving this discussion of the ground state wavefunction, it is useful to comment on the nature of the short range wavefunction as $E \to 0$. When the collision energy $E$ decreases towards zero, there will always be a characteristic quantum threshold connection between the asymptotic and short range wavefunction. It is possible to define a characteristic distance $R_Q$ where the WKB connection between the asymptotic and short range wavefunctions strongly breaks down for collision energies $E < E_Q$ [33, 34]. A necessary condition for onset of the threshold law behavior is $E \ll E_Q$. The values of $R_Q$ and $E_Q$ are determined by requiring that the maximum in the function $d\lambda(R, E)/dR$ satisfy the following condition:

$$
\frac{d\lambda(R_Q, E_Q)}{dR} = \frac{1}{2}. \tag{14}
$$

where the local deBroglie wavelength $\lambda(R, E)$ is defined by Eq. (63) in the Appendix A. For all $E < E_Q$ there is a range of distances around $R_Q$ where $d\lambda(R, E)/dR > 1/2$ and the WKB approximation fails. Using Eqs. (17) and (18) of [34],

$$
R_Q = \frac{20^{1/4}}{2^{1/2}(7a)^{1/6}} \quad R_B = 1.043 \, R_B, \tag{15}
$$

where $a = \frac{1}{27} \left( \frac{14}{3} \right)^3 \left( \frac{7}{2} \right)^{1/2} = 7.0419$. Thus, we find that $R_B = 0.96R_Q$, independent of potential parameters (since both have identical scalings with $C_6$ and $\mu$), and the defined parameters $R_B$ and $R_Q$ turn out to be fortuitously very close in magnitude. Since each of these only defines a qualitative range of distance associated with a change in the wavefunction, they can be used interchangeably. The WKB breakdown region is actually very broad (An example for a He mass is in Fig. 3 of Ref. [33]), and becomes broader as energy is lowered below $E_Q = 19 \, \text{mK}$ for Na or $E_Q = 1.5 \, \text{mK}$ for Rb [34]. Therefore, significant departure from the WKB form begins at distances well to the right of $R_Q$, and Eqs. (10) and (11) show that the amplitude of the intermediate range wavefunction remains much closer to its asymptotic amplitude $\propto 1/\sqrt{k_\infty}$ than to the local WKB amplitude $\propto 1/\sqrt{k(R, E)}$. Thus, the amplitude of the ground state wavefunction does not appreciably exhibit the acceleration due to the ground state potential unless $R$ is on the order of or less than $R_Q \approx R_B$. This is one of the reasons why a semiclassical analysis fails in the long range region as $E \to 0$.

The form of the wavefunction in Eq. (60) is completely rigorous at all distances and energies, providing that the Milne equation described in Appendix A is solved exactly. References [33, 34] show that the ground state wavefunction for the inner region $R \ll R_Q$ is well approximated by the form

$$
\Psi_g^+(R, E) = (A_i k_\infty)^{1/2} e^{i \eta _g} \left( \frac{2\mu}{\pi \hbar^2} \right)^{1/2} a_g^{\text{WKB}}(R, E) \times \sin(\beta_g^{\text{WKB}}(R, E))\tag{16}
$$

$$
= (A_i k_\infty)^{1/2} \Psi_g^{\text{WKB}^+}(R, E = 0), \tag{17}
$$

where $A_i$ is an energy-independent constant having the dimension of length and $a_g^{\text{WKB}}(R, E) = 1/\sqrt{k_g(R, E)}$ is the WKB amplitude. Equation (16) shows that the overall shape of the inner range wavefunction, $\Psi_g^{\text{WKB}^+}(R \ll R_Q)$, is independent of energy, whereas the overall amplitude decreases as $(A_i k_\infty)^{1/2}$ as $E \to 0$. This is illustrated in Fig. 4b, which shows a scattering wavefunction near threshold and the wavefunction for the last bound state, both normalized at short range to the same WKB form. Scattering wavefunctions near threshold, as well as the last bound state wavefunction, when given this common normalization, are almost indistinguishable for $R < R_Q$. The physical reason for this is that the local amplitude and phase are determined by the ground state potential in a region where it is very deep compared to the initial collision energy or bound state binding energy.

Both the inner range and outer range approximate wavefunctions, Eqs. (16) and (10), are proportional to $\sqrt{k_{\infty}}$, in accordance with the threshold law requirement that the ground state wavefunction for $R \ll 1/k_{\infty}$ everywhere vanishes as $\sqrt{k_{\infty}}$. This ensures that the probability for inelastic processes due to the ground state entrance channel vanish as $k_{\infty}$ as $E \to 0$. This is the basic threshold law for inelastic collision rates which must be satisfied for light-induced inelastic events for either red or blue detuning.


## 4. Collisions for Blue Detuning

The case of cold collisions in a blue detuned light field has been extensively studied recently, both experimentally and theoretically [14,15,9,35–41]. Figure 4a shows the ground and excited state potentials for the case of a very large detuning of $5 \, \text{cm}^{-1}$, or $300 \, \text{GHz}$, from atomic resonance. If the light intensity is strong enough (this will be defined more precisely below), the ground state atoms approaching one another encounter an effective repulsive interaction near the Condon point $R_C$ and are repelled. This gives rise to the phenomenon of optical shielding [15,9,35–41], by which the light prevents the atoms from approaching closer than $R_C$, thereby reducing the rate of ground state processes which require the atoms to be closer together than $R_C$. The light also modifies the ground state elastic scattering rate and scattering length, and results in the creation of hot excited state atoms which share the kinetic energy released, $\hbar \Delta_A$ [14,15,9]. Since we are considering the weak field limit here, the shielding effect is small and we will concentrate on the latter energy release process. The event rate coefficient for this process is

$$
K_c(\Delta_A) = \left\langle \frac{\pi v_g}{k_g^2} P_e(E, \Delta_A) \right\rangle = \left\langle \frac{\pi \hbar}{\mu k_g} P_e(E, \Delta_A) \right\rangle, \tag{18}
$$

where the brackets imply an average over the distribution of ground state velocities $v_g$, and

$$
P_e(E, \Delta_A) = |S_{eg}(E, \Delta_A)|^2 \tag{19}
$$

is the probability for the event by which two ground state atoms collide in a light field and produce one excited and one ground state atom, both of which have enough kinetic energy to escape any weak trapping potential.

When the radiative coupling is small, the radiative distorted wave approximation [24,26,27], can be used for the $S$-matrix element:

$$
S_{\text{eg}}(E, \Delta_A) = -2\pi i \langle \Psi_{\text{e}}(E + \hbar\Delta_A) | V_{\text{eg}}(R) | \Psi_{\text{g}}(E) \rangle, \tag{20}
$$

where $V_{\text{eg}}(R) = \hbar\Omega(R)$ from Eq. (2). The kinetic energy in the asymptotic ground and excited state channels are $E$ and $E + \hbar\Delta_A$ respectively. The asymptotic excited state wavefunction is:

$$
\left| \Psi_{\text{e}}(E, \Delta_A) \right\rangle \sim e^{-i\eta_e} \left( \frac{2\mu}{\pi\hbar^2 k_{e,\infty}} \right)^{1/2} \sin(k_{e,\infty}R + \eta_e). \tag{21}
$$

The ground and excited state wavefunctions are also illustrated in Fig. 6a. The excited state wavefunction oscillates much more rapidly than the ground state one because of the much greater kinetic energy in the exit channel.

By assuming that the radiative coupling $V_{\text{eg}}(R)$ is either independent of $R$ or slowly varying with $R$ near $R_C$, then this term can be removed from the integrand in Eq. (20), giving the radiative distorted wave result that

$$
P_e(E, \Delta_A) = 4\pi^2 V_C^2 |\langle \Psi_e(E, \Delta_A) | \Psi_g^+ (E) \rangle|^2 \tag{22}
$$

$$
= 4\pi^2 V_C^2 F_{eg}(E, \Delta_A), \tag{23}
$$

where $V_C = V_{eg}(R_C)$ and

$$
F_{eg}(E, \Delta_A) = |\langle \Psi_e(E, \Delta_A) | \Psi_g^+ (E) \rangle|^2 \tag{24}
$$

is a free-free Franck-Condon factor. Although direct evaluation of $F_{eg}$ by numerical quadrature does not converge, since both wavefunctions oscillate with finite amplitude to $R = \infty$, there are several methods available for evaluating $F_{eg}$ numerically [27], as well as approximate formulas based on the local nature of the integrand near the Condon point $R_C$. Here we use a two-state close coupled scattering calculation of the collision in a weak radiation field with an $R$-independent Rabi frequency, and extract $S_{eg}(e)$ from the asymptotic field-dressed wavefunction [24–27]. Then the Franck-Condon factor, independent of the laser intensity chosen for the calculation, is calculated from:

$$
F_{\text{eg}}(E, \Delta_A) = \frac{|S_{\text{eg}}(E, \Delta_A)|^2}{4\pi^2 V_C^2}, \tag{25}
$$

where $S_{\text{eg}}(E, \Delta_A)$ is calculated using a standard close coupling scattering code. This method can be generalized to a multichannel version when there are more than two channels [27], and thus could be used for atoms with hyperfine structure [12, 13].

Figure 7 shows $F_{\text{eg}}$ calculated for collision energy $E/k_B = 2 \, \mu K$ using a model ground state potential with the reduced mass for Na collisions and a calculated scattering length of +84.3 $a_0$. The detuning range corresponding to $R = 20 \, a_0$ to 200 $a_0$ is 8 THz to 8 GHz. The Franck-Condon pattern shows an oscillatory pattern versus $R_C$ or detuning.




## 5. Reflection Approximation

We will now turn our attention to developing approximations that will give considerable physical insight into the nature of light scattering at very low collision energy. Let us first look at semiclassical approximations. We will assume a single Condon point $R_c$. Thus, our analysis does not apply to states with significant contributions from two Condon points, such as the low vibrational levels of the $0_g^-$ state of Na$_2$ [12, 13]. A semiclassical approximation for the free-free Franck-Condon factor $F_{\text{eg}}^{\text{SC}}(E)$ is given by Eq. (46) of the reference [42] (we remove the uninteresting $V_c^2$ factor):

$$
F_{\text{eg}}^{\text{SC}}(E, \Delta_A) = \frac{2}{h v_c D_c}, \tag{26}
$$

where

$$
D_c = \left| \frac{d}{dR}(V_e(R) - V_g(R)) \right|_{R=R_C} \tag{27}
$$

$$
\approx \frac{3C_3}{R_C^4} = \frac{3}{R_C} |\Delta_A| \tag{28}
$$

is the difference in potential slopes evaluated at $R_C$ and $v_c = v_g(R_c) = \sqrt{2(E - V_g(R_c)/\mu)}$ is the local velocity at $R_c$. The second equation follows from neglecting $V_g$ in comparison to $V_e$. The corresponding semiclassical treatment in the field-dressed picture of Fig. 6a is given by the Landau-Zener (LZ) approximation [14,15,9] for $P_e$:

$$
P_e^{\text{LZ}}(E, \Delta_A) = 2 \, e^{-A_c} (1 - e^{-A_c}) \approx 2 \, A_c. \tag{29}
$$

The latter approximation applies when the dimensionless LZ adiabaticity parameter

$$
A_c = \frac{4\pi^2 V_c^2}{h v_c D_c} \tag{30}
$$

is small compared to unity. This condition also ensures the low intensity regime of linear variation of $P_e$ with light intensity. Using Eq. (25) to obtain $F_{eg}^{\text{SC}}(E)$ from Eq. (29) gives exactly the same expression as in Eq. (26). Note that both Eqs. (26) and (30) have left out the phase factor $\sin^2(\beta_g(R_C) - \beta_e(R_C))$. Actually, the phase factor has been replaced by its average value, 1/2. Note that $P_e^{\text{LZ}}$ given by Eq. (29), even with the phase factor, does not satisfy the threshold law requirement to vary as $k_\infty$ as $E \to 0$. In fact, $F_{eg}^{\text{SC}}(E)$ from Eq. (26) is in very poor agreement with the quantum mechanical $f_{eg}(E)$ in Fig. 7 and is not shown in the figure.

The usual stationary phase derivation of Eq. (26) can be adapted to give the correct threshold law as $E \to 0$. The details are given in Appendix B. The result is a key result of this paper, a simple reflection formula:

$$
F_{eg}^{\text{R}}(E, \Delta_A) = \frac{1}{D_C} |\Psi_g^+(R_C, E)|^2. \tag{31}
$$

The Franck-Condon factor is directly proportional to the square of the ground state wavefunction. It only depends on the excited state through the slope term $D_C$. This expression explicitly satisfies the threshold law, since at all distances $R \ll \lambda_\infty$, $|\Psi_g|^2$ is proportional to $k_\infty$ when $E$ is sufficiently smaller than $E_Q$ [33, 34]. When $R > R_Q$, the quantum wavefunction is well-approximated by Eqs. (10) – (12), and the intermediate range phase-amplitude approximation to $F_{\text{eg}}^R$ is:

$$
F_{\text{eg}}^{PA}(E, \Delta_A) = \frac{4}{h \nu_\infty D_C} a_c^2 \sin^2(k_\infty \rho_C). \tag{32}
$$

where $a_C = a(R_C)$ and $\rho_C = \rho(R_C)$. The basic difference between this formula and the Landau-Zener one, Eq. (26), other than the phase factor, is the presence of the asymptotic ground state velocity in the denominator instead of the local velocity $v_C$. If $R_C$ is in the range $R_Q \ll R_C \ll \lambda_\infty / 2$ so that the sin function is linear in its argument, then

$$
F_{\text{eg}}^{PA}(E, \Delta_A) = \frac{2\mu a_c^2 \rho_C^2}{\pi \hbar^2 D_C} k_\infty. \tag{33}
$$

The equivalent approximation for $P_e$ is found from Eq. (23),

$$
P_e(E, \Delta_A) = \frac{16\pi^2 V_C^2}{h \nu_\infty D_C} a_c^2 k_\infty^2 \rho_C^2. \tag{34}
$$

Figure 7 also shows the predictions of the $F^R$ and $F^{PA}$ formulas compared to the exact results for 2 μK collisions. The full reflection formula is an excellent approximation over a wide range of Condon points, and even remains very good into about 20 $a_0$ where the ground state has accelerated the atoms to a velocity much higher than their initial one. The $F^{PA}$ approximation formula is also excellent at intermediate range, until $R$ begins to approach $R_B \approx R_Q$. Figure 8 compares the exact and $F^{PA}$ results for other collision energies up to 2 mK. We see that the reflection approximation is very good for almost the whole range of temperatures encountered for trapped laser cooled atoms, including the $E \to 0$ limit.

## 6. Collisions for Red Detuning

We can carry out a very similar treatment for the case of the free-bound Franck-Condon factor for red detuning. Figure 6b illustrates the dressed potentials and wavefunctions for a red detuning case. The basic difference from blue detuning is that the attractive potential supports discrete bound states. When the laser frequency $\omega$ is tuned near the position of a particular bound level with vibrational quantum number $\nu$, the level can be excited and decay to some product $p$, which is no longer trapped. The decay process is primarily spontaneous emission leading to formation of molecular species or hot atoms [28, 42]. In the field dressed picture of Fig. 6b, the bound state is a scattering resonance embedded in the continuum very close to threshold. The rate coefficient for red detuning is also given by Eq. (18), but the $S$-matrix element is given by a modified resonant scattering form described by Napolitano et al. [5]:

$$
|S_{\text{pg}}(E, \nu, \Delta_A)|^2 = \frac{\gamma_p \gamma_s(E, \nu, \Delta_A)}{\left( \frac{E - \Delta_v}{\hbar} \right)^2 + (\gamma_v/2)^2}, \tag{35}
$$

where $\Delta_v$ is the detuning relative to the position $E_v$ of the bound state. The total decay rate of the excited bound state $\nu$ is $\gamma_\nu = \gamma_p + \gamma_s(E, \nu, \Delta_A) + \gamma_0$, where $\gamma_p$ is the rate by which the bound state resonance decays to the detected product, $\gamma_s(E, \nu, \Delta_A)$ is the stimulated emission rate back to the ground state continuum, and $\gamma_0$ is the decay rate due to any other undetected processes (such as molecular predissociation). The critical element for our purposes is the $\gamma_s(E, \nu, \Delta_A)$ factor, which describes how the cold colliding atoms couple to the excited bound state. For low light intensity, this factor is given by the Fermi golden rule expression [5]:

$$
\gamma_s(E, \nu, \Delta_A) = \frac{2\pi}{\hbar} |\langle \Psi_e(\nu) | V_{eg}(R) | \Psi_g^+(E) \rangle|^2, \tag{36}
$$

where $\Psi_e(\nu)$ is the unit-normalized bound state wavefunction of the excited bound state. Using the same factorization approximation as for Eq. (23), this can be written in terms of a bound-free Franck-Condon factor,

$$
\gamma_s(E, \nu, \Delta_A) = \frac{2\pi}{\hbar} V_C^2 |\langle \Psi_e(\nu) | \Psi_g^+(E) \rangle|^2 \tag{37}
$$

$$
= \frac{2\pi}{\hbar} V_C^2 F_{eg}(E, \nu, \Delta_A). \tag{38}
$$

The assumption is that $V_c^2$ is evaluated at a single Condon point; if there is more than one Condon point, the interference between the different amplitudes from each Condon point would need to be taken into account.

The derivation of the reflection approximation formula for the bound-free Franck-Condon factor $F_{eg}(E, \nu, \Delta_A)$ follows immediately from the same treatment in Appendix B that we used in deriving the free-free Franck-Condon factor. The essential difference is that the unit-normalized bound state wavefunction can also be written in energy-normalized phase-amplitude form just like Eq. (16), as is commonly done in generalized multichannel quantum defect theory [44]. It is only necessary to introduce the vibrational spacing

$$
\frac{\partial E_v}{\partial \nu} = h \nu_v, \tag{39}
$$

where $\nu_v$ is the vibrational frequency, the number of complete vibrational cycles per unit time. Then the unit normalized bound state wavefunction has the form [44]

$$
\Psi_e(R, \nu) = \left( \frac{\partial E_v}{\partial \nu} \right)^{1/2} \left( \frac{2\mu}{\pi \hbar^2} \right)^{1/2} \alpha_e(R, \nu) \sin(\beta_e(R, \nu)). \tag{40}
$$

where $\alpha$ and $\beta$ can be determined quantum mechanically from Eqs. (61) and (62), or alternatively, from the WKB form, Eq. (64). The derivation in Appendix A, adapted for a right hand turning point, carries through to give

$$
F_{eg}(E, \nu, \Delta_A) = \frac{\partial E_v}{\partial \nu} \frac{1}{D_C} |\Psi_g^+(R_C, E)|^2, \tag{41}
$$

where $\Psi_g^+(R_C, E)$ can be calculated exactly or taken from Eq. (10) above. The vibrational spacing function can be evaluated approximately from the discrete level spacing,

$$
\frac{\partial E_v}{\partial \nu} \approx \frac{E_{v+1} - E_{v-1}}{2}, \tag{42}
$$

or more rigorously from the wavefunction at some short range point $R_0$:

$$
\frac{\partial E_v}{\partial \nu} = \frac{\pi \hbar^2}{2\mu} \left( k_0 |\Psi_e(R_0, \nu)|^2 + \frac{1}{k_0} \left| \frac{d\Psi_e(R_0, \nu)}{dR} \right|^2 \right), \tag{43}
$$

where $k_0 = k_e(R_0)$. This equation immediately follows from Eq. (40) upon using the WKB forms in Eqs. (77)–(78). The result depends only weakly on the choice of $R_0$ as long as it is in the classical region of the potential well. We use Eq. (43) in the numerical results described below.

Although the free-free and free-bound Franck-Condon factors have different dimensionality, they may be compared by evaluating the free-bound Franck-Condon factor per unit energy, or $F_{\text{eq}}(\nu, \Delta_A)(\partial E_v / \partial \nu)^{-1}$. Figure 7 also shows the results of evaluating this function for a number of discrete bound levels using an attractive potential that has the same magnitude of the $C_3$ long range potential coefficient as for the repulsive state (see Fig. 3). Each bound level defines a distinct Condon point nearly equal to the outer classical turning point. The free-bound and free-free Franck-Condon factors fall on almost exactly the same curve in Fig. 7, even when $R_C$ is as small as 20 $a_0$. This is expected from the fact that the free-free and free-bound transitions in the model calculation have the same ground state wavefunction and $D_C$ at the same Condon points. The results in Fig. 7 show that the reflection approximation is just as good for bound states as for free states.

Now we can easily derive from Eqs. (38) and (41) a simple expression for the stimulated decay rate of the excited bound state to the ground continuum, $\gamma_s(E, \Delta_A)$:

$$
\gamma_s(E, \Delta_A) = \frac{2\pi}{\hbar} \frac{V_C^2}{D_C} h\nu_v |\Psi_g^+(R_C, E)|^2 \tag{44}
$$

$$
= \frac{2\pi}{\hbar} \frac{V_C^2}{D_C} h\nu_v \frac{4}{h\nu_\infty} a_C^2 \sin^2(k_\infty \rho_C) \tag{45}
$$

$$
= \left\{ \frac{16\pi^2 V_C^2}{h\nu_\infty D_C} a_C^2 k_\infty^2 \rho_C^2 \right\} v_b \tag{46}
$$

$$
= P_e(E)v_b \tag{47}
$$

The probability $P_e(E)$ in Eq. (47), defined by the expression in braces in Eq. (46), is identical in form to the probability in Eq. (34) for a free-free transition. The expression in Eq. (47) thus has a pleasing physical interpretation: the total rate of decay out of the bound state is the probability of decay during one vibration cycle (corresponding to a "complete" collision with incoming and outgoing parts) times the frequency of vibration (number of cycles per second). The overall probability for the photoassociation transition, given by the resonance scattering expression in Eq. (35), explicitly exhibits the threshold law form due to the $\gamma_s$ factor in the numerator.

The form in Eq. (44), proportional to the square of the ground state wavefunction, will also give the threshold law form for $p$- and $d$-waves, etc. It also explicitly shows why the photoassociation spectra map out the nodal structure of the ground state wavefunction in the intensity pattern versus vibrational quantum number [28, 17]: as detuning $\Delta_A$ changes from level to level, the Franck-Condon factor tracks the ground state wavefunction at the changing $R_c$. This effect is expected to be much cleaner in very low temperature spectra, where only $s$-waves contribute, than in most of the existing higher temperature experiments, where $s$-, $p$-, $d$-waves, etc., all may contribute. The $p$- and $d$-waves do not generally have the same nodal structure in the intermediate range as the $s$-wave does.



## 7. Collision Rates Near BEC

In order to estimate the effect of binary collisions in a cold dense atomic gas, it is necessary to compare the rate for the binary process with the atomic scattering rate $\gamma_{\text{atomic}}$ in Eq. (1). The binary event rate is

$$
\gamma_{\text{binary}} = K_e(\Delta_A)N, \tag{48}
$$

where $K_e$ is given by Eq. (18). For the purpose of estimating the relative importance of atomic and binary light scattering events in causing loss of trapped atoms due to heating, it is necessary to compare $\gamma_{\text{atomic}}$ and $2\gamma_{\text{binary}}$, since two atoms are lost per binary event. For the large detuning and moderate density conditions we consider, the influence of any collective effects on light scattering is not likely to alter significantly these basic magnitudes. We will base our estimates on the intermediate range formulas for $R > R_B$, Eqs. (34) and (46), since these apply to a wide range of detuning from near resonance to beyond 100 GHz.

Using Eqs. (34) in (18), the rate coefficient for trap loss events for blue detuning in the intermediate range is

$$
2K_e^{\text{blue}}(\Delta_A) = \frac{32\pi^3 V_c^2}{h D_C} a_C^2 \rho_c^2. \tag{49}
$$

This expression is independent of collision temperature, as it should be. Using Eqs. (2), (6) and (28) and the fact that we can write [43, 42]

$$
C_3 = f_3 \hbar \gamma_A \left( \frac{\lambda_A}{2\pi} \right)^3, \tag{50}
$$

the rate coefficient can be algebraically transformed to the form

$$
2K_{\text{ee}}^{\text{blue}}(\Delta_A) = \frac{2b_c^2 f_3}{3\pi} \gamma_A \left( \frac{\Omega_A}{\Delta_A} \right)^2 \frac{1}{N_\lambda} f_c. \tag{51}
$$

In Eq. (50) $f_3$ is a fraction of order unity depending on the particular molecular states involved (In Hund's case (a) it is 1/2 for a $\Sigma$ state and 1/4 for a $\Pi$ state; in general it will be a function of $R$ that can be worked out for any particular state). The following definitions are used in Eq. (51):

$$
b_c = b(R_C) \tag{52}
$$

$$
N_\lambda = \frac{1}{\lambda_A^3} \tag{53}
$$

$$
f_c = \left( 1 - \left( \frac{R_B}{R_C} \right)^4 \right)^2 \left( 1 - \frac{A_s}{R_C} - \frac{2}{3} \left( \frac{R_B}{R_C} \right)^4 \right)^2. \tag{54}
$$

Recall that $b(R)$ is defined by Eq. (2). The $2b_c^2 f_3 / 3\pi$ factor in Eq. (51) is a dimensionless molecular physics factor depending on the specific transitions involved, and it has a maximum value of

$$
\frac{4}{9\pi} \approx \frac{1}{7}.
$$

The density $N_\lambda$ corresponds to one atom per cubic $\lambda_A$. The density near BEC conditions in a cold atomic gas is typically larger than $N_\lambda$. The factor $f_c$ has a nominal order of magnitude unity and reflects the phase of the ground state wavefunction. It will have a node near $A_s$ if $A_s$ is positive and in the intermediate range.

Using Eq. (51), we find

$$
\frac{2\gamma_{\text{binary}}^{\text{blue}}}{\gamma_{\text{atomic}}} \approx \frac{1}{7} \frac{N}{N_\lambda} f_c. \tag{55}
$$

This fraction is nearly independent of the blue detuning $\Delta_A$ over a wide range, since $f_c \approx 1$ (except near the node). Since $N_\lambda = 5 \times 10^{12} \, \text{cm}^{-3}$ for Na and $2 \times 10^{12} \, \text{cm}^{-3}$ for Rb, we see that the order of magnitude of the light-induced binary collision loss rate is comparable to or larger than the atomic light scattering rate when the density is in the range of $10^{13}$ to $10^{14} \, \text{cm}^{-3}$.

It is also possible to get a simple expression for the rate coefficient for trap loss due to a bound state photoassociation resonance by using Eqs. (47) and (35) in Eq. (18). The thermal average can be greatly simplified at very low $T$ when $k_B T$ is very small compared to the linewidth $\gamma_v$ of the bound state photoassociation resonance $v$. Since the numerator of the resonance scattering $S$-matrix element, Eq. (35), satisfies the threshold law form, the energy-dependence disappears in the numerator of the resonance scattering rate coefficient expression. Then we are left only with the energy dependence in the $E - \Delta_v$ term in the denominator of Eq. (35). But since $k_B T$ is small compared to either of the terms in the denominator, the $E$ dependence is negligible and can be dropped. We also assume $\gamma_v = \gamma_p$, that is, each decay results in a loss event, since the stimulated decay rate is assumed to be small ($\gamma_s \ll \gamma_v$). Thus, the thermal average rate coefficient due to resonance $v$ becomes, in the $T \to 0$ limit,

$$
2K_e^{\text{red}}(v) = \left( \frac{\pi v_g}{k_\infty^2} \gamma_s(v, \Delta_A) \right) \frac{\gamma_p}{(\Delta_v)^2 + (\gamma_v/2)^2} \tag{56}
$$

$$
= 2K_e^{(1)} \frac{\nu_v \gamma_p}{(\Delta_v)^2 + (\gamma_v/2)^2}. \tag{57}
$$

In Eq. (57)

$$
2K_e^{(1)}(\Delta_A) = \frac{32\pi^3 V_C^2}{h D_C} a_C^2 \rho_C^2. \tag{58}
$$

is identical in form to $2K_e^{\text{blue}}$ from Eq. (49). It is the single-cycle loss rate coefficient, due to passing the crossing once in each direction. The net rate is determined by the resonance expression. We can envision two possible limits. The first is the exact resonance case when the laser is tuned to the bound level so $\Delta_v = 0$. In this case, the resonance enhancement factor over the single pass result reduces to $4\nu_v \tau_v$, where $\tau_v = 1/\gamma_v$ is the decay time of level $v$. But $\nu_v \tau_v$ is just the number $N_v$ of complete cycles in one lifetime. So the maximum loss rate coefficient is $2K_e^{\text{max}}(\nu) = 8K_e^{(1)} N_v$. The second limit is when the detuning is as far as possible from resonance. Assuming equal spacing of vibrational levels, the largest detuning is just half of the vibrational spacing; thus, the maximum detuning is just $\Delta_v = \pi \nu_v \gg \gamma_v$. This gives $1/(\pi^2 N_v) \ll 1$ for the factor multiplying $2K_e^{(1)}$ in Eq. (57). The minimum value the rate coefficient can take is $2K_e^{\text{min}} = 2K_e^{(1)}/(\pi^2 N_v)$. Of course, we must add the off-resonance contributions of all levels $v-1$, $v+1$, etc., to get the total off-resonant rate coefficient. If the vibrational spacing is assumed to be uniform, the minimum rate coefficient from summing over all such contributions is $\approx 2K_e^{(1)}/(4N_v)$. Thus, we estimate

$$
\frac{1}{4N_v} (2K_e^{(1)}) < (2K_e^{\text{red}}) < (4N_v)(2K_e^{(1)}). \tag{59}
$$

From Eq. (59) and (55), and the fact that $N_v \gg 1$ whenever $\Delta_A \gg \gamma_A$, we see that $2\gamma_{\text{binary}}^{\text{red}}$ will be a sharply peaked function that is much smaller than $2\gamma_{\text{binary}}^{\text{blue}}$ (for the same $|\Delta_A|$) when $\omega$ is tuned between resonances, but which is much larger than $2\gamma_{\text{binary}}^{\text{blue}}$ when $\omega$ is tuned to a photoassociation resonance. Therefore, by detuning to the red side of atomic resonance, the effect of binary collisions can be made to be either very large or very small compared to $\gamma_{\text{atomic}}$. The cold atomic gas will have a prominent photoassociation spectrum, and the rate for photodestruction at the peak positions will measure the ground state pair correlation function $\propto |\Psi_g(R_c)|^2$ at the Condon points for the transitions. There is a discrete set of Condon points $R_c(\nu)$, corresponding to the outer turning points for the vibrational levels of the upper molecular state. There are several well-known alkali dimer transitions that have already been studied [7] in much hotter traps than the $< 1 \, \mu K$ traps that are now available. The intriguing question remains whether 3-body or collective effects might perturb the binary photoassociation spectrum, causing broadening or shifts in the resonance line profiles. Kagan et al. [45] have suggested the possibility of observing quantum correlations in optical properties of low temperature spin-polarized gases. The photoassociation spectrum of a cold dense atomic gas near BEC might be a very fruitful source of experimental and theoretical investigation of 2- and 3-body interactions in such systems [11].

Certainly the analysis in this paper shows that light can induce significant loss processes, in comparison to that caused by free atom light scattering, due to collisions between atoms in a cold atomic gas near 1 μK or below at densities $> 10^{13}$ cm$^{-3}$. If the density should increase to $> 10^{15}$ cm$^{-3}$, the collisional loss rate will dominate that due to atomic recoil heating, except between photoassociation resonances for large enough red detuning. For the case of the MIT Na trap [3] the blue detuning of the laser used to plug the hole in the magnetic trap was so far off-resonance that any atomic or binary light scattering did not prevent the formation of a condensate. But for much smaller detunings the simple Franck-Condon formulas we have derived here give a way to estimate the binary collision rates for trap loss via excited state production. More detailed treatment, including incorporating the actual quasimolecular structure of alkali dimer states, could be readily incorporated into this framework. We have also developed a theory for treating the nonperturbative effect of light, including multiphoton effects and the modification of the ground state scattering length [9]. Careful attention to collective effects also needs to be given for the case of higher densities. In any case, it seems very unlikely that a condensate could be stable for very long in the presence of light tuned within a few hundred GHz of atomic resonance.


## 8. Appendix A. Milne Equation Analysis of Asymptotic Wavefunction

The use of the exact Milne quantum mechanical equations for the phase and amplitude of the wavefunction lets us do an exact analysis of the asymptotic wavefunction. Let the wavefunction be written in phase-amplitude energy-normalized form:

$$
\Psi(R, E) = \left( \frac{2\mu}{\pi\hbar^2} \right)^{1/2} \alpha(R, E) \sin(\beta(R, E)), \tag{60}
$$

where $\alpha$ satisfies the Milne equation [46, 47],

$$
\left( \frac{d^2}{dR^2} + k^2(R, E) \right) \alpha(R, E) - \frac{1}{\alpha(R, E)^3} = 0. \tag{61}
$$

The phase $\beta$ is calculated from $\alpha$ by

$$
\beta(R, E) = \int \frac{1}{\alpha(R, E)^2} \, dR, \tag{62}
$$

and the local wave vector is

$$
k(R, E) = \frac{2\pi}{\lambda(R)} = \sqrt{\frac{2\mu}{\hbar^2} (E - V(R))}. \tag{63}
$$

The asymptotic potential is $V(R) = -C_6/R^6$.

In the semiclassical picture, we have the identification of $\alpha$ with the WKB amplitude

$$
\alpha^{\text{WKB}}(R, E) = \frac{1}{\sqrt{k(R, E)}}, \tag{64}
$$

and the above forms are equivalent to the WKB wavefunction. The exact solution to the quantum equations [Eqs. (61) and (62)] give an exact quantum wavefunction. Here we will use an asymptotic analysis for the wavefunction at moderately long range.

At long range the amplitude becomes constant, and very large as $E \to 0$:

$$
\alpha_\infty = \frac{1}{\sqrt{k_\infty}} = \sqrt{\frac{\lambda_\infty}{2\pi}}. \tag{65}
$$

Therefore, we want to calculate the departure of this large, nearly independent of $R$, amplitude from its asymptotic limit. We do this by *approximating* the last term of Eq. (61) by $1/\alpha^3 \approx k_\infty^2 \alpha$. Then Eq. (61) becomes

$$
\frac{d^2\alpha}{dR^2} + (k^2(R) - k_\infty^2)\alpha = 0 \tag{66}
$$

$$
\frac{d^2\alpha}{dR^2} - \frac{2\mu}{\hbar^2} V(R)\alpha = 0 \tag{67}
$$

$$
\frac{d^2\alpha}{dR^2} = -\left(\frac{2\mu}{\hbar^2}C_6\right)\frac{1}{R^6}\alpha. \tag{68}
$$

Equation (68) can be immediately integrated to give

$$
\alpha(R) = \alpha_\infty\left(1 - \frac{2\mu C_6}{20\hbar^2 R^4}\right) \tag{69}
$$

$$
= \alpha_\infty\left(1 - \left(\frac{R_B}{R}\right)^4\right) \tag{70}
$$

where $R_B$ is defined by Eq. (13). When $R = 20^{1/4}R_B = 2.1R_B$, the amplitude $\alpha(R)$ has only changed by 5% from its asymptotic value $\alpha_\infty$. When $R = R_B$, the correction term is unity, and the asymptotic approximation used in setting up the approximate Eq. (66) breaks down. Therefore, the amplitude expression in Eq. (70) can only be applied for $R \gg R_B$.

Now we can turn our attention to deriving the correction to the asymptotic phase. This is done by substituting the above amplitude, Eq. (70), into the phase [Eq. (62)]. The asymptotic phase at some suitable large value of $R = R_\infty$ (a distance well beyond the range of the potential) is $\beta_\infty = k_\infty(R_\infty - A_s)$, where $A_s$ is the $s$-wave scattering length. The phase function at $R$ is calculated by integrating backwards from $R_\infty$,

$$
\beta(R) = k_\infty(R_\infty - A_s) + \int_{R_\infty}^R \frac{1}{\alpha(R)^2} \, dR
$$

$$
= k_\infty(R_\infty - A_s) - k_\infty \int_R^{R_\infty} \frac{dR}{\left(1 - \left(\frac{R_B}{R}\right)^4\right)^2}
$$

$$
\approx k_\infty(R_\infty - A_s) - k_\infty \int_R^{R_\infty} \left(1 + 2\left(\frac{R_B}{R}\right)^4\right) \, dR
$$

$$
= k_\infty \left(R - A_s - \frac{2}{3} \left(\frac{R_B}{R}\right)^4 R\right). \tag{72}
$$

Combining the corrected phase and amplitude expressions, Eqs. (72) and (70), in Eq. (60), we obtain the expression given in Eq. (10) in the text. Note that the normalization stays close to its *asymptotic* value, in spite of the fact that the local $k(R, E)$ can be much larger than $k_\infty$ in that part of the moderately long range region where $|V_g| \gg E$ (see Fig. 2). Thus, the semiclassical local WKB normalization does not apply. Note also that the node of the wavefunction at $R_n$ near $A_s$ for the positive scattering length case is shifted from its value projected from the asymptotic $A_s$. This is because the phase near $A_s$ has not yet reached its asymptotic limiting value. This shift in the actual node to larger $R$ can readily be estimated from Eq. (72):

$$
R_n - A_s - \frac{2}{3} \left( \frac{R_B}{R_n} \right)^4 R_n = 0 \tag{73}
$$

and

$$
R_n \approx A_s \text{ implies } R_n \approx A_s \left( 1 + \frac{2}{3} \left( \frac{R_B}{A_s} \right)^4 \right). \tag{74}
$$

## 9. Appendix B. Reflection Formula

This derivation of the reflection approximation expression follows Jablonski [48] and the Appendix of Ref. [49]. We begin by writing the ground and excited state wavefunctions in energy-normalized phase-amplitude form

$$
\Psi_g(R, E) = \left( \frac{2\mu}{\pi\hbar^2} \right)^{1/2} \alpha_g(R, E) \sin(\beta_g(R, E)) \tag{75}
$$

$$
\Psi_e(R, E_e) = \left( \frac{2\mu}{\pi\hbar^2} \right)^{1/2} \alpha_e(R, E_e) \sin(\beta_e(R, E_e)). \tag{76}
$$

where $E_e = E + \hbar\Delta_A$. The ground state amplitude and phase are given by Eqs. (70) and (72), whereas the excited state quantities can be taken to be the standard WKB ones:

$$
\alpha_e(R, E_e) = \frac{1}{\sqrt{k_e(R, E_e)}} \tag{77}
$$

$$
\beta_e(R, E_e) = \int_{R_t}^R k_e(R', E_e) \, dR' + \frac{1}{4}\pi, \tag{78}
$$

where $R_t$ is the inner turning point of the repulsive potential. The Franck-Condon factor is

$$
F_{eg}(E, \Delta_A) = \frac{2\mu}{\pi h^2} |I_{eg}(E, \Delta_A)|^2, \tag{79}
$$

where

$$
I_{eg}(E, \Delta_A) = \int_0^\infty \alpha_g \alpha_e \sin \beta_g \sin \beta_e \, dR \tag{80}
$$

$$
\approx \frac{1}{2} \int_0^\infty \alpha_g \alpha_e \cos(\beta_g - \beta_e) \, dR. \tag{81}
$$

In the last line we have made the standard approximation of neglecting the rapidly oscillating phase sum term. The phase difference is expanded in a Taylor series about a point $R_p$:

$$
\phi(R, E) = \beta_g(R, E) - \beta_e(R, E) \tag{82}
$$

$$
= b_0 + b_1(R - R_p) + \frac{1}{2} b_2(R - R_p)^2 + \dots, \tag{83}
$$

where

$$
b_0 = \beta_g(R_p, E) - \beta_e(R_p, E_e) \tag{84}
$$

$$
\approx \beta_g(R_p, E) - \frac{\pi}{4} \tag{85}
$$

$$
b_1 = \left. \frac{d\beta_g(R, E)}{dR} \right|_{R_P} - \left. \frac{d\beta_e(R, E_e)}{dR} \right|_{R_P} \tag{86}
$$

$$
= \frac{1}{\alpha(R_p, E)^2} - k_e(R_p, E) \tag{87}
$$

$$
\approx k_\infty - k_e(R_p, E_e) \tag{88}
$$

$$
b_2 = \left. \frac{d^2\beta_g(R, E)}{dR^2} \right|_{R_P} - \left. \frac{d^2\beta_e(R, E_e)}{dR^2} \right|_{R_P} \tag{89}
$$

$$
\approx -\frac{dk_e(R, E_e)}{dR} \bigg|_{R_P} \tag{90}
$$

$$
\approx -\frac{\mu D_C}{\hbar^2 k_e(R_P)} \tag{91}
$$

In the normal semiclassical theory, $R_p$ is taken to be the Condon point, where $k_g = k_e$ so that $b_1 = 0$. Here we simply take the point where $b_1$ vanishes. Since the excited state potential is so steep with respect to the effectively flat ground state potential, it is an excellent approximation to take $R_p = R_t = R_c$ to all be equivalent. Then from Eq. (78), $\beta_e(R_p, E) = \pi/4$. The expression for $b_2$ follows from neglecting the ground state contribution in comparison to the excited state one.

We thus evaluate

$$
I_{\text{eg}}(E) = \alpha_g(R_C, E)\alpha_e(R, E) \frac{1}{2} \int_{-\infty}^{\infty} \cos(b_0 + \frac{b_2}{2}x^2) dx
$$

$$
= \alpha_g(R_C, E) \left( \frac{\pi \hbar^2}{2\mu D_C} \right)^{1/2} \cos\left(\beta_g(R_C, E) - \frac{\pi}{2}\right)
$$

$$
= \left( \frac{\pi \hbar^2}{2\mu D_C} \right)^{1/2} \alpha_g(R_C, E) \sin(\beta_g(R_C, E)). \tag{92}
$$

where we have used

$$
\int_{-\infty}^{\infty} \cos\left(b_0 \pm \frac{|b_2|}{2}x^2\right) dx = \frac{2\pi}{|b_2|} \cos\left(b_0 \pm \frac{\pi}{4}\right). \tag{93}
$$

Using Eqs. (75) and (92) in Eq. (79) gives the desired reflection approximation to the Franck-Condon factor:

$$
F_{\text{eg}}(E, \Delta_A) = \frac{1}{D_C} |\Psi_g(R_C, E)|^2. \tag{94}
$$

