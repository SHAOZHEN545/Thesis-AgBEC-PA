# Hyperfine structure of the $Na_2$ $0_g^-$ long-range molecular state

Carl J. Williams,$^*$ Eite Tiesinga,$^\dagger$ and Paul S. Julienne  
Atomic Physics Division, National Institute of Standards and Technology, Gaithersburg, Maryland 20899  
Received 13 December 1995

$^*$ Permanent address: James Franck Institute, University of Chicago, Chicago, IL 60637.  
$^\dagger$ Permanent address: Eindhoven University of Technology, 5600 M. B. Eindhoven, The Netherlands.
DOI: https://doi.org/10.1103/PhysRevA.53.R1939
## Abstract

We report a full theoretical calculation of the rovibrational structure of the $Na_2$ $0_g^-$ state, including hyperfine structure. The purely long-range $0_g^-$ state has been observed in the photoassociation spectroscopy of ultracold trapped alkali-metal atoms. For the lighter alkali-metal atoms (Li, Na, and K), the purely long-range states are completely characterized by atomic data since the inner turning point of the potentials are at internuclear separations where exchange interactions are still negligible.

PACS number(s): 33.20.Wr, 2.70.Hm, 33.15.Pw, 34.20.Cf

Experimental development of ultracold samples of laser-cooled atoms provides access to a whole new regime of atomic collision physics [1,2]. This has led to a plethora of new types of experimental phenomena including high precision photoassociation spectroscopy [3–7] and the recent achievement of Bose-Einstein condensation in spin aligned alkali-metal atoms [8–10]. Photoassociation spectroscopy is complementary to standard bound-bound spectroscopy since the Franck-Condon factors between two colliding ultracold atoms strongly favor excitation of bound vibrational levels near an excited-state dissociation limit, in sharp contrast to the more deeply bound vibrational levels populated in most bound-bound spectroscopy. In combination with standard bound-bound spectroscopy, photoassociation spectroscopy can be used to directly measure the dissociation energy, $D_0$, of a diatomic molecule [11].

This paper presents a theoretical analysis of the vibrational, rotational, and hyperfine structure of the excited diatomic molecule produced in photoassociation spectroscopy, while ignoring the details of the initial ground-state collision and the optical excitation process. More specifically, we present a general theoretical and numerical framework for calculating the bound states of diatomic molecules, including hyperfine and rotational interactions. The methodology is applicable to finding bound vibrational levels for all electronic states correlating to two $S$-state atoms or one $S$-state and one $P$-state atom. The method is most appropriate near dissociation where several electronic states may be coupled together and the density of rovibrational levels is high. Here we present theoretical calculations relevant to the $Na_2$ $0_g^-$ photoassociation spectrum.

We examine the purely long-range $0_g^-$ state for $Na_2$ [4,12] since this state is completely characterized by atomic data. The $Na_2$ $0_g^-$ state, see Fig. 1, has an inner turning point of $55a_0$ ($a_0=0.0529$ nm), a well depth of 58 GHz, and an equilibrium internuclear separation of $71a_0$. By understanding the detailed nature of the $0_g^-$ state and the degree to which multichannel nonadiabatic interactions are important we plan on extracting a high precision Na lifetime from the experimental data [13]. In addition, a treatment of the intensities and line shapes of the $0_g^-$ and $A\,{}^1\Sigma_u^+$ state should allow for the extraction of Na $X\,{}^1\Sigma_g^+$ and $a\,{}^3\Sigma_u^+$ ground-state scattering lengths.

In order to obtain the exact rovibrational states of the $Na_2$ $0_g^-$ state we set up the full Hamiltonian $\mathcal{H}$ for all electronic states that correlate to the $Na(3\,{}^2P)+Na(3\,{}^2S)$ atomic limit. This Hamiltonian includes all internal electronic and nuclear spin degrees of freedom and the mechanical rotation of the molecule. A different $\mathcal{H}$ is constructed for each total parity $p$ and each value of the total angular momentum $F$, where $F=L+S+I+\ell$. $L$, $S$, $I$, and $\ell$ are the electronic orbital, the electronic spin, the nuclear spin, and the rotational angular momentum of the atoms, respectively. The total parity is the symmetry under inversion of all coordinates, both electronic and nuclear.

