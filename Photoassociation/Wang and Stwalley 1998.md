https://pubs.aip.org/aip/jcp/article-abstract/108/14/5767/182343/Ultracold-photoassociative-spectroscopy-of?redirectedFrom=fulltext
## III. THE FREE-BOUND FRANCK-CONDON FACTORS

At large internuclear distance $R$, the ground-state potential curves $[V(R) = -C_6''/R^6]$ are much flatter than the excited ones for both homonuclear and heteronuclear alkali diatomic molecules $[V(R) = -C_3'/R^3$ for the former, and $V(R) = -C_6'/R^6$ with $C_6' \gg C_6''$ for the latter]. For example, the excited-state $C_6'$ of the KRb molecule is about 60 times larger than the ground-state $C_6''$. Therefore, the Franck–Condon factors of the free-bound transitions are mainly determined by the slow-changing ground-state wave function only

$$
F_{v,J;E,J}(R) = |\langle \chi_{v,J}(R) | \chi_{E,J}(R) \rangle|^2\approx \frac{dE_v}{dv} \frac{1}{d_v} |\chi_{E,J}(R_{v+})|^2,
$$

where $\chi_{v,J}(R)$ and $\chi_{E,J}(R)$ are the bound and free radial wave functions, respectively, $E_v$ the excited vibrational level energy, $R_{v+}$ the classical outer turning point of the excited level $v$, and $d_v$ the difference in slopes between the ground and the excited potential curves at $R = R_{v+}$. At very large $R$, ignoring rotation, the interaction potential and the vibrational spacing can be expressed as

$$
V(R) = D - \frac{C_n'}{R^n} \quad \text{or} \quad E_v = D - \frac{C_n'}{R_{v+}^n}
$$

and

$$
\frac{dE_v}{dv} = K_n (D - E_v)^{(n+2)/2n} = K_n \left( \frac{C_n'}{R_{v+}^n} \right)^{(n+2)/2n}
$$

where

$$
K_n = \hbar \left( \frac{2\pi}{\mu} \right)^{1/2} \frac{\Gamma(1 + 1/n)}{\Gamma(1/2 + 1/n)} \frac{n}{(C_n')^{1/n}},
$$

and where $C'_n$ is the dominant long-range potential constant of the excited interaction, $D$ the dissociation energy, and $\mu$ the reduced mass. Since the excited long-range interactions are much stronger than the ground-state interactions, we have

$$
d_v = \left| \frac{d}{dR} [V'(R) - V''(R)] \right|_{R_{v+}}
$$

$$
\approx \left| \frac{d}{dR} V'(R) \right|_{R_{v+}} = \frac{nC'_n}{R_{v+}^{n+1}}, \tag{7}
$$

where $V'(R)$ and $V''(R)$ are the excited-state and the ground-state long-range potentials, respectively. Substituting Eqs. (5)–(7) into Eq. (3), we have the Franck–Condon factors for the heteronuclear free-bound transition ($n=6$) and the homonuclear transition ($n=3$)

$$
F_{v;E,J}(n=6) = (2\pi\hbar^2)^{1/2} \frac{\Gamma(7/6)}{\Gamma(2/3)}\times \mu^{-1/2} \left( \frac{C'_6}{R_{v+}^6} \right)^{-1/2} |\chi_{E,J}(R_{v+})|^2, \tag{8}
$$



$$
F_{v;E,J}(n=3) = (2\pi\hbar^2)^{1/2} \frac{\Gamma(4/3)}{\Gamma(5/6)} \times \mu^{-1/2} \left( \frac{C_3'}{R_v^3} \right)^{-1/2} |\chi_{E,J}(R_v)|^2. \tag{9}
$$

Equations (8) and (9) suggest that the heteronuclear molecules (with weak van der Waals excited-state potentials $C_6/R^6$) have more favorable Franck–Condon factors than the homonuclear ones (with much stronger resonant dipole–dipole potential $C_3/R^3$) at large internuclear distance. This is because the heteronuclear system has a smaller difference in slope between the ground and excited potentials than the homonuclear system.

At the ultracold temperatures ($T < 1$ mK), the ground-state $s$-wave wave function can be approximated at large $R$ as$^{24}$

$$
\chi_E(R) \approx e^{i\eta} \left( \frac{2\mu}{\pi\hbar^2 k_\infty} \right)^{1/2} k_\infty (R - a_s), \tag{10}
$$

where $a_s$ is the $s$-wave scattering length, $(2\mu/\pi\hbar^2 k_\infty)^{1/2}$ the energy normalization factor, and $k_\infty = (2\mu k_B T/\hbar^2)^{1/2}$ the thermal wave vector of the ground-state collision. $\eta = v_{\text{MAX}} \pi - k_\infty a_s$ is the asymptotic phase. This linear wave function extrapolates to an intercept near $R = a_s$. Using Eq. (10), the free-bound Franck–Condon factors, Eqs. (8) and (9), become

$$
F_{v;E}(n=6) = \frac{\Gamma(7/6)}{\Gamma(2/3)} \left( \frac{8\mu k_{\infty}^2}{\pi h^2} \right)^{1/2} (C_6')^{-1/2}\times R_v^5 \left( 1 - \frac{a_s}{R_v + } \right)^2, \tag{11}
$$


$$
F_{v;E}(n=3) = \frac{\Gamma(4/3)}{\Gamma(5/6)} \left( \frac{8\mu k_{\infty}^2}{\pi h^2} \right)^{1/2} (C_3')^{-1/2}\times R_v^{7/2} \left( 1 - \frac{a_s}{R_v + } \right)^2. \tag{12}
$$



Near $R = a_s$ ($a_s > 0$), the Franck–Condon factors go through zero, resulting in an intensity minimum in the photoassociation spectrum. Therefore, the excited-state spectral intensity distribution provides an accurate measurement of the ground-state scattering length. Equations (11) and (12) also show that at very large $R$, the Franck–Condon factors increase much faster as $R^5$ [Eq. (11)] for the heteronuclear molecules ($n = 6$) than as $R^{7/2}$ [Eq. (12)] for the homonuclear molecules ($n = 3$).

In order to express the Franck–Condon factors as a function of the vibrational quantum number $v$, we use

$$
D - E_v = X_0(n)(v_D - v)^{2n/(n-2)} = \frac{C_n'}{R_v^n}, \tag{13}
$$

and then

$$
R_v = \left[ \frac{C_n'}{X_0(n)} \right]^{1/n} (v_D - v)^{2/(2-n)}
$$

$$
= \left[ \frac{1}{X_0(n)} \right]^{1/n} (\mu C_n')^{1/(n-2)}(v_D - v)^{2/(2-n)}, \tag{14}
$$

where $X_0(n) = \overline X_0(n)[\mu^n(C_n')^2]^{1/(2-n)}$ and $\overline X_0(n)$ is a constant only depending on $n$. Therefore the heteronuclear Franck-Condon factor described by Eq. (11) becomes

$$
F_{v;E}(n=6) = \frac{\Gamma(7/6)}{\Gamma(2/3)} [\overline X_0(6)]^{-5/6} \left( \frac{8\mu^{7/2}k_\infty^2}{\pi\hbar^2} \right)^{1/2}
$$

$$
\times (C_6')^{3/4}(v_D - v)^{-5/2} \left( 1 - \frac{a_s}{R_v + } \right)^2. \tag{15}
$$

Equation (15) shows that for a given $v_D - v$, the long-range Franck–Condon factors for the heteronuclear photoassociation is proportional to $(C'_6)^{3/4}$, favoring these molecules which have larger $C'_6$ constants for their excited long-range states. Since $k_\infty \propto \mu^{1/2}$, the Franck–Condon factors also depend on the reduced mass of the molecule as a function of $\mu^{9/4}$, favoring the heavier species. Figure 4 shows the relative values (normalized to KRb) of the product of $[ \mu^{9/4}(C'_6)^{3/4} ]$ which determine the relative Franck–Condon factors for the different species at large $R$ ($R_{v+} \gg a_s$) and with the same $v_D - v$. The KRb system has long-range Franck–Condon factors more than a factor of 10 larger than the seven lighter species and a factor of 2 larger than KCs. The heaviest species, RbCs, has the largest value as seen in Fig. 4 due to its large mass. Since the scattering lengths for these heteronuclear collisions are not known, absolute values of the Franck–Condon factors cannot be estimated using the above analytical equations.

Substituting $n = 6$ in Eq. (14), we can obtain the classical outer turning points $R_{v+}$ as a function of the vibrational quantum number $v_D - v$ (long-range levels only) for the ten heteronuclear molecules. Note that $v_D$ is the effective vibrational quantum number at the dissociation limit (usually a noninteger) and varies for different states and different molecules. Therefore, $v_D - v$ counts the vibrational levels down from the dissociation limit. For example, $v_D - v$ has a value of $0 < v_D - v < 1$ for the last bound vibrational level $v_{\text{MAX}}$ and $4 < v_D - v < 5$ for the fifth level from the dissociation limit. Given $\overline X_0(6) = 7932.0$ (for energy in cm$^{-1}$, $R$ in Å, and $\mu$ in amu) from Ref. 25 and the long-range constants $C'_6$ ($\Sigma$ symmetry) from Ref. 23, we plot $R_{v+}$ as a function of $v_D - v$ for the last ten vibrational levels of the ten heteronuclear alkali-metal molecules in Fig. 5. The markers are at the half-integer on the vertical axis and indicate approximately where the outer turning points $R_{v+}$ are located on the horizontal axis (the actual $R_{v+}$ may vary in between the grid lines). As seen in Fig. 5, the KRb molecule has the largest range for the excited near-dissociation levels among the ten molecules due to its exceptionally large $C'_6$. The last bound vibrational level of KRb for the excited $S + P$ interaction has an outer turning point well beyond 100 Å while for the seven lighter molecules all the bound levels are crowded in much shorter range of $R$ and are not as easily probed by photoassociative spectroscopy.