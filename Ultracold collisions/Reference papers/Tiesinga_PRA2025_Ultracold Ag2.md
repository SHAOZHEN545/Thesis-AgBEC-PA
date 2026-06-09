# Ultracold silver-atom collisions and the formation of silver dimers by photo- and magneto-association

**Authors:** Eite Tiesinga; Jacek Kłos; Hui Li; Svetlana Kotochigova; David DeMille  
**Journal:** *Physical Review A* **111**, 062814 (2025)  
**Received:** 18 January 2025  
**Accepted:** 28 May 2025  
**Published:** 17 June 2025  
**DOI:** 10.1103/rd26-sgz1  
**Contact:** skotoch@temple.edu

## Abstract

We have performed three theoretical simulations relevant for describing collisions among laser-cooled silver atoms and for the formation of Ag$_2$ molecules from these colliding atoms. Firstly, we determined the relativistic electronic structure of Ag$_2$ molecules in ground and low-lying excited states. Secondly, we computed rotational and vibrational levels of the ground and excited electronic states as well as rovibrationally averaged electric transition dipole moments. Using this knowledge, we analyzed a simplified quantum-mechanical model of the one-photon photoassociation process to form electronically excited Ag$_2$ from microkelvin Ag atoms and make predictions for lineshapes and saturation effects as functions of laser frequency and intensity. Finally and thirdly, we performed coupled-channels calculations, numerical solutions of sets of coupled radial Schrödinger equations of ultracold ground-state Ag collisions in an external magnetic field. These calculations include the effects of two Born-Oppenheimer potentials as well as hyperfine Fermi-contact and Zeeman interactions. We discuss the expected range of s-wave scattering lengths as well as strengths and distribution of Fano-Feshbach resonances as a function of the magnetic-field strength for the $^{107}$Ag and $^{109}$Ag isotopes. We highlight the periodicity of the scattering length with small changes in the depths of the Born-Oppenheimer potentials. The Fano-Feshbach resonances can be used to magneto-associate ultracold Ag atoms into weakly bound ground-state Ag$_2$ dimers.

## I. Introduction

Recent theoretical analyses [1–4] suggest that silver-containing diatomic molecules, such as FrAg and RaAg, can be sensitive detectors of broken symmetries in the hadronic sector of particle physics. Specifically, the heavy, radioactive francium-223 ($^{223}$Fr) and radium-225 ($^{225}$Ra) isotopes have octupole-deformed nuclei with so-called PT-odd nuclear Schiff moments. A review on using atoms and molecules to address open questions in fundamental physics can be found in Ref. [5]. Our recent theoretical description on the formation of ultracold FrAg molecules from laser-cooled Fr and laser-cooled Ag atoms and on the efficient control of these molecules [6] provides information that can be used to guide and conduct the precision frequency measurements needed to detect the broken symmetries. Additional recent calculations have shown that the strong electron affinity of the Ag atom leads it to form ionic bonds with most alkali-metal atoms, resulting in molecules with exceptionally large electric dipole moments [7]. Such strongly polar alkali-metal-Ag molecules could be of great utility [8,9] for quantum simulations of strongly coupled many-body systems [10], quantum information processing [10–13], or the generation of entanglement for quantum-enhanced metrology [14].

Of course, an ultracold atomic or homonuclear-diatomic silver gasses are many-body systems that can also be brought to quantum degeneracy and, as its two stable isotopes are bosons, Bose condensation and other quantum degenerate phenomena as occur when particles are trapped in spatially and/or time periodic potentials should be observable [15,16]. These states of matter for silver have as yet to be observed and can be of interest in their own right.

For all these experiments, the starting point is an ultracold gas containing both Ag and optionally another atom with which to pair it. These gasses are at temperatures of tens of $\mu$K or well below. The ${}^2S$ ground state of the silver atom is an electronic configuration with a closed $4d^{10}$ shell and an easily polarizable singly occupied, open $5s$ outer shell. The lowest excited states of opposite parity are the $4d^{10}5p({}^2P_{j=1/2,3/2})$ and the long-lived $4d^95s^2({}^2D_{j=3/2,5/2})$ configurations with nearly degenerate and, in fact, interleaved energies [17]. Still, the electronic structure of Ag atoms is sufficiently similar to that of alkali-metal atoms, with their outer-most open $s$ electron orbital, that silver atoms can be manipulated with the same laser-cooling methods as alkali-metal atoms [8,18–21]. The first report on laser cooling and magneto-optical trapping of silver atoms on the 328 nm $5s({}^2S)$ to $5p({}^2P_{3/2})$ transition was published in Ref. [22]. These methods lead to sufficiently high atom number densities and sufficiently low temperatures, often corresponding to phase-space densities just below those required for the formation of Bose-Einstein condensates, that molecule assembly from ultracold atoms can be effective.

For molecular assembly of ultracold Ag-bearing molecules, including homonuclear Ag$_2$, we can use the method of photoassociation (PA) [23–45]. A review can be found in Ref. [46]. Here, one of the ultracold ${}^2S$ atoms resonantly absorbs a photon from a laser to assemble into a weakly bound rovibrational level of a molecular electronic excited state dissociating to one of the ${}^2S + {}^2P_j$ limits. That is, the energy of the laser photon is smaller than the ${}^2S$ to ${}^2P_{1/2}$ or ${}^2P_{3/2}$ transition energy. This rovibrational level of the electronically excited state then quickly falls apart into hot atom pairs, with typically tens to hundreds of kelvin relative kinetic energy, or into rovibrational states of the ground-state potentials by spontaneously emitting a photon in a random direction. A schematic representation of one-photon PA of two silver atoms, where the atom pair decays into a rovibrational level of a ground-state potential of Ag$_2$, is shown in Fig. 1. Spontaneous emission leads to a detectable decrease in the number of trapped atoms when the PA laser is “resonant” with a weakly bound rovibrational level. Matrix elements of the transition electric dipole moment with respect to the scattering and rovibrational wave functions determine the rate of atom loss or strength of the resonances. The rates and binding energies of a set of weakly bound rovibrational states can be used to accurately determine atomic transition dipole moments and s-wave scattering lengths, which quantify ultracold atomic collisions. Photoassociation experiments are typically performed without the use of a magnetic field.

> [!figure]
> ![[Fig. 1.png|center|500]]
> **Figure 1.** Schematic of one-photon photoassociation starting from two colliding Ag atoms (red spheres with black arrows) and using a laser with frequency $\omega_1$ (vertical red arrow). The sinusoidal curve represents spontaneous decay of a rovibrational level of an excited electronic state into a rovibrational level of a ground-state potential.

Homonuclear Ag$_2$ molecules can also be formed using Fano-Feshbach resonances that appear in the collision of ultracold silver atoms in the presence of an external magnetic field. A review on these resonances can be found in Ref. [47]. Some selected articles from this field are found in Refs. [48–55]. Slow time-dependent sweeps of the magnetic field near Fano-Feshbach resonances can transfer colliding atoms into weakly bound rovibrational states. This process is called magneto-association.

The experimental setup for a candidate molecule requires considerable investments and thus the need to carefully analyze and predict the atomic and molecular properties is beneficial. Analysis can include the determination of spectroscopic properties of and between electronic states as well as scattering cross sections and collisional rate coefficients, where electronic potential-energy surfaces, strengths of radiative electronic transitions and static and dynamic polarizabilities need to be computed.

In this paper, we first describe a calculation of the electronic potential-energy surfaces of the ground and energetically lowest excited states of Ag$_2$. We then analyze one-photon photoassociation spectroscopy of ultracold colliding Ag atoms to weakly bound molecular states in electronic excited states. Finally, we focus on magnetic Fano-Feshbach resonances in the collision of ultracold Ag atoms. These simulations require coupled-channel calculations accounting for spin-spin couplings between molecular electronic states and hyperfine and Zeeman interactions due to the nonzero electron and nuclear spins of Ag isotopes. Thus, these quantum-mechanical calculations include a breakdown of the adiabatic approximation as first defined by Born and Oppenheimer in 1927 [56].

For analytical insights into these photoassociation and collisional processes, we separate the atom-atom interactions into short- and long-range regions of the internuclear or atom-atom separation $R$. These two radial regions, roughly defined by whether the electron wave function of the atoms does or does not significantly overlap, are characterized by very different energy and length scales. Molecular physics is typically concerned with strong short-range interactions associated with tightly bound “ordinary molecules.” Ultracold physics is concerned with scattering states in the Wigner threshold limit near zero collision energy as well as weakly bound molecular states. In the long-range region electronic potential-energy surfaces are sums of polarization and dispersions terms, each proportional to $1/R^n$, where $n=3$ or $6$ for two neutral alkali-metal, alkaline-earth, and group-11 atoms, and (approximate) analytical solutions of the Schrödinger equation for scattering and rovibrational wave functions or binding energies are available. We use these analytical solutions to understand photoassociation rate coefficients and Fano-Feshbach resonances.

In this paper $h$ is the Planck constant, $\hbar$ is the reduced Planck constant, $e$ is the positive elementary charge, $k$ is the Boltzmann constant, and $c$ is the speed of light in vacuum. Furthermore, we use fine-structure constant $\alpha$, vacuum electric permittivity $\epsilon_0$, electron mass in atomic mass units $m_e/m_u$, Hartree energy $E_h$, and Bohr radius $a_0$. Their values were taken from Ref. [57]. The atomic masses of Ag isotopes in atomic mass units $m_u$ are found in Ref. [58].

## II. Electronic potential-energy surfaces of Ag$_2$

Silver atom dimers have been experimentally studied since the late 1950s. Schissel [59] determined dissociation energies of potential-energy surfaces of Ag$_2$ and other group 11, coinage metal dimers such as Cu$_2$ and Au$_2$. This researcher measured dissociation energy $D_e = 1.78(0.10)$ eV or, equivalently, $hc \times 14400(800)$ cm$^{-1}$ for the $X{}^1\Sigma_g^+$ electronic ground state of Ag$_2$, where the numbers in parentheses here and elsewhere are one standard-deviation uncertainties in the last significant digits. An early theoretical attempt to determine this dissociation energy by Andzelm et al. [60] using nonrelativistic calculations within the local-spin-density method and equivalent relativistic calculations including scalar-relativistic effects led to dissociation energies of 1.7 and 2.0 eV, respectively, for this electronic state.

In 2021, Jasik et al. [61] modeled the decay of hot silver dimer anions by spontaneous electron emission and by dissociation to a silver anion and a neutral atom in order to compare with experimental data for this process [62]. For this model, Jasik et al. determined nonrelativistic electronic potential-energy curves for the ground state of the anion Ag$_2^-$ and that of neutral Ag$_2$. They used the coupled-cluster method with an effective-core-potential and a large basis set including single, double, and noniterative triple [CCSD(T)] excitations. In the same year, Śmiałkowski et al. [7] published calculations of the electronic state of van der Waals complexes between alkali-metal atoms and Ag and Cu atoms, which also included results for the Ag$_2$ dimer. These authors also used the nonrelativistic CCSD(T) coupled-cluster method but with larger electron basis sets. Śmiałkowski et al. [7] provide spectroscopic parameters for the $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ states of Ag$_2$, both dissociating to two Ag atoms in their electronic ground state.

We have independently computed the adiabatic electronic potential-energy surfaces of ground and excited electronic states of Ag$_2$ as functions of atom-atom separation $R$. The $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ electronic states, dissociating to two silver atoms in their ${}^2S$ electronic ground state, have been calculated with a nonrelativistic spin-restricted coupled-cluster method, while relativistic adiabatic excited states dissociating to a silver atom in its ground state and a silver atom in its lowest-energy ${}^2P$ excited state have been calculated with a nonrelativistic multireference configuration-interaction method combined with spin-orbit matrix elements between all computed nonrelativistic ground and excited states. The configuration-interaction calculations do not include excitations to the $4d^95s^2$ configuration as, currently, the computations are impractical. Radial- or $R$-dependent energy shifts due to spin-orbit effects for the ground $X{}^1\Sigma_g^+$ state are small compared with the uncertainties in our nonrelativistic coupled-cluster calculations of this potential. Finally, we have computed the small second-order spin-orbit interaction, lifting degeneracies in the $a{}^3\Sigma_u^+$ state, using the nonrelativistic configuration-interaction method as well as methods with relativistic electrons. Details regarding these calculations and a comparison with the data from Refs. [7,61] can be found in Appendix A.

> [!figure]
> ![[Fig. 2.png|center|500]]
> **Figure 2.** Our potential-energy surfaces for the $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ states of the Ag$_2$ molecule as functions of internuclear separation $R$. The data have been obtained with a nonrelativistic spin-restricted coupled-cluster method. The data for these curves are available from the Supplemental Material [63].

Figure 2 shows the short-range shapes of the $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ potentials. They have depths or dissociation limits $D_e = hc \times 13\,837(200)$ cm$^{-1}$ and $hc \times 460(80)$ cm$^{-1}$, respectively. For separations larger than shown in the figure, both potentials approach the same attractive dispersion potential $-C_6/R^6$ with $C_6 = 342(85)E_h a_0^6$. In practice, we also include a small common $-C_8/R^8$ contribution with $C_8 = 61\,190E_h a_0^8$, as described in Appendix A.