It is important to set up the full close-coupled $\mathcal{H}$ for the system since hyperfine, spin-orbit, spin-spin dipole, and Coriolis interactions can couple the eight adiabatic Born-Oppenheimer (ABO) potentials that correlate to the $Na(3\,{}^2P)+Na(3\,{}^2S)$ atomic limit. The eight ABO potentials (see inset of Fig. 1) are the $A\,{}^1\Sigma_u^+$, $1\,{}^3\Sigma_g^+$, $1\,{}^1\Pi_g$, $b\,{}^3\Pi_u$, $2\,{}^1\Sigma_g^+$, $2\,{}^3\Sigma_u^+$, $B\,{}^1\Pi_u$, and $1\,{}^3\Pi_g$ states.

> [!figure]
> ![[Fig. 1.png|center|500]]
> **Figure 1.** The adiabatic $Na_2$ curves. The inset shows the eight ABO curves.

To a first approximation, the purely long-range $0_g^-$ state results from the spin-orbit avoided crossing of the attractive ${}^3\Sigma_{0g}^+$, which correlates with the $Na(3\,{}^2P_{3/2})+Na(3\,{}^2S)$ limit, and the repulsive ${}^3\Pi_{0g}$, which correlates with the $Na(3\,{}^2P_{1/2})+Na(3\,{}^2S)$ limit. Note that Fig. 1 shows only the $Na(3\,{}^2P_{3/2})+Na(3\,{}^2S)$ limit, the $P_{1/2}$ limit being 515 GHz lower in energy. Coriolis and hyperfine interactions allow the purely long-range state to mix with states of different electronic symmetry. Moreover, the $0_g^-$ state has hyperfine structure only as a result of this mixing. This mixing becomes increasingly important as the bound rovibrational levels approach dissociation. Below we briefly describe the numerical methods used to obtain the eigenvalues of the full Hamiltonian, before explaining various approximate treatments of the same Hamiltonian.

Solving for the eigenvalues of this system presents several numerical challenges. The Hamiltonian $\mathcal{H}$ is dominated by the resonant-dipole interaction at large internuclear separations and by the strong chemical bonding represented by the ABO potentials at short internuclear separations. Therefore, it is necessary to construct a basis set or discrete variable representation with reasonable dimensionality that can support both the fast oscillations of the nuclear wave function in the chemical bonding region and the long-wavelength oscillations present in the resonant dipole region. The latter region extends out beyond $300a_0$. Note that, although the $0_g^-$ vibrational wave functions lie solely at large internuclear separations, where the total binding energy is never more than 58 GHz, it is essential to span short internuclear separations as well, since mixing of the $0_g^-$ rovibrational states with rovibrational levels of different electronic symmetry is crucial to understanding the rovibrational levels nearest dissociation.

Ultimately this leads to a very large eigenvalue problem with dimension given by the product of the number of basis functions or radial collocation points times the total spin degeneracy of the system; i.e., the total number of ways that the electronic orbital, spin, nuclear, and mechanical angular momenta can couple to form a state of good total angular momentum $F$ and parity $p$. This latter turns out to be 96 for ${}^{23}Na_2$, ${}^{7}Li_2$, ${}^{39}K_2$, and ${}^{87}Rb_2$.

