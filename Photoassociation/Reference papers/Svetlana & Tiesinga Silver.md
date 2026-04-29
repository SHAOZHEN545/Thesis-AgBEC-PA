## III. ONE-COLOR PHOTOASSOCIATION OF ULTRACOLD SILVER ATOMS

One-color photoassociation of ultracold, ground-state silver atoms is the process whereby a pair of colliding silver atoms resonantly absorbs a photon from a continuous wave (cw) laser and is excited to a weakly bound rovibrational level of an electronically excited state. These excited levels are short lived and the atom pair decays back to two much-hotter ground state atoms or a ground-state molecule by spontaneous emission of a photon. These products are typically no longer held in the magnetic, optical, or magneto-optical trap in which the ultracold atoms are stored or held. Hence, resonant one-color photoassociation leads to loss of atoms from their trap, which can often be easily detected. A review of this process can be found in Ref. [46].

In simulating photoassociation of ultracold, ground-state silver atoms, we consider laser light with wave numbers detuned up to 100 cm$^{-1}$ to the red of the ground $4d^{10}5s(^2S)$ to excited $4d^{10}5p(^2P_{1/2})$ or $D1$ transition. Specifically, we imagine $^{107}\text{Ag}$ or $^{109}\text{Ag}$ atoms in a magneto-optical trap, where these atoms are in the energetically lowest $f = 1$ hyperfine state with all three Zeeman sublevels equally populated. Weakly bound rovibrational levels of attractive excited-state electronic potentials dissociating to the $5s(^2S_{1/2}) + 5p(^2P_{1/2})$ limit can be modeled using the relativistic adiabatic Hamiltonian of Ref. [65] for atom-atom separations $R$, where the binding energies of these potentials are significantly smaller than the spin-orbit splitting $\Delta \approx hc \times 920.6 \, \text{cm}^{-1}$ between the $5p(^2P_{1/2})$ and $5p(^2P_{3/2})$ states of Ag. We omit the effects of the nearly degenerate $4d^9 5s^2(^2D)$ configuration on the $4d^{10} 5p(^2P)$ states. The model of Ref. [65] has been successful in describing photoassociation of ultracold alkali-metal atom gasses [46].

There exist six relativistic adiabatic states whose potential energies approach that of the $5s(^2S_{1/2}) + 5p(^2P_{1/2})$ limit for large $R$. The energetically lowest state is labeled by $\Omega_{\sigma}^+ = 0_u^+$. For $\Omega = 0$ states hyperfine interactions can be ignored for our purposes. With the help of Ref. [65], we derive that the long-range tail of the excited $0_u^+$ state is well described by

$$
V(R; 0_u^+) = -\frac{4}{3} \frac{C_3}{R^3} - \left[ \frac{2}{9} \frac{(C_3)^2}{\Delta} + C_{6,0_u^+} \right] \frac{1}{R^6} + O\left(\frac{1}{R^8}\right),
$$

where the resonant dipole-dipole coefficient $C_3 = |\langle^2P||d||^2S\rangle|^2 / (4\pi \epsilon_0)$ with reduced matrix element $\langle^2P||d||^2S\rangle$ of the atomic dipole moment operator $d$ with respect to nonrelativistic atomic states $|^{2S+1}L\rangle$ using the conventions of Ref. [66]. Finally, the repulsive $C_{6,0_u^+}/R^6$ potential represents the dispersion contribution from doubly excited molecular states.

Table I gives our values for the parameters used in Eq. (1). The nonrelativistic or weighted atomic transition energies between the barycenters of ground state $4d^{10}5p(^2S)$ and excited state $4d^{10}5p(^2P)$ and the relativistic spin-orbit splitting between the $4d^{10}5p(^2P_{1/2})$ and $4d^{10}5p(^2P_{3/2})$ states have been derived from data in Ref. [17] and can be considered exact for our purposes. The table also gives the weighted line strength $S_{2p \rightarrow 2s}$, the square of the reduced transition matrix element for the $4d^{10}5p(^2S)$ and $4d^{10}5p(^2P)$ transition as well as the Einstein $A$ coefficient and natural linewidth $\gamma_P$ of the nonrelativistic $4d^{10}5p(^2P)$ state. We use the theoretical value for the line strength of Ref. [67] and obtained by third-order many-body perturbation theory. We conservatively inferred a 15 % standard uncertainty from the discussion in the first column of page 5 of Ref. [67]. The value for $S_{2p \to 2s}$ by Ref. [67] coincides with a recent theoretical evaluation in Ref. [68], while the authors of Refs. [69,70] prefer a value close to the lower bound of our $S_{2p \to 2s}$. Experimental determinations also favor a value close to this lower bound, approximately $15e^2a_0^2$ [71–73]. The most precise experimental evaluation gives $S_{2p \to 2s} = 15.10(5)e^2a_0^2$ [73]. A review of all measurements can be found in Ref. [74]. Our value for $C_3$ and $C_{6,0^{+}_{tt}}$, the latter derived from our electronic structure calculations of excited Ag$_2$ states, are listed in Table I.

