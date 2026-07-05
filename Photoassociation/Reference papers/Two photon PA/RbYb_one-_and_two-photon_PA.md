# Intercombination-line photoassociation spectroscopy of ⁸⁷Rb¹⁷⁰Yb

**Authors:** Tobias Franzen, Bastian Pollklesener, Christian Sillus, and Axel Görlitz

*Institut für Experimentalphysik, Heinrich-Heine Universität Düsseldorf, 40225 Düsseldorf, Germany*

Published in *Physical Review A* **107**, 023114 (2023). Received 1 December 2022; accepted 13 February 2023; published 23 February 2023.
DOI: [10.1103/PhysRevA.107.023114](https://doi.org/10.1103/PhysRevA.107.023114)

Corresponding authors: tobias.franzen@durham.ac.uk (present address: Joint Quantum Centre (JQC) Durham-Newcastle, Department of Physics, Durham University, South Road, Durham, DH1 3LE, United Kingdom); axel.goerlitz@hhu.de

## Abstract

We report on the observation of photoassociation (PA) near the [Rb] $5s\,{}^2S_{1/2}$ + [Yb] $6s\,6p\,{}^3P_1$ asymptote in a mixture of ⁸⁷Rb and ¹⁷⁰Yb. In a search spanning binding energies between 0.1 and 11 GHz, a single pair of interspecies PA resonances is detected around 3.1 GHz. These resonances are characterized by extracting PA rates, binding energies, and Zeeman shift coefficients. Using one of these resonances, two-photon photoassociation is performed, improving on previous measurements of the binding energies of the two least bound states in the electronic ground state and demonstrating intercombination-line photoassociation as a powerful spectroscopic tool. We discuss implications for pathways towards RbYb molecules in the absolute ground state.

## I. Introduction

The production of ultracold and ultimately quantum degenerate samples of polar molecules has recently attracted much attention, with applications in quantum simulation [1–4], quantum chemistry [5–7], and quantum computing [8,9]. Molecules with a $^2\Sigma$ ground state, such as dimers composed of an alkali and a closed-shell atom, promise to further extend the rich internal structure of these systems and provide an additional degree of freedom due to their magnetic dipole moment [1,10–15].

Despite considerable advances [16–21], direct laser cooling of molecules remains extremely challenging. An alternative route that has been applied to bialkalis [22–27], and the homonuclear closed-shell molecule Sr₂ [28] is the creation of ultracold molecules from ultracold atoms. In particular, in bialkalis great progress has been made recently, with several groups producing degenerate samples [29–31].

Magnetic Feshbach resonances [32] are the association mechanism of choice in bialkalis, where the interaction between electron spins provides strong coupling between channels. However, the picture is less clear for a combination of an alkali and a closed-shell atom, where the $^1S_0$ ground state means that these couplings are absent. While Feshbach resonances due to distance-dependent hyperfine couplings have been predicted [33–35] and observed in Rb + Sr [36], Li + Yb [37], and Cs + Yb [38], these resonances are extremely narrow and their use for magnetoassociation remains an outstanding challenge. Magnetic Feshbach resonances in Rb + Yb have been predicted [34] but not observed to date.

On the other hand, efficient all-optical production of Sr₂ molecules in the absolute ground state has recently been reported, demonstrating the feasibility of this approach. In that work narrow-line photoassociation was followed by spontaneous decay to a weakly bound level in the electronic ground state, from where the absolute ground state was reached by stimulated Raman adiabatic passage (STIRAP) [28]. Previous studies, also in Sr₂, have also demonstrated efficient free-bound STIRAP [39], suggesting the possibility of a fully coherent transfer. Photoassociation thus remains a promising alternative technique for the creation of alkali–closed-shell molecules.

The combination Rb + Yb is an attractive candidate, as cooling of both species to degeneracy is well established and the large number of stable isotopes in Yb allows the creation of both fermionic and bosonic molecules with a range of reduced masses. Previous photoassociation experiments in RbYb [40–43] have used the $^2\Pi_{1/2}$ potential corresponding to the atomic threshold [Rb] $5p\,{}^2P_{1/2}$ + [Yb] $6s^2\,{}^1S_0$, where the strong D1 line provides large photoassociation rates. These investigations included the measurement of the differential hyperfine shift in the $^2\Pi_{1/2}$ potential [41], which is analogous to the shift responsible for some of the Feshbach resonances in the ground state. In addition, the ground-state potential was characterized by two-photon photoassociation [42], leading to the accurate determination of the scattering lengths for all isotope combinations [43].

A unique feature of closed-shell atoms is the presence of narrow intercombination-line transitions. In Yb the transitions to the $^3P_j$ manifold exhibit natural linewidths ranging from the mHz range for the $^1S_0 \rightarrow {}^3P_0$ clock transition [44] to $2\pi \times 181$ kHz for the $^1S_0 \rightarrow {}^3P_1$ transition, which is commonly used for narrow-line laser cooling [45]. While the former provides an extremely sensitive spectroscopic probe allowing, for example, the measurement of on-site interactions in optical lattices [46,47], photoassociation would be extremely challenging due to the small transition dipole moments. Instead we chose to work near the $^1S_0 \rightarrow {}^3P_1$ transition, as illustrated in Fig. 1. With a transition linewidth about 30 times smaller than that of the D1 line of Rb, it allows for spectroscopy of more weakly bound states with significantly higher resolution, while still providing sufficient transition strength to locate resonances without prior knowledge of binding energies. The [Rb] $5s\,{}^2S_{1/2}$ + [Yb] $6s\,6p\,{}^3P_1$-asymptote connects to three potentials labeled by $(2S+1)\Lambda = {}^1\Pi_{1/2}$, ${}^1\Sigma^-_{1/2}$, ${}^2\Pi_{3/2}$ in the short range with Hund's case (a), and $n(\Omega) = (5)\tfrac{1}{2}$, $(1)-\tfrac{1}{2}$, $(2)\tfrac{3}{2}$ in the long range with Hund's case (c) [48]. Prior to this work no experimental data on these potentials was available.

Further motivation to explore bound states of the $^3P_j$ manifold is given by the recent prediction of Feshbach resonances between Rb and metastable Yb in the $j = 0, 2$ states [49,50].

This paper is organized as follows: In Sec. II we briefly describe our apparatus and the preparation sequence used for the measurements reported here. Our observations of intercombination-line photoassociation resonances and their characterization are presented in Sec. III. Finally, in Sec. IV we describe two-photon photoassociation using this transition and precisely determine the binding energy of the two least bound states of the electronic ground state.

> [!figure]
> ![[Fig. 1.png|center|500]]
> **Figure 1.** Schematic diagram of the relevant ground- and excited-state potentials of RbYb and the free-bound (L1) and bound-bound (L2) transitions used in this work.

## II. Experimental setup

In our apparatus (described in detail elsewhere [51]), Rb and Yb are prepared in separate vacuum chambers by magneto-optical trapping and microwave-driven evaporation in a quadrupole trap for Rb and an intercombination-line magneto-optical trap (MOT) for Yb. Both species are then loaded into single-beam optical dipole traps and subsequently transported to a common science chamber by axial translation of these traps. Here further evaporative cooling and merging of the two samples takes place in crossed optical dipole traps. All dipole traps operate close to 1064 nm, leading to trap depths that are significantly higher for Rb than for Yb. This in turn leads to a similar difference in temperature.

We chose the combination of ⁸⁷Rb + ¹⁷⁰Yb due to its favorable intra- and interspecies scattering lengths of $a_{\text{Rb–Rb}} = 100\,a_0$ [52], $a_{\text{Yb–Yb}} = 64\,a_0$ [53], and $a_{\text{Rb–Yb}} = -11\,a_0$ [43]. These values ensure efficient preparation of each species by evaporative cooling in optical dipole traps as well as miscibility. The previous observation of phase separation well before the onset of degeneracy in mixtures of ⁸⁷Rb + ¹⁷⁴Yb [54] demonstrates this cannot be taken for granted even in thermal samples.

In a typical experiment we prepare $3 \times 10^5$ ¹⁷⁰Yb atoms at a temperature of 1.5 µK and $2 \times 10^5$ Rb atoms at a temperature of 10 µK in a crossed optical dipole trap. The calculated trap frequencies along the principal directions of the trap are $\omega_{\text{Yb}} = 2\pi \times (80\text{ Hz}, 250\text{ Hz}, 260\text{ Hz})$ and $\omega_{\text{Rb}} = 2\pi \times (0.35\text{ kHz}, 1.1\text{ kHz}, 1.1\text{ kHz})$, resulting in estimated peak densities of $n_{\text{Yb}} \approx 1 \times 10^{13}\text{ cm}^{-3}$ and $n_{\text{Rb}} \approx 2 \times 10^{13}\text{ cm}^{-3}$, respectively, with phase space densities of $\sim 10^{-2}$ for both species. Due to the small interspecies scattering cross section, no appreciable interspecies thermalization, which with our current trapping potentials would lead to the loss of Yb, is observed. Rb is prepared almost exclusively in the $(f=1, m_f=-1)$ hyperfine state.

Photoassociation light is applied for typically 1 s, after which the remaining atom number is detected. Despite similar atom numbers before photoassociation, rapid loss of Yb from off-resonant excitation near the atomic line limits the contrast observed in the Rb atom number, and the resonances are more easily detected in the Yb atom number. Light to drive the free-bound and bound-bound transitions is generated using a frequency-doubled fiber laser system, with the frequency stabilized at a tunable offset from the MOT laser system (see Appendix A). Light to address the bound-bound transition is derived from the same light source (see Appendix B).

## III. One-photon photoassociation

The narrow linewidth of the atomic transition and the lack of prior information make the search for intercombination-line photoassociation (PA) resonances challenging. Ab initio calculations predict the $C_6$ coefficient [55] but not the fractional part of the dissociation quantum number $\nu_D$ and can thus be used to estimate the spacing of bound levels but not their actual positions in a given isotopologue. In a Hund's case (c) picture the relevant potential energy curves have either $|\Omega| = \tfrac{1}{2}$ or $|\Omega| = \tfrac{3}{2}$.

We perform photoassociation spectroscopy at detunings between 0.1 and 11 GHz, locating a single pair of resonances around 3.1 GHz, shown in Fig. 2. In measurements in the absence of Rb, these features disappear, ruling out the (remote) possibility of an intraspecies photoassociation resonance.

> [!figure]
> ![[Fig. 2.png|center|500]]
> **Figure 2.** Free-bound photoassociation lines observed in the Yb atom number. The solid line is a Gaussian fit as a guide to the eye.

To quantify the strength of the PA line, we measure the time dependence of the atom number for each species with the PA laser tuned on and off resonance, as shown in Fig. 3. We fit the data with solutions of a simple rate equation model for the atomic densities $n_{\text{Rb}}$ and $n_{\text{Yb}}$ given by

$$
\dot{n}_{\text{Rb}} = -n_{\text{Rb}} K_{\text{Rb}} - n_{\text{Rb}} n_{\text{Yb}} K_{\text{PA}},
$$

$$
\dot{n}_{\text{Yb}} = -n_{\text{Yb}} K_{\text{Yb}} - n_{\text{Rb}} n_{\text{Yb}} K_{\text{PA}},
$$

with the photoassociation rate constant $K_{\text{PA}}$ and the single-species loss constants $K_{\text{Rb}}, K_{\text{Yb}}$ [56]. From this fit we extract a photoassociation rate constant of $K_{\text{PA}} \approx 5 \times 10^{-14}\text{ cm}^3/\text{s}$ for the slightly stronger resonance at $-3057$ MHz for a PA laser intensity of $\sim 40\text{ W/cm}^2$. Even considering the difference in atomic linewidths, this is significantly larger than predictions made for RbSr in [57] but nonetheless orders of magnitude smaller than typical PA rate constants obtained near the alkali D-line asymptotes. The single-species loss constant of $0.7\text{ s}^{-1}$ for Yb is an order of magnitude larger than for Rb [58].

> [!figure]
> ![[Fig. 3.png|center|500]]
> **Figure 3.** Decay curves for (a) Yb and (b) Rb with the PA light on and off resonance for the stronger transition located at −3057 MHz.

We attribute the relatively large loss rate for Rb to heating from the multimode trapping laser, which is explained by off-resonant scattering. While the PA rate is not saturated and could be increased with higher laser intensity, this would also lead to a corresponding increase in the Yb single-species loss.

Despite extensive efforts, we could not locate any other resonances. For most of the search range, transitions with a PA rate constant $K_{\text{PA}} \gtrsim 2 \times 10^{-14}\text{ cm}^3/\text{s}$ would have been detected with a high probability. Sensitivity is, however, strongly degraded for binding energies less than $\sim h \times 2$ GHz, due to increased off-resonant excitation of the atomic transition, and in the immediate vicinity of Yb₂ resonances, both requiring a reduction in photoassociation pulse area by several orders of magnitude. We note that with the observed resonance position and the $C_6$ coefficients predicted in Ref. [55], the two neighboring PA resonances are indeed expected to be close to Yb₂ resonances. Sensitivity would also be degraded by a factor of up to 4 [58] for transitions with an effective linewidth of less than the typical step size of $2\pi \times 1$ MHz.

To further characterize the observed resonances, we measure their Zeeman shift as shown in Fig. 4. The magnetic field values were calibrated using microwave spectroscopy in Rb. The polarization was undefined for this measurement, so potentially both $\pi$ and $\sigma^\pm$ transitions contribute to the spectrum. Additionally, residual background field contributions may cause a shift in magnetic field orientation at low fields.

> [!figure]
> ![[Fig. 4.png|center|500]]
> **Figure 4.** Investigation of the Zeeman shift of the observed transitions. (a) Spectra at various magnetic fields, offset by the magnetic field strength. (b) Reconstructed shift of A and B from Gaussian fits shown in (a).

Both loss features are fit by Gaussians and their center positions, taking into account the Zeeman shift of the atomic threshold, are shown in Fig. 4(b). The fits shown yield shift coefficients of 0.6(1) MHz/G and 0.3(1) MHz/G, respectively, with zero-field-transition frequencies of $-3057.2(3)$ MHz and $-3074.3(3)$ MHz. Thus the two peaks obviously remain split even at zero magnetic field. Yet their close proximity and similar strength suggest that they are, in fact, closely related. Given the small binding energies, it appears reasonable to treat the molecular states as combinations of the atomic states. The shift coefficients for the Rb states in $f=1$ are $-m_f \times 0.7$ MHz/G, while the excited $^3P_1$ state of Yb shifts with $m_j \times 2.1$ MHz/G. All combinations of these states will thus shift with multiples of 0.7 MHz/G and cannot satisfactorily explain the observed shifts. Our efforts to explain the Zeeman shift in the framework of Hund's case (c) or (e) have also failed to deliver a consistent assignment.

In addition to the shifts, Fig. 4 shows a significant broadening of the peaks with increasing magnetic field. For the zero-field FWHM of the peak at $-3057.2(3)$ MHz, a value of 3 MHz is extrapolated. Even this linewidth is still an order of magnitude larger than the atomic linewidth. No further reduction of the linewidth was observed when reducing the PA intensity, ruling out saturation broadening. We rule out an increase in magnetic field noise for higher fields as the cause for the broadening by microwave spectroscopy on Rb, which is also used for the calibration of the field.

Significant broadening of the intercombination-line photoassociation resonances has previously been observed in RbSr [59]. In that work it was argued that this could be caused by strong radiative decay to bound states in the electronic ground state. In contrast to the alkali D lines, the $^1S_0 \rightarrow {}^3P_1$ transition is only weakly allowed by mixing of the $^3P_1$ and $^1P_1$ states. At shorter internuclear distances, the presence of the Rb atom leads to further mixing, increasing the transition dipole moment [48]. However, from simple estimates based on model potentials and the transition dipole moment curves calculated by Shundalau and Minko [48], we expect the increase in transition dipole moment for this state to be less than 10% of the atomic dipole moment. This mechanism thus seems unlikely to significantly affect the state lifetime or transition rates in the case of RbYb.

Another possible explanation for the observed linewidths is nonradiative decay within the $^3P$ manifold, for example, through predissociation to the $^3P_0$ state. Such decay has, for example, been encountered in the analysis of Feshbach resonances associated with the $^3P_2$ state [49], where it leads to strongly decayed resonances, in which the closed channel lifetime is limited to the order of microseconds by predissociation to the $^3P_0$ continuum.

Interestingly, the calculations performed for Feshbach resonances in the $^3P_2$ state also show a decay width that is increasing with magnetic field in the same range that is covered by our measurements [49]. If a similar effect occurs for the $^3P_1$ state, this could explain the observed behavior of the linewidths.

A somewhat similar situation has also been described for the $^3P_j$ manifold of the molecular ion HeN⁺ [60]. Notably, this leads to many transitions being broadened—in particular, in the presence of a magnetic field—to an extent that makes them unobservable and might provide an explanation for the fact that we have only observed a single pair of seemingly related transitions. A definitive assignment of the observed lines and thus the observed Zeeman shifts and linewidths will require further experimental and theoretical work beyond the scope of this paper.

Taking into account the Zeeman effects and thermal shift, the binding energies of the two states—assuming they can be assigned to the $f=1$ threshold of Rb—are measured to be 3057.0(5) MHz and 3074.1(5) MHz and are thus split by 17.1(7) MHz. Taking the $C_6$ values calculated by Porsev *et al.* [55], these binding energies correspond to a classical outer turning point of $45\,a_0$ to $46\,a_0$ for $|\Omega| = \tfrac{1}{2}$ and $|\Omega| = \tfrac{3}{2}$, respectively. This is at significantly longer range than the most weakly bound level that was observed for photoassociation near the D1 line of Rb with an outer turning point around $35\,a_0$ [40,41]. This is due to the difference in $C_6$ coefficients and the lower linewidth allowing for spectroscopy closer to the asymptote. In combination with the predicted $C_6$ coefficients, the neighboring levels may be predicted to have binding energies around 1.2 and 6 GHz, respectively, though with large uncertainties. Both of these are, however, close to Yb₂ resonances, which could obscure the RbYb resonances.

The low photoassociation rate and the significant off-resonant light scattering on the atomic transition will make the use of the observed transitions for the efficient production of RbYb molecules challenging. However, intercombination-line photoassociation presents a powerful tool for the characterization of weakly bound states in both the electronically excited and the electronic ground state.

## IV. Two-photon photoassociation

Precise knowledge of weakly bound states in the electronic ground states will be critical for finding pathways to efficient molecule production, be it through photoassociation or magnetoassociation. The measurement of these binding energies is possible by two-photon photoassociation [61], where a second laser field couples the bound state in the electronically excited state to a bound state in the electronic ground state. We label the vibrational states with $\Delta\nu'$ counting from the threshold, with $\Delta\nu' = -1$ being the least bound state. Binding energies for the two least bound states in the electronic ground state of ⁸⁷Rb¹⁷⁰Yb have previously been determined by two-photon photoassociation near the Rb D1 line with uncertainties of around 15 MHz [42,43]. Here we report an improvement of two orders of magnitude by performing two-photon photoassociation near the intercombination line.

By keeping the free-bound laser stabilized to one of the free-bound transitions [62] ($\delta_{\text{FB}} = 0$) and scanning the laser driving the bound-bound transition (bound-bound laser) and thus the two-photon detuning $\Delta_{2\gamma}$, the photoassociation loss is suppressed when the bound-bound laser comes close to resonance, as shown in Fig. 5(a). The two-photon detuning is given by $\Delta_{2\gamma} = \delta_{\text{FB}} - \delta_{\text{BB}}$, and its magnitude is equal to that of the scanning photon because we always keep one transition on resonance. On the other hand, when keeping the bound-bound laser on resonance and scanning the frequency of the free-bound laser we obtain the well-known dark resonance line shape [63] shown in Fig. 5(b).

In all the experiments presented here, the atoms are only weakly trapped with $\hbar\omega_{\text{trap}} \ll k_B T$ and the scattering state is thus a continuum with thermally distributed energies rather than a well-defined single state. The mean collision energy is on the order of $h \times 0.2$ MHz (ensuring that only $s$-wave collisions are relevant) for typical experimental conditions. This gives rise to an asymmetrical broadening of the observed lines that is obvious in the spectra in Fig. 5(a) and somewhat more subtle in the dark resonances in Fig. 5(b). In the latter case, it also prevents us from extracting the true lifetime of the dark state—which is expected to be much longer than that corresponding to the thermal linewidth—from the measured spectra. This thermal spread of energies poses a significant obstacle to the implementation of coherent techniques like STIRAP. To implement a STIRAP scheme for the production of RbYb molecules, this will have to be overcome in future experiments, for example, by tight confinement of the atoms in an optical lattice.

> [!figure]
> ![[Fig. 5.png|center|500]]
> **Figure 5.** Observation of two-photon photoassociation resonances (a) by scanning the bound-bound laser with the free-bound laser locked on resonance and (b) by scanning the free-bound laser while the bound-bound laser is locked on resonance (dark-resonance configuration). The energy levels on the sketches on the left-hand side are labeled with |1⟩ for the scattering state, |2⟩ for the bound state in the electronic ground state, and |3⟩ for the electronically excited state. The scattering state and the vibrational ground state are separated with the binding energy $E_B$ and the thermal energy $E_{\text{therm}}$.

All spectra are fitted using a thermal average over an expression for the loss rate obtained from solving the optical Bloch equations, which is given by [63]

$$
\frac{\dot{N}}{N} = \frac{2\Gamma_{\text{FB}}}{4}\,\frac{\Delta_{2\gamma}^2 + \left(\dfrac{\Gamma_{\text{eff}}}{2}\right)^2 \Omega_{\text{BB}}^2 + \Gamma_{\text{eff}}\left|\Omega_{\text{BB}}^2 + (\Gamma + 2i\delta_{\text{FB}})(\Gamma_{\text{eff}} + 2i\Delta_{2\gamma})\right|^2} \tag{3}
$$

with the free-bound and bound-bound Rabi frequencies $\Omega_{\text{FB}}$ and $\Omega_{\text{BB}}$, the decay rate of the excited state $\Gamma$, and the effective decay rate $\Gamma_{\text{eff}}$ accounting for decoherence of the dark state. For the data shown, the values extracted from the fit are $\Omega_{\text{FB}} \approx 2\pi \times 1$ kHz and $\Omega_{\text{BB}} \approx 2\pi \times 1$ MHz for both transitions, with a free-bound laser intensity of $26\text{ W/cm}^2$ and bound-bound laser intensities of $5\text{ W/cm}^2$ for the $\Delta\nu' = -1$ state and $1\text{ W/cm}^2$ for the $\Delta\nu' = -2$ state, respectively.

For both observed states the Zeeman shift of the two-photon transition was determined to be less than 0.1 MHz/G, consistent with zero. It can thus be assumed that the Zeeman levels probed in the ground states are of the same $(F=1, m_F=-1)$ character as the scattering state. The fact that no transitions with a different magnetic moment were observed indicates that the bound-bound laser does not induce a significant coupling between the Rb Zeeman or hyperfine states.

Taking into account the thermal shifts, the measured binding energies are $E_B(\Delta\nu' = -1) = h \times 101.9(1)$ MHz and $E_B(\Delta\nu' = -2) = h \times 1011.0(1)$ MHz. Future work will extend these measurements to more deeply bound levels, in particular, those with binding energies just above the hyperfine splitting of Rb, which give rise to magnetic Feshbach resonances at moderate fields. For ⁸⁷Rb¹⁷⁰Yb, this would be the $\Delta\nu' = -4$ state with the lowest resonance predicted around 1300 G [34].

## V. Conclusion

We have observed a pair of photoassociation resonances in ⁸⁷Rb¹⁷⁰Yb and characterized them with regards to photoassociation rate, binding energy, and Zeeman shift. We have identified possible causes for the failure to observe more resonances, but like the assignment of the observed lines, this question will require further spectroscopy and quantum chemistry calculations well beyond the scope of this work. As expected, the observed PA rates are orders of magnitude smaller than those observed near the alkali D lines. However, by preparing both species in a mixed Mott insulator, the achievable Rabi frequencies may be greatly enhanced in future experiments. Starting from the motional ground state of a lattice site rather than a thermal continuum will enable much greater control over the association process and may even allow for free-bound STIRAP [39]. However, due to the unfavorable ratio of PA rate to off-resonant atomic excitation on the observed lines, it may be preferable to perform photoassociation near the D1 line of rubidium.

Nonetheless, intercombination-line photoassociation is a powerful spectroscopic tool. We have demonstrated its use for the precise measurement of bound-state energies by two-photon photoassociation, improving the uncertainties on previously determined values by two orders of magnitude. The precise knowledge of bound-state energies in the electronic ground state will allow us to pinpoint the predicted position of magnetic Feshbach resonances, which may provide an alternative route for the initial association of weakly bound molecules. This spectroscopy technique will also allow for highly sensitive detection of light shifts to the bound levels. This will be invaluable for spectroscopy of more deeply bound states in the electronically excited potential, which will be required to identify a suitable intermediate level for STIRAP transfer to the absolute ground state [64].

## Acknowledgments

We thank R. Stephan for his work on the electronic and mechanical components and Matthew D. Frye for insightful discussions. T.F. acknowledges a fellowship from Prof. W. Behmenburg-Schenkung. The experimental apparatus was funded by DFG under Grant No. INST 208/614-1 FUGG.

## Appendix A: Laser stabilization

The free-bound photoassociation laser is stabilized at a tuneable offset of up to 11 GHz to the MOT laser using a beatnote lock. The MOT laser in turn is stabilized to a Zerodur cavity over short timescales and to the atomic transition via active stabilization of the vertical MOT position [65] over long timescales. The beatnote utilizes the fundamental output of fiber lasers at 1112 nm before frequency doubling to 556 nm, effectively doubling the accessible offset frequency range.

For beatnote detection we utilize a so-called small form-factor pluggable (SFP) module intended for fiberoptic networking equipment operating at 1.3 or 1.5 µm. This module provides an InGaAs detector coupled to a single-mode fiber socket, a transimpedance amplifier, and a limiting amplifier in a compact package and requires only minimal supporting circuitry, while providing bandwidth and signal-to-noise far exceeding that of a simple photodiode connected to a 50-Ω rf amplifier.

To lock the beatnote to the desired offset frequency we use an Analog Devices ADF4159 fractional-N phase-locked loop (PLL) chip mounted on an evaluation board. This allows us to lock the beatnote to arbitrary offset frequencies up to $\sim 10$ GHz without the need for a matching microwave reference frequency. We note the range of offset frequencies explored is not limited by the locking setup but rather by the time-consuming nature of the experiments.

## Appendix B: Bound-bound light generation

Light used to drive the bound-bound transitions in Sec. IV is derived from the same laser used for the free-bound transition. To bridge the frequency gap, two different methods are used.

For the $\Delta\nu' = -1$ transition the frequency difference is realized by frequency shifting in two acousto-optical modulators (AOM), before both beams are combined and coupled into a common single-mode fiber to ensure overlap. The $\Delta\nu' = -2$ transition, on the other hand, is driven by a sideband generated using a bulk electro-optical modulator (EOM) placed in the free-bound laser path. A split ring resonator [66] allows us to obtain a modulation index of $\beta \approx 1$, corresponding to 20% of the input power in each first-order sideband, at a moderate drive power of 1 W. As the resonator can be constructed and tuned by simple means, this provides an attractive way for generating light at offset frequencies in the GHz range, where typical AOM setups become impractical. However, it comes at the cost of having both the carrier and further, undesired sidebands present in the output. In particular, the third harmonic of the $\Delta\nu' = -2$ transition probed in Sec. IV is very close to the binding energy of the intermediate states used here. This leads to one such sideband being almost resonant with the atomic transition and causing excessive trap loss even at low powers.

## References

[1] A. Micheli, G. Brennen, and P. Zoller, A toolbox for lattice-spin models with polar molecules, Nat. Phys. **2**, 341 (2006).

[2] I. M. Georgescu, S. Ashhab, and F. Nori, Quantum simulation, Rev. Mod. Phys. **86**, 153 (2014).

[3] B. Gadway and B. Yan, Strongly interacting ultracold polar molecules, J. Phys. B: At., Mol. Opt. Phys. **49**, 152002 (2016).

[4] A. J. Daley, I. Bloch, C. Kokail, S. Flannigan, N. Pearson, M. Troyer, and P. Zoller, Practical quantum advantage in quantum simulation, Nature (London) **607**, 667 (2022).

[5] R. V. Krems, Cold controlled chemistry, Phys. Chem. Chem. Phys. **10**, 4079 (2008).

[6] N. Balakrishnan, Perspective: Ultracold molecules and the dawn of cold controlled chemistry, J. Chem. Phys. **145**, 150901 (2016).

[7] Y. Liu and K.-K. Ni, Bimolecular chemistry in the ultracold regime, Annu. Rev. Phys. Chem. **73**, 73 (2022).

[8] P. D. Gregory, J. A. Blackmore, S. L. Bromley, J. M. Hutson, and S. L. Cornish, Robust storage qubits in ultracold polar molecules, Nat. Phys. **17**, 1149 (2021).

[9] R. Sawant, J. A. Blackmore, P. D. Gregory, J. Mur-Petit, D. Jaksch, J. Aldegunde, J. M. Hutson, M. R. Tarbutt, and S. L. Cornish, Ultracold polar molecules as qudits, New J. Phys. **22**, 013027 (2020).

[10] G. Quéméner and J. L. Bohn, Shielding $^2\Sigma$ ultracold dipolar molecular collisions with electric fields, Phys. Rev. A **93**, 012704 (2016).

[11] E. Abrahamsson, T. V. Tscherbul, and R. V. Krems, Inelastic collisions of cold polar molecules in nonparallel electric and magnetic fields, J. Chem. Phys. **127**, 044302 (2007).

[12] J. Pérez-Ríos, F. Herrera, and R. V. Krems, External field control of collective spin excitations in an optical lattice of $^2\Sigma$ molecules, New J. Phys. **12**, 103007 (2010).

[13] F. Herrera, Y. Cao, S. Kais, and K. B. Whaley, Infrared-dressed entanglement of cold open-shell polar molecules for universal matchgate quantum computing, New J. Phys. **16**, 075001 (2014).

[14] M. Karra, K. Sharma, B. Friedrich, S. Kais, and D. Herschbach, Prospects for quantum computing with an array of ultracold polar paramagnetic molecules, J. Chem. Phys. **144**, 094301 (2016).

[15] K. Asnaashari and R. V. Krems, Quantum annealing with pairs of $^2\Sigma$ molecules as qubits, Phys. Rev. A **106**, 022801 (2022).

[16] N. J. Fitch and M. R. Tarbutt, Laser-cooled molecules, Adv. At. Mol. Opt. Phys. **70**, 157 (2021).

[17] D. J. McCarron, M. H. Steinecker, Y. Zhu, and D. DeMille, Magnetic Trapping of an Ultracold Gas of Polar Molecules, Phys. Rev. Lett. **121**, 013202 (2018).

[18] L. W. Cheuk, L. Anderegg, B. L. Augenbraun, Y. Bao, S. Burchesky, W. Ketterle, and J. M. Doyle, Λ-Enhanced Imaging of Molecules in an Optical Trap, Phys. Rev. Lett. **121**, 083201 (2018).

[19] L. Anderegg, L. W. Cheuk, Y. Bao, S. Burchesky, W. Ketterle, K.-K. Ni, and J. M. Doyle, An optical tweezer array of ultracold molecules, Science **365**, 1156 (2019).

[20] S. Truppe, H. J. Williams, M. Hambach, L. Caldwell, N. J. Fitch, E. A. Hinds, B. E. Sauer, and M. R. Tarbutt, Molecules cooled below the Doppler limit, Nat. Phys. **13**, 1173 (2017).

[21] H. J. Williams, L. Caldwell, N. J. Fitch, S. Truppe, J. Rodewald, E. A. Hinds, B. E. Sauer, and M. R. Tarbutt, Magnetic Trapping and Coherent Control of Laser-Cooled molecules, Phys. Rev. Lett. **120**, 163201 (2018).

[22] K.-K. Ni, S. Ospelkaus, M. H. G. de Miranda, A. Pe'er, B. Neyenhuis, J. J. Zirbel, S. Kotochigova, P. S. Julienne, D. S. Jin, and J. Ye, A high phase-space-density gas of polar molecules, Science **322**, 231 (2008).

[23] F. Lang, K. Winkler, C. Strauss, R. Grimm, and J. Hecker Denschlag, Ultracold Triplet Molecules in the Rovibrational Ground State, Phys. Rev. Lett. **101**, 133005 (2008).

[24] J. G. Danzl, E. Haller, M. Gustavsson, M. J. Mark, R. Hart, N. Bouloufa, O. Dulieu, H. Ritsch, and H.-C. Nägerl, Quantum gas of deeply bound ground state molecules, Science **321**, 1062 (2008).

[25] P. K. Molony, P. D. Gregory, Z. Ji, B. Lu, M. P. Köppinger, C. R. Le Sueur, C. L. Blackley, J. M. Hutson, and S. L. Cornish, Creation of Ultracold ⁸⁷Rb¹³³Cs Molecules in the Rovibrational Ground State, Phys. Rev. Lett. **113**, 255301 (2014).

[26] J. W. Park, S. A. Will, and M. W. Zwierlein, Ultracold Dipolar Gas of Fermionic ²³Na⁴⁰K Molecules in Their Absolute Ground State, Phys. Rev. Lett. **114**, 205302 (2015).

[27] F. Seeßelberg, N. Buchheim, Z.-K. Lu, T. Schneider, X.-Y. Luo, E. Tiemann, I. Bloch, and C. Gohle, Modeling the adiabatic creation of ultracold polar ²³Na⁴⁰K molecules, Phys. Rev. A **97**, 013405 (2018).

[28] K. Leung, E. Tiberi, B. Iritani, I. Majewska, R. Moszynski, and T. Zelevinsky, Ultracold ⁸⁸Sr₂ molecules in the absolute ground state, New J. Phys. **23**, 115002 (2021).

[29] J. Cao, H. Yang, Z. Su, X.-Y. Wang, J. Rui, B. Zhao, and J.-W. Pan, Preparation of a quantum degenerate mixture of ²³Na⁴⁰K molecules and ⁴⁰K atoms, Phys. Rev. A **107**, 013307 (2023).

[30] L. De Marco, G. Valtolina, K. Matsuda, W. G. Tobias, J. P. Covey, and J. Ye, A degenerate Fermi gas of polar molecules, Science **363**, 853 (2019).

[31] A. Schindewolf, R. Bause, X.-Y. Chen, M. Duda, T. Karman, I. Bloch, and X.-Y. Luo, Evaporation of microwave-shielded polar molecules to quantum degeneracy, Nature (London) **607**, 677 (2022).

[32] C. Chin, R. Grimm, P. Julienne, and E. Tiesinga, Feshbach resonances in ultracold gases, Rev. Mod. Phys. **82**, 1225 (2010).

[33] P. S. Żuchowski, J. Aldegunde, and J. M. Hutson, Ultracold RbSr Molecules Can Be Formed by Magnetoassociation, Phys. Rev. Lett. **105**, 153201 (2010).

[34] D. A. Brue and J. M. Hutson, Prospects of forming ultracold molecules in $^2\Sigma$ states by magnetoassociation of alkali-metal atoms with Yb, Phys. Rev. A **87**, 052709 (2013).

[35] D. A. Brue and J. M. Hutson, Magnetically Tunable Feshbach Resonances in Ultracold Li-Yb Mixtures, Phys. Rev. Lett. **108**, 043201 (2012).

[36] V. Barbé, A. Ciamei, B. Pasquiou, L. Reichsöllner, F. Schreck, P. S. Żuchowski, and J. M. Hutson, Observation of Feshbach resonances between alkali and closed-shell atoms, Nat. Phys. **14**, 881 (2018).

[37] A. Green, H. Li, J. H. See Toh, X. Tang, K. C. McCormick, M. Li, E. Tiesinga, S. Kotochigova, and S. Gupta, Feshbach Resonances in p-Wave Three-Body Recombination within Fermi-Fermi Mixtures of Open-Shell ⁶Li and Closed-shell ¹⁷³Yb atoms, Phys. Rev. X **10**, 031037 (2020).

[38] T. Franzen, A. Guttridge, K. E. Wilson, J. Segal, M. D. Frye, J. M. Hutson, and S. L. Cornish, Observation of magnetic Feshbach resonances between Cs and ¹⁷³Yb, Phys. Rev. Res. **4**, 043072 (2022).

[39] A. Ciamei, A. Bayerle, C.-C. Chen, B. Pasquiou, and F. Schreck, Efficient production of long-lived ultracold Sr₂ molecules, Phys. Rev. A **96**, 013406 (2017).

[40] N. Nemitz, F. Baumer, F. Münchow, S. Tassy, and A. Görlitz, Production of heteronuclear molecules in an electronically excited state by photoassociation in a mixture of ultracold Yb and Rb, Phys. Rev. A **79**, 061403(R) (2009).

[41] C. Bruni and A. Görlitz, Observation of hyperfine interaction in photoassociation spectra of ultracold RbYb, Phys. Rev. A **94**, 022503 (2016).

[42] F. Münchow, C. Bruni, M. Madalinski, and A. Görlitz, Two-photon photoassociation spectroscopy of heteronuclear YbRb, Phys. Chem. Chem. Phys. **13**, 18734 (2011).

[43] M. Borkowski, P. S. Żuchowski, R. Ciuryło, P. S. Julienne, D. Kędziera, L. Mentel, P. Tecmer, F. Münchow, C. Bruni, and A. Görlitz, Scattering lengths in isotopologues of the RbYb system, Phys. Rev. A **88**, 052708 (2013).

[44] S. G. Porsev, A. Derevianko, and E. N. Fortson, Possibility of an optical clock using the $6\,{}^1S_0 \rightarrow 6\,{}^3P^o_0$ transition in ¹⁷¹,¹⁷³Yb atoms held in an optical lattice, Phys. Rev. A **69**, 021403(R) (2004).

[45] T. Kuwamoto, K. Honda, Y. Takahashi, and T. Yabuzaki, Magneto-optical trapping of Yb atoms using an intercombination transition, Phys. Rev. A **60**, R745 (1999).

[46] F. Scazza, C. Hofrichter, M. Höfer, P. De Groot, I. Bloch, and S. Fölling, Observation of two-orbital spin-exchange interactions with ultracold SU(N)-symmetric fermions, Nat. Phys. **10**, 779 (2014).

[47] L. Franchi, L. F. Livi, G. Cappellini, G. Binella, M. Inguscio, J. Catani, and L. Fallani, State-dependent interactions in ultracold ¹⁷⁴Yb probed by optical clock spectroscopy, New J. Phys. **19**, 103037 (2017).

[48] M. Shundalau and A. Minko, Ab initio multi-reference perturbation theory calculations of the ground and some excited electronic states of the RbYb molecule, Comput. Theor. Chem. **1103**, 11 (2017).

[49] B. Mukherjee, M. D. Frye, and J. M. Hutson, Feshbach resonances and molecule formation in ultracold mixtures of Rb and Yb($^3P$) atoms, Phys. Rev. A **105**, 023306 (2022).

[50] B. Mukherjee, M. D. Frye, and J. M. Hutson, Magnetic Feshbach resonances between atoms in $^2S$ and $^3P_0$ states: Mechanisms and dependence on atomic properties, Phys. Rev. Res. **5**, 013102 (2023).

[51] B. Pollklesener, T. Franzen, C. Sillus, and A. Görlitz (unpublished).

[52] K. M. Mertes, J. W. Merrill, R. Carretero-González, D. J. Frantzeskakis, P. G. Kevrekidis, and D. S. Hall, Nonequilibrium Dynamics and Superfluid Ring Excitations in Binary Bose-Einstein Condensates, Phys. Rev. Lett. **99**, 190402 (2007).

[53] M. Kitagawa, K. Enomoto, K. Kasa, Y. Takahashi, R. Ciuryło, P. Naidon, and P. S. Julienne, Two-color photoassociation spectroscopy of ytterbium atoms and the precise determinations of s-wave scattering lengths, Phys. Rev. A **77**, 012719 (2008).

[54] F. Baumer, F. Münchow, A. Görlitz, S. E. Maxwell, P. S. Julienne, and E. Tiesinga, Spatial separation in a thermal mixture of ultracold ¹⁷⁴Yb and ⁸⁷Rb atoms, Phys. Rev. A **83**, 040702(R) (2011).

[55] S. G. Porsev, M. S. Safronova, A. Derevianko, and C. W. Clark, Relativistic many-body calculations of Van der Waals coefficients for Yb-Li and Yb-Rb dimers, Phys. Rev. A **89**, 022703 (2014).

[56] Inclusion of three-body losses does not improve the fit due to the relatively low Rb density at this stage of the experiment.

[57] A. Devolder, E. Luc-Koenig, O. Atabek, M. Desouter-Lecomte, and O. Dulieu, Proposal for the formation of ultracold deeply bound RbSr dipolar molecules by all-optical methods, Phys. Rev. A **98**, 053411 (2018).

[58] Assuming their linewidth is no smaller than the atomic linewidth of $2\pi \times 182$ kHz.

[59] A. Ciamei, Taming ultracold RbSr and Sr₂, Ph.D. thesis, Universiteit van Amsterdam, 2018.

[60] P. Soldán and J. M. Hutson, Near-dissociation states and coupled potential curves for the HeN⁺ complex, J. Chem. Phys. **117**, 3109 (2002).

[61] E. R. I. Abraham, W. I. McAlexander, C. A. Sackett, and R. G. Hulet, Spectroscopic Determination of the s-Wave Scattering Length of Lithium, Phys. Rev. Lett. **74**, 1315 (1995).

[62] The data presented here is obtained using transition A, but we have verified similar spectra can be obtained using transition B.

[63] M. Fleischhauer, A. Imamoglu, and J. P. Marangos, Electromagnetically induced transparency: Optics in coherent media, Rev. Mod. Phys. **77**, 633 (2005).

[64] K. Winkler, F. Lang, G. Thalhammer, P. v. d. Straten, R. Grimm, and J. H. Denschlag, Coherent Optical Transfer of Feshbach Molecules to a Lower Vibrational State, Phys. Rev. Lett. **98**, 043201 (2007).

[65] C. Sillus, T. Franzen, B. Pollklesener, and A. Görlitz, Active position stabilization of an atomic cloud in a narrow-line magneto-optical trap using a Raspberry Pi, Rev. Sci. Instrum. **92**, 033204 (2021).

[66] J. F. Kelly and A. Gallagher, Efficient electro-optic modulator for optical pumping of Na beams, Rev. Sci. Instrum. **58**, 563 (1987).