In view of these considerations it is essential to find as an efficient representation of $\mathcal{H}$ as possible. We achieve this in two steps: first, we introduce a nonlinear coordinate transformation that changes the imbalance in potential and kinetic energy between short and large $R$. That is, the wave function in the transformed space is made to have less variation in its local de Broglie wavelength since the potential in this new space looks more like a “square well.” Coordinate transformations in general introduce first-order derivatives in the kinetic-energy operator. However, the use of an appropriate transformation on the wave function will insure that this derivative disappears. The resulting equivalent differential equation in this transformed space and for the transformed wave function contains only second derivatives. The newly transformed kinetic operator is then discretized using a Fourier-grid discrete variable representation [14]. Thus, the kinetic-energy operator is represented as an analytical matrix on a nonuniform grid in $R$ space, while the rest of the $\mathcal{H}$ is diagonal in coordinate space. Alternative schemes for representing the kinetic-energy operator in this transformed space could use distributed approximating functions [15]. The coordinate transformation leads to a number of grid points equal to twice the number of vibrational levels supported by the deepest ABO potential. For the $Na_2$, this yields 400 points and the total dimension of $\mathcal{H}$ is roughly $40000\times 40000$.

Direct eigenvalue solvers require memory to store the complete matrix. The requirements for $Na_2$ put this well out of reach of most present day computers. In order to solve the resulting eigenvalue problem it is essential to use iterative methods and to take optimal advantage of the block diagonal structure of the kinetic and potential portions of $\mathcal{H}$ [16]. Finding eigenvalues near the dissociation limit, however, requires looking for levels in the middle of the spectral representation of $\mathcal{H}$. Additionally, because of the long-range $1/R^3$ resonant dipole interaction the density of states increases dramatically near the dissociation limit; in fact, the vibrational spacing goes as $(v_D-v)^5$ where $v_D$ is the vibrational defect at dissociation [17].

The high density of states introduces two problems. First, it forces us to recast our problem since iterative methods typically converge most rapidly when the requested eigenvalues lie on the edges of the spectrum. Therefore following [18], we calculate the eigenvalues of $G=(\mathcal{E}-\mathcal{H})^{-1}$ that have the largest magnitude, where $\mathcal{E}$, the energy, is chosen to be near the levels of interest. We now obtain eigenvalues and eigenvectors by solving the equation $(\mathcal{E}-\mathcal{H})x=\phi$ for a given initial vector $\phi$, using the general minimum residual program GMRES [19]. This now presents the second problem, which is that GMRES will not converge for the highest bound vibrational levels without preconditioning $(\mathcal{E}-\mathcal{H})$. Preconditioning is obtained by ignoring the hyperfine interaction and including the mechanical rotation via an effective-centrifugal energy. This breaks up the full $\mathcal{H}$ into subspaces with definite Hund’s case (c) symmetry. These Hund’s case (c) subspace Hamiltonians are essentially the Movre-Pichler Hamiltonians [20]. Solving for all eigenvalues and eigenfunctions of the approximate Hund’s case (c) Hamiltonian $\mathcal{H}_0$, the preconditioner $G_0=1/(\mathcal{E}-\mathcal{H}_0)$ is evaluated and used to speed up convergence of the GMRES.

For homonuclear diatomic molecules, Bose statistics under interchange of the two identical atoms requires that $(-1)^{\sigma+\ell+I}p_a p_b=1$, where $\sigma=0$ (1) for $g$ ($u$) respectively, $p_a$ is the parity of atom $a$, and the total parity $p$ is given by $(-1)^\ell p_a p_b$. By virtue of the zero projection of $\mathbf{J}=\mathbf{F}-\mathbf{I}$ on the internuclear axis, the $0_g^-$ state is only weakly affected by the hyperfine interaction. Moreover, as long as $J$ remains approximately good, the correlation even $J$, even $\ell$ (or equivalently even $J$, odd $I$) is valid as well. The rigorous conservation of total angular momentum $F$ and parity $p$ results in four distinct forms for the approximate $0_g^-$ Hamiltonians (see Table I). The rovibrational levels of the purely long-range $0_g^-$ state are well characterized by $J$ and their $0_g^-$ parentage to within 8 GHz of dissociation. Note that this does not hold true for $1_g$ and $0_u^+$ states in this same region.

**Table I.** Structure of the four $0_g^-$ Hamiltonians.