In Fig. 3 we show the sixteen excited-state potentials dissociating to the relativistic $4d^{10}5p({}^2P_{j=1/2,3/2}) + 4d^{10}5s({}^2S)$ limits. The main figure shows the short-range, small-$R$ behavior of the potentials. Here, the relativistic spin-orbit interactions are small compared with nonrelativistic splittings and states can be assigned Hund’s case-(a) ${}^{2S+1}\Lambda_{g/u}$ labels, where quantum number $S=0$ or $1$ represents the total molecular electron spin and $\Lambda=\Sigma$ or $\Pi$ for 0 or 1, respectively, represents the absolute value of the projection of the total molecular electron orbital angular momentum. Gerade and ungerade ($g$ and $u$) states indicate even and odd inversion symmetry with respect to the center of charge of the molecule. Our short-range excited-state potentials compare favorably with those obtained in Ref. [64].

> [!figure]
> ![[Fig. 3.png|center|500]]
> **Figure 3.** The sixteen relativistic adiabatic potentials of states dissociating to a silver atom in its ${}^2S$ ground state and one in the ${}^2P_{1/2,3/2}$ states as functions of internuclear separation $R$. Molecular states are assigned Hund’s case-(a) ${}^{2S+1}\Lambda_{g/u}$ labels as well as Hund’s case-(c) $\Omega_{g/u}^{\pm}$ labels in parentheses after each Hund’s case-(a) label. The inset shows the long-range behavior of the potentials. The zero of energy is the energy of the separated atom limit for two ${}^2S$ ground-state atoms. The data have been obtained with a nonrelativistic multireference configuration-interaction method plus spin-orbit matrix elements between all computed nonrelativistic states. The nearly degenerate $4d^95s^2$ configuration was not included in these simulations. The gerade and ungerade potentials are represented by the dashed and solid lines, respectively. Black, red, orange, and blue lines represent $0^+$, $1$, $0^-$, and $2$ states, respectively. The data for these curves are available from the Supplemental Material [63].

The long-range, large-$R$ behavior of the excited-state potentials is shown in the inset of Fig. 3. For these separations the spin-orbit interactions are the dominant interactions and states are better described by Hund’s case-(c) $\Omega_{g/u}^{\pm}$ labels. Here, $\Omega$ is the absolute value of the projection of the total electronic spin and orbital angular momentum on the internuclear axis and, when $\Omega=0$, superscript $\pm$ represents even or odd reflection symmetry of the electron wave function through a plane containing the internuclear axis. For separations larger than those shown in the inset, the potentials are proportional to $C_3/R^3$ with a positive or negative $\Omega_{g/u}^{\pm}$-dependent $C_3$ coefficient that is fully determined by the product of the line strength of the $4d^{10}5s({}^2S)$ and $4d^{10}5p({}^2P)$ transition and a matrix element describing a recoupling of the electron spins and orbital angular momenta. See Ref. [65] for a derivation.

A glance at Figs. 2 and 3 and Figs. 7 and 8 of Ref. [46] shows that there are similarities with the potential-energy surfaces for heavy homonuclear diatomic alkali-metal molecules. This is due to the single active open valence $s$ orbital of both alkali-metal and silver atoms. Thus, we find a deep $X{}^1\Sigma_g^+$ ground state and a shallow $a{}^3\Sigma^+$ state in Fig. 2. These states dissociate to two ${}^2S$ ground-state atoms. Next, we observe a crossing between the ${}^1\Sigma_u^+$ and ${}^3\Pi_u$ potentials that dissociate to an excited ${}^2P$ atom and a ground ${}^2S$ atom at a separation $R$ near $4.5a_0$, just smaller than the equilibrium separation of the ${}^3\Pi_u$ potential. More precisely, this is an avoided crossing between two $0_u^+$ Hund’s case-(c) levels. For alkali-metal dimers these Hund’s case-(c) states and their avoided crossing also exist, except that the avoided crossing now occurs at a separation that is larger than the equilibrium separation of the ${}^3\Pi_u$ potential. Other similarities exist as well.

We stress that we cannot yet include the $4d^95s^2({}^2D)$ configuration in our simulations. We expect additional potential-energy curves and avoided crossings among the curves in Fig. 3 as, for example, the energy of the ${}^2D_{5/2}$ lies in between that of the ${}^2P_{j=1/2,3/2}$ states. For simulations of photoassociation rate coefficients described in the next section, we focus on weakly bound vibrational levels of electronic states with energies just below the ${}^2S + {}^2P_{j=1/2}$ limit. Then these vibrational levels are mostly unaffected by the $4d^95s^2({}^2D)$ configuration.

> [!figure]
> ![[Fig. 4.png|center|500]]
> **Figure 4.** The splitting between the $\Omega=1_u$ and $0_u^-$ components of the $a{}^3\Sigma_u^+$ state of Ag$_2$ as a function of internuclear separation $R$ due to the second-order spin-orbit interaction (red filled circles) as well as that due to minus the magnetic dipole-dipole interaction (green curve). The orange dashed line segment corresponds to the inner turning point of the $a{}^3\Sigma_u^+$ potential at zero collision energy. The black curve corresponds to a least-squares fit to these data assuming the double-exponential function given in the figure with length parameters in units of $a_0$ and energies in units $hc$ cm$^{-1}$. The gray banded region is the 40 % fractional standard uncertainty in the splitting.

Figure 4 shows the small, positive splitting $V_{\Omega=1}(R)-V_{\Omega=0}(R)$ between the $\Omega=1_u$ and $0_u^-$ components of the $a{}^3\Sigma_u^+$ state (dropping the sub- and superscripts in the formula for clarity) due to the relativistic spin-orbit interaction as a function of interatomic separation $R$. The splitting, which only appears in second-order perturbation theory in the spin-orbit interaction, is a rapidly decreasing function with increasing $R$, whose parametrization in terms of the sum of two exponentials is shown in the figure. An exponential $R$ dependence with length scales of order $1/a_0$ implies that the effect depends on the exponentially suppressed overlap of the $5s$ valence electron from the two Ag atoms. The inner turning point of the $a{}^3\Sigma_u^+$ potential at zero collision energy is located at $R \approx 5.2a_0$. The second-order spin-orbit splitting is approximately $hc \times 1.3$ cm$^{-1}$ at this separation. The standard uncertainty of $V_{\rm 2nd-SO}(R)$ is 40 % independent of $R$, found by comparing the splitting obtained with various electronic structure methods.

**Table I.** Summary of parameters relevant for the scattering of two ultracold $^{109}$Ag atoms and for one-color photoassociation spectroscopy near the Ag $4d^{10}5s({}^2S)$ to $4d^{10}5p({}^2P)$ transition. Reduced matrix elements $\langle{}^{2S+1}L'\Vert d\Vert{}^{2S+1}L\rangle$ of the atomic electric dipole moment operator $d$ between nonrelativistic atomic states $|{}^{2S+1}L\rangle$ and $|{}^{2S+1}L'\rangle$ are defined using the conventions of Ref. [66]. Numbers in parentheses are one standard deviation uncertainties in the last significant digit(s) of the value. The origin of these values and their uncertainties is discussed in the text. Values for parameters are independent of isotopologues of Ag with the exceptions of $\beta_6$, $\bar{a}$, and $E_6$, which are evaluated for the homonuclear $^{109}$Ag + $^{109}$Ag system.

| Quantity | Equation | Value |
|---|---:|---:|
| **Atomic properties** |||
| Transition energy between barycenters of the ${}^2P$ and ${}^2S$ states | $\Delta E = E({}^2P)-E({}^2S)$ | $hc \times 30\,166$ cm$^{-1}$ |
| Spin-orbit splitting between the ${}^2P_{3/2}$ and ${}^2P_{1/2}$ states | $\Delta = E({}^2P_{3/2})-E({}^2P_{1/2})$ | $hc \times 920.6$ cm$^{-1}$ |
| Line strength of the ${}^2P$ to ${}^2S$ transition | $S_{{}^2P\to{}^2S}$ | $17.4(2.5)e^2a_0^2$ |
| Square of the reduced ${}^2P$ to ${}^2S$ transition dipole moment | $|\langle{}^2P\Vert d\Vert{}^2S\rangle|^2=S_{{}^2P\to{}^2S}/6$ | $2.9(4)e^2a_0^2$ |
| Einstein $A$ coefficient of the $4d^{10}5p({}^2P)$ excited state | $A_P=\frac{4}{3}\frac{E_h}{\hbar}\alpha^3(\Delta E/E_h)^3|\langle{}^2P\Vert d/(ea_0)\Vert{}^2S\rangle|^2$ | $1.6(2)\times10^8$ s$^{-1}$ |
| Natural linewidth of the $4d^{10}5p({}^2P)$ excited state | $\gamma_P=\hbar A_P/h$ | $2\pi\times25.6(3.7)$ MHz |
| **Ground-state ${}^2S+{}^2S$ collisions** |||
| van der Waals coefficient for the ${}^2S+{}^2S$ collision | $C_6$ | $342(80)E_h a_0^6$ |
| van der Waals length | $\beta_6=(2\mu C_6/\hbar^2)^{1/4}$ | $90.8(5.3)a_0$ |
| Mean van der Waals scattering length | $\bar{a}\approx0.478\beta_6$ | $43.4(2.5)a_0$ |
| van der Waals energy | $E_6=\hbar^2/(2\mu\beta_6^2)$ | $k\times193(23)$ $\mu$K |
| **Excited-state ${}^2S+{}^2P$ interaction strengths** |||
| Strength of the resonant ${}^2S\leftrightarrow{}^2P$ dipole-dipole interaction | $C_3=|\langle{}^2P\Vert d\Vert{}^2S\rangle|^2/(4\pi\epsilon_0)$ | $2.9(4)E_h a_0^3$ |
| Nonresonant dispersion coefficient | $C_{6,0_u^+}$ | $1600(400)E_h a_0^6$ |

## III. One-color photoassociation of ultracold silver atoms

One-color photoassociation of ultracold, ground-state silver atoms is the process whereby a pair of colliding silver atoms resonantly absorbs a photon from a continuous wave (cw) laser and is excited to a weakly bound rovibrational level of an electronically excited state. These excited levels are short lived and the atom pair decays back to two much-hotter ground state atoms or a ground-state molecule by spontaneous emission of a photon. These products are typically no longer held in the magnetic, optical, or magneto-optical trap in which the ultracold atoms are stored or held. Hence, resonant one-color photoassociation leads to loss of atoms from their trap, which can often be easily detected. A review of this process can be found in Ref. [46].

In simulating photoassociation of ultracold, ground-state silver atoms, we consider laser light with wave numbers detuned up to 100 cm$^{-1}$ to the red of the ground $4d^{10}5s({}^2S)$ to excited $4d^{10}5p({}^2P_{1/2})$ or $D1$ transition. Specifically, we imagine $^{107}$Ag or $^{109}$Ag atoms in a magneto-optical trap, where these atoms are in the energetically lowest $f=1$ hyperfine state with all three Zeeman sublevels equally populated. Weakly bound rovibrational levels of attractive excited-state electronic potentials dissociating to the $5s({}^2S_{1/2})+5p({}^2P_{1/2})$ limit can be modeled using the relativistic adiabatic Hamiltonian of Ref. [65] for atom-atom separations $R$, where the binding energies of these potentials are significantly smaller than the spin-orbit splitting $\Delta\approx hc\times920.6$ cm$^{-1}$ between the $5p({}^2P_{1/2})$ and $5p({}^2P_{3/2})$ states of Ag. We omit the effects of the nearly degenerate $4d^95s^2({}^2D)$ configuration on the $4d^{10}5p({}^2P)$ states. The model of Ref. [65] has been successful in describing photoassociation of ultracold alkali-metal atom gasses [46].

There exist six relativistic adiabatic states whose potential energies approach that of the $5s({}^2S_{1/2})+5p({}^2P_{1/2})$ limit for large $R$. The energetically lowest state is labeled by $\Omega_\sigma^\pm=0_u^+$. For $\Omega=0$ states hyperfine interactions can be ignored for our purposes. With the help of Ref. [65], we derive that the long-range tail of the excited $0_u^+$ state is well described by

$$
V(R;0_u^+)=-\frac{4}{3}\frac{C_3}{R^3}-\left[\frac{2}{9}\frac{(C_3)^2}{\Delta}+C_{6,0_u^+}\right]\frac{1}{R^6}+O\left(\frac{1}{R^8}\right)
\tag{1}
$$

where the resonant dipole-dipole coefficient $C_3=|\langle{}^2P\Vert d\Vert{}^2S\rangle|^2/(4\pi\epsilon_0)$ with reduced matrix element $\langle{}^2P\Vert d\Vert{}^2S\rangle$ of the atomic dipole moment operator $d$ with respect to nonrelativistic atomic states $|{}^{2S+1}L\rangle$ using the conventions of Ref. [66]. Finally, the repulsive $C_{6,0_u^+}/R^6$ potential represents the dispersion contribution from doubly excited molecular states.

