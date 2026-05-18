# Feshbach resonances in ultracold atomic and molecular collisions: threshold behaviour and suppression of poles in scattering lengths

**Author:** Jeremy M Hutson  
**Affiliation:** Department of Chemistry, University of Durham, South Road, Durham, DH1 3LE, UK  
**E-mail:** J.M.Hutson@durham.ac.uk  
**Journal:** New Journal of Physics 9 (2007) 152  
**Received:** 27 February 2007  
**Published:** 24 May 2007  
**Online:** http://www.njp.org/  
**DOI:** 10.1088/1367-2630/9/5/152

## Abstract

In the absence of inelastic scattering, Feshbach resonances produce poles in scattering lengths and very large peaks in elastic cross-sections. However, inelastic scattering removes the poles. Whenever the resonant state is coupled comparably to the elastic and inelastic channels, the scattering length exhibits only a small oscillation and peaks in cross-sections are significantly suppressed. A resonant scattering length is defined to characterize the amplitude of the oscillation, and is shown to be small for many collisions of ultracold molecules. The results suggest that cross-sections for some ultracold collision processes will be much less sensitive to details of the potential than has been expected.

## 1. Introduction

A Feshbach resonance [1] occurs when a bound state of a two-particle system lies above a dissociation threshold and is coupled to the continuum. Collision properties show sharp features (peaks and troughs) near the energy of the resonance. In recent years, Feshbach resonances have come into prominence in the study of ultracold atomic gases. In these systems the positions of resonances can often be adjusted using applied magnetic fields, and it is possible to control the interactions between atoms by tuning resonances to near-zero collision energy [2]–[4]. Magnetic tuning through Feshbach resonances has been used to produce molecules in both bosonic and fermionic quantum gases. Long-lived molecular Bose–Einstein condensates of fermion dimers have been produced, and the first signatures of ultracold triatomic and tetraatomic molecules have been observed. The new capabilities in atomic physics have had important applications in other areas: for example, the tunability of atomic interactions has been used to explore the crossover between Bose–Einstein condensation (BEC) and Bardeen–Cooper–Schrieffer (BCS) behaviour in dilute gases. There is now great interest in extending the capabilities from ultracold atomic to molecular systems, to explore the properties of dipolar quantum gases and develop new forms of quantum control.

Most interpretations of Feshbach resonances have used concepts from the two-channel model [4], in which the bound state and the continuum are each represented by one scattering channel. This captures much of the crucial resonant behaviour observed in ultracold atom–atom scattering. In particular, it predicts that the scattering length passes through a pole and the elastic scattering cross-section exhibits a very large peak at a zero-energy resonance. However, it is known from early work on nuclear reactions [5] that inelastic processes suppress resonant peaks in cross-sections. The purpose of this paper is to explore the consequences of such effects for ultracold atomic and molecular collisions. Whenever the resonant state is coupled comparably to the incoming and inelastic channels, the scattering length exhibits only a small oscillation and the peaks in cross-sections are dramatically suppressed. This is particularly important for the prospect of controlling molecular collisions.

This paper will first summarize the results of two-channel resonance theory, to define notation and establish a basis for comparison. The major differences introduced by inelastic scattering will then be considered. The results are general, but to assist visualization the equations will be illustrated with examples taken from the elastic and inelastic scattering of NH molecules with He [6].

## 2. Resonances in the absence of inelastic scattering

When there is only a single open channel with orbital angular momentum $l$, the long-range wavefunction may be written

$$
\psi^\mathrm{open}(r) = N k^{-1/2} r^{-1} \sin[kr - l\pi/2 + \delta(k)],
\tag{1}
$$

where $\delta(k)$ is the phase shift and the wavevector $k$ is defined in terms of the kinetic energy $E_\mathrm{kin}$ and reduced mass $\mu$ by $E_\mathrm{kin} = \hbar^2 k^2/2\mu$. In the ultracold regime, cross-sections are dominated by s-wave scattering, with $l = 0$. The most important parameter is the energy-dependent s-wave scattering length $a(k)$, defined by

$$
a(k) = -\frac{\tan \delta(k)}{k}.
\tag{2}
$$

This becomes constant at limitingly low energy, with corrections given by effective range theory [7],

$$
a(k) = a(0) + \frac{1}{2} k^2 r_0 a(0)^2 + O(k^4),
\tag{3}
$$