| Parity | Even $F$ | Odd $F$ | Degeneracy |
|---|---|---|---|
| $+$ | $J=\{F-1, F+1\}$ | $J=\{F-2, F\ (2\times), F+2\}$ | 6<br>(even $I$) |
| $-$ | $J=\{F-2, F\ (2\times), F+2\}$ | $J=\{F-3, F-1\ (2\times), F+1\ (2\times), F+3\}$ | 10<br>(odd $I$) |

In Fig. 2 we present all rotational levels up to $J=4$ ($F=7$, $p=-1$, and $F=5$, $p=+1$) for selected $v$’s. The calculations clearly show that for $v=0$, $J$ is an excellent quantum number. $J$ remains an approximately good quantum number at $v=6$ and even at $v=11$. Although the rotational structure is basically unobservable for $v=11$, the hyperfine splitting for a given parity (and thus for even or odd $J$’s) remains smaller than the separation between adjacent even and odd $J$ levels. Clearly, the hyperfine splitting has grown with increasing $v$ while simultaneously lifting the $J$ degeneracy. For $v=15$, the spectrum has become complex, and $J$ is no longer a good quantum number. Moreover, some of the $0_g^-$ rotational levels observed for lower values of $v$ no longer have sufficient $0_g^-$ character to be tracked. These levels have become mixed with other nearly degenerate rovibrational levels of different Hund’s case (c) symmetry.

> [!figure]
> ![[Fig. 2.png|center|500]]
> **Figure 2.** Hyperfine structure of the $0_g^-$ state for selected $v$’s and $J=0$–4.

In Table II we present the $J=1$ and 2 eigenvalues for $F=1$, $p=+1$ ($-1$), respectively. In addition, we present several approximate calculations that provide insight into the nature of the $0_g^-$ rovibrational levels. The $0_g^-$ subspace calculations involve a ${}^3\Pi_{0g}$ and ${}^3\Sigma_{0g}^+$ state of identical $J$ and $I$, but which are uncoupled from the other $0_g^-$ states of the same $F$ and $p$ with different $J$ and/or $I$. The subspace calculations are “essentially” the Movre-Pichler Hamiltonian [20] with the inclusion of the correct rotational potential. The $0_g^-$ subspace calculations for two rovibrational levels with the same $J$ but different $I$ give eigenvalues that are identical to within 1 MHz. The eigenvalues obtained from the subspace are used for preconditioning $G_0$ used in the exact eigenvalue calculation. It is interesting to note that, although the $0_g^-$ subspace calculations produce nearly identical eigenvalues for a given $v$ and $J$, the difference between the exact eigenvalues for the same $J$ but different $I$ varies from 3 MHz for $v=0$ to 40 MHz for $v=11$, $J=1$.

**Table II.** Energy levels of $F=1$, $p=\pm1$ for selected $v$’s. The approximations are discussed in the text. The energies and energy differences are given in MHz. The exact energies are given with respect to the ${}^2P_{3/2}(f_a=3)+{}^2S(f_b=2)$ asymptote.

| $v$ | $J$ | Exact energy | $\Delta E=E^{\mathrm{approx}}-E^{\mathrm{Exact}}$: $0_g^-$ subspace | $\Delta E=E^{\mathrm{approx}}-E^{\mathrm{Exact}}$: van Vleck | $\Delta E=E^{\mathrm{approx}}-E^{\mathrm{Exact}}$: Adiabatic$^a$ |
|---:|---:|---:|---:|---:|---:|
| 0 | 1 | -54041.1 | -4.8 | 0.5 | 0.6 |
| 0 | 1 | -54038.1 | -3.0 | -0.5 | 1.3 |
| 0 | 2 | -53917.9 | -3.1 | -0.0 | 1.2 |
| 0 | 2 | -53915.2 | -4.3 | -0.1 | 0.5 |
| 6 | 1 | -22198.2 | -1.4 | 2.3 | -1.0 |
| 6 | 1 | -22183.9 | -14.9 | -2.3 | -0.5 |
| 6 | 2 | -22111.3 | -10.1 | -0.1 | -0.2 |
| 6 | 2 | -22099.4 | -21.3 | -0.7 | -1.0 |
| 11 | 1 | -9147.4 | -5.1 | 7.1 | -2.2 |
| 11 | 1 | -9107.9 | -43.7 | -3.8 | -0.2 |
| 11 | 2 | -9073.1 | -32.2 | -1.7 | 1.7 |
| 11 | 2 | -9044.7 | -59.9 | 1.5 | 3.1 |