Table I gives our values for the parameters used in Eq. (1). The nonrelativistic or weighted atomic transition energies between the barycenters of ground state $4d^{10}5p({}^2S)$ and excited state $4d^{10}5p({}^2P)$ and the relativistic spin-orbit splitting between the $4d^{10}5p({}^2P_{1/2})$ and $4d^{10}5p({}^2P_{3/2})$ states have been derived from data in Ref. [17] and can be considered exact for our purposes. The table also gives the weighted line strength $S_{{}^2P\to{}^2S}$, the square of the reduced transition matrix element for the $4d^{10}5p({}^2S)$ and $4d^{10}5p({}^2P)$ transition as well as the Einstein $A$ coefficient and natural linewidth $\gamma_P$ of the nonrelativistic $4d^{10}5p({}^2P)$ state. We use the theoretical value for the line strength of Ref. [67] and obtained by third-order many-body perturbation theory. We conservatively inferred a 15 % standard uncertainty from the discussion in the first column of page 5 of Ref. [67]. The value for $S_{{}^2P\to{}^2S}$ by Ref. [67] coincides with a recent theoretical evaluation in Ref. [68], while the authors of Refs. [69,70] prefer a value close to the lower bound of our $S_{{}^2P\to{}^2S}$. Experimental determinations also favor a value close to this lower bound, approximately $15e^2a_0^2$ [71–73]. The most precise experimental evaluation gives $S_{{}^2P\to{}^2S}=15.10(5)e^2a_0^2$ [73]. A review of all measurements can be found in Ref. [74]. Our value for $C_3$ and $C_{6,0_u^+}$, the latter derived from our electronic structure calculations of excited Ag$_2$ states, are listed in Table I.

> [!figure]
> ![[Fig. 5.png|center|500]]
> **Figure 5.** Eigenenergies (colored line segments) of the “rotationless” $J=1$ vibrational levels of the excited $0_u^+$ potential of $^{109}$Ag$_2$ within $hc \times 100$ cm$^{-1}$, $hc \times 10$ cm$^{-1}$, and $hc \times 1$ cm$^{-1}$ of its $5s({}^2S_{1/2})+5p({}^2P_{1/2})$ dissociation limit in panels (a), (b), and (c), respectively. The orange curve correspond to the $0_u^+$ potential. We have used $C_3=2.9E_h a_0^3$ for this graph.

Figure 5 shows the long-range potential-energy curve of our $0_u^+$ state as well as eigenenergies $E_v$ of $J=1$ vibrational levels $v$ of this potential for the $^{109}$Ag$_2$ isotopologue. From left to right the three panels in the figure show eigenenergies down to $hc \times 100$ cm$^{-1}$, $hc \times 10$ cm$^{-1}$, and $hc \times 1$ cm$^{-1}$ below its $5s({}^2S_{1/2})+5p({}^2P_{1/2})$ dissociation limit, respectively. The eigenenergies have been computed numerically by discretizing the Hamiltonian containing the sum of the relative radial kinetic-energy operator of the atoms $-(\hbar^2/2\mu)d^2/dR^2$ with reduced mass $\mu$, centrifugal potential $\hbar^2J(J+1)/(2\mu R^2)$, and the potential-energy curve of our $0_u^+$ state using the discrete variable representation of Ref. [75] and solving the resulting matrix eigenvalue problem with a linear algebra package. For small separations, where the binding energies of the $0_u^+$ potential are larger than $hc \times 100$ cm$^{-1}$, we smoothly connect the long-range potential in Eq. (1) to our electronic structure calculation of this state as described in Sec. II.

We observe that the outer turning points $R_O$, defined as $V(R_O;0_u^+)=E_v$, range from $20a_0$ for binding energies near $hc \times 100$ cm$^{-1}$ to around $200a_0$ for binding energies near $hc \times 0.1$ cm$^{-1}$. The accuracy of our $0_u^+$ potential is not sufficient to predict the location of individual levels. The level spacing or density, however, is reasonably accurate.

Within the model of Ref. [65] we can also estimate the molecular transition dipole moments to, and natural linewidths of, weakly bound rovibrational levels of the excited $0_u^+$ state dissociating to the $4d^{10}5s({}^2S)+4d^{10}5p({}^2P_{1/2})$ limit. First, we realize that in one-color photoassociation experiments with an ultracold Ag gas with atoms in the $f=1$ hyperfine state and equal population in the $m$ states, we collide in superpositions of the $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ electronic states. Photon selection rules only allow transitions from the $X{}^1\Sigma_g^+$ component of the superposition to the excited $0_u^+$ state. Some algebra shows that the molecular electric transition dipole moment between the $X{}^1\Sigma_g^+$ and the excited $0_u^+$ states and the natural linewidth of the excited $0_u^+$ state are

$$
d_{\rm eff}(0_u^+)=\sqrt{\frac{2}{3}}\langle{}^2P\Vert d\Vert{}^2S\rangle\quad\text{and}\quad\gamma_{0_u^+}=\frac{2}{3}\gamma_P
\tag{2}
$$

respectively. We expect that the transition dipole moment for the superposition state is within factors of two from $d_{\rm eff}(0_u^+)$ and, for simplicity, we assume that $d_{\rm eff}(0_u^+)$ is the correct value for the dipole moment for the remainder of this paper.

Second, we recall that for $R>20a_0$ the potential energies of the $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ states are identical and to good approximation are given by the van der Waals potential $V_{\rm vdW}(R)=-C_6/R^6$. Our preferred values for dispersion coefficient $C_6$, van der Waals length $\beta_6=(2\mu C_6/\hbar^2)^{1/4}$, and energy $E_6=\hbar^2/(2\mu\beta_6^2)$ are given in Table I. From Fig. 5, we observe that for $R>20a_0$ the rovibrational levels of the excited $0_u^+$ state have binding energies less than $hc \times 100$ cm$^{-1}$.

We are now ready to introduce the event rate coefficient of photoassociation for two ultracold atoms colliding with relative kinetic or collision energy $E$ assuming that $s$ or $\ell=0$ partial-wave collisions contribute to rovibrational level $v$ of the $J=1$ excited $0_u^+$ state using laser light with photon energy $\hbar\omega$. In fact, we have the event rate coefficient [76–78]

$$
K_v(\hbar\omega,E)=v_{\rm rel}\frac{\pi}{k_{\rm rel}^2}\frac{\hbar^2\gamma_{0_u^+}\gamma_v(E)}{\{E+\hbar\omega-[E_\infty+E_v(0_u^+)]\}^2+\hbar^2[\gamma_{0_u^+}+\gamma_v(E)]^2/4}
\tag{3}
$$

for each vibrational level $v$, where $E=\hbar^2k_{\rm rel}^2/2\mu=\mu v_{\rm rel}^2/2$, $\gamma_{0_u^+}$ is the natural linewidth of the excited-state vibrational level, $E_\infty$ is the asymptotic energy of the excited $0_u^+$ state relative to that of the ground state when $R\to\infty$, $E_v(0_u^+)<0$ is the binding energy of the vibrational level, and stimulated width

$$
\gamma_v(E)=\frac{2\pi}{\hbar}\left|\langle\Psi_v(0_u^+)|\mathbf{d}\cdot\mathbf{E}_{\rm elec}|\psi_g^{(+)}(E)\rangle\right|^2
\tag{4}
$$

Here, $\psi_g^{(+)}(R,E)=\langle R|\psi_g^{(+)}(E)\rangle$ and $\Psi_v(R;0_u^+)=\langle R|\Psi_v(0_u^+)\rangle$ are radial wave functions of the ground and excited state as functions of $R$, respectively. Excited $0_u^+$ rovibrational wave functions are unit normalized with $\int_0^\infty dR|\Psi_v(R;0_u^+)|^2=1$ and the s-wave scattering wave function is energy-normalized with

$$
\psi_g^{(+)}(R,E)\to e^{i\eta_g(E)}\sqrt{\frac{2\mu}{\pi\hbar^2}}\frac{\sin[k_{\rm rel}R+\eta_g(E)]}{\sqrt{k_{\rm rel}}}
\tag{5}
$$

for $R\to\infty$, where $\eta_g(E)$ is the scattering phase shift. Moreover, operator $-\mathbf{d}\cdot\mathbf{E}_{\rm elec}$ represents the light-induced coupling, where vector $\mathbf{d}$ is the dipole moment operator and vector $\mathbf{E}_{\rm elec}=\mathcal{E}_0\boldsymbol{\epsilon}\cos(k_Lz-\omega t)$ is the electric field of the laser beam propagating along the space-fixed $z$ axis. The field has polarization $\boldsymbol{\epsilon}$, wave number $k_L=\omega/c$, and electric-field strength $\mathcal{E}_0$. Using the rotating-wave approximation and Eq. (2) we have

$$
-\mathbf{d}\cdot\mathbf{E}_{\rm elec}\to-\frac{1}{2}d_{\rm eff}(0_u^+)\mathcal{E}_0=-Q\frac{d_{\rm eff}(0_u^+)}{ea_0}\sqrt{\frac{I}{\mathrm{W/cm^2}}}
\tag{6}
$$

energy $Q=a_0[2\pi\alpha\hbar(1\,\mathrm{W/cm^2})]^{1/2}=h\times17.561\,264$ MHz, and laser intensity $I$. In addition to the approximations inherent in Eq. (2), we have also omitted angular-momentum factors, of order unity, from evaluating $\mathbf{d}\cdot\boldsymbol{\epsilon}$ for colliding $f=1$ hyperfine states and $J=1$ levels of the $0_u^+$ state.

In ultracold-atom experiments both atoms are lost in the photoassociation process and thus the observed thermalized loss rate coefficient is $K_{\rm tot}(\hbar\omega,kT)=2\sum_v\langle K_v(\hbar\omega,E)\rangle$, where the angled brackets indicate a thermal average assuming a Boltzmann distribution at temperature $T$ of the atomic gas. Photoassociation lineshapes of $K_{\rm tot}(\hbar\omega,kT)$ have been studied in Ref. [79]. In practice, energy widths $\hbar\gamma_s$ and $kT$ are orders of magnitude smaller than the energy spacing between vibrational levels. Finally inspection of Eq. (3) and the observation that $\gamma_v(E)\propto\sqrt{E}$ for small $E$, as shown later on, implies that $K_v(\hbar\omega,E)$ is independent of $E$ for $E\to0$.

Julienne in Ref. [77] also derived that for ultracold collisions the stimulated width $\gamma_v(E)$ has an accurate analytical form based on the reflection approximation, where (1) the matrix element of $-\mathbf{d}\cdot\mathbf{E}_{\rm elec}$ is mainly determined by the radial scattering and bound-state wave functions over a small spatial region near the outer turning point $R_O$ or more precisely the Condon point $R_C$ of the transition and (2) $|V_{\rm vdW}(R)|\ll|V(R;0_u^+)|$ for $R>20a_0$. The Condon point is that separation, where for a given laser frequency the local kinetic energies in the ground and excited state are the same. Then the reflection approximation gives

$$
\gamma_v(E)=\frac{2\pi}{\hbar}Q^2\frac{I}{\mathrm{W/cm^2}}\left(\frac{d_{\rm eff}(0_u^+)}{ea_0}\right)^2\frac{dE_v(0_u^+)}{dv}\frac{1}{D_C}\left|\psi_g^{(+)}(R_C,E)\right|^2
\tag{7}
$$

a function proportional to the square of the absolute value of the ground-state scattering wave function, where slope

$$
D_C=\left|\frac{d}{dR}[V(R;0_u^+)-V_{\rm vdW}(R)]_{R=R_C}\right|\approx4\frac{C_3}{R_C^4}
\tag{8}
$$

and the Condon point is found from

$$
-\frac{4}{3}\frac{C_3}{R_C^3}=E_v(0_u^+)
\tag{9}
$$

ignoring the dispersion contributions from both potentials. Furthermore, the LeRoy-Bernstein approximation for weakly bound states of an attractive $1/R^3$ potential [80] gives

$$
\frac{dE_v(0_u^+)}{dv}=s_3\left(-\frac{E_v(0_u^+)}{E_3}\right)^{5/6}E_3
\tag{10}
$$

with energy $E_3=\hbar^2/(2\mu\beta_3^2)$, length $\beta_3=2\mu(4C_3/3)/\hbar^2$ evaluated for the coefficient of the $1/R^3$ potential of the $0_u^+$ state, and $s_3=6\sqrt{\pi}\Gamma(4/3)/\Gamma(5/6)=8.413\,092\ldots$, where $\Gamma(z)$ is the Gamma function.

> [!figure]
> ![[Fig. 6.png|center|500]]
> **Figure 6.** Stimulated widths $\gamma_v(E)$ for the transition from two colliding ultracold $^{109}$Ag atoms to $J=1$ vibrational levels of the excited $0_u^+$ state as functions of their binding energy at laser intensity $I=1$ W/cm$^2$ and collision energy $E=E_6\approx k\times193$ $\mu$K. The colored and dashed curves are for the scattering lengths $a=-0.5\beta_6$, $0$, $0.25\beta_6$, $0.5\beta_6$, $\beta_6$, and $2\beta_6$, respectively. We have used the nominal, most-likely value for the van der Waals coefficient $C_6$ for the ground-state collision and nominal values for $4C_3/3$, $d_{\rm eff}(0_u^+)$, and $\gamma_{0_u^+}$ using Eq. (2) and the data in Table I. Widths for other laser intensities and collision energies $E\le E_6$ can be found from $\gamma_v(E)\propto I\sqrt{E}$.