Figure 5 shows the long-range potential-energy curve of our $0_u^+$ state as well as eigenenergies $E_v$ of $J = 1$ vibrational levels $v$ of this potential for the $^{109} \text{Ag}_2$ isotopologue. From left to right the three panels in the figure show eigenenergies down to $hc \times 100 \, \text{cm}^{-1}$, $hc \times 10 \, \text{cm}^{-1}$, and $hc \times 1 \, \text{cm}^{-1}$ below its $5s(^{2}S_{1/2}) + 5p(^{2}P_{1/2})$ dissociation limit, respectively. The eigenenergies have been computed numerically by discretizing the Hamiltonian containing the sum of the relative radial kinetic-energy operator of the atoms $-(\hbar^2/2\mu)d^2/dR^2$ with reduced mass $\mu$, centrifugal potential $\hbar^2J(J+1)/(2\mu R^2)$, and the potential-energy curve of our $0_u^+$ state using the discrete variable representation of Ref. [75] and solving the resulting matrix eigenvalue problem with a linear algebra package. For small separations, where the binding energies of the $0_u^+$ potential are larger than $hc \times 100 \, \text{cm}^{-1}$, we smoothly connect the long-range potential in Eq. (1) to our electronic structure calculation of this state as described in Sec. II. We observe that the outer turning points $R_0$, defined as $V(R_0; 0_u^+) = E_v$, range from $20a_0$ for binding energies near $hc \times 100 \, \text{cm}^{-1}$ to around $200a_0$ for binding energies near $hc \times 0.1 \, \text{cm}^{-1}$. The accuracy of our $0_u^+$ potential is not sufficient to predict the location of individual levels. The level spacing or density, however, is reasonably accurate.

Within the model of Ref. [65] we can also estimate the molecular transition dipole moments to, and natural linewidths of, weakly bound rovibrational levels of the excited $0_u^+$ state dissociating to the $4d^{10}5s(2S) + 4d^{10}5p(2P_{1/2})$ limit. First, we realize that in one-color photoassociation experiments with an ultracold Ag gas with atoms in the $f = 1$ hyperfine state and equal population in the $m$ states, we collide in superpositions of the $X^1\Sigma_g^+$ and $a^3\Sigma_u^+$ electronic states. Photon selection rules only allow transitions from the $X^1\Sigma_g^+$ component of the superposition to the excited $0_u^+$ state. Some algebra shows that the molecular electric transition dipole moment between the $X^1\Sigma_g^+$ and the excited $0_u^+$ states and the natural linewidth of the excited $0_u^+$ state are

$$
d_{\text{eff}}(0_u^+) = \sqrt{\frac{2}{3}} \langle P || d ||^2 S \rangle \quad \text{and} \quad \gamma_{0_u^+} = \frac{2}{3} \gamma_P,
$$

respectively. We expect that the transition dipole moment for the superposition state is within factors of two from $d_{\text{eff}}(0_u^+)$ and, for simplicity, we assume that $d_{\text{eff}}(0_u^+)$ is the correct value for the dipole moment for the remainder of this paper.

Second, we recall that for $R > 20a_0$ the potential energies of the $X^1\Sigma_g^+$ and $a^3\Sigma_u^+$ states are identical and to good approximation are given by the van der Waals potential $V_{\text{vdW}}(R) = -C_6/R^6$. Our preferred values for dispersion coefficient $C_6$, van der Waals length $\beta_6 = (2\mu C_6/\hbar^2)^{1/4}$, and energy $\mathcal{E}_6 = \hbar^2/(2\mu\beta_6^2)$ are given in Table I. From Fig. 5, we observe that for $R > 20a_0$ the rovibrational levels of the excited $0_u^+$ state have binding energies less than $hc \times 100 \, \text{cm}^{-1}$.