$^a$ $\Delta E$ adiabatic includes the diagonal nonadiabatic correction.

By performing additional calculations in which the $0_g^-$ subspace is allowed to couple to the $1_g$ or $0_u^+$ subspaces, we know that the primary contributions to shifting the $0_g^-$ rovibrational levels are second-order Coriolis interactions (i.e., $\boldsymbol{\ell}\cdot\mathbf{J}$) with the molecular $1_g$ states or via hyperfine interactions (i.e., $\mathbf{S}\cdot\mathbf{I}$) with the $0_u^+$ state. Moreover, the calculations suggest that the majority of the shift of the $0_g^-$ rovibrational levels can be interpreted as the sum of that from the $1_g$ state and $0_u^+$ state, but if higher accuracy is required it is necessary to include interactions to all other states.

In order to verify our understanding of the interactions between the $0_g^-$ subspace and the other subspaces we made a van Vleck type transformation of the full potential. Breaking the full potential of $Na_2$ (including hyperfine, spin-orbit, and diagonal and off-diagonal rotational interactions) as

$$
V=\begin{pmatrix} V_a & V_{ab} \\ V_{ba} & V_b \end{pmatrix},
\tag{1}
$$

we define the van Vleck potential for the subspace $a$ as

$$
V_a^{\mathrm{van\ Vleck}}(R)=V_a(R)+V_{ab}(R)\frac{1}{V_a(R)-V_b(R)}V_{ba}(R).
\tag{2}
$$

In Eq. (1), the individual components of $V$ are actual matrices and in the case of the $0_g^-$ state $V_a$ would include the full set of interactions between all ${}^3\Pi_{0g}$ and ${}^3\Sigma_{0g}^+$ states. Finding the eigenvalues of $\mathcal{H}_a^{\mathrm{van\ Vleck}}=T+V_a^{\mathrm{van\ Vleck}}$, where $T$ is the kinetic-energy operator, produces results that are in good agreement with the exact calculations. The van Vleck results do appear to worsen as $v$ increases.

A simpler approximation is found by using a fully adiabatic analysis of the $0_g^-$ state, including the diagonal nonadiabatic correction resulting from the spin-orbit avoided crossing of the ${}^3\Pi_{0g}$ and ${}^3\Sigma_{0g}^+$ states. The fully adiabatic analysis is accomplished by diagonalizing the full interaction potential at each $R$. At short internuclear separations we follow states of a given Hund’s case (a) symmetry, while at large internuclear separations we follow the states adiabatically. In addition to the new adiabatic potentials we also include the diagonal nonadiabatic correction that results from the $R$-dependent nature of the diagonalizations [21]. The benefit of the latter calculations is that once the full potential matrix has been diagonalized for the system, the eigenvalues are obtained from a single adiabatic potential. The results presented in Table II show that the adiabatic calculations with diagonal nonadiabatic corrections produce results that are in excellent agreement with the exact calculations. The adiabatic results appear to provide good approximations for even the highest vibrational levels. It is currently unclear why the adiabatic calculations perform so well.

In conclusion, we have shown that we can obtain exact eigenvalues for the full Hamiltonian, including hyperfine structure, of an alkali-metal dimer dissociating to a ground and excited alkali-metal atom. This will permit us to synthesize photoassociation spectra that can be compared with experimental data. This will be accomplished by calculating the matrix element between the close-coupled wave function of two colliding ultracold ground-state atoms that are optically coupled to the multichannel bound states described herein. Work in this area along with the calculation of bound states of other Hund’s case symmetries is in progress.