Our final ingredient in obtaining an analytical expression for the stimulated width is observing that the s-wave ground-state wave function for collision energies around and below the van der Waals energy $E_6$, i.e., assuming the Wigner threshold law for $E\to0$, is [28,81–83]

$$
\psi_g^{(+)}(R,E)=\frac{1}{\sqrt{2\pi}}\frac{1}{\sqrt{E_6\beta_6}}\sqrt{k_{\rm rel}\beta_6}\sqrt{x}\left[\Gamma(3/4)J_{-1/4}\left(\frac{1}{2x^2}\right)-2\frac{a}{\beta_6}\Gamma(5/4)J_{1/4}\left(\frac{1}{2x^2}\right)\right]
\tag{11}
$$

for $R>20a_0$ and $k_{\rm rel}|R-a|<\pi/2$, where $x=R/\beta_6$, $a$ is the scattering length, and $J_\nu(z)$ is the Bessel function of the first kind. Inserting Eq. (11) into Eq. (7) shows that the stimulated width $\gamma_v(E)\propto\sqrt{E}$ as promised. Currently, the uncertainties of the short-range, $R<20a_0$ shape of the potentials of the $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ states is such that the value for $a$ is unknown and can lie between $-\infty$ and $+\infty$. The authors of Ref. [81], however, have shown that the probability distribution for $a$ is a Cauchy or Lorentz distribution with its maximum at the mean scattering length $\bar{a}=\Gamma(3/4)\beta_6/[2\sqrt{2}\Gamma(5/4)]\approx0.478\beta_6$ and its half-width at half-maximum (HWHM) also equal to $\bar{a}$. See Table I for the value for $\bar{a}$ for $^{109}$Ag + $^{109}$Ag.

Figure 6 shows stimulated widths for the excited $0_u^+$ state and ultracold $^{109}$Ag atoms at laser intensity $I=1$ W/cm$^2$ and collision energy $E=E_6$ based on our analytical expression for s-wave collisions as functions of binding energy $E_v(0_u^+)$ for several scattering lengths $a$ around $\bar{a}$. A laser intensity of 1 W/cm$^2$ is typical for photoassociation experiments while the temperature of Ag atoms in a magneto-optical trap is of order $E_6/k$. In optical dipole traps the temperature is much smaller than $E_6/k$. In an experiment the curves are only sampled at a discrete set of $E_v(0_u^+)$ corresponding to the measured binding energies. We have used the nominal, most likely parameter values from Table I. The stimulated widths for other $I$ and $E<E_6$ follow from the fact that $\gamma_v(E)\propto I\sqrt{E}$.

The stimulated widths as a function of binding energy in Fig. 6 alternate between zeros and maxima with maximum values ranging from $2\pi\times0.01$ MHz to $2\pi\times0.1$ MHz for energies $|E_v(0_u^+)|<hc\times5$ cm$^{-1}$. The location of the zeros is very sensitive to the scattering length, where for increasing $a$ the zeros move to less negative binding energies. These zeros in the widths correspond to the zeros of the radial scattering wave function of Eq. (11) using the relationship between the Condon point and $E_v(0_u^+)$ from Eq. (9). In fact, the zeros in $\gamma_v(E)$ for binding energies in $hc\times[-40,-15]$ cm$^{-1}$ and $<hc\times-10$ cm$^{-1}$ correspond to nodes in the scattering wave function between $R=[27a_0,40a_0]$ and $R>40a_0$, respectively. Hence, the precise binding energy of the zeros in the stimulated width can be used to determine the scattering length and, to a lesser extent, the van der Waals coefficient. Finally, the various curves cross at $E_v(0_u^+)/hc\approx46.0$ cm$^{-1}$ and $14.9$ cm$^{-1}$, where the Bessel function multiplying the scattering length is zero. While visually striking, the crossings cannot be used to determine $a$ from experimental data.

For binding energies in $hc\times[-1,0]$ cm$^{-1}$, the stimulated width is on the order of the natural linewidth of $2\pi\times17(3)$ MHz for the $0_u^+$ state even for $I=1$ W/cm$^2$. For vibrational levels in this binding-energy range, the event rate coefficient can thus saturate and approach the unitarity limit $v_{\rm rel}\pi/k_{\rm rel}^2$ when $\gamma_v(E)=\gamma_{0_u^+}$, which is $1.8\times10^{-11}$ cm$^3$/s at $E=E_6$ for Ag + Ag.

Finally, we note that the validity of the Wigner threshold law with which we derived Eq. (11) is not guaranteed for collision energies near $E_6$, especially for scattering lengths $a\gg\beta_6$. For example, phase factor $e^{i\eta_g(E)}$ in Eq. (5) can significantly deviate from one. In practice, numerical simulations of the scattering wave function are required for energies larger than $E_6$. Nevertheless, we show widths at $E=E_6$ as it is the natural energy scale of the van der Waals potential and we can use their $\sqrt{E}$ dependence to infer widths at smaller collision energies.

> [!figure]
> ![[Fig. 7.png|center|500]]
> **Figure 7.** Stimulated widths $\gamma_v(E)$ for the transition from two colliding ultracold $^{109}$Ag atoms to $J=1$ vibrational levels of the excited $0_u^+$ state as functions of their binding energy at $I=1$ W/cm$^2$ and $E=E_6\approx k\times193$ $\mu$K. The two curves correspond to widths at two different line strengths $S_{{}^2P\to{}^2S}$ but the same $a=0.5\beta_6$. We have used the nominal value for the van der Waals coefficient $C_6$ from Table I. Widths for other laser intensities and collision energies $E\le E_6$ can be found from $\gamma_v(E)\propto I\sqrt{E}$.

Figure 7 shows stimulated widths as a function of binding energy between $hc\times[-10,0]$ cm$^{-1}$ for two line strengths $S_{{}^2P\to{}^2S}$ but the same van der Waals coefficient and scattering length $a=+0.5\beta_6$, close to the mean scattering length. The two $S_{{}^2P\to{}^2S}$ correspond to our nominal value of $17.4e^2a_0^2$ from Table I and that obtained from the most accurate measurement of Ref. [73] of $15.1e^2a_0^2$. A different line strength implies a change in the long-range $-(4/3)C_3/R^3$ potential of the excited $0_u^+$ state. Hence, even though the zeros in the scattering wave function are at the same separations, Eq. (9) implies that in the binding-energy domain the zeros of the stimulated width occur at different $E_v(0_u^+)$. For $a=+0.5\beta_6$ we have a zero near $hc\times-4$ cm$^{-1}$, where the vibrational level spacing is about $hc\times0.25$ cm$^{-1}$ from Fig. 5(b).

## IV. Fano-Feshbach resonances in ultracold silver atom collisions

In this section we describe our simulations of ultracold collisions between two silver atoms in their electronic spin-1/2 ${}^2S$ ground state. The goal is to determine the properties of Fano-Feshbach resonances in these collisions. The structure of the Hamiltonian for two silver atoms is the same as that for alkali-metal atoms [48,84]. The kinetic-energy operator contained in the Hamiltonian is $(-\hbar^2d^2/dR^2+\ell^2/R^2)/2\mu$, where $\ell$ is the relative mechanical angular-momentum operator for the two atoms. Next, Fermi-contact interactions describe the coupling between the electron spin $\mathbf{s}_j$ of silver atom $j=1$ or $2$ couples to its nuclear spin $\mathbf{i}_j$. Zeeman interactions for each spin describe the effects of a magnetic field with strength $B$, where the direction of the magnetic field defines our quantization axis for the spins. The nuclear-spin quantum number of both $^{107}$Ag and $^{109}$Ag isotopes is 1/2.

Three additional interactions that depend on separation $R$ and/or orientation $\hat{R}$ relative to the magnetic-field direction are included. The strongest by far leads to the $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ Born-Oppenheimer (BO) electronic states. These are states with total molecular electron spin $\mathbf{S}=\mathbf{s}_1+\mathbf{s}_2$ equal to 0 and 1, respectively. Their electronic potential-energy surfaces are shown in Fig. 2. The remaining interactions are the weaker and anisotropic second-order spin-orbit and magnetic dipole-dipole interactions that couple the electron spins $\mathbf{s}_j$ of the atoms to the mechanical rotation of the di-atom and lift the degeneracy of the $\Omega=0_u^-$ and $1_u$ components of the $a{}^3\Sigma_u^+$ state, where $\Omega$ is the absolute value of the projection quantum number of the sum of all electron angular momenta along the internuclear axis. The splitting between the $\Omega=0_u^-$ and $1_u$ components is shown in Fig. 4.

> [!figure]
> ![[Fig. 8.png|center|500]]
> **Figure 8.** The four hyperfine states of the electronic ground state of (a) $^{107}$Ag and (b) $^{109}$Ag isotopes as functions of magnetic field strength $B$. The four states are labeled $a$, $b$, $c$, and $d$ in order of increasing energy. Here, a field strength of 1 G corresponds to 0.1 mT [85].

The energies of the hyperfine states of $^{107}$Ag and $^{109}$Ag atoms as functions of $B$ are shown in Fig. 8. Absent a magnetic field, the total atomic angular momentum $\mathbf{f}_j=\mathbf{s}_j+\mathbf{i}_j$ and its projection operator $f_{jz}$ along the magnetic-field direction are conserved with quantum numbers $f_j=0$ or $1$ and $m_j$. At finite $B$ only $f_{jz}$ is conserved and atomic hyperfine states are $B$-dependent superpositions of $f_j=0$ and $f_j=1$ states for $m_j=0$ and pure $f_j=1$ states for $m_j=\pm1$. Unlike atomic hydrogen, both silver isotopes have an inverted hyperfine structure, where at $B=0$, the three states with quantum number $f_j=1$ have lower energies than that of the $f_j=0$ state. For the remainder of this paper, we label the four states by $a$, $b$, $c$, and $d$ in order of increasing energy. Further details about the Hamiltonian can be found in Appendix B.

> [!figure]
> ![[Fig. 9.png|center|500]]
> **Figure 9.** Scattering length $a_s$ for the zero energy collision of $^{107}$Ag atoms in hyperfine state (a) $a$ and (b) $b$ as functions of magnetic field $B$. Notice the different scales along the $y$ axes of the two panels. We have used our nominal atom-atom interaction potentials.

Figures 9(a) and 9(b) show scattering lengths $a_s$ as functions of $B$ up to 1500 G for ultracold, colliding $^{107}$Ag atoms with both atoms in hyperfine states $a$ and $b$, respectively, using our nominal, most likely BO potentials and second-order spin-orbit interaction. Absent inelastic processes, where the hyperfine state of one or both atoms changes in the collision, the scattering length for $\ell=0$ collisions is defined as $a_s=-[\tan\eta(E)]/k\in(-\infty,+\infty)$ in the limit $E\to0$ [47] with collision energy $E=\hbar^2k^2/2\mu$, collision wave number $k$, and reduced mass $\mu$ given by half the mass of the silver atom. Here, $\eta(E)$ is the energy-dependent $\ell=0$ scattering phase shift of the only open channel in the calculation. For the collision between two $a$ hyperfine states, we have $m_{\rm tot}=-2$ and only include $\ell=0$ and 2 states; that is, $s$ and $d$ partial waves. This choice leads to eight coupled channels, with exactly one s-wave channel. Only the s- and d-wave $|\{aa\}_+\rangle$ or $a+a$ channels are open. For the collision of two $b$ hyperfine states, we have $m_{\rm tot}=0$ and only include $\ell=0$ or s-wave channels. This choice leads to four coupled channels, where the $|\{bb\}_+\rangle$ or $b+b$ channel is the only open channel. In actuality, the calculations presented in this figure and other figures concerning Fano-Feshbach resonances have been performed at $E=k\times1$ $\mu$K. Finally, we note that experimentally gasses of ultracold atoms can be prepared in any hyperfine state using microwave spectroscopy. A description of this technique applied to cesium atoms can be found in Ref. [86].

We observe that Figs. 9(a) and 9(b) have magnetic-field regions where the scattering length rapidly changes between $+\infty$ and $-\infty$. These are the Fano-Feshbach resonances [47] of colliding ultracold silver atoms and near each resonance the scattering length can be modeled by the function [87]

$$
a_s(B)=a_{\rm bg}\left(1-\frac{\Delta}{B-B_0}\right)
\tag{12}
$$

where $a_{\rm bg}$ is the $B$-independent background scattering length, $B_0$ is the resonant magnetic-field strength, and $\Delta$ is the magnetic width of the resonance. Here, $a_{\rm bg}$ and $\Delta$ can have negative or positive values. The scattering length is zero when $B=B_0+\Delta$. The nearest-neighbor spacing between the resonances is typical for that observed for alkali-metal and chromium atoms [47] and is thus orders of magnitude larger than that observed for magnetic lanthanide atoms [52].