We are now ready to introduce the **event rate coefficient** of photoassociation for two ultracold atoms colliding with relative kinetic or collision energy $E$ assuming that $s$ or $\ell = 0$ partial-wave collisions contribute to rovibrational level $v$ of the $J = 1$ excited $0_u^+$ state using laser light with photon energy $\hbar\omega$. In fact, we have the **event rate coefficient** [76–78]

$$
K_v(\hbar\omega, E) = \frac{\pi}{k_{\text{rel}}^2} \frac{\hbar^2 \gamma_{0_u^+} \gamma_v(E)}{[E + \hbar\omega - [E_\infty + E_v(0_u^+)]^2 + \hbar^2[\gamma_{0_u^+} + \gamma_v(E)]^2/4]}
$$

for each vibrational level $v$, where $E = \hbar^2 k_{\text{rel}}^2/2\mu = \mu v_{\text{rel}}^2/2$, $\gamma_{0_u^+}$ is the natural linewidth of the excited-state vibrational level, $E_\infty$ is the asymptotic energy of the excited $0_u^+$ state relative to that of the ground state when $R \to \infty$, $E_v(0_u^+) < 0$ is the binding energy of the vibrational level, and stimulated width

$$
\gamma_v(E) = \frac{2\pi}{\hbar} |\langle \Psi_v(0_u^+) | \mathbf{d} \cdot \mathbf{E}_{\text{elec}} | \psi_g^{(+)}(E) \rangle|^2.
$$

Here,

$$
\psi_g^{(+)}(R, E) = \langle R | \psi_g^{(+)}(E) \rangle \quad \text{and} \quad \Psi_v(R; 0_u^+) = \langle R | \Psi_v(0_u^+) \rangle
$$

are radial wave functions of the ground and excited state as functions of $R$, respectively. Excited $0_u^+$ rovibrational wave functions are unit normalized with

$$
\int_0^\infty dR |\Psi_v(R; 0_u^+)|^2 = 1
$$

and the $s$-wave scattering wave function is energy-normalized with

$$
\psi_g^{(+)}(R, E) \to e^{i\eta_g(E)} \sqrt{\frac{2\mu}{\pi \hbar^2}} \frac{\sin[k_{\text{rel}}R + \eta_g(E)]}{\sqrt{k_{\text{rel}}}}
$$

for $R \to \infty$, where $\eta_g(E)$ is the scattering phase shift. Moreover, operator $-\mathbf{d} \cdot \mathbf{E}_{\text{elec}}$ represents the light-induced coupling, where vector **d** is the dipole moment operator and vector $\mathbf{E}_{\text{elec}} = \mathcal{E}_0 \epsilon \cos(k_L z - \omega t)$ is the electric field of the laser beam propagating along the space-fixed $z$ axis. The field has polarization $\epsilon$, wave number $k_L = \omega / c$, and electric-field strength $\mathcal{E}_0$. Using the rotating-wave approximation and Eq. (2) we have

$$
-\mathbf{d} \cdot \mathbf{E}_{\text{elec}} \rightarrow -\frac{1}{2} d_{\text{eff}}(0_u^+) \mathcal{E}_0 = -Q \frac{d_{\text{eff}}(0_u^+)}{ea_0} \sqrt{\frac{I}{\text{W/cm}^2}},
$$

energy $Q = a_0 [2\pi \alpha \hbar (1 \, \text{W/cm}^2)]^{1/2} = h \times 17.561 \, 264 \, \text{MHz}$, and laser intensity $I$. In addition to the approximations inherent in Eq. (2), we have also omitted angular-momentum factors, of order unity, from evaluating $\mathbf{d} \cdot \epsilon$ for colliding $f = 1$ hyperfine states and $J = 1$ levels of the $0_u^+$ state.