## Acknowledgments

We acknowledge support from the U.S. Army Research Office and the Office of Naval Research. C.J.W. would also like to acknowledge partial support of the National Science Foundation through Grant No. PHY92-23853 and through a grant for the Institute for Theoretical Atomic and Molecular Physics at Harvard University and the Smithsonian Astrophysical Observatory.

## References

[1] P.D. Lett, P.S. Julienne, and W.D. Phillips, Ann. Rev. Phys. Chem. 46, 423 (1995).

[2] J. Weiner, Adv. At. Mol. Opt. Phys. 35, 45 (1995).

[3] W.I. Alexander, E.R.I. Abraham, N.W.M. Ritchie, C.J. Williams, H.T.C. Stoof, and R.G. Hulet, Phys. Rev. A 51, R871 (1995).

[4] L.P. Ratliff, M.E. Wagshul, P.D. Lett, S.L. Rolston, and W.D. Phillips, J. Chem. Phys. 101, 2638 (1994).

[5] P.D. Lett, K. Helmerson, W.D. Phillips, L.P. Ratliff, S.L. Rolston, and M.E. Wagshul, Phys. Rev. Lett. 71, 2200 (1993).

[6] H. Wang, P.L. Gould, and W.C. Stwalley, Phys. Rev. A 53, R1216 (1996).

[7] R.A. Cline, J.D. Miller, and D.J. Heinzen, Phys. Rev. Lett. 73, 632 (1994); 71, 2204 (1993).

[8] M.H. Anderson, J.R. Ensher, M.R. Matthews, C.E. Weiman, and E.A. Cornell, Science 269, 198 (1995).

[9] C. Bradley, C. Sackett, J. Tollett, and R. Hulet, Phys. Rev. Lett. 75, 9 (1995).

[10] K.B. Davis, M.-O. Mewes, M.R. Andrews, N.J. Van Druten, D.S. Durfee, D.M. Kurn, and W. Ketterle, Phys. Rev. Lett. 75, 3969 (1995).

[11] S. Maleki, K.M. Jones, S. Bize, P.D. Lett, C.J. Williams, H. Richling, H. Knöckel, E. Tiemann, H. Wang, P.L. Gould, and W.C. Stwalley (unpublished).

[12] W.C. Stwalley, Y.H. Uang, and G. Pichler, Phys. Rev. Lett. 41, 1164 (1978).

[13] K.M. Jones, P.D. Lett, C.J. Williams, E. Tiesinga, P.S. Julienne, L.P. Ratliff, and W.D. Phillips (unpublished).

[14] D.T. Colbert and W.H. Miller, J. Chem. Phys. 96, 1982 (1992).

[15] Y. Huang, D.J. Kouri, M. Arnold, T.L. Marchioro II, and D.K. Hoffmann, Comput. Phys. Commun. 80, 1 (1994); J. Chem. Phys. 99, 1028 (1993).

[16] D. Sorenson, SIAM J. Matrix Anal. Appl. 13, 357 (1992); P. Pendergast, Z. Darakjian, E.F. Hayes, and D.C. Sorenson, J. Comput. Phys. 113, 201 (1994).

[17] R.J. LeRoy and R.B. Bernstein, J. Chem. Phys. 52, 3869 (1970).

[18] R. Wyatt, Phys. Rev. E 51, 3643 (1995).

[19] R. Barrett, M. Berry, T. Chan, J. Demmel, J. Donato, J. Dongarra, V. Eijkhout, R. Pozo, C. Romine, and H. van der Vorst, *Templates for the Solution of Linear Systems: Building Blocks for Iterative Methods* (Society for Industrial and Applied Mathematics, Philadelphia, 1994).

[20] M. Movre and G. Pichler, J. Phys. B 10, 2631 (1977).

[21] M.S. Child, *Molecular Collision Theory* (Academic Press, London, 1974), pp. 86–90.