The magnetic widths of the Fano-Feshbach resonances for $a+a$ collisions in Fig. 9(a) are positive and no larger than 0.1 G (but typically much smaller). These widths, found by fitting $a_s(B)$ for a small-$B$-field region around each resonance to Eq. (12), are sufficiently large for experiments aiming to form weakly bound molecular states using magneto-association. The seven resonances in the $a+a$ collision are absent when only the single s-wave channel is included in the scattering calculations. Hence, they are d-wave resonances where coupling between s- and d-wave channels is solely due to the weak anisotropic second-order spin-orbit and magnetic dipole-dipole interactions. Angular-momentum analysis shows that the s-wave channel is, in fact, a molecular electron spin $S=1$ state and we find that the background scattering length away from the resonances is to very good approximation equal to the $+14.7a_0$ scattering length of our nominal $a{}^3\Sigma_u^+$ potential.

The magnetic widths of the three Fano-Feshbach resonances for $b+b$ collisions in Fig. 9(b) are also positive and on the order of 10 G, much larger than those for $a+a$ collisions. The resonances define so-called s-wave resonances. When we add d-wave channels with $m_{\rm tot}=0$ in the calculations for $b+b$ collisions, not shown in this panel, the rate coefficients for the inelastic or spin-flip processes to $\ell=2$, $a+b$ and $\ell=2$, $a+a$ channels are extremely small, less than $10^{-13}$ cm$^3$/s for all $B<1500$ G, except when $|B-B_0|\lesssim\Delta$. Including d-wave channels also adds narrow Fano-Feshbach resonances with magnetic widths of the same order of magnitude as those observed in $a+a$ collisions. The broader s-wave Feshbach resonances can be useful for simulating quantum many-body Hamiltonians. The background scattering length for $b+b$ collisions in Fig. 9(b) is approximately $20a_0$, decreases by about $5a_0$ over 1500 G, and neither corresponds to the scattering length of the our nominal $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ potentials.

We can compare the background scattering lengths for $a+a$ and $b+b$ collision with the most likely or mean value for the scattering length [81] defined in the previous section. For $^{107}$Ag + $^{107}$Ag, we have $\bar{a}=43.2(2.5)a_0$. In other words, for our nominal interaction potentials the background scattering lengths are relatively small. Table I lists $\bar{a}$ for the $^{109}$Ag + $^{109}$Ag isotopologue.

> [!figure]
> ![[Fig. 10.png|center|500]]
> **Figure 10.** (a) Scattering length $a_s$ for the zero-energy collision of $^{107}$Ag atoms in hyperfine state $a$ and (b) the energies of the least-bound $m_{\rm tot}=-2$ di-atomic bound states as functions of magnetic field $B$. The scattering length is infinite when a bound state has zero binding energy. Blue curves correspond to calculations that only include s- and d-wave channels. Red curves correspond to calculations that include s-, d-, and g-wave channels. On the scale of the figures the red and blue curves are often indistinguishable and thus underneath each blue curve there lies a red curve. We have used the nominal atom-atom interaction potentials.

Figure 10 provides two additional observations about the Fano-Feshbach resonances of $^{107}$Ag. Figure 10(a) shows the scattering length of ultracold $a+a$ collisions as a function of $B$ when we only include s- and d-wave channels with $m_{\rm tot}=-2$ as well as when we include all $\ell=4$ or g-wave channels with $m_{\rm tot}=-2$. We observe additional narrow so-called g-wave resonances when we include g-wave channels. The already present d-wave resonances change their resonance position by no more than 0.05 G. Similarly, the value of the resonance width and background scattering length does not change significantly, i.e., by less than 1 %.

Figure 10(b) shows the binding energies of the most weakly bound bound states with $m_{\rm tot}=-2$ as functions of the magnetic field. Each collisional Fano-Feshbach resonance in Fig. 10(a) corresponds to the appearance of a bound state with zero binding energy at the same magnetic-field strength. Less visible is that all bound levels avoid each other as a function of $B$. We also observe that the magnetic field lifts Zeeman level degeneracies at $B=0$. At $B=0$ and ignoring the weak anisotropic interactions, orbital angular momentum $\ell$, molecular angular momentum $\mathbf{F}=\mathbf{f}_1+\mathbf{f}_2$, and its space-fixed projection operator $F_z$ are conserved. Hence, we assign the corresponding quantum numbers $\ell$, $F$, and $M$ to each bound level. For example, the single level with a $B$-independent binding energy of $-h\times0.25$ GHz is the last s-wave bound state of the $a{}^3\Sigma_u^+$ potential. The two levels with a binding energy of $-h\times0.85$ GHz at $B=0$ are d-wave $F=1$ levels with $M=0$ and $-1$ leading to Fano-Feshbach resonances near $B=290$ G and 460 G, respectively.

The shapes of the two Born-Oppenheimer potentials are to a certain degree uncertain because both their depth and the common long-range van der Waals coefficient have uncertainties. For example, the potentials of the $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ states have 131(1) and 38.0(0.5) $\ell=0$ or s-wave vibrational levels for $^{107}$Ag$_2$ when $C_6=342E_h a_0^6$, respectively, where the number in parentheses corresponds to the standard uncertainty in the number of bound states when the depths of the short-range potentials are varied within their standard uncertainties of $hc\times200$ cm$^{-1}$ for the $X{}^1\Sigma_g^+$ state and $hc\times80$ cm$^{-1}$ for the $a{}^3\Sigma_u^+$ state. Changing the shape of the potentials changes the location and magnetic width of the Fano-Feshbach resonances as well as the background scattering length.

In Fig. 11 we show the changes in resonance locations $B_0$ and magnetic widths $\Delta$ for $^{107}$Ag $a+a$ collisions including only s- and d-wave channels with $m_{\rm tot}=-2$ as functions of the change in depth $\Delta V_X$ of the $X{}^1\Sigma_g^+$ potential by just over one standard uncertainty of the depth of this potential. The depth change in $\Delta V_X$ is $hc[-255,5]$ cm$^{-1}$, where our nominal $X{}^1\Sigma_g^+$ potential has $\Delta V_X/hc=0$ cm$^{-1}$. The depth of the $a{}^3\Sigma_u^+$ potential and the long-range dispersion coefficients are those used to obtain the two previous figures; that is, $\Delta V_a/hc=0$ cm$^{-1}$ and $C_6=342E_h a_0^6$. We describe how the depth of the Born-Oppenheimer potentials is changed without introducing discontinuities in Appendix A.

> [!figure]
> ![[Fig. 11.png|center|500]]
> **Figure 11.** Panel (a) shows locations $B_0$ of the narrow d-wave Fano-Feshbach resonances for $a+a$ collisions of $^{107}$Ag atoms as functions of the change in depth $\Delta V_X$ of the $X{}^1\Sigma_g^+$ Born-Oppenheimer potential at fixed long-range van der Waals coefficient $C_6=342E_h a_0^6$. S- and d-wave channels with $m_{\rm tot}=-2$ have been included. The horizontal black dashed lines highlight the “repeating” locations of the Fano-Feshbach resonances as explained in the text. Panel (b) shows a parametric graph of magnetic widths $\Delta$ and resonance locations $B_0$ as a function of $\Delta V_X$. The range of $\Delta V_X$ is the same as that shown in panel (a). Note that a blue (red) section of the curve in panel (b) corresponds to one and only one blue (red) curve in panel (a).

Figure 11(a) shows that the locations of the resonance over this range of depth are “repeating” over a depth range of $\approx hc\times270$ cm$^{-1}$, slightly larger than shown in the figure. That is, the resonance positions and their slopes $dB_0/d\Delta V_X$ on the left- and right-hand sides of Fig. 11(a) are the same. This behavior is reinforced in Fig. 11(b), where we parametrically plot the resonance widths $\Delta$ and positions as functions of $\Delta V_X$ for each of the seven resonances. The seven sections form a single continuous curve, where the broadest but still narrow resonances occur around magnetic field values of 1500 G. Following Ref. [47] resonances are considered narrow when $\Delta\ll1$ G. The origin of the repeating pattern and the continuous $\Delta$ versus $B_0$ function is the fact that, over a depth range of $\approx hc\times270$ cm$^{-1}$ the $X{}^1\Sigma_g^+$ potential loses exactly one s- as well as one d-wave bound state. Moreover, the last s-wave $X{}^1\Sigma_g^+$ bound state for $\Delta V_X=hc\times-255$ cm$^{-1}$ has approximately the same binding energy as its last s-wave bound state when $\Delta V_X=hc\times15$ cm$^{-1}$, as the least-bound bound states have outer turning points where the potential is well characterized by the dispersion potential. Small breakdowns to this repeating pattern exist and are due to the finite depth of the $X{}^1\Sigma_g^+$ potential.

> [!figure]
> ![[Fig. 12.png|center|500]]
> **Figure 12.** Panel (a) shows locations $B_0$ of the broad s-wave Fano-Feshbach resonances for $b+b$ collisions of $^{107}$Ag atoms as functions of the change in depth $\Delta V_X$ of the $X{}^1\Sigma_g^+$ Born-Oppenheimer potential at fixed long-range van der Waals coefficient $C_6=342E_h a_0^6$. Only s-wave channels with $m_{\rm tot}=0$ have been included. The horizontal black dashed lines highlight the “repeating” locations of the Fano-Feshbach resonances as explained in our discussion of Fig. 11. Panel (b) shows a parametric graph of magnetic widths $\Delta$ and resonance locations $B_0$ as a function of $\Delta V_X$. The range of $\Delta V_X$ is the same as that shown in panel (a). Note again that a blue (red) section of the curve in panel (b) corresponds to one and only one blue (red) curve in panel (a).

Figure 12 shows similar data for $^{107}$Ag $b+b$ collisions including only s-wave channels with $m_{\rm tot}=0$ and showing a slightly different range of $\Delta V_X$. The repetition with respect to depth change $\Delta V_X$ over $\approx hc\times270$ cm$^{-1}$ is again apparent. The magnetic width of the resonances, however, is large with values as large as 180 G.

The full dependence of the Ag + Ag resonance locations and widths follows from varying both the depths of the singlet $X{}^1\Sigma_g^+$ and the triplet $a{}^3\Sigma_u^+$ potentials as well as van der Waals coefficient and second-order spin-orbit strength. For a changing depth of the $a{}^3\Sigma_u^+$ potential the resonance locations repeat when this triplet potential loses a bound state. In fact, at a fixed van der Waals coefficient and second-order spin-orbit strength, the repeating pattern of resonance locations can be encoded on the surface of a torus. Changing the van der Waals coefficient or the second-order spin-orbit strength does not lead to repeating patterns.

The parameters in the $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ Born-Oppenheimer potentials, i.e., $\Delta V_X$, $\Delta V_a$, and $C_6$, can also be constrained by comparing the positions of the Fano-Feshbach resonance for the three isotopologues $^{107}$Ag + $^{107}$Ag, $^{109}$Ag + $^{109}$Ag, and $^{107}$Ag + $^{109}$Ag. The only changes in the Hamiltonian are the values for the reduced mass in the kinetic-energy operator, the hyperfine constants, and nuclear $g$ factors. That is, to very good approximation the Born-Oppenheimer potentials are independent of isotopologue. Figure 13 shows such a comparison for the collision, where both Ag atoms are in hyperfine state $b$ including only the allowed s-wave channels with $m_{\rm tot}=0$ and $E/k=1$ $\mu$K. The graphs shows resonance locations $B_0$ as functions of the change in depth of the $X{}^1\Sigma_g^+$-state potential over the same range as in Figs. 11 and 12, again using the nominal $a{}^3\Sigma_u^+$ potential and $C_6=342E_h a_0^6$. We observe two or three s-wave resonances in the magnetic-field range below 1500 G for each of the homonuclear $^{107}$Ag + $^{107}$Ag and $^{109}$Ag + $^{109}$Ag isotopologues, and twice as many for the heteronuclear $^{107}$Ag + $^{109}$Ag system (corresponding to the near doubling of the number of closed channels).

> [!figure]
> ![[Fig. 13.png|center|500]]
> **Figure 13.** Locations $B_0$ of the broad s-wave Fano-Feshbach resonances for $b+b$ collisions of $^{107}$Ag + $^{107}$Ag (red curves), $^{109}$Ag + $^{109}$Ag (blue curves), and $^{107}$Ag + $^{109}$Ag (orange curves) isotopologues as functions of the change in depth $\Delta V_X$ of the $X{}^1\Sigma_g^+$ Born-Oppenheimer potential at fixed long-range van der Waals coefficient $C_6=342E_h a_0^6$. Only s-wave channels with $m_{\rm tot}=0$ have been included.

## V. Conclusion

In this paper, we have reported on computations probing bound states of the ground and excited states of the Ag$_2$ molecule by one-photon photoassociation spectroscopy and magneto-association. We have suggested means to accurately determine the long-range dispersion coefficients for ground and excited-state potentials. Our findings will aid efforts to produce ultracold gases of Ag atoms, as knowledge of s-wave scattering lengths is needed to perform efficient evaporative cooling. Our results are also an important step towards efficient and coherent production of Ag$_2$ molecules via association from ultracold atoms using Fano-Feshbach resonances. Ultracold Ag$_2$ molecules have bright prospects for novel quantum gases with long-range and anisotropic interactions, and applications in precision measurements.

## Acknowledgments

Work at Temple University is supported by the Gordon and Betty Moore Foundation Grant No. GBMF12330, U.S. National Science Foundation Grant No. PHY-2409425, and the U.S. Air Force Office of Scientific Research Grant No. FA9550-21-1-0153.

## Data availability

The data that support the findings of this article are not publicly available. The data are available from the authors upon reasonable request.