where $r_0$ is the effective range. The elastic cross-section is given exactly in terms of $a(k)$ by

$$
\sigma_\mathrm{el}(k) = \frac{4\pi a^2}{1 + k^2a^2}.
\tag{4}
$$

For collisions of identical bosons, the factor of 4 is replaced by 8. However, the present work will omit such extra factors of 2.

If there is only one open channel, the behaviour of the phase shift $\delta$ is sufficient to characterize a resonance. It follows a Breit–Wigner form as a function of energy,

$$
\delta(E) = \delta_\mathrm{bg} + \tan^{-1}\left[\frac{\Gamma_E}{2(E_\mathrm{res} - E)}\right],
\tag{5}
$$

where $\delta_\mathrm{bg}$ is a slowly varying background term, $E_\mathrm{res}$ is the resonance position and $\Gamma_E$ is its width (in energy space). The phase shift thus increases sharply by $\pi$ across the width of the resonance. In general the parameters $\delta_\mathrm{bg}$, $E_\mathrm{res}$ and $\Gamma_E$ are weak functions of energy, but this is neglected in the present work apart from threshold behaviour.

As a function of magnetic field at constant $E_\mathrm{kin}$, the phase shift follows a form similar to equation 5,

$$
\delta(B) = \delta_\mathrm{bg} + \tan^{-1}\left[\frac{\Gamma_B}{2(B_\mathrm{res} - B)}\right],
\tag{6}
$$

where $B_\mathrm{res}$ is the field at which $E_\mathrm{res} = E = E_\mathrm{thresh} + E_\mathrm{kin}$. The width $\Gamma_B$ is a signed quantity given by $\Gamma_B = \Gamma_E/\Delta\mu$, where the magnetic moment difference $\Delta\mu$ is the rate at which the energy $E_\mathrm{thresh}$ of the open-channel threshold tunes with respect to the resonance energy,

$$
\Delta\mu = \frac{dE_\mathrm{thresh}}{dB} - \frac{dE_\mathrm{res}}{dB}.
\tag{7}
$$

$\Gamma_B$ is thus negative if the bound state tunes upwards through the energy of interest.

Across an elastic scattering resonance, the $S$-matrix element $S = e^{2i\delta}$ describes a circle of radius 1 in the complex plane as a function of either energy or magnetic field, as shown in the left panel of figure 1. In the ultracold regime, the background phase shift $\delta_\mathrm{bg}$ goes to zero as $k \to 0$ according to equation 2 (with $a_\mathrm{bg}$ constant and finite), but the resonant term still exists. The scattering length passes through a pole when $\delta = (n + \frac{1}{2})\pi$, corresponding to $S = -1$. The scattering length follows the formula [8],

$$
a(B) = a_\mathrm{bg}\left(1 - \frac{\Delta_B}{B - B_\mathrm{res}}\right).
\tag{8}
$$

The elastic cross-section given by equation (4) thus shows a sharp peak of height $4\pi/k^2$ at resonance. The two widths $\Gamma_B$ and $\Delta_B$ are related by

$$
\Gamma_B = -2a_\mathrm{bg}k\Delta_B.
\tag{9}
$$

At limitingly low energy, $\Gamma_B$ is proportional to $k$ [2] while $\Delta_B$ is constant.

> [!figure]
> ![[Fig. 1.png|center|500]]
> **Figure 1.** The resonant circles described by $S$ matrix elements for low-energy elastic scattering for two different resonances in He + NH ($^3\Sigma^-$). Left-hand panel: the circle of radius 1 when only elastic scattering is allowed: incoming channel $n = 0$, $m_s = -1$ at $E_\mathrm{kin} = 10^{-6}$ K. Right-hand panel: the much smaller circles (note the different scale) when both elastic and inelastic scattering are allowed: incoming channel $n = 0$, $m_s = 0$ at $E_\mathrm{kin} = 10^{-6}$ K (green, smaller circle) and $4 \times 10^{-6}$ K (red, larger circle). The crosses show values far from resonance. In both cases the resonant state has $n = 0$, $m_s = +1$.

## 3. Resonances in the presence of inelastic scattering