In ultracold-atom experiments both atoms are lost in the photoassociation process and thus the observed thermalized loss rate coefficient is $K_{\text{tot}}(\hbar \omega, kT) = 2 \sum_v \langle K_v(\hbar \omega, E) \rangle$, where the angled brackets indicate a thermal average assuming a Boltzmann distribution at temperature $T$ of the atomic gas. Photoassociation lineshapes of $K_{\text{tot}}(\hbar \omega, kT)$ have been studied in Ref. [79]. In practice, energy widths $\hbar \gamma_s$ and $kT$ are orders of magnitude smaller than the energy spacing between vibrational levels. Finally inspection of Eq. (3) and the observation that $\gamma_v(E) \propto \sqrt{E}$ for small $E$, as shown later on, implies that $K_v(\hbar \omega, E)$ is independent of $E$ for $E \to 0$.

Julienne in Ref. [77] also derived that for ultracold collisions the stimulated width $\gamma_v(E)$ has an accurate analytical form based on the reflection approximation, where (1) the matrix element of $-\mathbf{d} \cdot \mathbf{E}_{\text{elec}}$ is mainly determined by the radial scattering and bound-state wave functions over a small spatial region near the outer turning point $R_0$ or more precisely the Condon point $R_C$ of the transition and (2) $|V_{\text{vdW}}(R)| \ll |V(R; 0_u^+)|$ for $R > 20a_0$. The Condon point is that separation, where for a given laser frequency the local kinetic energies in the ground and excited state are the same. Then the reflection approximation gives

$$
\gamma_v(E) = \frac{2\pi}{\hbar} Q^2 \frac{I}{W/\text{cm}^2} \left( \frac{d_{\text{eff}}(0_u^+)}{ea_0} \right)^2 \frac{dE_v(0_u^+)}{dv} \frac{1}{D_C} |\psi_g^{(+)}(R_C, E)|^2,
$$

a function proportional to the square of the absolute value of the ground-state scattering wave function, where slope

$$
D_C = \left| \frac{d}{dR}[V(R; 0_u^+)] - V_{\text{vdW}}(R)]_{R=R_C} \right| \approx 4 \frac{C_3}{R_C^4}
$$

and the Condon point is found from

$$
-\frac{4}{3} \frac{C_3}{R_C^3} = E_v(0_u^+).
$$

state, and $s_3 = 6\sqrt{\pi}\Gamma(4/3)/\Gamma(5/6) = 8.413092 \ldots$, where $\Gamma(z)$ is the Gamma function.

Our final ingredient in obtaining an analytical expression for the stimulated width is observing that the $s$-wave ground-state wave function for collision energies around and below the van der Waals energy $\mathcal{E}_6$, i.e., assuming the Wigner threshold law for $E \to 0$, is [28,81–83]

$$
\psi_g^{(+)}(R, E) = \frac{1}{\sqrt{2\pi}} \frac{1}{\sqrt{\mathcal{E}_6\beta_6}} \sqrt{k_{\text{rel}}\beta_6} \sqrt{x} \left\{ \Gamma(3/4)J_{-1/4}(1/[2x^2]) - 2\frac{a}{\beta_6}\Gamma(5/4)J_{1/4}(1/[2x^2]) \right\}
$$

for $R > 20a_0$ and $k_{\text{rel}}|R - a| < \pi/2$, where $x = R/\beta_6$, $a$ is the scattering length, and $J_\nu(z)$ is the Bessel function of the first kind. Inserting Eq. (11) into Eq. (7) shows that the stimulated width $\gamma_\nu(E) \propto \sqrt{E}$ as promised. Currently, the uncertainties of the short-range, $R < 20a_0$ shape of the potentials of the $X^1\Sigma_g^+$ and $a^3\Sigma_u^+$ states is such that the value for $a$ is unknown and can lie between $-\infty$ and $+\infty$. The authors of Ref. [81], however, have shown that the probability distribution for $a$ is a Cauchy or Lorentz distribution with its maximum at the mean scattering length $\bar{a} = \Gamma(3/4)\beta_6/[2\sqrt{2}\Gamma(5/4)] \approx 0.478\beta_6$ and its half-width at half-maximum (HWHM) also equal to $\bar{a}$. See Table I for the value for $\bar{a}$ for $^{109}\text{Ag}^+ + ^{109}\text{Ag}$.