## Appendix A: Electronic potential-energy surfaces

We have determined the electronic potential-energy surfaces correlating to the Ag($5s$)-Ag($5s$) asymptote with the nonrelativistic partially spin-restricted coupled-cluster method [88,89] using effective-core-potentials and large basis sets of quintuple-$\zeta$ quality augmented with additional midbond-functions and using single, double, and perturbational triple excitations [RCCSD(T)], as implemented in Molpro [90,91]. The reference electronic wave function or determinant for the ground spin singlet $X{}^1\Sigma_g^+$ and excited spin triplet $a{}^3\Sigma_u^+$ states in the coupled-cluster method are taken from restricted Hartree-Fock calculations. The shape of the molecular orbitals are optimized during the coupled-cluster calculations, i.e., the orbitals are not frozen.

We describe the electronic structure of Ag atoms using an effective core-potential (ECP) that accounts for scalar-relativistic effects. The core potential describes the first 28 electrons and is denoted ECP28MDF in the Stuttgart library [92]. The remaining 19 electrons of each Ag atom are treated explicitly with the augmented, correlation-consisted quintuple-$\zeta$ basis set (aug-cc-pwcv5z-PP) of Peterson et al. [93] with weighted core-valence correlation. The basis set was obtained from the Basis Set Exchange Platform [94]. We further augment this atomic basis with $3s3p2d2f1g$ mid-bond functions as used by Śmiałkowski et al. [7]. The mid-bond functions improve the description of electronic correlation between the atoms and bring the computed energy closer toward the complete basis set limit.

We perform the coupled-cluster calculations on a discrete grid of 106 separations from $R=3.25a_0$ to $36a_0$ for the $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ states. We observed that the single reference Hartree-Fock wave function provides a good description for the $X{}^1\Sigma_g^+$ state up to around $R=8a_0$. For larger separations the single-reference approach fails and the potential has unphysical repulsive maximum. The spin triplet $a{}^3\Sigma_u^+$ surface behaves correctly for large $R$ as for high-spin cases the dissociation can be described by a single Hartree-Fock determinant.

Coupled-cluster calculations determine the total energies of the eigenstates of the electron Hamiltonian as functions of atom-atom separation $R$. In principle, potential-energy surfaces can be obtained by subtracting the total energies for $R\to\infty$. We, however, compute these surfaces using the supermolecular method to correct for the basis set superposition error by applying the counter-poise correction procedure of Ref. [95]. In brief, at each $R$ the interaction energy is computed by subtracting total energies of the Ag atoms computed using the same dimer-centered basis set from the total energy of the Ag$_2$ dimer.

**Table II.** Equilibrium separation $R_e$ and well depths $D_e$ of the $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ of Ag$_2$ for nonrelativistic restricted CCSD(T) potentials and a comparison with experimental data where available. Numbers in parentheses for $D_e$ are standard uncertainties in the last two or three significant digits.

| State | Reference | Type | $R_e/a_0$ | $D_e/hc$ (cm$^{-1}$) |
|---|---|---:|---:|---:|
| $X{}^1\Sigma_g^+$ | This work | Theory | 4.769 | 13837(200) |
| $X{}^1\Sigma_g^+$ | Jasik et al. (2021) [61] | Theory | 4.769 | 13694.94 |
| $X{}^1\Sigma_g^+$ | Śmiałkowski et al. (2021) [7] | Theory | 4.904 | 13902 |
| $X{}^1\Sigma_g^+$ | Schissel (1957) [59] | Expt. | — | 14360(800) |
| $X{}^1\Sigma_g^+$ | Beutel et al. (1993) [96] | Expt. | 4.782 | 13400(250) |
| $a{}^3\Sigma_u^+$ | This work | Theory | 5.936 | 460(80) |
| $a{}^3\Sigma_u^+$ | Śmiałkowski et al. (2021) [7] | Theory | 5.937 | 459 |

Table II shows our equilibrium interatomic separations $R_e$ and well depths $D_e$ for the $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ Ag$_2$ potentials and compares those with several other experimental and theoretical results from the literature. Our standard uncertainties for the depths of the $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ potentials correspond to the differences in depth from calculations using the quintuple-$\zeta$ basis with additional mid-bond and the less extensive quadruple-$\zeta$ (aug-cc-pwcvqz-PP) basis now without mid-bond functions. We find that our calculated well depth of the $X{}^1\Sigma_g^+$ state potential is in good agreement with experimental results of Beutel et al. [96] and the older experimental result of Schissel [59] taking their large uncertainties into account. The equilibrium separation of the $X{}^1\Sigma_g^+$ state computed in our work agrees very well with the experimental result by Beutel et al. Our computed well depths for both the $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ state agree very well with theoretical results of Śmiałkowski et al. [7]. We, however, find that the equilibrium separation of the $X{}^1\Sigma_g^+$ state potential is slightly overestimated by Śmiałkowski et al. [7]. We find the same $R_e$ for the ground-state potential as reported by Jasik et al. [61].

The short-range parts of the $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ potentials, $V_{X,\rm CC}(R)$ and $V_{a,\rm CC}(R)$ as computed with the coupled-cluster method, are connected to the same long-range attractive dispersion potential $V_{\rm disp}(R)=-C_6/R^6-C_8/R^8$. We use the van der Waals coefficient $C_6=342(85)E_h a_0^6$ from Refs. [70,97] with a standard uncertainty of 25 % based on their analysis of the uncertainties of atomic transition dipole moments and polarizabilities. This value can be compared with $C_6=258E_h a_0^6$ from Śmiałkowski et al. [7]. Fitting the long-range tail of the $X{}^1\Sigma_g^+$ potential of Ref. [61] gives $C_6=330E_h a_0^6$. The $C_6$ coefficient for Ag + Ag is 5 to 10 times smaller than those between alkali-metal atoms. We use $C_8=61\,190E_h a_0^8$ found from fitting the long-range tail of the $a{}^3\Sigma_u^+$ state potential after subtracting the van der Waals contribution using the smaller $C_6$ value of Ref. [7]. This $C_8$ value is three times larger than that found in Ref. [97]. As the uncertainty of $C_6$ is rather large and the $-C_8/R^8$ potential is comparatively small for $R>20a_0$, we choose to use a fixed value for $C_8$ and do not quote an uncertainty.

In routines to numerically construct the $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ potentials, we interpolate potentials determined on a discrete set of separations using the reproducing kernel Hilbert space (RKHS) method [98] and smoothly join the short and long range using

$$
V_k(R)=S_k(R)[V_{k,\rm CC}(R)+\Delta V_k]+[1-S_k(R)]V_{\rm disp}(R)
\tag{A1}
$$

with $k=X$ or $a$ and $S_k(R)=\{1-\tanh[\beta_k(R-R_{0,k})]\}/2$, where $R_{0,k}=7.15a_0$ and $18.15a_0$ and $\beta_k=2.5/a_0$ and $1.1/a_0$ for $k=X$ and $a$, respectively. Finally, variables $\Delta V_k$ are user-controlled energies that can shift the short-range coupled-cluster potentials within their uncertainties. The nominal shifts are $\Delta V_k/hc=0$ cm$^{-1}$. In this paper, ultracold scattering cross sections and Fano-Feshbach resonances are studied as functions of these shifts.

Next, we describe our calculations of excited adiabatic relativistic electronic potentials of electronic states dissociating to an excited ${}^2P$ and a ground state ${}^2S$ silver atom. These states can be accessed in one-photon photoassociation experiments. We employ nonrelativistic multireference configuration-interaction calculations with single and double excitations and Davidson corrections to estimate the effect of higher excitations (i.e., MRCISD + Q), as implemented in Molpro [90]. The relativistic potentials are obtained by first computing matrix elements of electronic spin-orbit interactions described within the Breit-Pauli Hamiltonian with respect to the MRCISD + Q wave functions and then diagonalize the resulting, small matrix Hamiltonian.

The MRCISD + Q calculations are performed with the segmented all-electron relativistically contracted basis set of Rolfes et al. [99] designed for scalar relativistic Douglas-Kroll Hamiltonian with triple-zeta size (SARC-DKH2-TZVP). This SARC-DKH2-TZVP basis is specially tailored to describe the silver atom and provides a better description of spin-orbit splittings in atomic Ag compared with the ECP-based aug-cc-pwcv5z-PP basis set of Peterson et al. [93]. The MRCISD+Q calculations have been performed using the symmetry group $D_{2h}$ with eight active molecular orbitals, that is, the $5s$ and $5p$ orbitals, and 18 molecular orbitals kept doubly occupied but whose shape is optimized in the Hartree-Fock stage of the simulations. The remaining inner orbitals are static and kept as a frozen core. The $4d^95s^2$ configuration is not included in our molecular calculations due to computational limitations.

> [!figure]
> ![[Fig. 14.png|center|500]]
> **Figure 14.** Excitation energies of the $4d^{10}5p({}^2P_j)$ (black lines) and $4d^95s^2({}^2D_j)$ (red lines) excited states of the silver atom relative to that of its electronic ground state. From left to right, we compare theoretical data from MRCISD + Q + spin-orbit calculations using two electronic basis sets to the experimental data from NIST’s atomic spectra database [17].

It is informative to show the effects of the SARC-DKH2-TZVP and aug-cc-pwcv5z-PP basis sets on the energy levels of a silver atom. For an atom we can simultaneously include the $4d^{10}5s$, $4d^{10}5p$, as well as the $4d^95s^2$ configurations in the active space. In Fig. 14 we compare the calculated excitation energies of excited states of silver using the approach based on MRCISD+Q with spin-orbit matrix elements with the two basis sets to the experimental transition energies found in the NIST atomic spectra database [17]. The two fine-structure states of the $4d^{10}5p({}^2P)$ and $4d^95s^2({}^2D)$ intermingle, where those of the ${}^2D_j$ state are inverted. Only the levels based on the SARC-DKH2-TZVP basis set, however, have the correct order for the Ag atom.

We finish with a discussion of the second-order spin-orbit splitting of the $a{}^3\Sigma_u^+$ state. We have computed this splitting with three distinct approaches to solving the electronic motion. The first is the same as the one we used to determine the excited adiabatic relativistic electronic potentials described in the previous two paragraphs (MRCISD + Q plus spin-orbit matrix elements). The second and third methods rely on the relativistic Dirac Hamiltonian for the electrons with Coulomb interactions among the charged particles. Then our second approach uses the relativistic equation-of-motion coupled-cluster method with single and double excitations (EOM-CCSD) with aug-cc-pwcvqz-PP basis [93] and ECP28MDF [92] effective core potential as implemented in the DIRAC software package [100]. The third approach is a configuration-interaction calculation using a relativistic valence-bond (CI-RVB) method [101] based on numerical atomic electron orbitals rather than Gaussian-based molecular electron orbitals. The spin-orbit splittings predicted by the MRCISD + Q, EOM-CCSD, and CI-RVB methods are all rapidly decreasing functions of $R$, where that from the MRCISD + Q method is smaller than that from the EOM-CCSD method which is smaller than that from the CI-RVB method. We have chosen the splittings from the EOM-CCSD calculation as the most likely and taken a 40 % standard uncertainty, independent of $R$, reflecting the differences between the three approaches.

## Appendix B: Fano-Feshbach resonances and magneto-association of Ag atoms

The Hamiltonian for ultracold collisions between two ground-state silver atoms has multiple contributing terms. The first is the kinetic energy for the relative motion of the two atoms $-\hbar^2\nabla^2/2\mu$ with differential nabla operator $\nabla$ for relative coordinate $\mathbf{R}$ and where $\mu$ is the reduced mass of the atom pairs. The next terms are the Fermi-contact and Zeeman interactions for each atom, which are assumed to be independent of the atom-atom separation $R$ and orientation $\hat{R}$. Both stable isotopes of silver, $^{107}$Ag and $^{109}$Ag, have nuclear spin 1/2 and are composite bosons. The atomic masses, strengths of the contact interaction, and electronic and nuclear $g$ factors of these isotopes can be found in Refs. [58,102,103].

Three interactions that depend on coordinate $\mathbf{R}=(R,\hat{R})$ with separation $R$ and orientation $\hat{R}$ relative to the magnetic-field direction are included. The strongest by far leads to the $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ Born-Oppenheimer (BO) electronic states. These are states with total molecular electron spin $\mathbf{S}=\mathbf{s}_1+\mathbf{s}_2$ equal to 0 and 1, respectively. The corresponding BO potentials only depend on $R$ and have depths $D_e=hc\times13\,837(200)$ cm$^{-1}$ and $hc\times460(80)$ cm$^{-1}$ for the $X{}^1\Sigma_g^+$ and $a{}^3\Sigma_u^+$ states, respectively, as discussed in the previous sections. For large separations, the BO potentials approach the same attractive dispersion potential $-C_6/R^6-C_8/R^8$ with coefficients $C_6=342(85)E_h a_0^6$ and $C_8=61\,190E_h a_0^8$.