In the presence of inelastic collisions, the scattering matrix has elements $S_{ii'}$. The diagonal $S$-matrix element in the incoming channel 0 has magnitude $|S_{00}| \le 1$ and may be written in terms of a complex phase shift $\delta_0$ with a positive imaginary part [9],

$$
S_{00}(k_0) = e^{2i\delta_0(k_0)},
\tag{10}
$$

where $k_0$ is the wavevector in the incoming channel. This can be expressed in terms of a complex energy-dependent scattering length, $a(k_0) = \alpha(k_0) - i\beta(k_0)$ [10, 11], defined by analogy with equation (2) as

$$
a(k_0) = -\frac{\tan \delta_0(k_0)}{k_0} = \frac{1}{ik_0}\left(\frac{1 - S_{00}(k_0)}{1 + S_{00}(k_0)}\right).
\tag{11}
$$

$a(k_0)$ again becomes constant at limitingly low energy. The elastic and total inelastic cross-sections are exactly [12]

$$
\sigma_\mathrm{el}(k_0) = \frac{4\pi |a|^2}{1 + k_0^2|a|^2 + 2k_0\beta}
\tag{12}
$$

and

$$
\sigma_\mathrm{inel}^\mathrm{tot}(k_0) = \frac{4\pi\beta}{k_0(1 + k_0^2|a|^2 + 2k_0\beta)}.
\tag{13}
$$

When there are several open channels, the quantity that follows the Breit–Wigner form (5) or (6) is the $S$-matrix eigenphase sum [13, 14], which is the sum of phase shifts obtained from the eigenvalues of the $S$-matrix. The eigenphases and the eigenphase sum are real, unlike the phases $\delta_i$ obtained from individual diagonal elements, because the $S$-matrix is unitary, so that all its eigenvalues have modulus 1.

Across a resonance, the individual $S$-matrix elements describe circles in the complex plane [15, 16],

$$
S_{ii'}(E) = S_{\mathrm{bg},ii'} - \frac{i g_{Ei} g_{Ei'}}{E - E_\mathrm{res} + i\Gamma_E/2},
\tag{14}
$$

where $g_{Ei}$ is complex. The radius of the circle in $S_{ii'}$ is $|g_{Ei}g_{Ei'}|/\Gamma_E$. The partial width for channel $i$ is usually defined as a real quantity, $\Gamma_{Ei} = |g_{Ei}|^2$, but here we also need a corresponding phase $\phi_i$ to describe the direction of the circle in the complex plane, $g_{Ei}^2 = \Gamma_{Ei}e^{2i\phi_i}$. For a narrow resonance, the total width is just the sum of the partial widths,

$$
\Gamma_E = \sum_i \Gamma_{Ei}.
\tag{15}
$$

As a function of magnetic field at constant $E_\mathrm{kin}$,

$$
S_{ii'}(B) = S_{\mathrm{bg},ii'} - \frac{i g_{Bi} g_{Bi'}}{B - B_\mathrm{res} + i\Gamma_B/2},
\tag{16}
$$

where $g_{Bi} = g_{Ei}/\Delta\mu^{1/2}$ and the width $\Gamma_B$ and partial widths $\Gamma_{Bi}$ are signed quantities, $\Gamma_B = \Gamma_E/\Delta\mu$ and $\Gamma_{Bi} = \Gamma_{Ei}/\Delta\mu$.

The partial widths for elastic channels (degenerate with the incoming channel) are proportional to $k_0$ at low energy. We may define a reduced partial width $\gamma_{E0}$ or $\gamma_{B0}$ for the incoming channel by

$$
\Gamma_{E0}(k_0) = 2k_0\gamma_{E0} \quad \text{or} \quad \Gamma_{B0}(k_0) = 2k_0\gamma_{B0},
\tag{17}
$$

and the reduced widths are independent of $k_0$ at low energy. By contrast, the partial widths for inelastic channels depend on open-channel wavefunctions with large wavevectors $k_i$ and are effectively independent of $k_0$ in the ultracold regime. If the inelastic partial widths $\Gamma_{Ei}$ (or $\Gamma_{Bi}$) are nonzero, they eventually dominate $\Gamma_{E0}$ (or $\Gamma_{B0}$) as $k_0$ decreases. The radius of the circle (16) described by $S_{00}$ thus drops linearly to zero as $k_0$ decreases, as shown in the right-hand panel of figure 1. This is qualitatively different from the behaviour in the absence of inelastic channels.

As a function of magnetic field, the scattering length passes through a pole only if $\delta_0$ passes through $(n + \frac{1}{2})\pi$, corresponding to $S_{00} = -1$. If there is any inelastic scattering, $|\Gamma_{B0}| < |\Gamma_B|$ and this does not occur. When the circle in $S_{00}$ is small, the phase shift $\delta_0$ and the scattering length $a$ show only small peaks or oscillations across a resonance.

The expression (12) for the elastic scattering cross-section saturates at a value $\sigma_\mathrm{el} \approx 4\pi/k_0^2$ when $|a| \gg k_0^{-1}$. Such values of $|a|$ occur only when $|\delta_0 - (n + \frac{1}{2})\pi| \ll 1$ and thus when $\Gamma_B$ is strongly dominated by $\Gamma_{B0}$. Since $\Gamma_{B0}$ is proportional to $k_0$ and the inelastic contributions $\Gamma_{Bi}$ are independent of $k_0$, there is a lower bound on the value of $k_0$ at which this occurs. Denoting the sum of inelastic contributions to $\Gamma_B$ as $\Gamma_B^\mathrm{inel}$, this is given by

$$
|\Gamma_B^\mathrm{inel}| \ll |\Gamma_{B0}| = 2k_0|\gamma_{B0}|,
\tag{18}
$$

$$
k_0 \gg \frac{\Gamma_B^\mathrm{inel}}{2\gamma_{B0}}.
\tag{19}
$$

The radius of the circle in $S_{00}$ is $\Gamma_{B0}/\Gamma_B$. For small $k_0$, where equation (17) applies, this is approximately $2k_0\gamma_{B0}/\Gamma_B^\mathrm{inel}$. The formula followed by the complex scattering length is

$$
a(B) = a_\mathrm{bg} + \frac{a_\mathrm{res}}{2(B - B_\mathrm{res})/\Gamma_B^\mathrm{inel} + i},
\tag{20}
$$

where $a_\mathrm{res}$ is a resonant scattering length that characterizes the strength of the resonance,

$$
a_\mathrm{res} = \frac{2\gamma_{B0}}{\Gamma_B^\mathrm{inel}}e^{2i(\phi_0 + k_0\alpha_\mathrm{bg})}.
\tag{21}
$$

Both $a_\mathrm{res}$ and the background term $a_\mathrm{bg}$ can in general be complex and are independent of $k_0$ at low energy. The phase correction $+2k_0\alpha_\mathrm{bg}$ in equation (21) is needed to keep the phase of $a_\mathrm{res}$ independent of $k_0$. The explicit expressions for the real and imaginary parts of $a(B)$ are

$$
\alpha(B) = \alpha_\mathrm{bg} + \frac{\alpha_\mathrm{res}[2(B - B_\mathrm{res})/\Gamma_B^\mathrm{inel}] + \beta_\mathrm{res}}{[2(B - B_\mathrm{res})/\Gamma_B^\mathrm{inel}]^2 + 1},
\tag{22}
$$

$$
\beta(B) = \beta_\mathrm{bg} + \frac{\alpha_\mathrm{res} + \beta_\mathrm{res}[2(B - B_\mathrm{res})/\Gamma_B^\mathrm{inel}]}{[2(B - B_\mathrm{res})/\Gamma_B^\mathrm{inel}]^2 + 1},
\tag{23}
$$

where $a(B) = \alpha(B) - i\beta(B)$ and similarly for $a_\mathrm{res}$ and $a_\mathrm{bg}$. The peak profiles for the elastic and total inelastic cross-sections are given by equations (12) and (13).

In the special case where the background scattering is elastic ($a_\mathrm{bg}$ is real), unitarity requires that the circle in $S_{00}$ must loop towards the origin. This requires that $a_\mathrm{res}$ is also real. Across the width of the resonance, the real part $\alpha(B)$ of the scattering length $a(B)$ then oscillates about $a_\mathrm{bg}$ by $\pm a_\mathrm{res}/2$ and the imaginary part peaks at $\beta(B) = a_\mathrm{res}$. When the background scattering is inelastic, however, $a_\mathrm{res}$ can be complex and the circle in $S_{00}$ does not point directly towards the origin. The lineshapes are then unsymmetrical, and $\beta(B)$ (and hence the inelastic rate) can show a trough as well as a peak. Nevertheless, the overall magnitude of the oscillations in the scattering length is still governed by $a_\mathrm{res}$.

The behaviour derived here is analogous to that observed when laser light is used to tune scattering lengths [10, 17]. However, in that case the amplitude of the oscillation depends on the ratio of excitation and spontaneous emission rates, which both depend on the same dipole strength (though the ratio of rates can be tuned with laser intensity). In the present case $a_\mathrm{res}$ depends on independent elastic and inelastic couplings. If $a_\mathrm{res}$ is small, the resonant oscillations in cross-sections and the scattering length are small.

The results (20) to (23) are valid when $k_0|a_\mathrm{res}| \ll 1$. Whenever $k_0|a_\mathrm{res}| \not\ll 1$, equation (8) fails at values of $|a|$ small enough to reduce the height of the peak in the elastic cross-section given by equation (12). Conversely, when $k_0|a_\mathrm{res}| \gg 1$, $S_{00}$ describes a circle of radius close to 1 in the complex plane; the behaviour of the scattering length is then well described by a two-channel model and the peak in the elastic cross-section is of height $\sim 4\pi/k_0^2$.

The elastic partial width $\Gamma_{B0}$ is proportional to $k_0$ at low energy but becomes constant at high energy. It may be written [18]

$$
\Gamma_{B0}(k_0) = \bar{\Gamma}_{B0}C_0(k_0)^{-2},
\tag{24}
$$

where $\bar{\Gamma}_{B0}$ is independent of $k_0$ and depends on the short-range coupling between the bound state and the incoming channel. The factor $C_0(k_0)^{-2}$ is the amplitude matching function of multichannel quantum defect theory, which is 1 at high energy but near threshold is [18]

$$
C_0(k_0)^{-2} = k_0\bar{a}\left[1 + \left(1 - \frac{a_\mathrm{bg}}{\bar{a}}\right)^2\right],
\tag{25}
$$

where $\bar{a}$ is the mean scattering length [19] and $\bar{a} = 0.478(2\mu C_6/\hbar^2)^{1/4}$ for a van der Waals potential $-C_6/r^6$. The transition between the linear and constant regimes depends on $C_6$ and the reduced mass [20], but typically occurs around $E_\mathrm{kin}/k_B = 1$ mK.

The height of the peak (or size of the oscillation) in the total inelastic cross-section is proportional to $|a_\mathrm{res}|$. This in turn depends principally on the ratio of $\bar{\Gamma}_{B0}$ and $\Gamma_B^\mathrm{inel}$. Two very different cases may be distinguished. If the same coupling term connects the bound state to the incoming and inelastic channels, it is likely that $\bar{\Gamma}_{B0}$ and $\Gamma_B^\mathrm{inel}$ will be comparable. Under these circumstances $a_\mathrm{res}$ will be of the order of $\bar{a}$ and there will be relatively small oscillations in the scattering length. Conversely, if coupling to the inelastic (exoergic) channels is much weaker than coupling to the elastic channel, $a_\mathrm{res}$ will be large and the scattering length will exhibit a large oscillation resembling a pole.

It is important to realize that $a_\mathrm{res}$ (and thus the strength of the resonance) depends on the relative magnitudes of the couplings from the resonant state to the elastic and inelastic channels. This is not necessarily the same as saying that the degree of suppression depends on the strength of inelastic scattering.

The peaks in individual inelastic cross-sections can be rather larger than those in $\sigma_\mathrm{inel}^\mathrm{tot}$, because the radius of the circle in $S_{0i}$ is $(2k_0|a_\mathrm{res}|\Gamma_{Ei}/\Gamma_E^\mathrm{inel})^{1/2}$, which is considerably larger than $2k_0|a_\mathrm{res}|$ for small $k_0$.

## 4. Examples from low-energy atomic and molecular scattering

For atomic collisions, the couplings to inelastic channels are sometimes weak enough that a two-channel model remains accurate even when inelastic scattering is energetically allowed. For example, Donley et al [21] and Thompson et al [22] have produced $^{85}\mathrm{Rb}_2$ molecules by magnetic tuning in the vicinity of a Feshbach resonance between $(f, m_f) = (2, -2)$ states of $^{85}\mathrm{Rb}$ near 155 G. The $(2, -2)$ state is not the lowest in a magnetic field, and the molecules can decay by spontaneous spin relaxation to atomic levels with $f = 2$ and $m_f > -2$. The resonant state has $M_F = m_{f1} + m_{f2} = -4$, so this decay requires a change in $M_F$ and involves very weak magnetic dipole coupling. However, the coupling between the resonant state and the incoming channel (also $M_F = -4$) is through much stronger central terms in the potential. Köhler et al [23] have used coupled channel calculations including spin relaxation to characterize the resonance and obtained $a_\mathrm{bg} = -484.1\ a_0$ and $\Delta_B = 10.65$ G. Their lifetime $\tau = 32\ \mu\mathrm{s}$ for the bare resonance state corresponds to $\Gamma_B^\mathrm{inel} = \hbar/(\tau\Delta\mu) = 0.090$ G. With these parameters, $a_\mathrm{res} = 1.14 \times 10^5\ a_0$. The temperature in the experiments of Thompson et al [22] is 30 nK, corresponding to $k_0 = 4.3 \times 10^{-4}\ a_0^{-1}$. In this system, therefore, $k_0a_\mathrm{res} \approx 50$ and the resonant behaviour of the scattering length and the elastic cross-section is well approximated by a two-channel model.

The situation is very different for rotationally inelastic molecular scattering, where the potential anisotropy couples the resonant bound state to both the incoming and inelastic channels. Under these circumstances $a_\mathrm{res}$ will generally be small. In separate work, we have described numerical tests of the equations derived here for He + NH($^3\Sigma^-$) scattering in a magnetic field [6]. This is a very weakly coupled system, and for the rotational ground state ($n = 0$) of NH the channels with different spin projections $m_s$ are coupled only indirectly via excited rotational levels. The background scattering is essentially elastic, so $a_\mathrm{bg}$ and $a_\mathrm{res}$ are real. Figure 2 shows the real and imaginary parts of the scattering length for magnetic tuning across an inelastic scattering Feshbach resonance in this system. Even for He + NH, where the inelastic couplings are much weaker than in most other molecular systems, $a_\mathrm{res} \approx 9\ \text{Å}$ and $k_0a_\mathrm{res} \ll 1$. The oscillations in scattering lengths and elastic cross-sections are strongly suppressed at low energies.

> [!figure]
> ![[Fig. 2.png|center|500]]
> **Figure 2.** Real (red) and imaginary (green) parts of the scattering length for $^3\mathrm{He}$ + NH collisions in the vicinity of an inelastic Feshbach resonance at a kinetic energy of $10^{-6}$ K. The lines show the results of equation 20. This is the same resonance as shown in the right-hand panel of figure 1.

There are also atomic systems where the coupling to inelastic channels is strong enough to suppress the oscillations in scattering lengths. Such effects have been observed, for example, in calculations on collisions of Sr ($^2P_2$) atoms [24], where the bound state is coupled to both the incoming and inelastic channels by anisotropic potential terms.

Equations (20) to (23) can be adapted to apply to any parameter $\lambda$ that tunes scattering resonances across a threshold. The ratio $\Gamma_{\lambda0}/\Gamma_\lambda^\mathrm{inel}$ is the same for any such parameter (and is equal to $\Gamma_{E0}/\Gamma_E^\mathrm{inel}$). The resonant scattering length therefore has the same value for any parameter $\lambda$. $a_\mathrm{res}$ is a universal measure of the strength of a low-energy resonance, independent of the parameter used to tune it through a threshold.

This explains previously puzzling results obtained in low-energy reactive scattering. Quéméner et al [25] and Cvitaš et al [12] have investigated the sensitivity of scattering cross-sections in $\mathrm{Na} + \mathrm{Na}_2$ and $\mathrm{Li} + \mathrm{Li}_2$ to variations in the potential energy surface. Scaling the potential tunes reactive scattering resonances across threshold, and this produces oscillations in the elastic and inelastic cross-sections. In these systems the couplings to individual vibrationally inelastic channels are somewhat reduced by the large kinetic energy release, so that for low initial $v$ (with relatively few inelastic channels) some significant resonant peaks remain. For initial $v = 1$, the cross-sections oscillate by about a factor of 10 as resonances cross threshold. Even this corresponds to a relatively small oscillation in the complex scattering length (small $a_\mathrm{res}$). However, the amplitudes of the oscillations decrease substantially with increasing vibrational excitation of the colliding molecules and are almost smooth for $v = 3$ for both $\mathrm{Na} + \mathrm{Na}_2$ [25] and $\mathrm{Li} + \mathrm{Li}_2$ [12].

Quite different behaviour has been observed in $\mathrm{F} + \mathrm{H}_2$ reactions [26], but is also explained by the present theory. Bodo et al [26] investigated the effect of scaling the reduced mass and observed pole-like behaviour in the scattering length and large reactive cross-sections as a resonance was tuned across threshold. In this case the resonant state is localized in the entrance channel of the reaction, while the only exoergic channels are reactive ones that are separated from the entrance channel by a high barrier. $\Gamma_E^\mathrm{inel}$ is thus reduced relative to $\Gamma_{E0}$. Because of this, $a_\mathrm{res}$ is large ($>100\ \text{Å}$) and no strong suppression of the resonant peaks occurs.

The considerations of the present paper lead to a remarkable conclusion. It has been commonly believed that collision cross-sections in the ultracold regime are extremely sensitive to details of the potential energy surface, and that for molecules these dependences would be even more limiting than for atoms. The present paper has shown that this is true only when the resonant state is coupled much more weakly to inelastic (exoergic) channels than to the incoming channel. There are some systems where inelastic processes are weak enough for scattering lengths to reach near-infinite values at zero-energy resonances. However, in other cases inelastic processes will suppress this behaviour. In general terms, the resonant peaks are suppressed by inelastic scattering unless there is a specific mechanism that reduces the coupling to inelastic channels.

## Acknowledgments

I am grateful to Paul Julienne, Maykel Leonardo González-Martínez and Marko Cvitaš for comments on the paper.

## References

[1] Feshbach H 1958 *Ann. Phys.* **5** 357

[2] Timmermans E, Tommasini P, Hussein M and Kerman A 1999 *Phys. Rep.* **315** 199

[3] Hutson J M and Soldan P 2006 *Int. Rev. Phys. Chem.* **25** 497

[4] Köhler T, Goral K and Julienne P S 2006 *Rev. Mod. Phys.* **78** 1311

[5] Bethe H A and Placzek G 1937 *Phys. Rev.* **51** 450

[6] González-Martínez M L and Hutson J M 2007 *Phys. Rev. A* **75** 022702

[7] Hinckelmann O and Spruch L 1971 *Phys. Rev. A* **3** 642

[8] Moerdijk A J, Verhaar B J and Axelsson A 1995 *Phys. Rev. A* **51** 4852

[9] Mott N F and Massey H S W 1996 *The Theory of Atomic Collisions* 3rd edn (Oxford: Clarendon)

[10] Bohn J L and Julienne P S 1997 *Phys. Rev. A* **56** 1486

[11] Balakrishnan N, Kharchenko V, Forrey R C and Dalgarno A 1997 *Chem. Phys. Lett.* **280** 5

[12] Cvitaš M T, Soldán P, Hutson J M, Honvault P and Launay J-M 2007 *J. Chem. Phys.* at press (Preprint physics/0703136)

[13] Hazi A U 1979 *Phys. Rev. A* **19** 920

[14] Ashton C J, Child M S and Hutson J M 1983 *J. Chem. Phys.* **78** 4025

[15] Brenig W and Haag R 1959 *Fortschr. Phys.* **7** 183

[16] Taylor J R 1972 *Scattering Theory: The Quantum Theory of Nonrelativistic Collisions* (New York: Wiley)

[17] Fedichev P O, Kagan Y, Shlyapnikov G V and Walraven J T M 1996 *Phys. Rev. Lett.* **77** 2913

[18] Julienne P S and Gao B 2006 Simple theoretical models for resonant cold atom interactions *Atomic Physics 20 AIP Conf. Proc.* vol 869 ed C Roos, H Haffner and R Blatt (New York: AIP) pp 261–8 (Preprint physics/0609013)

[19] Gribakin G F and Flambaum V V 1993 *Phys. Rev. A* **48** 546

[20] Julienne P S and Mies F H 1989 *J. Opt. Soc. Am. B* **6** 2257

[21] Donley E A, Claussen N R, Thompson S T and Wieman C E 2002 *Nature* **417** 529

[22] Thompson S T, Hodby E and Wieman C E 2005 *Phys. Rev. Lett.* **94** 020401

[23] Köhler T, Tiesinga E and Julienne P S 2005 *Phys. Rev. Lett.* **94** 020402

[24] Kokoouline V, Santra R and Greene C H 2003 *Phys. Rev. Lett.* **90** 253201

[25] Quéméner G, Honvault P and Launay J-M 2004 *Eur. Phys. J. D* **30** 201

[26] Bodo E, Gianturco F A, Balakrishnan N and Dalgarno A 2004 *J. Phys. B: At. Mol. Opt. Phys.* **37** 3641