Figure 6 shows stimulated widths for the excited $0_u^+$ state and ultracold $^{109}\text{Ag}$ atoms at laser intensity $I = 1 \text{W/cm}^2$ and collision energy $E = \mathcal{E}_6$ based on our analytical expression for $s$-wave collisions as functions of binding energy $E_v(0_u^+)$ for several scattering lengths $a$ around $\bar{a}$. A laser intensity of 1 W/cm$^2$ is typical for photoassociation experiments while the temperature of Ag atoms in a magneto-optical trap is of order $\mathcal{E}_6/k$. In optical dipole traps the temperature is much smaller than $\mathcal{E}_6/k$. In an experiment the curves are only sampled at a discrete set of $E_v(0_u^+)$ corresponding to the measured binding energies. We have used the nominal, most likely parameter values from Table I. The stimulated widths for other $I$ and $E < \mathcal{E}_6$ follow from the fact that $\gamma_v(E) \propto I\sqrt{E}$.

The stimulated widths as a function of binding energy in Fig. 6 alternate between zeros and maxima with maximum values ranging from $2\pi \times 0.01$ MHz to $2\pi \times 0.1$ MHz for energies $|E_v(0_u^+)| < hc \times 5 \, \text{cm}^{-1}$. The location of the zeros is very sensitive to the scattering length, where for increasing $a$ the zeros move to less negative binding energies. These zeros in the widths correspond to the zeros of the radial scattering wave function of Eq. (11) using the relationship between the Condon point and $E_v(0_u^+)$ from Eq. (9). In fact, the zeros in $\gamma_v(E)$ for binding energies in $hc \times [-40, -15] \, \text{cm}^{-1}$ and $<hc \times -10 \, \text{cm}^{-1}$ correspond to nodes in the scattering wave function between $R = [27a_0, 40a_0]$ and $R > 40a_0$, respectively. Hence, the precise binding energy of the zeros in the stimulated width can be used to determine the scattering length and, to a lesser extent, the van der Waals coefficient. Finally, the various curves cross at $E_v(0_u^+)/hc \approx 46.0 \, \text{cm}^{-1}$ and $14.9 \, \text{cm}^{-1}$, where the Bessel function multiplying the scattering length is zero. While visually striking, the crossings cannot be used to determine $a$ from experimental data.

For binding energies in $hc \times [-1, 0] \, \text{cm}^{-1}$, the stimulated width is on the order of the natural linewidth of $2\pi \times 17(3) \, \text{MHz}$ for the $0_u^+$ state even for $I = 1 \, \text{W/cm}^2$. For vibrational levels in this binding-energy range, the event rate coefficient can thus saturate and approach the unitarity limit $v_{\text{rel}} \pi / k_{\text{rel}}^2$ when $\gamma_v(E) = \gamma_{0_u^+}$, which is $1.8 \times 10^{-11} \, \text{cm}^3/\text{s}$ at $E = \mathcal{E}_6$ for Ag + Ag.

Finally, we note that the validity of the Wigner threshold law with which we derived Eq. (11) is not guaranteed for collision energies near $\mathcal{E}_6$, especially for scattering lengths $a \gg \beta_6$. For example, phase factor $e^{in_g(E)}$ in Eq. (5) can significantly deviate from one. In practice, numerical simulations of the scattering wave function are required for energies larger than $\mathcal{E}_6$. Nevertheless, we show widths at $E = \mathcal{E}_6$ as it is the natural energy scale of the van der Waals potential and we can use their $\sqrt{E}$ dependence to infer widths at smaller collision energies.

Figure 7 shows stimulated widths as a function of binding energy between $hc \times [-10, 0] \, \text{cm}^{-1}$ for two line strengths $S_{2p \to 2s}$ but the same van der Waals coefficient and scattering length $a = +0.5\beta_6$, close to the mean scattering length. The two $S_{2p \to 2s}$ correspond to our nominal value of $17.4e^2a_0^2$ from Table I and that obtained from the most accurate measurement of Ref. [73] of $15.1e^2a_0^2$. A different line strength implies a change in the long-range $-(4/3)C_3/R^3$ potential of the excited $0_u^+$ state. Hence, even though the zeros in the scattering wave function are at the same separations, Eq. (9) implies that in the binding-energy domain the zeros of the stimulated width occur at different $E_v(0_u^+)$. For $a = +0.5\beta_6$ we have a zero near $hc \times -4 \, \text{cm}^{-1}$, where the vibrational level spacing is about $hc \times 0.25 \, \text{cm}^{-1}$ from Fig. 5(b).