The two remaining interactions are the weaker and anisotropic second-order spin-orbit and magnetic dipole-dipole interactions that couple the electron spins $\mathbf{s}_j$ of the atoms to the mechanical rotation of the di-atom and lift the degeneracy of the $\Omega=0_u^-$ and $1_u$ components of the $a{}^3\Sigma_u^+$ state. Equivalently, the sum of the two anisotropic interactions is given by $V_{\rm aniso}(R)[3(\mathbf{s}_1\cdot\hat{R})(\mathbf{s}_2\cdot\hat{R})-(\mathbf{s}_1\cdot\mathbf{s}_2)]$, where $V_{\rm aniso}(R)=V_{\rm 2nd-SO}(R)-\alpha^2E_h a_0^3(g_e/2)^2/R^3$ and $g_e$ is the $g$ factor of the electrons of the electronic ground state of silver. The positive second-order spin-orbit strength $V_{\rm 2nd-SO}(R)$ is a rapidly decreasing exponential with increasing $R$, while the magnetic dipole-dipole interaction decreases slowly as $1/R^3$. Figure 4 shows the splitting $V_{\Omega=1}(R)-V_{\Omega=0}(R)=3V_{\rm aniso}(R)/2$ between the $\Omega=1_u$ and $0_u^-$ components of the $a{}^3\Sigma_u^+$ state due to the second-order spin-orbit interaction as well as that due to minus the magnetic dipole-dipole interaction. For $R<9a_0$ the second-order spin-orbit strength is larger than that of the magnetic dipole-dipole interaction and the $\Omega=1_u$ state has a higher energy than the $\Omega=0_u^-$ state. For $R>9a_0$ the $\Omega=0_u^-$ state has a larger energy.

The scattering and bound-state solutions of the Hamiltonian are found by numerically solving coupled radial Schrödinger equations, where each equation corresponds to a basis function or channel $Y_{\ell m}(\hat{R})|\{\beta_1\beta_2\}_\sigma\rangle$, where $\beta_j\in\{a,b,c,d\}$ are the $B$-dependent hyperfine states of atom $j$ and $Y_{\ell m}(\hat{R})$ are spherical harmonic functions as functions of the orientation of the internuclear axis $\hat{R}$. The spherical harmonic functions are unit-normalized eigenfunctions of the square of the relative orbital angular-momentum operator $\ell$ of the di-atom. Moreover, $\sigma=(-1)^\ell$ for our bosonic isotopes, $|\{\beta_1\beta_2\}_\sigma\rangle=(|\beta_1\beta_2\rangle+\sigma|\beta_2\beta_1\rangle)/\sqrt{2(1+\delta_{\beta_1\beta_2})}$, $\beta_1\le\beta_2$ assuming the alphabetic ordering of states, and $\delta_{ij}$ is the Kronecker $\delta$ function. Only even and odd $\ell$ are coupled by the Hamiltonian while $m_{\rm tot}=m_1+m_2+m$ is conserved. The two BO potentials only couple channels with the same $\ell$ and $m$, and thus the same $m_1+m_2$, while the anisotropic second-order spin-orbit and magnetic dipole-dipole interactions couple states with different $\ell$ and $m$. Channels are open or closed depending on whether the total energy in a collision is larger or smaller than the sum of the atomic hyperfine energies. We use the conventions of Ref. [66] for the required angular-momentum algebra to set up the Hamiltonian. We assume that the BO potentials and $V_{\rm aniso}(R)$ are the same for the $^{107}$Ag and $^{109}$Ag isotopes and that only the radial kinetic energy and atomic hyperfine and Zeeman operators depend on the isotope.

## References

[1] M. Verma, A. M. Jayich, and A. C. Vutha, Electron electric dipole moment searches using clock transitions in ultracold molecules, Phys. Rev. Lett. 125, 153201 (2020).

[2] T. Fleig and D. DeMille, Theoretical aspects of radiumcontaining molecules amenable to assembly from laser-cooled atoms for new physics searches, New J. Phys. 23, 113039 (2021).

[3] D. F. J. Kimball, D. Budker, T. E. Chupp, A. A. Geraci, S. Kolkowitz, J. T. Singh, and A. O. Sushkov, Probing fundamental physics with spin-based quantum sensors, Phys. Rev. A 108, 010101 (2023).

[4] A. Marc, M. Hubert, and T. Fleig, Candidate molecules for next-generation searches of hadronic charge-parity violation, Phys. Rev. A 108, 062815 (2023).

[5] J. Ye and P. Zoller, Essay: Quantum sensing with atomic, molecular, and optical platforms for fundamental physics, Phys. Rev. Lett. 132, 190001 (2024).

[6] J. Kłos, H. Li, E. Tiesinga, and S. Kotochigova, Prospects for assembling ultracold radioactive molecules from laser-cooled atoms, New J. Phys. 24, 025005 (2022).

[7] M. Śmiałkowski and M. Tomza, Highly polar molecules consisting of a copper or silver atom interacting with an alkalimetal or alkaline-earth-metal atom, Phys. Rev. A 103, 022802 (2021).

[8] J. L. Bohn, A. M. Rey, and J. Ye, Cold molecules: Progress in quantum engineering of chemistry and quantum matter, Science 357, 1002 (2017).

[9] L. D. Carr, D. DeMille, R. V. Krems, and J. Ye, Cold and ultracold molecules: science, technology and applications, New J. Phys. 11, 055049 (2009).

[10] S. L. Cornish, M. R. Tarbutt, and K. R. A. Hazzard, Quantum computation and quantum simulation with ultracold molecules, Nat. Phys. 20, 730 (2024).

[11] D. DeMille, Quantum computation with trapped polar molecules, Phys. Rev. Lett. 88, 067901 (2002).

[12] S. F. Yelin, K. Kirby, and R. Côté, Schemes for robust quantum computation with polar molecules, Phys. Rev. A 74, 050301(R) (2006).

[13] S. F. Yelin, D. DeMille, and R. Côté, Quantum information processing with ultracold polar molecules, in Cold Molecules: Theory, Experiment, Applications, edited by R. Krems, B. Friedrich, and W. C. Stwalley (CRC Press, Boca Raton, 2009), Chap. 17.

[14] D. DeMille, N. R. Hutzler, A. M. Rey, and T. Zelevinsky, Quantum sensing and metrology for fundamental physics with molecules, Nat. Phys. 20, 741 (2024).

[15] I. Bloch, J. Dalibard, and W. Zwerger, Many-body physics with ultracold gases, Rev. Mod. Phys. 80, 885 (2008).

[16] N. R. Cooper, J. Dalibard, and I. B. Spielman, Topological bands for ultracold atoms, Rev. Mod. Phys. 91, 015005 (2019).

[17] A. Kramida, Yu. Ralchenko, J. Reader, and NIST ASD Team, NIST Atomic Spectra Database (version 5.11), https://doi. org/10.18434/T4W30F available at https://physics.nist.gov/ asd (National Institute of Standards and Technology, Gaithersburg, MD, USA).

[18] T. M. Rvachov, H. Son, A. T. Sommer, S. Ebadi, J. J. Park, M. W. Zwierlein, W. Ketterle, and A. O. Jamison, Long-lived ultracold molecules with electric and magnetic dipole moments, Phys. Rev. Lett. 119, 143001 (2017).

[19] H. Yang, D.-C. Zhang, L. Liu, Y.-X. Liu, J. Nan, B. Zhao, and J.-W. Pan, Observation of magnetically tunable Feshbach resonances in ultracold $^{23}$Na$^{40}$K + $^{40}$K collisions, Science 363, 261 (2019).

[20] K.-K. Ni, S. Ospelkaus, M. H. G. de Miranda, A. Pe’er, B. Neyenhuis, J. J. Zirbel, S. Kotochigova, P. S. Julienne, D. S. Jin, and J. Ye, A high phase-space-density gas of polar molecules, Science 322, 231 (2008).

[21] P. K. Molony, P. D. Gregory, Z. Ji, B. Lu, M. P. Köppinger, C. R. Le Sueur, C. L. Blackley, J. M. Hutson, and S. L. Cornish, Creation of ultracold $^{87}$Rb$^{133}$Cs molecules in the rovibrational ground state, Phys. Rev. Lett. 113, 255301 (2014).

[22] G. Uhlenberg, J. Dirscherl, and H. Walther, Magneto-optical trapping of silver atoms, Phys. Rev. A 62, 063404 (2000).

[23] R. A. Cline, J. D. Miller, and D. J. Heinzen, Study of Rb2 longrange states by high-resolution photoassociation spectroscopy, Phys. Rev. Lett. 73, 632 (1994).

[24] J. D. Miller, R. A. Cline, and D. J. Heinzen, Photoassociation spectrum of ultracold Rb atoms, Phys. Rev. Lett. 71, 2204 (1993).

[25] R. Côté, A. Dalgarno, Y. Sun, and R. G. Hulet, Photoabsorption by ultracold atoms and the scattering length, Phys. Rev. Lett. 74, 3581 (1995).

[26] J. L. Bohn and P. S. Julienne, Semianalytic treatment of two-color photoassociation spectroscopy and control of cold atoms, Phys. Rev. A 54, R4637 (1996).

[27] E. R. I. Abraham, W. I. McAlexander, J. M. Gerton, R. G. Hulet, R. Côté, and A. Dalgarno, Singlet s-wave scattering lengths of $^6$Li and $^7$Li, Phys. Rev. A 53, R3713 (1996).

[28] E. Tiesinga, C. J. Williams, P. S. Julienne, K. M. Jones, P. D. Lett, and W. D. Phillips, A spectroscopic determination of scattering lengths for sodium atom collisions, J. Res. Natl. Inst. Stand. Technol. 101, 505 (1996).

[29] P. Pillet, A. Crubellier, A. Bleton, O. Dulieu, P. Nosbaum, I. Mourachko, and F. Masnou-Seeuws, Photoassociation in a gas of cold alkali atoms: I. perturbative quantum approach, J. Phys. B: At. Mol. Opt. Phys. 30, 2801 (1997).

[30] R. Côté and A. Dalgarno, Photoassociation intensities and radiative trap loss in lithium, Phys. Rev. A 58, 498 (1998).

[31] A. Crubellier, O. Dulieu, F. Masnou-Seeuws, M. Elbs, H. Knöckel, and E. Tiemann, Simple determination of Na2 scattering lengths using observed bound levels at the ground state asymptote, Eur. Phys. J. D 6, 211 (1999).

[32] D. Comparat, C. Drag, A. Fioretti, O. Dulieu, and P. Pillet, Photoassociative spectroscopy and formation of cold molecules in cold cesium vapor: Trap–loss spectrum versus ion spectrum, J. Mol. Spectrosc. 195, 229 (1999).

[33] A. Fioretti, D. Comparat, C. Drag, C. Amiot, O. Dulieu, F. Masnou-Seeuws, and P. Pillet, Photoassociative spectroscopy of the long-range state, Eur. Phys. J. D 5, 389 (1999).

[34] R. Côté and A. Dalgarno, Mechanism for the production of $^6$Li$_2$ and $^7$Li$_2$ ultracold molecules, J. Mol. Spectrosc. 195, 236 (1999).

[35] C. J. Williams, E. Tiesinga, P. S. Julienne, H. Wang, W. C. Stwalley, and P. L. Gould, Determination of the scattering lengths of $^{39}$K from 1u photoassociation line shapes, Phys. Rev. A 60, 4427 (1999).

[36] A. N. Nikolov, E. E. Eyler, X. T. Wang, J. Li, H. Wang, W. C. Stwalley, and P. L. Gould, Observation of ultracold ground-state potassium molecules, Phys. Rev. Lett. 82, 703 (1999).

[37] A. Fioretti, C. Drag, D. Comparat, B. L. Tolra, O. Dulieu, A. Crubellier, C. Amiot, F. Masnou-Seeuws, and P. Pillet, Formation of cold Cs2 molecules through photoassociation, AIP Conf. Proc. 500, 198 (2000).

[38] C. M. Dion, C. Drag, O. Dulieu, B. L. Tolra, F. MasnouSeeuws, and P. Pillet, Resonant coupling in the formation of ultracold ground state molecules via photoassociation, Phys. Rev. Lett. 86, 2253 (2001).

[39] S. Kotochigova, E. Tiesinga, and P. S. Julienne, Photoassociative formation of ultracold polar KRb molecules, Eur. Phys. J. D 31, 189 (2004).

[40] M. Kitagawa, K. Enomoto, K. Kasa, Y. Takahashi, R. Ciuryło, P. Naidon, and P. S. Julienne, Two-color photoassociation spectroscopy of ytterbium atoms and the precise determinations of s-wave scattering lengths, Phys. Rev. A 77, 012719 (2008).

[41] P. G. Mickelson, Y. N. Martinez, A. D. Saenz, S. B. Nagel, Y. C. Chen, T. C. Killian, P. Pellegrini, and R. Côté, Spectroscopic determination of the s-wave scattering lengths of $^{86}$Sr and $^{88}$Sr, Phys. Rev. Lett. 95, 223002 (2005).

[42] E. Juarros, P. Pellegrini, K. Kirby, and R. Côté, One-photonassisted formation of ultracold polar molecules, Phys. Rev. A 73, 041403(R) (2006).

[43] R. Roy, R. Shrestha, A. Green, S. Gupta, M. Li, S. Kotochigova, A. Petrov, and C. H. Yuen, Photoassociative production of ultracold heteronuclear YbLi∗ molecules, Phys. Rev. A 94, 033413 (2016).

[44] M. Borkowski, P. Morzyński, R. Ciuryło, P. S. Julienne, M. Yan, B. J. DeSalvo, and T. C. Killian, Mass scaling and nonadiabatic effects in photoassociation spectroscopy of ultracold strontium atoms, Phys. Rev. A 90, 032713 (2014).

[45] A. Green, J. H. S. Toh, R. Roy, M. Li, S. Kotochigova, and S. Gupta, Two-photon photoassociation spectroscopy of the ${}^2\Sigma^+$ YbLi molecular ground state, Phys. Rev. A 99, 063416 (2019).

[46] K. M. Jones, E. Tiesinga, P. D. Lett, and P. S. Julienne, Ultracold photoassociation spectroscopy: Long-range molecules and atomic scattering, Rev. Mod. Phys. 78, 483 (2006).

[47] C. Chin, R. Grimm, P. Julienne, and E. Tiesinga, Feshbach resonances in ultracold gases, Rev. Mod. Phys. 82, 1225 (2010).

[48] E. Tiesinga, B. J. Verhaar, and H. T. C. Stoof, Threshold and resonance phenomena in ultracold ground-state collisions, Phys. Rev. A 47, 4114 (1993).

[49] S. Inouye, M. R. Andrews, J. Stenger, H.-J. Miesner, D. M. Stamper-Kurn, and W. Ketterle, Observation of Feshbach resonances in a Bose–Einstein condensate, Nature (London) 392, 151 (1998).

[50] P. Courteille, R. S. Freeland, D. J. Heinzen, F. A. van Abeelen, and B. J. Verhaar, Observation of a Feshbach resonance in cold atom scattering, Phys. Rev. Lett. 81, 69 (1998).

[51] C. L. Blackley, C. R. Le Sueur, J. M. Hutson, D. J. McCarron, M. P. Köppinger, H.-W. Cho, D. L. Jenkin, and S. L. Cornish, Feshbach resonances in ultracold $^{85}$Rb, Phys. Rev. A 87, 033611 (2013).

[52] T. Maier, H. Kadau, M. Schmitt, M. Wenzel, I. Ferrier-Barbut, T. Pfau, A. Frisch, S. Baier, K. Aikawa, L. Chomaz, M. J. Mark, F. Ferlaino, C. Makrides, E. Tiesinga, A. Petrov, and S. Kotochigova, Emergence of chaotic scattering in ultracold Er and Dy, Phys. Rev. X 5, 041029 (2015).

[53] P. Weckesser, F. Thielemann, D. Wiater, A. Wojciechowska, L. Karpa, K. Jachymski, M. Tomza, T. Walker, and T. Schaetz, Observation of Feshbach resonances between a single ion and ultracold atoms, Nature (London) 600, 429 (2021).

[54] A. Ciamei, S. Finelli, A. Trenkwalder, M. Inguscio, A. Simoni, and M. Zaccanti, Exploring ultracold collisions in $^6$Li-$^{53}$Cr Fermi mixtures: Feshbach resonances and scattering properties of a novel alkali-transition metal system, Phys. Rev. Lett. 129, 093402 (2022).

[55] F. Thielemann, J. Siemund, D. von Schoenfeld, W. Wu, P. Weckesser, K. Jachymski, T. Walker, and T. Schaetz, Exploring atom-ion Feshbach resonances below the s-wave limit, Phys. Rev. X 15, 011051 (2025).

[56] M. Born and R. Oppenheimer, Zur quantentheorie der molekeln, Ann. Phys. (Berlin, Ger.) 389, 457 (1927).

[57] E. Tiesinga, P. J. Mohr, D. B. Newell, and B. N. Taylor, CODATA recommended values of the fundamental physical constants: 2018, Rev. Mod. Phys. 93, 025010 (2021).

[58] M. Wang, W. J. Huang, F. G. Kondev, G. Audi, and S. Naimi, The AME 2020 atomic mass evaluation (II). Tables, graphs and references, Chin. Phys. C 45, 030003 (2021).

[59] P. Schissel, Dissociation energies of Cu2, Ag2, and Au2, J. Chem. Phys. 26, 1276 (1957).

[60] J. Andzelm, E. Radzio, and D. R. Salahub, Model potential calculations for second–row transition metal molecules within the local–spin–density method, J. Chem. Phys. 83, 4573 (1985).

[61] P. Jasik, J. Franz, D. Kȩdziera, T. Kilich, J. Kozicki, and J. E. Sienkiewicz, Spontaneous electron emission vs dissociation in internally hot silver dimer anions, J. Chem. Phys. 154, 164301 (2021).

[62] E. K. Anderson, A. F. Schmidt-May, P. K. Najeeb, G. Eklund, K. C. Chartkunchand, S. Rosén, Å. Larson, K. Hansen, H. Cederquist, H. Zettergren, and H. T. Schmidt, Spontaneous electron emission from hot silver dimer anions: Breakdown of the Born-Oppenheimer approximation, Phys. Rev. Lett. 124, 173001 (2020).

[63] See Supplemental Material at http://link.aps.org/supplemental/ 10.1103/rd26-sgz1 for data used in Figs. 2 and 3 as ASCII files (one for each potential-energy curve).

[64] H. Zhang and K. Balasubramanian, Spectroscopic constants and potential energy curves for 15 electronic states of Ag2, J. Chem. Phys. 98, 7092 (1993).

[65] M. Movre and G. Pichler, Resonance interaction and selfbroadening of alkali resonance lines. I. Adiabatic potential curves, J. Phys. B: At. Mol. Phys. 10, 2631 (1977).

[66] D. M. Brink and G. R. Satchler, Angular Momentum, 3rd ed. (Clarendon Press, Oxford, 1993).

[67] U. I. Safronova, I. M. Savukov, M. S. Safronova, and W. R. Johnson, Third-order relativistic many-body calculations of energies and lifetimes of levels along the silver isoelectronic sequence, Phys. Rev. A 68, 062505 (2003).

[68] R. K. Chaudhuri and S. Chattopadhyay, Theoretical investigations of electronic spectra of silver atom using all-electron scalar relativistic basis, AIP Adv. 12, 125019 (2022).

[69] H.-S. Chou and W. R. Johnson, Relativistic many-body perturbation-theory calculations of transition rates for copperlike, silverlike, and goldlike ions, Phys. Rev. A 56, 2424 (1997).

[70] J. Y. Zhang, J. Mitroy, H. R. Sadeghpour, and M. W. J. Bromley, Long-range interactions of copper and silver atoms with hydrogen, helium, and rare-gas atoms, Phys. Rev. A 78, 062710 (2008).

[71] G. M. Lawrence, J. K. Link, and R. B. King, The absolute oscillator strengths of lines in the spectra of ten elements, Astrophys. J. 141, 293 (1965).

[72] N. L. Moise, Absolute transition rates of atomic transitions of copper, silver, and gold, Astrophys. J. 144, 774 (1966).

[73] J. Carlsson, P. Jönsson, and L. Sturesson, Accurate timeresolved laser spectroscopy on silver atoms, Z. Phys. D: At. Mol. Clusters 16, 87 (1990).

[74] P. S. Doidge, A compendium and critical review of neutral atom resonance line oscillator strengths for atomic absorption analysis, Spectrochim. Acta, Part B 50, 209 (1995).

[75] D. T. Colbert and W. H. Miller, A novel discrete variable representation for quantum mechanical reactive scattering via the S–matrix Kohn method, J. Chem. Phys. 96, 1982 (1992).

[76] R. Napolitano, J. Weiner, C. J. Williams, and P. S. Julienne, Line shapes of high resolution photoassociation spectra of optically cooled atoms, Phys. Rev. Lett. 73, 1352 (1994).

[77] P. S. Julienne, Cold binary atomic collisions in a light field, J. Res. Natl. Inst. Stand. Technol. 101, 487 (1996).

[78] J. L. Bohn and P. S. Julienne, Semianalytic theory of laserassisted resonant cold collisions, Phys. Rev. A 60, 414 (1999).

[79] K. M. Jones, P. D. Lett, E. Tiesinga, and P. S. Julienne, Fitting line shapes in photoassociation spectroscopy of ultracold atoms: A useful approximation, Phys. Rev. A 61, 012501 (1999).

[80] D. Comparat, Improved LeRoy–Bernstein near-dissociation expansion formula, and prospect for photoassociation spectroscopy, J. Chem. Phys. 120, 1318 (2004).

[81] G. F. Gribakin and V. V. Flambaum, Calculation of the scattering length in atomic collisions using the semiclassical approximation, Phys. Rev. A 48, 546 (1993).

[82] J. R. Taylor, Scattering Theory (Dover Publications, New York, 1972).

[83] N. F. Mott and H. S. W. Massey, Theory of Atomic Collisions, 3rd ed. (Oxford University Press, Oxford, UK, 1965).

[84] H. T. C. Stoof, J. M. V. A. Koelman, and B. J. Verhaar, Spin-exchange and dipole relaxation rates in atomic hydrogen: Rigorous and simplified calculations, Phys. Rev. B 38, 4688 (1988).

[85] The policy of NIST is to use the International System of Units in all publications. In this document, however, units are presented in the system prevalent in the relevant discipline, although in some cases more than one system of units may be presented.

[86] C. Chin, V. Vuletić, A. J. Kerman, S. Chu, E. Tiesinga, P. J. Leo, and C. J. Williams, Precision Feshbach spectroscopy of ultracold Cs2, Phys. Rev. A 70, 032701 (2004).

[87] A. J. Moerdijk, B. J. Verhaar, and A. Axelsson, Resonances in ultracold collisions of $^6$Li, $^7$Li, and $^{23}$Na, Phys. Rev. A 51, 4852 (1995).

[88] P. J. Knowles, C. Hampel, and H.-J. Werner, Coupled cluster theory for high spin, open shell reference wave functions, J. Chem. Phys. 99, 5219 (1993).

[89] P. J. Knowles, C. Hampel, and H.-J. Werner, Erratum: Coupled cluster theory for high spin, open shell reference wave functions [J. Chem. Phys. 99, 5219 (1993)], J. Chem. Phys. 112, 3106 (2000).

[90] H.-J. Werner, P. J. Knowles, G. Knizia, F. R. Manby, and M. Schütz, Molpro: A general-purpose quantum chemistry program package, Wiley Interdiscip. Rev. Comput. Mol. Sci. 2, 242 (2012).

[91] Any mention of commercial products is for information only; it does not imply recommendation or endorsement by NIST.

[92] D. Figgen, G. Rauhut, M. Dolg, and H. Stoll, Energyconsistent pseudopotentials for group 11 and 12 atoms: adjustment to multi-configuration Dirac-Hartree-Fock data, Chem. Phys. 311, 227 (2005).

[93] K. A. Peterson and C. Puzzarini, Systematically convergent basis sets for transition metals. II. Pseudopotential-based correlation consistent basis sets for the group 11 (Cu, Ag, Au) and 12 (Zn, Cd, Hg) elements, Theor. Chem. Acta 114, 283 (2005).

[94] B. P. Pritchard, D. Altarawy, B. Didier, T. D. Gibson, and T. L. Windus, New basis set exchange: An open, up-to-date resource for the molecular sciences community, J. Chem. Inf. Model. 59, 4814 (2019).

[95] S. F. Boys and F. Bernardi, The calculation of small molecular interactions by the differences of separate total energies. Some procedures with reduced errors. Mol. Phys. 19, 553 (1970).

[96] V. Beutel, H. G. Kramer, G. L. Bhale, M. Kuhn, K. Weyers, and W. Demtröder, High-resolution isotope selective laser spectroscopy of Ag2 molecules, J. Chem. Phys. 98, 2699 (1993).

[97] J. Jiang, J. Mitroy, Y. Cheng, and M. W. J. Bromley, Effective oscillator strength distributions of spherically symmetric atoms for calculating polarizabilities and long-range atom– atom interactions, At. Data Nucl. Data Tables 101, 158 (2015).

[98] T.-S. Ho and H. Rabitz, A general method for constructing multidimensional molecular potential energy surfaces from ab initio calculations, J. Chem. Phys. 104, 2584 (1996).

[99] J. D. Rolfes, F. Neese, and D. A. Pantazis, All-electron scalar relativistic basis sets for the elements Rb-Xe, J. Comput. Chem. 41, 1842 (2020).

[100] DIRAC, a relativistic ab-initio electronic structure program, Release DIRAC21 (2021), written by R. Bast, A. S. P. Gomes, T. Saue, L. Visscher, and H. J. A. Jensen, http://dx.doi.org/10. 5281/zenodo.4836496, see also http://www.diracprogram.org.

[101] S. Kotochigova and E. Tiesinga, Ab initio relativistic calculation of the RbCs molecule, J. Chem. Phys. 123, 174304 (2005).

[102] H. Dahmen and S. Penselin, Measurement of the nuclear magnetic dipole moment of $^{197}$Au and hyperfine structure measurements in the ground states of $^{197}$Au, $^{107}$Ag, $^{109}$Ag and $^{39}$K , Eur. Phys. J. A 200, 456 (1967).

[103] N. J. Stone, Table of nuclear magnetic dipole and electric quadrupole moments, Technical Report No. INDC(NDS)– 0658, International Atomic Energy Agency (IAEA), Austria, 2014.
