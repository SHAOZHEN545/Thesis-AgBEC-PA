# Ultracold photoassociation spectroscopy: Long-range molecules and atomic scattering

**Authors:** Kevin M. Jones; Eite Tiesinga; Paul D. Lett; Paul S. Julienne

**Affiliations:**

- Physics Department, Williams College, 33 Lab Campus Drive, Williamstown, Massachusetts 01267, USA
- Atomic Physics Division, National Institute of Standards and Technology, 100 Bureau Drive, Stop 8424, Gaithersburg, Maryland 20899, USA

**Published:** 22 May 2006

**DOI:** 10.1103/RevModPhys.78.483

**PACS number(s):** 34.50.Rk, 39.25.+k, 39.30.+w

## Abstract

Photoassociation is the process in which two colliding atoms absorb a photon to form an excited molecule. The development of laser-cooling techniques for producing gases at ultracold (<1 mK) temperatures allows photoassociation spectroscopy to be performed with very high spectral resolution. Of particular interest is the investigation of molecular states whose properties can be related, with high precision, to the properties of their constituent atoms with the “complications” of chemical binding accounted for by a few parameters. These include bound long-range or purely long-range vibrational states in which two atoms spend most or all of their time at large internuclear separations. Low-energy atomic scattering states also share this characteristic. Photoassociation techniques have made important contributions to the study of all of these. This review describes what is special about photoassociation spectroscopy at ultracold temperatures, how it is performed, and a sampling of results including the determination of scattering lengths, their control via optical Feshbach resonances, precision determinations of atomic lifetimes from molecular spectra, limits on photoassociation rates in a Bose-Einstein condensate, and briefly, production of cold molecules. Discussions are illustrated with examples on alkali-metal atoms as well as other species. Progress in the field is already past the point where this review can be exhaustive, but an introduction is provided on the capabilities of photoassociation spectroscopy and the techniques presently in use.

## Contents

- I. Introduction
- II. Molecular States from an Atomic Viewpoint
- III. Cold Collisions and Free→Bound Spectra
- IV. Experimental Considerations
- V. Results on Singly Excited States
- VI. Doubly Excited States and Continua
- VII. Ground Electronic States
- VIII. Time-Resolved Photoassociation
- IX. Applications of Photoassociation Beyond Spectroscopy
- X. Prospects for Future Developments
  - A. What is photoassociation spectroscopy?
  - B. Photoassociation favors the study of “physicists’ molecules”
  - C. Photoassociation spectroscopy measures absolute binding energies
  - D. Photoassociation creates slowly rotating molecules
  - E. Photoassociation spectra yield information on atomic collisions
  - F. Photoassociation modifies atomic collisions
  - G. Photoassociation of cold atoms makes cold molecules
  - H. Photoassociation accesses a wide variety of molecular symmetries
  - I. Scope of this review
  - A. A few facts about alkali-metal atoms
  - B. Nonrelativistic atoms and diatoms
  - C. Long-range dispersion forces
  - D. Spin-orbit interaction
  - E. Movre-Pichler model
  - F. Mechanical rotation and Hund’s cases
  - G. Hyperfine interactions in ground electronic states
  - H. Hyperfine interactions in excited states
  - I. Selection rules
  - A. Length and energy scales for a van der Waals potential
  - B. Near-threshold wave functions and scattering properties
  - C. Theory of free→bound spectral line shapes
  - D. Approximate calculations of line strengths
  - A. Laser cooling and trapping
  - B. Detection techniques
  - A. A brief note on the early days of photoassociation
  - B. Measurement of the depth of a molecular potential
  - C. Broad spectral maps
  - D. Modeling of observed spectra
  - E. Purely long-range states
  - F. Determining Cn coefficients and atomic lifetimes
  - G. Mixed alkalis
  - H. Other atoms
  - I. Determining scattering lengths from nodes
  - A. Autler-Townes spectroscopy
  - B. Determining scattering lengths
  - C. Probing mean-field effects in a Bose condensate
  - D. Photoassociation in an optical lattice
  - A. Ground-state molecule production
  - B. PA rates in a BEC
  - C. PA as a monitor of magnetic-field-induced changes to the initial scattering state
  - D. PA as an optical Feshbach resonance
- Acknowledgments
- References

## I. Introduction

### A. What is photoassociation spectroscopy?

When a gas of atoms is illuminated with light of just the right frequency, two colliding atoms can absorb a photon and photoassociate to form a bound, electronically excited molecule:
$$
A + B + \gamma \to (AB)^* \tag{1}
$$
As shown in Fig. 1 this is a resonant process: viewed in the center-of-mass frame of the two colliding atoms, the sum of the initial kinetic energy of the atoms plus the energy of the absorbed photon must add up to the energy of the bound molecular state. In a typical experiment the molecule thus formed quickly decays by emitting a photon. Depending on the energy of the decay photon γd, the final product can be either two free atoms or a bound, ground electronic state molecule,
$$
(AB)^* \to A + B + \gamma_d \quad \text{or} \quad (AB)^* \to AB + \gamma_d \tag{2}
$$
The free atoms produced by the first process may have more or less kinetic energy than the initial colliding pair.

Stimulated decay, in which the energy, polarization, and direction of the decay photon are the same as the absorbed photon and thus the energy of the final atom pair is equal to that of the initial pair, is of particular interest as it raises the possibility of coherently modifying the collision between two atoms.

With the development of laser-cooling methods for producing ultracold—1 mK or less—atoms, photoassociation (hereafter PA) has become a high-resolution spectroscopy technique. For these very cold samples the spread in the initial kinetic energies of the colliding atoms is small and thus the spread in photon frequencies needed to drive the resonant PA process is small. In fact, this spread in frequencies can be comparable to, or smaller than, the natural linewidth of the electronically excited molecular state, set by the spontaneous emission processes of Eq. (2).

As an example, consider the PA of sodium atoms to molecular states using a laser tuned just red of the strongly allowed 3S→3P atomic resonance transition.

These molecular states typically have radiative lifetimes on the order of the atomic 3P radiative lifetime, which is ≈16 ns. Thus transitions to these states have a minimum linewidth, Γ=2π×10 MHz.

To achieve high resolution with PA spectroscopy, the temperature needs to be low enough that the spread in the initial kinetic energy of the colliding atoms, expressed in frequency units, is on the order of or less than Γ/(2π). Thus the required temperature T≲ ℏΓ/$k_B$, where $k_B$ is the Boltzmann constant, is ≈0.5 mK or less.

Such temperatures are easily reached by laser cooling for many atomic species. For these cold samples, free →bound PA transitions appear as sharply defined resonances, just like conventional bound→bound optical transitions observed in high-resolution Doppler-free spectroscopy of hot atoms or molecules. It is perfectly possible to observe PA at higher temperatures, but not with high spectral resolution (in the sense that we use the term). Some history of photoassociation and related diffuse band spectroscopy can be found in the articles of Pichler et al. (1983), Jones et al. (1993), and Schloss et al. (1993).

In the experiments we shall discuss, laser-cooled atoms are held in some kind of an atom trap, such as a magneto-optical trap (MOT) or a far-off-resonance optical trap (FORT). Introductory material on laser cooling and trapping may be found in the papers of Chu (1998), Cohen-Tannoudji (1998), Phillips (1998), and Metcalf and van der Straten (2003). The light which drives the PA process is typically supplied by a separate narrowfrequency, continuous-wave laser. In its simplest form, a PA spectrum measures the number of excited molecules produced as a function of the frequency of the applied light. One way to measure the number of molecules produced is to use a second laser to ionize some of these excited molecules and count the resulting molecular ions. Figure 2 shows a spectrum produced in this way starting with a sodium gas at 450 μK. At this temperature, the spectrum shows sharp lines with widths only slightly larger than the natural linewidth of the excited molecular level.

> [!figure]
> ![[Fig. 1.png|center|500]]
> **Figure 1.** A schematic of the photoassociation (PA) process A +B+γ→(AB)*. Two potential-energy curves are shown as a function of the internuclear separation of two atoms. The upward arrow labeled PA is the photoassociation transition, the downward dashed arrow labeled “decay” indicates radiative decay out of the excited molecular state. As drawn, the decay would produce two free atoms with higher energy than the initial collision. Transitions to lower or same energy atoms or to a bound-state molecule are also possible. For clarity the size of the incident thermal collision energy of the atom pair, Eth, is greatly exaggerated. Eat is the energy to excite one atom (here atom A) at infinite separation and Eb is the binding energy of the molecular vibrational level. For many purposes one can consider the PA transition as occurring at the outer turning point, Rv+, of the vibrational level of the excited molecular state.

In addition to the thermal broadening due to the spread in collision energies, there is also Doppler broadening due to the center-of-mass motion of the colliding pair of atoms. Depending on the radiative lifetime of the molecular states being studied, Doppler broadening may or may not be important in comparison to the natural linewidth. For alkali metals most PA spectroscopy is to short-lived states and Doppler broadening is a minor contribution to the observed linewidth. For PA with alkaline-earth atoms accessing molecular states just red of the so-called intercombination transition, Doppler broadening is the dominant contribution to the linewidth.

A skeptical reader will be forgiven for asking, “Isn’t photoassociation a rather hard way to do molecular spectroscopy—particularly for a molecule like $\mathrm{Na}_2$ which is readily produced simply by heating some sodium metal in a vacuum? Why bother?” In the rest of this Introduction we try to address that question by providing a brief overview of some of the features of PA spectroscopy which make it interesting, despite the relative complexity of the sample preparation step. In addition, we discuss some of the applications of PA beyond spectroscopy per se which have emerged as the field has developed.

### B. Photoassociation favors the study of “physicists’ molecules”

A significant part of the interest in ultracold PA spectroscopy has been the nature of the molecular states which are readily produced and studied using this technique. It is an obvious truism that the properties of a diatomic molecule are related to the properties of the two constituent atoms. However, the degree to which this atom ↔ molecule connection can be explicitly made in practice depends a great deal on the internuclear separation. At what we shall call short range, chemical bonding is important and atomic electron clouds are strongly distorted. At these small separations a description of the molecular wave function in terms of atomic orbitals necessarily requires a sum over many terms. In contrast, when the two constituent atoms are far apart the atomic electron clouds remain undistorted. Even in the absence of chemical bonding there are still nonnegligible electrostatic forces, such as van der Waals or dipole-dipole forces, between the atoms. The strength of these long-range forces is directly related to atomic properties alone. Other molecular properties, such as the spin orbit and hyperfine structure, are directly traceable to the atomic properties as well.

A vibrating diatomic molecule is often used as a textbook example of a quantum harmonic oscillator. For low levels of vibrational excitation this is true, but for higher levels the molecular vibration is highly anharmonic. The effective interatomic “spring” is very soft at large internuclear separation and thus a high vibrational level spends most of its time near its classical outer turning point Rv+ in Fig. 1. As a result, the properties of these levels are largely determined by the long-range portion of the molecular potential.

High vibrational levels can usefully be called “longrange molecules” (LeRoy, 1973; Stwalley, 1978) and provide one example of what one might more generally class as physicists’ molecules, i.e., molecules whose properties can be related (with high precision) to the properties of the constituent atoms. It is possible to understand their properties using a model which accurately treats the (relatively simple) long-range part of the potential and only approximately treats the (relatively complicated) short-range part of the potential. The nature of the PA process is such that it tends to favor production of molecules in very high vibrational levels. In this sense PA spectroscopy complements more traditional bound →bound molecular spectroscopy in which (typically) it is easier to reach low vibrational levels rather than high ones.

An even better approximation to the ideal physicists’ molecule is the so-called purely long-range molecules (or, more precisely, bound vibrational states in purely long-range potentials). A purely long-range potential has vibrational levels with both inner and outer turning points at large internuclear separation. These unusual potential wells can result from avoided crossings between the various molecular potentials dissociating to a given separated atom limit. In comparison to ordinary chemically bound potentials, these purely long-range potentials are very shallow. Particularly for light molecules, it is possible for the entire range of internuclear separations relevant to bound states to lie at such large range that chemical bonding plays no role. Only with the advent of ultracold PA spectroscopy has it become possible to produce high-resolution spectra of these levels.

> [!figure]
> ![[Fig. 2.png|center|500]]
> **Figure 2.** A sample PA spectrum of $^{23}$Na at an initial temperature of 450 μK. Electronically excited molecules, $\mathrm{Na}_2$ *, produced by PA are ionized by a second color laser and the resulting molecular ions, $\mathrm{Na}_2$ +, are detected and counted to produce the signal. The different peaks correspond to different rotational levels (labeled J=0 to 4) within a single vibrational state (v=1) of a purely long range potential discussed in Sec. II.E. The natural linewidth of this molecular state is 20 MHz; the observed linewidth is larger due to thermal broadening. The binding energy of this level is ≈47 GHz below the 3 2 S1/2+3 2 P3/2 atomic asymptote.

Several important results have flowed from the ability of PA spectroscopy to study molecular states whose properties can be accurately connected to those of the constituent atoms. One is the precise determination of atomic radiative lifetimes for alkali-metal atoms, revealing systematic errors in earlier direct measurements.

Closely related is the first observation of retardation contributions to molecular bonding, i.e., the modification of the strength of a molecular bond due to the finite time for information to propagate from one atom to another (even though the atoms in question are only ≈10−17 light seconds apart).

### C. Photoassociation spectroscopy measures absolute binding energies

Photoassociation spectroscopy differs from conventional bound→bound molecular spectroscopy in that it directly measures the absolute binding energy of molecular levels. In PA spectroscopy the natural reference point for the energy scale is two free atoms at rest (i.e., the dissociation limit), whereas in bound→bound spectroscopy it is the lowest vibrational level in the ground electronic potential of the dimer. This distinction turns out to play an important role in extracting physical results from PA spectra.

As shown in Fig. 1, the photon energy EPA required to reach a particular excited molecular state is smaller than Eat, the energy required to drive the asymptotic atomic ground→excited transition. In an experiment it is straightforward to locate the atomic transition and then measure the detuning of the laser relative to that point.

Ignoring for the moment the small contribution of the initial thermal collision energy Eth, the molecular binding energy is simply Eb=EPA−Eat and is thus directly observed. To obtain the highest precision, it is necessary to correct for the effects of the initial thermal energy Eth. Typically this thermal spread leads to a correction in the resonance location of order $k_B T$/h, i.e., 20 MHz for a sample at T=1 mK. The details of the PA line shape are discussed in Sec. III.C.

Over the years spectroscopists have exercised considerable ingenuity in devising extrapolation schemes for determining binding energies from measured bound →bound transition frequencies (Birge and Sponer, 1926; LeRoy and Bernstein, 1970). A textbook summary is given by Steinfeld (1985). PA spectroscopy naturally provides a direct measure of the absolute binding energy, obviating the need for any extrapolation.

### D. Photoassociation creates slowly rotating molecules

An important concept in scattering theory is the rotational barrier due to the combination of the centrifugal potential and the molecular binding. The higher the angular momentum ℓ of the collision, the higher the energy of the barrier. For a fixed collision energy, this barrier prevents the atoms from closely approaching one another unless the angular momentum is sufficiently small. For the ultracold gases used as the starting point for PA spectroscopy, only the lowest few “partial waves” are able to make it over, or tunnel through, the rotational barrier. Since the absorption of a photon adds at most only one unit of angular momentum, PA typically produces excited molecules in low rotational levels. For example, the rotational features in Fig. 2 have rotational quantum numbers J=0 through 4. This is a consequence of the low initial temperature (450 μK) which limits collisions to ℓ=0, 1, or 2 (s, p, and d waves). Often, in bound→bound molecular spectroscopy, it is difficult to reach these low rotational levels. For the molecular spectroscopist, the ability of PA spectroscopy to directly measure low rotational levels eliminates the need to extrapolate when determining a rotationless potential.

### E. Photoassociation spectra yield information on atomic collisions

The long, and eventually spectacularly successful, effort to achieve Bose-Einstein condensation of dilute atomic gases has generated an intense interest in atomic collisions at ultracold temperatures. A crucial parameter in determining whether or not a particular atomic species will Bose condense, and its properties if it does, is the scattering length. The scattering length parametrizes the extreme low-energy scattering properties and is connected to the phase shift atoms experience in a collision.

If the scattering length is positive, a stable Bose condensate can be formed. PA has been widely used to measure scattering lengths and other aspects of cold atomic collisions. There are two distinct ways in which this has been done: the first is based on mapping the collisional wave function, while the second is to measure the binding energy of the most weakly bound levels of the ground-state potential [i.e., the bound states of the potential (AB) in Fig. 1].

The mapping of the collisional wave function by PA spectroscopy is possible because the probability of making a PA transition, i.e., of producing an excited bound molecule, is largely determined by the amplitude of the ground-state scattering wave function at the outer turning point Rv+ of the bound excited-state wave function.

In general, the probability of making a molecular transition, including a free→bound PA transition, depends on the Franck-Condon factor, i.e., the square of the overlap between initial and final vibrational wave func-

tions. Typical examples of wave functions for the case of PA spectroscopy are sketched in Fig. 3. For the excited state the long-range part of the potential is determined by the 1/R3 resonant dipole interaction while for the ground state the potential is given by the much-shorterranged 1/R6 van der Waals interaction. This is the situation for PA of two identical alkali-metal atoms as well as some other systems. As one might guess from the rapid oscillatory behavior of wave functions at short range, the Franck-Condon factor is predominately determined by contributions near the last lobe in the excitedstate wave function. In fact, the probability of making a PA transition is directly proportional to the square of the ground-state wave function at Rv+. In particular, it follows that the PA signals to an excited state whose outer turning point lies directly over a node in the ground-state wave function will be very weak.

Once a node in the scattering wave function has been located it is possible to determine the scattering length which characterizes the low-energy collision physics of the system. In order to do this, one must know the shape of the ground-state potential at separations larger than the nodal position. In practice, this means that the node needs to be at a sufficiently large separation so that the ground-state potential is predominately determined by the van der Waals interaction. Thus measuring the line shapes and relative intensities of different vibrational and rotational PA features gives us the ability to probe the ground-state collisional wave function for a few partial waves over a range of relatively large internuclear distances where only the van der Waals potential is needed to characterize the ground-state physicists’ molecule.

An alternative approach for determining scattering lengths is to directly measure the binding energy of the highest few bound levels in the ground molecular potential. This can be done in a two-color PA experiment in which photons of one color drive the free→bound PA transition while more energetic photons drive a bound →bound transition back down to a bound state of the ground potential. The details of this ‘‘Autler-Townes spectroscopy’’ are discussed in Sec. VII. From the laserfrequency difference one can infer the absolute binding energy of the ground-state levels. Coupled with a knowledge of the long-range, van der Waals dominated, shape of the potential, one can derive the scattering length.

### F. Photoassociation modifies atomic collisions

The scattering wave function which describes the collision of two cold atoms at a particular energy and angular momentum has a fixed pattern of nodes (see, e.g., Fig. 3). This wave function can be viewed as a standingwave pattern set up between an incoming wave and the wave reflected by the short-range interatomic potential.

As discussed in the previous section, this nodal pattern is directly related to the scattering length for the system and hence to the scattering properties of cold atoms.

Any process which changes this standing-wave interference pattern changes the scattering properties of the atoms.

As shown in Fig. 4(a), the presence of a PA laser tuned near a PA resonance introduces another path into this atomic interferometer: incoming atoms can not only “bounce off” the interatomic potential but may alternatively be photoassociated to the excited bound molecular state. When the intensity of the PA laser is low, the most likely next step is for atoms (now a molecule) to spontaneously emit a photon and become a pair of hot atoms or possibly a cold molecule [Eq. (2)]. Frequently, the pair of atoms thus formed has enough kinetic energy to escape the trap. Moreover, molecules formed in this way are usually not trapped. In either case, atoms are lost from the initial collision channel. Counterexamples to these generalizations can lead to interesting results, as shown in the article by Leonard et al. (2004), in which atoms are recaptured, and in that of Vanhaecke et al. (2002), in which molecules are accumulated. Thus the PA process introduces a loss channel into the atomic collision, reduces the amplitude of the reflected wave, and hence modifies the contrast of the standing-wave pattern describing the collision. More interesting effects occur when the intensity of the PA laser is increased.

Stimulated emission from the bound excited state back to the initial collision state becomes important and this introduces an extra elastic pathway into the collision.

This new pathway, via the excited molecular state, interferes with the original path (bouncing off the interatomic potential) and modifies the positions of the nodes in the ground-state wave function and hence the scattering length. This process potentially offers the experi- menter a tool for manipulating the properties of a cold atomic sample.

> [!figure]
> ![[Fig. 3.png|center|500]]
> **Figure 3.** Schematic representation of the initial low-energy scattering radial wave function |E, ℓ⟩ and the final bound vibrational wave function |b⟩ as a function of internuclear separation. The scattering wave function is calculated for the case ℓ =0 and Rv+ is the classical outer turning point of the excitedstate vibration. At very large separations the scattering wave function oscillates with a wavelength much larger than the scale of this figure.

An alternative interpretation of the modification of atomic scattering by a PA laser is given by the “dressedstate” view shown in Fig. 4(b). The optical field of the PA laser dresses the excited-state bound molecular level.

By tuning the laser frequency the experimenter can choose to set the dressed level below, at, or above the zero of collision energy. This situation—a bound level embedded in a continuum—is known as a Feshbach resonance. Results of initial experiments with optical Feshbach resonances are discussed in Sec. IX.D. Magnetically induced Feshbach resonances have proven to be an extremely useful tool for modifying the collision properties of cold gases; it is possible that optical methods will also develop to be a useful tool for the experimenter to employ.

### G. Photoassociation of cold atoms makes cold molecules

The enormous impact of laser-cooling techniques on atomic physics has naturally raised the question of how to produce similarly cold molecules. Direct laser cooling of molecules is difficult and has not been demonstrated to date. The problem is that to slow a room-temperature atom or molecule to mK temperatures requires that the atom or molecule undergo many cycles of absorbing and reemitting photons. The atom or molecule must have a closed cycling transition, i.e., a pair of levels such that spontaneous emission from the upper level always (or almost always) returns the system to the lower level. In molecules the large number of vibrational and rotational levels appears to preclude finding a closed cycling transition.

When cold atoms are photoassociated the resulting molecules are translationally cold as well, thus PA spectroscopy inherently involves production of cold molecules, even if only on a transient basis. Once these molecules are produced by PA, they are available for subsequent study. The simplest such experiment is an optical-optical double-resonance scheme in which one laser is fixed on a known PA resonance so as to produce a steady population of electronically excited molecules, while a second laser is scanned to produce a spectrum of higher-lying excited states. Figure 5 shows an example of a spectrum produced in this way. In this particular case the final molecular state produced by the absorption of two photons is autoionizing ($\mathrm{Na}_2$ ** →$\mathrm{Na}_2$ + +e−). Thus the experimental signature that the double-resonance condition has been fulfilled is the production of $\mathrm{Na}_2$ + ions.

> [!figure]
> ![[Fig. 4.png|center|500]]
> **Figure 4.** Modification of atomic scattering by an optical Feshbach resonance. (a) An intense laser tuned near a PA transition adds a new path to the quantum-mechanical interferometer, which produces the nodal pattern of the ground-state collisional state wave function. The arrows labeled “photoassociative absorption” and “stimulated emission” are driven by the same laser; the arrow labeled “spontaneous emission” [see Eq. (2)] represents an inelastic loss process for the collision. The multiple arrows labeled “reflected waves” indicate that at low collision energies reflection occurs not only at the inner turning point but over a wide range of internuclear separations. (b) Dressed-state picture of the same process. The excited bound state |b⟩ with n−1 photons has approximately the same energy as the initial collision state |E, ℓ⟩ with n photons. The shaded region represents the continuum of collision states, weighted according to the thermal energy distribution of an ultracold gas with maximum population of states near zero energy. Viewed this way the physics of PA is similar to that of magnetic Feshbach resonances, hence the name “optical Feshbach resonance.”

> [!figure]
> ![[Fig. 5.png|center|500]]
> **Figure 5.** Molecular spectroscopy using a sample of cold molecules produced by photoassociating cold atoms. PA of 450 μK $^{23}$Na atoms by a fixed-frequency laser produces a steady population of cold, electronically excited $^{23}\mathrm{Na}_2$ molecules in a single known rovibrational level [here 1g(3/2), v=52, J=1]. A second, scanning laser promotes some of these molecules to doubly excited states. An ion detector counts the resulting $\mathrm{Na}_2$ + ions and this count rate is plotted as a function of the total energy of the two photons. Three rotational lines of the doubly excited state J=1,2,3 are shown, each split into two “Λdoubling” components. The rotational spacings for this Rydberg state are ≈100 times larger than those for the state shown in Fig. 2, reflecting the fact that the vibrational wave function for the Rydberg state lies at much shorter internuclear separations.

Actually, in this particular experiment there is another ionization pathway for molecules produced by the PA step, namely, absorption of a second photon from the PA laser. This other path produces the steady background ion signal observable in the experimental trace.

In the experiment which produced the data shown in Fig. 5, the cold molecules created by PA are in an electronically excited state with a lifetime of order tens of ns. At any given time, only a tiny fraction of the cold atoms in the trap are photoassociated to form molecules.

While this situation is quite sufficient for many spectroscopy experiments, it is only a limited step towards the goal of “producing cold molecules.” For many purposes, such as studying collisions, one wants to produce larger numbers of molecules and have them be in a stable (or at least metastable) state. A number of schemes for producing cold ground-state molecules have been demonstrated. The simplest version is to let the excited-state molecules spontaneously decay. As noted earlier, this spontaneous emission (see Fig. 1) may produce either a pair of free atoms or a bound molecule in the ground electronic state, typically a highly excited vibrational state. The experimental challenge is to produce an interesting number of molecules in the desired rovibrational level(s) of the ground state. Progress in this direction will be discussed in Sec. IX.A. Other techniques besides PA have been employed to produce cold ground-state molecules [see, for example, de Carvalho et al. (1999), Bethlem et al. (2000), Greiner et al. (2003)] but will not be discussed here.

The two types of experiments on cold molecules discussed thus far can be understood in terms of population transfer. A related class of multiphoton experiments depends on quantum interferences between molecular states. Of particular importance has been experiments to probe ground-state rovibrational levels by “frustrating” the PA process. Unlike the experiment illustrated in Fig.

5 in which both photons drive upward transitions, in these experiments the second photon is tuned to drive a downward transition starting from the excited bound level back to a bound level in the ground electronic state. When the laser driving the bound-bound transition is sufficiently intense, the two bound levels are strongly mixed. This induces an Autler-Townes-type splitting of the PA line, reducing the PA rate. This approach, discussed in Sec. VII, has proven to be an important tool for probing the high-lying vibrational levels of the ground electronic potential.

### H. Photoassociation accesses a wide variety of molecular symmetries

A feature of PA spectroscopy is that the initial atomic collision state is often a mixture of many different molecular symmetries. A PA transition can thus reach a variety of bound molecular states. In contrast, experiments which begin with bound molecules are typically restricted by selection rules to probing certain types of states, at least as a first approximation. Consider, for example, $\mathrm{Na}_2$. Each sodium atom has one unpaired electron spin and thus the total spin of two colliding atoms can be either 0 (singlet) or 1 (triplet). In fact, a collision is typically a mixture of these two, especially when there is atomic hyperfine structure, and thus electric dipole transitions are allowed to either singlet or triplet upper states.

### I. Scope of this review

By now the body of experimental and theoretical work on PA of cold atoms is sufficiently large that it is no longer possible to discuss all of the important papers.

In this review we have tried to provide representative examples of the kind of work that has been done, especially more recent trends. An early review by Lett et al. (1995) discussed some pioneering work that we shall not be able to include here. Closely related to the work we discuss are magneto-optical trap (MOT) trap-loss experiments in which the trap lasers act as the PA laser and thus are tuned so close to the atomic transition that no bound-state structure is resolved. Also closely related are experiments on optical shielding in which the PA laser is tuned to excite pairs of colliding atoms to a repulsive molecular potential. Some fairly recent work (Weiner et al., 1999; Weiner, 2003) has covered these experiments and other related areas as well as some of the same topics we discuss here. A review by Stwalley and Wang (1999) covered many aspects of PA as a spectroscopic technique, with an especially thorough coverage of work on $\mathrm{K}_2$. A review by Masnou-Seeuws and Pillet (2001) also discussed ultracold photoassociation and molecule formation in some detail, with an emphasis on $\mathrm{Cs}_2$.

PA spectroscopy is able to access high vibrational levels which probe the long-range parts of molecular potentials but it is not the only way to reach these high vibrational levels; it is possible to begin with bound-state molecules and optically pump to these high levels. Of particular relevance to our present discussion is the work by Tiemann’s group [see, for example, Samuelis et al. (2001)], which has achieved results very competitive with those from PA experiments.

This review is organized as follows. The next three sections introduce general background concepts, illustrated with occasional examples. Starting in Sec. V we discuss specific experiments and their interpretation. To date the most extensive results have been obtained in experiments with single-species alkali-metal atoms (and hence homonuclear diatomic molecules). This choice reflects the relative ease of laser-cooling alkali-metal atoms. From here on we shall illustrate our discussion using sodium as our example atom, partly to streamline the discussion, and partly, we confess, because most of our own experimental work has been with that particu-

lar atom. Most of what we say about sodium applies directly to the other alkali-metal atoms. In the course of discussing specific experiments, we shall broaden the coverage to include mixed-species systems (e.g., KRb), alkaline-earth atoms (e.g., Ca), and noble-gas atoms (e.g., metastable He).

## II. Molecular States from an Atomic Viewpoint

Much of the interest in PA spectroscopy comes from its ability to probe molecular states in which the two atoms of the diatomic molecule are often (or always) quite far apart and the overlap of the electron clouds of the two atoms is negligible. Here we examine some of these molecular states. To make the discussion concrete we shall choose the specific example of sodium (Na +Na+γ→$\mathrm{Na}_2$ *). Even for other systems where there might be important differences, such as mixed species (e.g., Na+Rb+γ→NaRb*), alkaline-earth atoms (e.g., Ca), or metastable rare-gas atoms (e.g., helium in the 1s2s electronic state), an understanding of the singlespecies alkali-metal system is a useful point of departure.

We shall endeavor to briefly introduce spectroscopic concepts, such as symmetry labels and Hund’s angular momentum coupling cases (Hund, 1927) as needed. For a more complete discussion, the reader is referred to the extensive literature on the spectroscopy of diatomic molecules (Herzberg, 1950; Hougen, 1970; Steinfeld, 1985; Lefebvre-Brion and Field, 1986; Zare, 1988).

### A. A few facts about alkali-metal atoms

As a reminder, Fig. 6 shows a schematic view of the lowest two electronic levels of the Na atom. The large number of digits given for the level positions is meant to convey that, for many purposes, the level structure and splittings are “exactly” known. The one optical frequency transition indicated on the figure is the 3 2 S(f =2)→3 2 P3/2(f=3) transition used for laser cooling.

Many interesting PA spectroscopy results have been obtained using a photoassociation laser detuned red from this transition by only tens of GHz.

### B. Nonrelativistic atoms and diatoms

Figure 6 shows the full structure of the Na atom including spin-orbit and hyperfine interactions. For purposes of modeling the dimer it is useful to initially consider the simpler “nonrelativistic atom” ignoring spinorbit and hyperfine interactions. States are labeled by the total electron orbital angular momentum l and spin s or succinctly 2s+1 l. The electronic ground state of an alkali-metal atom is 2 S or l=0 and s=1/2.

We now consider a molecule formed from two such nonrelativistic atoms, ignoring for the time being rota- tion of the molecule so that the interatomic axis is fixed in space. Taking into account electrostatic interactions between the constituent particles, and allowed symmetries, one can compute the potential energy of the pair at each interatomic separation R. Examples are shown in Fig. 7. We shall refer to potential curves derived this way as the “adiabatic Born-Oppenheimer potentials.”

> [!figure]
> ![[Fig. 6.png|center|500]]
> **Figure 6.** Schematic view of the lowest energy levels of the Na atom. The splittings are greatly exaggerated: the actual 3 2 P3/2↔3 2 P1/2 fine-structure splitting is a factor of ≈1000 smaller than the 3 2 S↔2 P splitting, while the ground-state f =2↔f=1 hyperfine splitting is an additional factor of ≈300 smaller still. The arrow indicates the optical transition typically used for laser cooling of Na.

> [!figure]
> ![[Fig. 7.png|center|500]]
> **Figure 7.** (Color online) The ten energetically lowest nonrelativistic Born-Oppenheimer potentials of the sodium dimer as a function of internuclear separation R. For the eight curves dissociating to the 2 S+2 P limit it is helpful to realize that for R ≳15a0 the Σ potentials go as ±2C3/R3, while the Π potentials go as ±$C_3$/R3, where $C_3$ is the resonant dipole coefficient. The vertical arrow is meant to suggest typical minimum internuclear separations and typical largest energy detunings important for PA, in contrast to the more schematic Fig. 1. The curves are from Magnier et al. (1993). Potentials for other homonuclear alkali-metal dimers will be similar in shape.

In the spirit of the classic Heitler-London or valencebond calculation of the H2 potentials (Herzberg, 1950), the curves shown in Fig. 7 can be computed by modeling the molecular electronic wave function as a combination of many atomic electronic wave functions. At large R the molecular wave function is accurately described as a product of just two atomic wave functions. The term ‘‘physicists’ molecule’’, coined in the Introduction, is meant to bring to mind this atomic picture of the molecule. At short range the electron clouds distort and many additional atomic configurations are required to obtain an accurate description of the molecular wave function and thus accurate potentials. The implications of these observations are that we can hope to model the long-range portion of the potentials to high accuracy but we can only approximately model the short-range portion. The properties of the atomic collisions and molecular states observed in PA spectroscopy are mainly determined by the long-range portion of the potential. Effects of the short-range parts of the potential need to be included but can be handled approximately and can often be encapsulated in a few parameters. Hence much of the rest of this section is devoted to developing the theory of the long-range molecular potentials using an atomic valence-bond picture.

The Born-Oppenheimer potentials in Fig. 7 are labeled by quantum numbers indicating the symmetry of the electronic wave functions. The allowed symmetries can be inferred from the atomic properties at the dissociation limit. In the nonrelativistic, nonrotating approximation, the total electron spin S ⃗ =s ⃗a+s ⃗b is conserved, where sα (α=a or b) are the electron spins of the individual atoms. For example, the potentials dissociating to the 2 S+2 S limit in Fig. 7 can be either singlet, S=0, or triplet, S=1. In contrast, the total electronic orbital angular momentum L ⃗ =l ⃗ a+l ⃗ b is not conserved, as a frozen dimer is not spherically symmetric in space. The molecule is cylindrically symmetric around the internuclear axis, however, and thus the absolute value of the projection Λ=λa+λb of L along the internuclear axis is conserved. Here λα (α=a or b) are the projections of the atomic electron orbital angular momentum lα along the internuclear axis. For example, for the potentials dissociating to the 2 S+2 P limit, Λ=0 or |Λ| =1. The conventional notation for the molecular states is 2s+1 |Λ|, where Λ is encoded as Σ, Π, Δ,... for |Λ| =0,1,2,.... The convention in the literature is to take Λ to be positive definite when labeling potentials but to allow Λ to be a signed quantity when discussing electronic wave functions. We shall do so as well.

While in general L is not a good quantum number, at sufficiently large internuclear separations, where the electronic wave function simplifies into a product of just two atomic wave functions, only certain values of L are allowed. The values are those consistent with vector addition of the two well-defined atomic values. For example, for the potentials dissociating to the 2 S+2 S limit in Fig. 7, L=0 is the only allowed value at long range.

For the potentials dissociating to the 2 S+2 P limit, L=1.

In constructing a theoretical model, it is often acceptable to make the approximation that L at all internuclear separations is determined by adding up fixed atomic angular momenta even when this is not strictly true. This is related to the ‘‘pure precession’’ approximation used in deriving Λ doubling. Many subtleties in using the pure precession approximation arise, as discussed in the literature (Herzberg, 1950; Lefebvre-Brion and Field, 1986; Zare, 1988).

Figure 7 also shows that there are other symmetries that label the Born-Oppenheimer potentials. The ± superscript indicates a reflection symmetry of the spatial component of the electronic wave function through a plane containing the internuclear axis. This symmetry only exists for Σ states. The gerade/ungerade (g/u) subscript indicates the inversion of all electrons through the center of charge. This symmetry only exists for homonuclear dimers. Moreover, for homonuclear dimers in which both atoms are in the same electronic state, the quantum numbers of S, Λ, and ± symmetry uniquely determine the g/u symmetry.

### C. Long-range dispersion forces

The long-range behavior of the adiabatic Born-Oppenheimer potentials may be derived using the separated atom picture. In general the potential can be expressed as a power series in 1/R. For two ground-state S atoms the long-range interaction is an attractive, induced-dipole–induced-dipole or van der Waals interaction which goes as $C_6$/R6 to leading order, where $C_6$ is the van der Waals dispersion coefficient. The X 1 Σg + and a 3 Σu + potentials in Fig. 7 have the same $C_6$ coefficient and thus at long range the two potentials are degenerate. The potentials become distinct at shorter distances where exchange forces become important. On the scale of Fig. 7 the region where the potential is dominated by the van der Waals force seems quite unimportant. It is necessary to keep in mind that the thermal energies of the ≲1 mK colliding atoms used in PA experiments are $k_B T$/hc≲0.001 cm−1, while the potential at 15a0 (where 1a0=0.0529 nm is the Bohr radius) is about 30 cm−1 deep. Therefore the scattering wave function at 15a0 is already strongly modified from its asymptotic form; see Sec. III.B.

For the excited states in Fig. 7, where one alkali-metal atom is in a 2 P state, the potential is a result of the resonant dipole-dipole 1/R3 interaction. The much longer range of the excited-state interaction, 1/R3, compared to the ground-state interaction, 1/R6, is clearly visible in Fig. 7. The figure also shows that the strength and sign of the resonant dipole interaction depends on

the 2S+1 Λ symmetry of the electronic wave function. The eight potentials fall into four groups of 2 and can all be written in terms of a single constant $C_3$. The Σ states go as ±2C3/R3 while the Π states go as ±$C_3$/R3.

The 1/R3 behavior of the excited states is peculiar to homonuclear molecules and is a result of two atoms sharing the excitation back and forth, hence the term resonant dipole interaction. A useful, if somewhat handwaving, semiclassical picture to have in mind is that each atom is in a superposition of ground and excited state and has a real oscillating dipole moment. Depending on how the dipoles on the atoms are oriented, the interaction can be attractive or repulsive. For example, two dipoles oscillating perpendicular to the molecular axis will have an interaction which is either ±$C_3$/R3 depending on whether the dipoles are in phase or 180° out of phase.

A more precise quantum-mechanical description of the origin of the 1/R3 potential starts from the longrange electrostatic interaction Vdd = 1 4πε0 d ⃗ a · d ⃗ b −3daz′dbz′
$$
V_{dd}=\frac{1}{4\pi\epsilon_0}\frac{\vec d_a\cdot\vec d_b-3d_{az\prime}d_{bz\prime}}{R^3} \tag{3}
$$
where the coordinate system is chosen such that the z′ axis is along the interatomic axis, and d ⃗ α and dαz′ (α=a and b) are the atomic dipole operator and its projection along z′, respectively. The constant ε0 is the electric constant.

The molecular wave function |laλa,lbλb⟩=|00,1λb⟩ is the product of a ground-state atom a and an excited atom b. When the operator Vdd is applied to this state it produces a state proportional to |1λb,00⟩, so that the excitation has been transferred to the other atom. Here λa,b are the projections of the atomic orbital angular momentum la,b along the internuclear axis and Λ=λa+λb.

The linear combinations
$$
\left|L=1,\Lambda=\lambda_b,p\right\rangle=\frac{1}{\sqrt{2}}\left(\left|00,1\lambda_b\right\rangle+p\left|1\lambda_b,00\right\rangle\right) \tag{4}
$$
diagonalize the resonant dipole interaction. Here p is ±1. In the definition of the ket on the left side of the equation we have realized that, since la=0, it follows that L=lb=1 and Λ=λb. The eigenenergies are the adiabatic Born-Oppenheimer potentials and depend on Λ and p.

Although there are no electron-spin-dependent terms in this nonrelativistic Hamiltonian, the full electronic wave functions have an electron-spin component and are of the form
$$
\left|L\Lambda S\Sigma\sigma\right\rangle=\left|L\Lambda p\right\rangle\left|S\Sigma\right\rangle \tag{5}
$$
where Σ is the projection of S ⃗ on the internuclear axis and σ≠0/1 for gerade/ungerade symmetry. Although p emerges from our discussion as a natural label for the wave function, the conventional label for the electron wave function is gerade/ungerade symmetry. This symmetry depends on both the electron spin and spatial wave function. For homonuclear alkali-metal dimers, p =(−1)S+σ.

The $C_3$ coefficient which emerges from the above analysis is given by the single-atom matrix element $C_3$ =|⟨10|dbz′|00⟩|2 /4πε0, where the bras and kets denote |lbλb⟩. This same matrix element appears in the expression for the radiative lifetime τ of the excited P state. In
$$
\tau=\frac{3\hbar c^3}{4C_3\omega^3} \tag{6}
$$
where ℏω is the atomic transition energy. Thus there is an intrinsic connection between the strength of the 1/R3 molecular interaction and the atomic radiative lifetime.

This fact has been exploited to make very precise measurements of atomic lifetimes as discussed in Sec. V.E.

Our focus thus far has been on homonuclear alkali dimers. For heteronuclear alkali molecules the dominant long-range interaction in both ground and lowest excited state is 1/R6. This difference has a major impact on the character of the PA spectrum. If both atoms are in states with nonzero orbital angular momentum, such as metastable rare-earth atoms (Doery et al., 1998) or metastable alkaline-earth atoms (Derevianko et al., 2003; Santra et al., 2004), the long-range potentials can have significant contributions from 1/R5 quadrupolequadrupole interaction.

### D. Spin-orbit interaction

The “nonrelativistic” description determines the largest energy scales in atoms and molecules. Weaker relativistic interactions, such as the spin-orbit and hyperfine interactions, are, nevertheless, still vastly larger than the kinetic energy of the colliding atoms and the typical spectroscopic accuracy obtainable in PA spectroscopy.

The strongest relativistic interaction is the spin-orbit interaction (Lefebvre-Brion and Field, 1986). The usual way to introduce the spin-orbit interaction in atoms is in the form of an effective Hamiltonian involving the total electron orbital angular momentum l ⃗ and total electron spin s ⃗. The simplest effective Hamiltonian is Al ⃗·s ⃗, where A is the spin-orbit constant. In this case j, found from j ⃗ =l ⃗+s ⃗, as well as l and s are good quantum numbers.

Atomic states can then be described by 2s+1 lj. For alkalimetal atoms we encounter 2 S1/2,2 P1/2, and 2 P3/2 states.

For many atoms this treatment is sufficient, but in general only j is a good quantum number.

In the ‘‘physicists’ molecule’’, in which the molecular electronic wave function is well represented by a product of atomic wave functions, the molecular spin-orbit interaction is the sum of the atomic spin-orbit interactions. In many cases one does not need to evaluate spinorbit constants from electronic structure but can instead use measured values of the atomic A constants. When this approach is sufficient, a relatively simple analytical calculation (see Sec. II.E) captures the major effects of spin-orbit interactions in the molecule. In general, the

spin-orbit interaction in a molecule requires a more complex effective Hamiltonian that describes the R dependence of the interaction (Lefebvre-Brion and Field, 1986; Kokoouline et al., 2000).

Regardless of the detailed form of the spin-orbit interaction, the molecular electronic wave functions have certain symmetry properties. Since a dimer is cylindrically symmetric, Ω, the absolute value of the projection of j ⃗ =j ⃗a+j ⃗b=L ⃗ +S ⃗ along the internuclear axis, is conserved.

Here subscripts again indicate atom a and b and j ⃗ is the total electron angular momentum. In general j is not conserved. Molecular potentials computed taking into account both the electrostatic and spin-orbit interactions are shown in Fig. 8 for our example of two sodium atoms. Note that the figure focuses on potentials near the 2 S+2 P dissociation limit. The energy scale is 100 times smaller than Fig. 7. The distance scale is ~10 times larger. These “relativistic adiabatic” potentials are labeled by Ωg/u ±,where many labels appear more than once.

The superscript ± for Ω=0 states is a reflection symmetry of the total electron wave function through a plane containing the internuclear axis. It differs from the reflection symmetry of nonrelativistic Σ states.

Each curve in Fig. 8 will approach one of the Born-Oppenheimer potentials in Fig. 7 for internuclear separations ≤30a0. There are 16 potentials in Fig. 8 and only 8 Born-Oppenheimer potentials dissociating to 2 S+2 P, hence several of the relativistic adiabatic potentials approach the same Born-Oppenheimer potential. This connection is shown in Fig. 9. For example, four relativistic adiabatic potentials, with symmetries 0u ±, 1u, and 2u, approach the Born-Oppenheimer potential state labeled 3 Πu. Within the relativistic calculation these four will not be exactly degenerate but will be split by the spin-orbit interaction. On the scale of Fig. 7 this splitting (roughly 10 cm−1 for $\mathrm{Na}_2$) would hardly be noticeable. Two of the relativistic adiabatic potentials approach the 3 Σg + potential. These are degenerate since the spin-orbit interaction is zero for the Σ state.

### E. Movre-Pichler model

The Movre-Pichler model (Movre and Pichler, 1977; Stwalley et al., 1978) has played a crucial role in the development of quantitative models of ultracold photoassociation. It gives an elegant description of the longrange forces between a ground 2 S and excited 2 P alkalimetal atom resulting from the combination of the resonant dipole and spin-orbit interactions. This model describes the potentials shown in Fig. 8. These potentials are given in terms of two atomic parameters: the atomic 2 P3/2↔2 P1/2 spin-orbit splitting Δ and the $C_3$ coefficient (i.e., the atomic S↔P electric dipole matrix element).

> [!figure]
> ![[Fig. 8.png|center|500]]
> **Figure 8.** (Color online) The 16 relativistic adiabatic interaction potentials as a function of internuclear separation near the 2 S+2 Pj dissociation limit of $\mathrm{Na}_2$. Clearly visible is the splitting between the P1/2 and P3/2 states. Each potential is labeled by Ωg/u ±. To distinguish between these states it is helpful to indicate the dissociation limit as well, e.g., 1g(2 S+2 P3/2); as a shorthand this is denoted 1g(3/2). Since, usually, it is the attractive potentials that are of interest, that labeling is generally sufficient.

> [!figure]
> ![[Fig. 9.png|center|500]]
> **Figure 9.** The connection between the Born-Oppenheimer potentials of Fig. 7 (distance regions I and II) and the relativistic adiabatic potentials of Fig. 8 (distance regions III and IV) for homonuclear alkali-metal dimers. In each of the four distance regions the vertical order indicates the energy ordering of the states. Gerade (ungerade) states in one region connect only to gerade (ungerade) states in other regions. The dissociation limits are labeled for the specific case of $\mathrm{K}_2$. From Wang, Gould, et al., 1997, where the distance scales are defined.

The Movre-Pichler model was instrumental in predicting the presence of the purely long-range potentials (Stwalley et al., 1978) alluded to in the Introduction.

With minor modifications this model can be made fully quantitative for many systems (Jones et al., 1996; McAlexander et al., 1996; Wang et al., 1997; Boesten et al., 1999; Amiot et al., 2002; Bergeman et al., 2002).

This section will illustrate the Movre-Pichler approach for the specific case of the two 0g −potentials shown in Fig. 8 and whose connection to short-range Born-Oppenheimer potentials and long-range dissociation limits are shown in Fig. 9. To distinguish between these two potentials it is convenient to append an additional label indicating whether the state is the one dissociating to the upper, 2 S+2 P3/2, or the lower, 2 S+2 P1/2, limit.

Thus we use 0g −(3/2) to indicate the upper potential and 0g −(1/2) to indicate the lower potential. The upper potential is a purely long-range potential. Careful inspection of Fig. 8 suggests that the 0g −(3/2) potential has a minimum around 70a0. This is indeed the case. A blowup is shown in Fig. 10. This potential well is sufficiently deep in $\mathrm{Na}_2$ to support many vibrational bound states; several levels are indicated in Fig. 10.

The Movre-Pichler model starts with the nonrelativistic electronic wave functions |LΛSΣp⟩ which diagonalize the resonant dipole interaction as discussed in Sec. II.B.

It extends this model by including an atomic spin-orbit interaction of the form Al ⃗·s ⃗ for each of the atoms, where A is the atomic fine-structure constant. In the specific case we are discussing when one atom is in an S state, only one atom has a nonzero contribution.

To find potentials with 0g −symmetry we first identify the wave functions with Λ+Σ=0 and gerade symmetry.

They are
$$
\left|L\Lambda S\Sigma\sigma\right\rangle=\left|111{-}1g\right\rangle \quad \text{and} \quad \left|1{-}111g\right\rangle \tag{7}
$$
with 3
$$
\left|1010g\right\rangle \tag{8}
$$
with 3
$$
\left|1000g\right\rangle \tag{9}
$$
with 1 Σg + symmetry. These four states do not necessarily have definite parity with respect to reflection through a plane containing the internuclear axis (i.e., the ± symmetry which distinguishes 0±
$$
\frac{1}{\sqrt{2}}\left(\left|111{-}1g\right\rangle+\left|1{-}111g\right\rangle\right) \tag{10}
$$
and |1010g⟩. Using these two basis states, designated Π
$$
V_{\mathrm{MP}}=\begin{pmatrix}\dfrac{C_3}{R^3}-\dfrac{2\Delta}{3} & \dfrac{\sqrt{2}\Delta}{3} \\ \dfrac{\sqrt{2}\Delta}{3} & -\dfrac{2C_3}{R^3}-\dfrac{\Delta}{3}\end{pmatrix} \tag{11}
$$
where Δ=3A/2 is the atomic spin-orbit splitting and the zero of energy is set at the 2 S+2 P3/2 asymptote. In this “molecular” basis the resonant dipole interaction is diagonal, while the atomic spin-orbit interaction has offdiagonal matrix elements as well. The eigenvalues of this matrix are the relativistic adiabatic potentials shown in Fig. 8. The upper 0g −(3/2) potential has a shallow well and is shown in more detail in Fig. 10 for $\mathrm{Na}_2$. The well depth is Δ/9, independent of $C_3$, the potential minimum is at Re=(9C3/2Δ)1/3, and at long range the potential goes as −$C_3$/R3. A sample spectrum of one vibrational level (v=1) is shown in Fig. 2 and another (v=0) in Fig.

30. For the lower potential, 0g −(1/2), the coefficient of the 1/R3 term is zero, and the leading term, including only effects of the resonant dipole interaction, is −(2C3 2 /Δ)/R6. The two 0g −states are an R-dependent mixture of the Σ and Π basis states.

A similar approach yields expressions for the other potentials which dissociate to the 2 S+2 P3/2 and 2 S +2 P1/2 limits. Of particular interest is the 1u(3/2) potential indicated in Fig. 10 which, like the 0g −(3/2) potential, is also a purely long-range potential but with an even larger equilibrium position. As for the 0g −(3/2) potential, the depth is independent of $C_3$ and depends only on Δ.

At short range (≤20a0 for $\mathrm{Na}_2$) the 1u(3/2) potential becomes the well-known B1 Πu potential.

The elegance of the Movre-Pichler model is that once the necessary Hamiltonian matrices are in hand, it is a simple matter to generate the potential curves for any given values of Δ and $C_3$. As noted above, for precise comparison to experiment it is necessary to extend this model. For the heavier alkali-metal dimers it is necessary to correct for chemical bonding, higher-order dispersion contributions ($C_6$/R6, etc.), and atomic relativistic corrections, which make the transition dipole moment for the 2 S→2 P3/2 transition different from that for the 2 S→2 P1/2 transition. For all alkali-metal dimers it is important to include hyperfine interactions, nonadiabatic corrections, and retardation corrections to the resonant dipole interaction.

> [!figure]
> ![[Fig. 10.png|center|500]]
> **Figure 10.** (Color online) A blowup of the relativistic adiabatic potential-energy curves shown in Fig. 8, showing the purely long-range 0g −and 1u potentials. Some of the vibrational levels of the 0g −potential are indicated. Only attractive states are labeled. From Tiesinga et al., 2005.

### F. Mechanical rotation and Hund’s cases

So far we have discussed two kinds of interactions: electrostatic interactions and relativistic spin-orbit interactions. As a shorthand, we use the term “Born-Oppenheimer interaction” to refer to the combined effects of the electrostatic interactions and electron exchange, which give rise to the splittings between the Born-Oppenheimer potentials discussed in Sec. II.B. In this section we let the molecule rotate. The rotation of the molecule introduces another angular momentum into the problem, ℓ ⃗. This rotation is often called R ⃗ in the spectroscopy literature (Hougen, 1970; Lefebvre-Brion and Field, 1986; Zare, 1988) but we adopt the convention of the scattering literature. The rotational angular momentum ℓ ⃗ is, by definition, perpendicular to the internuclear axis.

The Hund’s cases classify the relative strengths of the Born-Oppenheimer interactions, the spin-orbit interaction, and rotation. In other words, they describe the way in which the angular momenta in the molecule are coupled together. The nonrelativistic Born-Oppenheimer interaction locks the total electron orbital angular momentum L ⃗ to the internuclear axis, i.e., its projection Λ is a good quantum number, the spin-orbit interaction couples L ⃗ with the electron spin S ⃗, and rotation couples the electron angular momenta, L ⃗ and S ⃗, to the rotational angular momentum ℓ ⃗. Often the coupling scheme changes with internuclear separation R as the interactions change.

Rotation enters as the deceptively simple term ℏ2 ℓ ⃗2 /(2μR2) in the molecular Hamiltonian, where μ is the reduced mass. If there were no other angular momenta in the problem, ℓ would be a good quantum number and the probability of finding the internuclear axis pointing in a particular direction in space R̂ would be given by |⟨R̂| ℓmℓ⟩|2 =|Yℓmℓ (R̂)|2. Here the quantum number mℓ is the projection of ℓ along a spaced-fixed z axis and Ylm is a spherical harmonic.

In the real molecule ℓ is not the only angular momentum and the molecular axis may nutate and precess, and thus a “rotational” energy level does not always have a well-defined value of ℓ. From this point of view, the Hund’s cases, by classifying the way in which the various angular momenta couple, describe the motion of the internuclear axis. From a practical point of view, a spectroscopist observes vibrational and rotational energy levels and wants to know how to label them and how to determine from them a “rotationless” potential. The five Hund’s cases, (a)–(e), are simple limiting coupling cases in which the rotational energy levels for a given vibrational level satisfy Erot=BvX(X+1)+¯, where X is an angular momentum quantum number, determined by the way the individual angular momenta couple in a particular Hund’s case, and Bv is the rotational constant.

The total angular momentum J ⃗=ℓ ⃗ +L ⃗ +S ⃗ =ℓ ⃗ +(⃗ is a good quantum number and one might naively expect that X =J, but this is not always true.

The most commonly occurring coupling schemes in conventional molecular spectroscopy of dimers are Hund’s cases (a) and (b). These two schemes occur for tightly bound states in the potentials shown in Fig. 7. A tightly bound molecule typically has inner and outer turning points Rt<20a0. For such separations the splittings between various Born-Oppenheimer potentials are typically large compared to both relativistic spin-orbit interactions and rotational energies. The two Hund’s cases differ in the relative strength of the spin-orbit and rotational interaction. For Hund’s case (a), the spin-orbit interaction is strongest and Ω as well as S and Λ are good quantum numbers (i.e., 2S+1 ΛΩ states). The rotational spectrum is then BvJ(J+1)+ ¯. For Hund’s case (b), the rotational interaction is strongest and Ω is not a good quantum number even though S and Λ are. The rotational spectrum is BvN(N+1)+¯, where N ⃗ =ℓ ⃗ +L ⃗.

The subtle distinction between cases (a) and (b) is best illustrated with some examples. Typically for Λ≠0 and S≠0, Hund’s case (a) is valid for low J. For example, for the b 3 Πu state of sodium in Fig. 7, the spin-orbit interaction energy is on the order of 10 cm−1 and the rotational energy for low rotational levels is approximately 0.1 cm−1. Therefore the states are labeled by 3 Π0,1,2 and J≥Ω. Typically, Λ=0 and S≠0 states satisfy the Hund’s case (b) coupling scheme. For a sodium dimer, the a 3 Σu + and 1 3 Σg + states are described by case (b) coupling. For singlet S=0 states, cases (a) and (b) are equivalent and the case (a) notation is used. The X 1 Σg + and A 1 Σu + states of sodium are described by case (a) coupling.

Hund’s case (c) typically applies when states with different Ω are widely separated, as in Figs. 8 and 10. Here the spin-orbit and Born-Oppenheimer interactions are comparable and both are larger than the rotational interaction. This ensures that the projection Ω is always a good quantum number. If the spin-orbit interaction is smaller than the Born-Oppenheimer interaction, we recover the Hund’s case (a) coupling scheme. In case (c) the rotational progression has X=J, just as for case (a).

The two Hund’s cases in which X=ℓ are (d) and (e).

Both coupling schemes occur when neither L ⃗ nor S ⃗ is coupled to the internuclear axis. In case (e) the spinorbit coupling between L ⃗ and S ⃗ is strong while in case

(d) it is weak. A good example of Hund’s case (e) observed in PA spectroscopy is the 0g −potential dissociating to the 2 S+2 P1/2 limit (the lower 0g −discussed in Sec. II.E) and observed in $\mathrm{Rb}_2$ by Boesten et al. (1999). A detailed analysis of the electronic wave function of this state, as calculated in the Movre-Pichler model, shows that j ⃗=j ⃗a +j ⃗b=L ⃗ +S ⃗ is zero and thus a good quantum number. This also implies that J ⃗=ℓ ⃗.

Weakly bound states of the two alkali-metal dimer electronic ground-state potentials, X 1 Σg + and a 3 Σu +, can be described by Hund’s case (d). Here the molecular electronic wave function can be well represented by two atomic S-state atoms, thus L=0, there is no spin-orbit interaction, thus X=ℓ. As we shall show in the next section, the hyperfine interaction, which “strongly” couples the electron spin to the nuclear spin, cannot be ignored in describing these weakly bound states, further complicating the distinction between the different Hund’s cases. Other corrections to the case (d) coupling scheme also play a role in these states. Weak second-order spinorbit and magnetic spin-spin interactions need to be taken into account for quantitative descriptions (Stoof et al., 1988; Mies et al., 1996). Both interactions weakly couple the electron spin to the internuclear axis.

### G. Hyperfine interactions in ground electronic states

The resolution of PA spectroscopy is sufficiently high that it is essential to include hyperfine interactions in the description of the molecule. For the initial scattering state used in PA spectroscopy, the thermal energy is typically orders of magnitude smaller than the atomic hyperfine splittings, except of course for those atoms which have no hyperfine splitting (such as common alkaline-earth isotopes). For alkali-metal atoms the atomic ground-state hyperfine structure (see Fig. 6) is given by the Hamiltonian ahfs ⃗·i ⃗, where i ⃗ is the nuclear spin of the atom and ahf is the hyperfine constant. Just as the molecular spin-orbit interaction can be calculated from the sum of the atomic spin-orbit interactions, the molecular hyperfine interaction can be calculated from the sum of the atomic ones.

Hyperfine interactions can couple the adiabatic Born-Oppenheimer potentials with different g/u symmetry or different total electron spin S. For a homonuclear molecule like $\mathrm{Na}_2$, shown in Fig. 7, hyperfine interactions couple the X 1 Σg + and a 3 Σu + states. Figure 11 shows the long-range potentials which result. At very long range the potentials are labeled by the atomic hyperfine quantum numbers fa and fb, where f ⃗ α=s ⃗α+i ⃗α (α=a or b). The potentials are split by the atomic hyperfine splitting (1.77 GHz for Na, see Fig. 6). At the separations shown in Fig. 11, the two Born-Oppenheimer potentials are degenerate since they both have the same long-range dispersion interactions (dominated by the attractive −$C_6$/R6 van der Waals interaction). Thus when the hyperfine interaction is taken into account the resulting potentials are split by one atomic hyperfine splitting for all separations shown in the figure. Each of the three curves shown has unresolved degeneracies. These can be labeled by the quantum number f, where f ⃗=f ⃗ a+f ⃗ b. For example, the lowest 1+1 curve has a twofold degeneracy with f=0,2. On the other hand, S is not a good quantum number.

At short range, inside the separations shown in Fig.

11, the X 1 Σg + and a 3 Σu + potentials are well split. At these short distances the effective hyperfine interaction is aeffS ⃗ ·I ⃗, where I ⃗ is the total nuclear spin i ⃗a+i ⃗b. The connection between the long-range and short-range behavior is subtle. Although one can construct adiabatic potentials, labeled by f, which smoothly connect the long and short range, similar to those discussed in regard to the spin-orbit interaction in Sec. II.E, this picture is somewhat misleading if not interpreted carefully. For the ground-state potentials, nonadiabatic couplings, arising from the nuclear kinetic-energy operator, are not negligible for scattering at ultracold temperatures. One cannot think of a scattering wave function for each adiabatic potential but instead one must think of the scattering wave function as a multichannel object having several components. The application of a multichannel approach to cold-atom collisions is described by Gao (1996) and Stoof et al. (1988). Roughly speaking the collision process is a kind of interferometer. A wave starts inward from long range. When the wave reaches the distance where the hyperfine and exchange interactions become comparable in size, the wave splits. One part of the wave samples the singlet potential and one part samples the triplet potential. The two parts bounce off the inner wall of their respective potentials and recombine on the way back out. Finally, the interference be- tween the incoming wave and the outgoing wave establishes the nodal pattern of the scattering wave function.

> [!figure]
> ![[Fig. 11.png|center|500]]
> **Figure 11.** (Color online) The long-range hyperfine structure, at zero magnetic field, of a ground-state 3 2 S+3 2 S Na dimer. The three curves are separated by the Na ground-state hyperfine splitting and behave as −$C_6$/R6. The three curves are labeled by the separated atom hyperfine levels: fa+fb. The dotted line indicates the location of the van der Waals length scale $R_{\mathrm{vdW}}$ defined in Eq. (13).

When molecular rotation is added to the picture, one finds that the orbital angular quantum number ℓ is still a good quantum number as discussed for Hund’s case (d) in Sec. II.F. Consequently, to find the potentialenergy curves associated with a particular degree of rotational excitation, one needs only add a term ℏ2 ℓ(ℓ+1)/(2μR2), ignoring very small effects mentioned in Sec. II.F. Figure 12 shows an example of the mixed hyperfine/rotation structure in a weakly bound vibrational level of the ground electronic state of $^{23}\mathrm{Na}_2$. A model calculation of the structure is compared to the observed spectrum. The model assumes that the state is a pure triplet state; small deviations between this prediction and the observed pattern signal that hyperfineinduced mixing of the singletX 1 Σg + and triplet a 3 Σu + states is important here.

### H. Hyperfine interactions in excited states

For the excited states reached by PA spectroscopy hyperfine structure is also important. As before, the molecular hyperfine interaction can be calculated from the atomic one. Here one atom has the excited-state hyperfine structure and one the ground-state structure. Unlike the case of scattering wave functions on the ground electronic states, for bound levels in excited-state potentials, the nonadiabatic couplings are typically small. Here the interesting issue is the competition between rotation and the hyperfine interaction. Ultimately the distinction between ground-state scattering wave functions and wave functions of excited bound states can be traced back to the fact that the ground state has zero electron orbital angular momentum (L=0).

Of most interest for PA spectroscopy are levels close to the 2 S+2 P atomic dissociation limits (see Fig. 8).

Evaluation of the effects of the hyperfine interaction for these states shows that, to first order, states with Ω=0 have no hyperfine structure. Thus, for example, the spectrum of the purely long-range 0g −state of $\mathrm{Na}_2$ shown in Fig. 2 has a J(J+1) rotational progression but no hyperfine splittings [Williams et al. (1996) show that hyperfine structure cannot be ignored for high vibrational levels]. States with Ω>0 have first-order hyperfine structure. An example is the 1g(1/2) component of the 1 3 Σg + state. A sample spectrum is shown in Fig. 13 along with a stick spectrum generated using the model of Williams et al. (1999) originally developed to describe the rotational and hyperfine structure of the $\mathrm{K}_2$ purely longrange 1u(3/2) state. The difference in behavior between Ω=0 and Ω>0 states with regard to hyperfine structure is similar to that encountered earlier for the spin-orbit interaction: Σ states show no spin-orbit splitting while Π states with nonzero spin do.

> [!figure]
> ![[Fig. 12.png|center|500]]
> **Figure 12.** (Color online) Analysis of the hyperfine/rotation structure of the v=14 vibrational level in the $^{23}\mathrm{Na}_2$ lowest triplet (“ground”) state, a 3 Σu +. From top to bottom, the panels show the vibrational position, the hyperfine structure calculated from the known atomic splitting (Fig. 6), the combined effects of rotation and hyperfine, and an experimental spectrum. Rotation simply adds a second copy of the hyperfine pattern, shifted up in energy. Solid lines are ℓ=0, dashed lines are ℓ=2. The hyperfine pattern is calculated assuming that this is a pure triplet state. The lowest (f=2) line in the calculated hyperfine pattern (marked with a small arrow) does not quite match the observed position (indicated by * for each ℓ). This is the signature of singlet-triplet mixing. The data are from the experiment described in the article of de Araujo et al. (2003), which also details the model.

> [!figure]
> ![[Fig. 13.png|center|500]]
> **Figure 13.** (Color online) Analysis of the complex hyperfine/ rotational structure of a vibrational level in the $^{87}\mathrm{Rb}_2$ 1g(1/2) state about 10 cm−1 below the 5 2 S+5 2 P1/2 dissociation limit. Panel (a) shows the vibrational position (set to be zero frequency); panel (b) adds in hyperfine structure given by AvΩ·ι, where Av is a vibrational-level-dependent hyperfine constant, and ι is the projection of the total nuclear spin I along the internuclear axis; panel (c) adds rotation where each line is now labeled by the total angular momentum of the molecule F; and panel (d) is an experimental trap-loss spectrum (Heinzen, 2005). The model is similar to that described by Williams et al., 1999.

For further examples and a theoretical discussion of hyperfine structure, see Abraham, McAlexander, Stoof et al. (1996), Williams et al. (1996, 1999), and Tiesinga et al. (2005).

### I. Selection rules

A knowledge of electric dipole selection rules is important in assigning observed spectra. In PA spectroscopy the initial state and final state are typically in different coupling cases. Still it is possible to establish basic guidelines. The starting point is that the photon carries one unit of angular momentum and consequently the total angular momentum of the two atoms changes by at most one in a PA transition. Further, the photon only acts on the electron orbital degrees of freedom, i.e., it does not directly change the electron spin, nuclear spin, or mechanical rotation of the molecule. For example, for sodium, PA only changes L, from zero in the ground state to one in the excited state.

In bound-bound spectroscopy the familiar selection rule is that the photon couples g states to u states and vice versa. In PA spectroscopy of atoms with hyperfine structure, the initial ground-state collision does not have a definite g/u symmetry so transitions to both g and u excited states are allowed. Likewise the collision does not have a well-defined singlet or triplet character so transitions to both kinds of upper state are allowed.

However, there are still restrictions on allowed transitions. The initial collision is a mixture of 1 Σg + and 3 Σu + only, so that transitions to 1 Πg or 3 Σu + excited states are forbidden.

The low temperatures in ultracold gases lead to a second kind of limitation on excited states that can be observed by PA. As mentioned in Sec. I.D, the number of partial waves in the initial collision that contribute to the PA signal is limited. This in turn limits the maximum angular momentum in the excited state. For example, the purely long-range 0g −(3/2) state described in Sec. II.E has a rotational spectrum described by Hund’s case (c) coupling. It has a rotational progression in J ⃗=ℓ ⃗ +j ⃗. The values of j are found by vector addition of ja and jb from the individual atoms; here ja=1/2 and jb=1/2 or jb =3/2. Since allowed values of j are thus ≤2 and those of ℓ are also ≤2, only J≤4 levels are observable, as seen in the spectrum shown in Fig. 2. In contrast, the 0g −(1/2) state has Hund’s case (e) coupling for vibrational levels bound by less than the atomic fine-structure splitting and only three rotational lines can be observed, namely, ℓ=0, 1, and 2.

A third kind of selection rule occurs for transitions to states of homonuclear dimers with either Λ=0 or Ω=0.

A given rotational line in such a state can be reached from only odd or only even partial waves in the initial collision. The precise relationship, whether odd partial wave goes to odd rotational line or odd goes to even, depends on whether the nuclei are bosons or fermions and whether the state has g or u symmetry. For example, the odd rotational lines of vibrational levels of the $\mathrm{Na}_2$ A 1 Σu +, which has a Hund’s case (a) coupling scheme, can only be observed from even partial-wave collisions. A sample spectrum is shown in Fig. 25. Typically in PA spectra the strongest lines come from s-wave scattering.

This is the case here where the J=1 line is largest. For the $\mathrm{Na}_2$ 0g −(3/2) state (Fig. 2), even rotational lines come from even partial waves and as a result the J=2 feature is largest.

## III. Cold Collisions and Free→Bound Spectra

This section summarizes some basic properties of the initial scattering wave function in a potential in which the 1/R6 van der Waals interaction dominates at long range. In particular, the connection between the nodal pattern of the wave function and scattering length is elucidated. This then leads into the theory of the PA line shape and the evaluation of the transition strength via the “reflection approximation.”

### A. Length and energy scales for a van der Waals potential

In Sec. II.G we have described ground-state scattering and noted that a quantitative treatment requires consideration of the coupling between potentials arising from the combined effects of hyperfine interactions, electrostatic forces, and rotation. Further, for a complete description, one must consider the effects of the shortrange chemical bonding part of the ground-state potentials. Still, much insight into scattering relevant to most PA experiments can be gained from considering a simplified, single-channel problem using only the longrange part of the potential. The effect of the inner, chemically bound part of the potential and the multichannel character can be summarized in a few parameters at an internuclear separation Rbond characterizing the separation outside of which chemical bonding is negligible. Typically this is on the order of 20a0. The main reason such a simplification is possible is that the depth of the 1/R6 van der Waals potential at Rbond is much larger than either the hyperfine or collision energies.

Further, the excited molecular states of interest in PA have outer turning points outside Rbond and, as noted in the discussion of Fig. 3, only the ground-state wave function near this turning point is important for determining PA probabilities.

To specify completely the collision channels for alkalimetal ground-state atoms at low magnetic field requires the quantum numbers famafbmbℓmℓ, where the m values give the projections on a laboratory axis. Since for

S-state atoms all long-range potentials for any combinations of these quantum numbers have the same van der Waals coefficients, and since the PA transition typically is associated with the long-range region (see Fig. 1), we now consider the properties of the dispersion potential in the region beyond Rbond, including only the lead van der Waals term and the centrifugal potential with rota-
$$
V(R)=-\frac{C_6}{R^6}+\frac{\hbar^2}{2\mu}\frac{\ell(\ell+1)}{R^2} \tag{12}
$$
Values of $C_6$ interaction coefficients were tabulated for like alkali-metal atoms by Derevianko et al. (1999), for unlike alkali-metal atoms by Derevianko et al. (2001), and for like alkaline-earth-metal atoms by Porsev and Derevianko (2002). For some systems, such as metastable neon (Doery et al., 1998), the situation is more complicated and a single-channel approach has limitations. Higher-order terms can be included but are not discussed here. Values for some $C_8$ and $C_{10}$ coefficients can be found in the paper by Porsev and Derevianko (2003).

A straightforward consideration of the units in Eq. (12) suggests that it is useful to define length and energy scales $R_{\mathrm{vdW}}$ = 1 2 (2μ$C_6$ ℏ2)1/4 and $E_{\mathrm{vdW}}$ =
$$
R_{\mathrm{vdW}}=\frac{1}{2}\left(\frac{2\mu C_6}{\hbar^2}\right)^{1/4}\quad\text{and}\quad E_{\mathrm{vdW}}=\frac{\hbar^2}{2\mu}\frac{1}{R_{\mathrm{vdW}}^2} \tag{13}
$$
where the 1/2 out front in the definition of $R_{\mathrm{vdW}}$ is chosen for later convenience (Williams et al., 1999). Table I gives the values of $R_{\mathrm{vdW}}$ and $E_{\mathrm{vdW}}$ for several cases. With these definitions, the long-range potential is
$$
\frac{V(R)}{E_{\mathrm{vdW}}}=-\frac{16}{r^6}+\frac{\ell(\ell+1)}{r^2} \tag{14}
$$
where r=R/$R_{\mathrm{vdW}}$. The values of $E_{\mathrm{vdW}}$ are larger than typical temperatures reached by laser cooling, at least for the lighter species in Table I. The outer turning points of excited states easily accessible by PA tend to be of similar size or larger than the van der Waals length $R_{\mathrm{vdW}}$.

Figure 14 shows the long-range potential for the lowest few partial waves. The competition between the van der Waals attraction and the effective potential due to rotation results in a potential-energy barrier of height EC(ℓ) at distance RC(ℓ), except for s waves for which there is no barrier. For a collision energy E less than EC(ℓ), there will be a classical turning point at some R >RC(ℓ). Although there is penetration of the barrier due to quantum-mechanical tunneling, no partial waves other than s waves can contribute to the collision if E is sufficiently close to 0. The position and height of the centrifugal barriers for partial wave ℓ are RC(ℓ) =2{3/[ℓ(ℓ+1)]}1/4 $R_{\mathrm{vdW}}$ and EC(ℓ)= 1 2[ℓ(ℓ+1)/3]3/2 $E_{\mathrm{vdW}}$.

For example, for two colliding sodium atoms, the height of the p-wave and d-wave barriers are 1.0 and 5.3 mK, respectively. Figure 2 shows a PA spectrum at 450 μK.

Its largest feature (J=2) arises principally from s-wave scattering with perhaps a small contribution from d waves. For this state the odd rotational lines must come from odd partial waves (see Sec. II.I), hence here they come from p-wave collisions. The J=4 feature must come from d-wave scattering. This is a consequence of the fact that the total electron angular momentum j is at most 2 so there must be at least two units of initial nuclear rotation to sum to 4. At a temperature of 450 μK, the presence of spectral features arising from d-wave scattering is only possible because of tunneling through the barrier. In fact, for sodium this is a consequence of a “shape resonance” (a quasibound state in the short-range part of the molecular potential; see Sec.

V.I for other examples). For PA in a Bose-condensed gas, the potential barriers are enormous compared to

**Table I.** Characteristic van der Waals scales $R_{\mathrm{vdW}}$ and $E_{\mathrm{vdW}}$ for several atomic species (1 amu = 1/12 mass of a $^{12}$C atom; 1 a.u. = $1E_h a_0^6$, where $E_h = 4.35974\\times10^{-18}\,\\mathrm{J}$ and $a_0=0.0529177\ldots$ nm).

| Species | Mass (amu) | $C_6$ (a.u.) | $R_{\mathrm{vdW}}$ ($a_0$) | $E_{\mathrm{vdW}}/k_B$ (mK) | $E_{\mathrm{vdW}}/h$ (MHz) |
|---|---:|---:|---:|---:|---:|
| $^{6}$Li | 6.0151223 | 1393.39ᵃ | 31.26 | 29.47 | 614.0 |
| $^{23}$Na | 22.9897680 | 1556ᵇ | 44.93 | 3.733 | 77.77 |
| $^{40}$K | 39.9639987 | 3897ᵇ | 64.90 | 1.029 | 21.44 |
| $^{40}$Ca | 39.962591 | 2221ᶜ | 56.39 | 1.363 | 28.40 |
| $^{87}$Rb | 86.909187 | 4691ᵇ | 82.55 | 0.2925 | 6.094 |
| $^{88}$Sr | 87.905616 | 3170ᶜ | 75.06 | 0.3497 | 7.287 |
| $^{133}$Cs | 132.905429 | 6860ᵈ | 101.0 | 0.1279 | 2.665 |

ᵃ Yan et al. (1996).
ᵇ Derevianko et al. (1999).
ᶜ Porsev and Derevianko (2002).
ᵈ Chin et al. (2004).

> [!figure]
> ![[Fig. 14.png|center|500]]
> **Figure 14.** (Color online) The long-range van der Waals potentials for several partial waves. The dots indicate the top of the barrier with height EC(ℓ) at RC(ℓ) defined in the text. As discussed in Sec. III.B, the last s-wave bound state of the potential must lie between the boundaries indicated by the dashed lines, E=0 and E=−39.5...$E_{\mathrm{vdW}}$. The outer classical turning points for all bound vibrational levels except the last must be less than 0.848...$R_{\mathrm{vdW}}$.

collision energies and only s-wave collisions are expected to contribute.

Two alternative approaches to defining a characteristic length for a van der Waals potential arrive at almost the same result as simple scaling (and in fact lead us to include the factor of 1/2 in our definition of $R_{\mathrm{vdW}}$). Gribakin and Flambaum (1993) defined a “mean scattering length” Ā=0.956...$R_{\mathrm{vdW}}$. Julienne and Mies (1989) and Weiner et al. (1999) considered the breakdown of the Wentzel-Kramers-Brillouin (WKB) approximation for low-energy scattering and arrived at a distance RQ =0.99...$R_{\mathrm{vdW}}$. A semiclassical WKB connection between the s-wave scattering function for R≫$R_{\mathrm{vdW}}$ and R ≪$R_{\mathrm{vdW}}$ fails when E is on the order of $E_{\mathrm{vdW}}$ or less.

### B. Near-threshold wave functions and scattering properties

The length $R_{\mathrm{vdW}}$ marks a characteristic internuclear separation where a transition occurs between the asymptotic long-range and short-range behavior of the s-wave scattering wave function when E<$E_{\mathrm{vdW}}$. For these collision energies and R>$R_{\mathrm{vdW}}$, the de Broglie wavelength of the collisional wave function is ≥2π$R_{\mathrm{vdW}}$.

The radial part of this long-range s-wave scattering wave function f(R,E), takes the form (Mott and Massey, 1965;
$$
f(R,E)\to\left(\frac{2\mu}{\pi\hbar^2}\right)^{1/2}\frac{\sin(kR+\eta)}{\sqrt{k}} \tag{15}
$$
where E=ℏ2 k2 /(2μ), η is the collisional phase shift, and the factors ensure normalization per unit energy. At sufficiently low energy, the phase shift η has a very simple energy dependence: η=−kA, where A is the scattering length. Thus once A is known, all of the long-range behavior of the wave function is determined. In particular, 4πℏ2 A/(2μ) characterizes the strength of interactions between atoms in a Bose condensate. Determining A for various collisional systems has been a major goal of PA spectroscopy.

The short-range, R<$R_{\mathrm{vdW}}$, s-wave wave function exhibits multiple oscillations on a scale short compared with $R_{\mathrm{vdW}}$ due to the accelerating effect of the attractive potential. Still, f(R,E) can be written in a phaseamplitude form (Julienne and Mies, 1989; Mies and
$$
f(R,E)=\left(\frac{2\mu}{\pi\hbar^2}\right)^{1/2}\frac{1}{C(E)}a(R,E)\sin\!\left[b(R,E)\right] \tag{16}
$$
If R<$R_{\mathrm{vdW}}$ and V(R) is deep compared to $E_{\mathrm{vdW}}$, a(R,E) and b(R,E) are well approximated by the standard WKB forms: a(R,E)=1/√klocal(R,E) and b(R,E) =∫klocal(R′,E)dR′+π/4, using the local wave number klocal(R,E)=√k2 −2μV(R)/ℏ2. The R-independent normalization factor 1/C(E) relates the WKB wave function to the actual one. Because the magnitude of the potential |V(R)| is large compared to E when R≪$R_{\mathrm{vdW}}$, the local wave number klocal(R,E) is large compared to k and is nearly independent of E. The shape of the wave function [i.e., a(R,E) and b(R,E)] inside $R_{\mathrm{vdW}}$ is thus nearly independent of E. In particular, the positions of the nodes are nearly insensitive to energy. However, the overall amplitude 1/C(E) of the short-range wave function is very sensitive to E. At large E the amplitude 1/C(E) is unity since the WKB approximation is accurate at all R. As E→0 consideration of the solution of the full Schrödinger equation for all internuclear separations (Mies and Raoult, 2000) leads to the form
$$
C(E)^{-2}=k\bar A\left[1+\left(\frac{A}{\bar A}-1\right)^2\right] \tag{17}
$$
where Ā is the mean scattering length defined in the previous section (Gribakin and Flambaum, 1993). The amplitude 1/C(E) varies as √k. This result is consistent with the required general properties of low-energy quantum threshold scattering wave functions and has important implications for the line shapes observed in PA spectra. This point is discussed further in the next section.

> [!figure]
> ![[Fig. 15.png|center|500]]
> **Figure 15.** (Color online) Characteristic long-and short-range forms of the s-wave scattering wave function. Upper panel: Scattering length A=0, for E/$E_{\mathrm{vdW}}$=0.0001, 0.01, and 1 (kRvdW=0.01, 0.1, and 1). The effect of the 1/R6 potential is imperceptible at these distance scales. Lower panel: The threshold s-wave scattering wave functions C(E)f(R,E) as E →0 for R≈$R_{\mathrm{vdW}}$, where the 1/R6 van der Waals potential dominates. The different curves are for different values of A/$R_{\mathrm{vdW}}$. The wave function is truncated at very short range where the detailed behavior is determined by chemical bonding. The solid circles show the location of the last, Nth, node of the zero-energy wave function f(R,0).

Figure 15 illustrates the characteristic long-and shortrange forms of the s-wave scattering wave function. The top panel shows the oscillations on a length scale much larger than $R_{\mathrm{vdW}}$ for three collision energies ≤$E_{\mathrm{vdW}}$. The figure is drawn assuming a scattering length A=0. For A≠0, the nodes of the wave function will shift by A/$R_{\mathrm{vdW}}$ [as long as η=−kA in Eq. (15)]. The shift is negligible on the scale of the figure unless |A| ≳$R_{\mathrm{vdW}}$.

Nevertheless, it is this phase shift of the wave function that determines the scattering properties. The lower panel shows the function C(E)f(R,E) in the E→0 limit for four choices of the scattering length A on a distance scale comparable to $R_{\mathrm{vdW}}$. The wave function is multiplied by C(E) to remove the strong energy dependence and to allow the curves to be shown in a single graph.

The short-range structure shown here is imperceptible in the upper panel.

The position of the node of the short-range wave function f(R,E) in the vicinity of R=$R_{\mathrm{vdW}}$ is very sensitive to A. An experimental determination of the position of this (or any other) node determines the scattering length, provided one knows the potential from this node outwards. As mentioned in the Introduction (Sec. I.E), PA experiments can map the nodal pattern in the ground-state wave function. For the four wave functions shown in the lower panel of Fig. 15, this last node in the zero-energy scattering wave function is indicated with a dot. For any positive energy there will be an infinite number of additional nodes at larger R but typically these will be at very much larger R (see, for example, the E=0.0001EvdW wave function shown in the upper panel).

When the node near $R_{\mathrm{vdW}}$ is labeled by the integer N, then the zero-energy scattering wave function will have N−1 nodes inside this last node. This integer N is also the number of bound states in the potential.

Figure 16 shows the relationship between the location of a node z and the scattering length A for an attractive 1/R6 van der Waals potential (Tiesinga et al., 1996; Crubellier et al., 1999). When A is negative, the last node will lie between approximately 0.848RvdW and 0.998RvdW, whereas if A is positive, it will lie between 0.998RvdW and +∞. This behavior of the node position can also be observed in the lower panel of Fig. 15. The position of the (N−1)th node is constrained to lie between the two vertical dashed lines in Fig. 16.

Not only are the nodal positions uniquely determined by the scattering length but so too is the binding energy of the highest vibrational level in the ground-state potential. Consequently, measurements of the binding energy of the highest vibrational level using two-color PA spectroscopy is an effective alternative strategy for determining scattering lengths. As shown in Fig. 14 and derived by Gao (2000), the binding energy of the highest bound state of a van der Waals potential lies between approximately −39.5EvdW and zero. As A→ +∞, the highest bound state approaches zero energy from below and is to good approximation given by −ℏ2 /[2μ(A −Ā)2 ] (Gribakin and Flambaum, 1993). As A→−∞, the binding energy of the highest bound state approaches its minimum value of −39.5EvdW.

### C. Theory of free→bound spectral line shapes

The PA process is the coupling of a scattering state to a bound state and can readily be treated by resonant scattering theory (Fano, 1961; Mott and Massey, 1965).

The bound state is viewed as a quasibound level embedded in a continuum of free scattering states as shown in Fig. 4(b). This is the approach originally taken by Thorsheim et al. (1987) for cold-atom photoassociation and subsequently developed by others [see, for example, Napolitano et al. (1994) and Bohn and Julienne (1999)]. The strength of the optical coupling between the bound state |b⟩ and collisional state |E, ℓ⟩ at energy E with partial wave ℓ is given by the matrix element Vb(E, ℓ) = (2πI c)1/2 ⟨b|d ⃗ · e
$$
V_b(E,\ell)=\left(\frac{2\pi I}{c}\right)^{1/2}\left\langle b\middle|\vec d\cdot\vec e\middle|E,\ell\right\rangle \tag{18}
$$
where e ⃗ is the polarization vector of the incident light with intensity I, c is the speed of light, and d ⃗ is the R-dependent molecular electric dipole moment. In general, it is necessary to account for the ground-state quantum numbers famafbmbℓmℓ, the excited-state quantum numbers (see Sec. II.F), and the polarization e ⃗ (Tiesinga et al., 1996, 2005; Burke et al., 1999; Williams et al., 1999).

Basic PA line-shape theory can be developed more simply by considering a single ground and excited state with an effective coupling and summing over contributions from the various pairs of quantum numbers. The effective coupling comes from averaging over all collision directions with respect to e ⃗ and projections m of ℓ [see, for example, Machholm et al. (2001)]. This two-state picture describes unsaturated PA spectra quite well and even serves to incorporate some effects of saturation.

> [!figure]
> ![[Fig. 16.png|center|500]]
> **Figure 16.** The relationship between the nodal positions z in the zero-energy s-wave threshold scattering wave function and the scattering length A. If the scattering length is zero, the position of the Nth node is approximately 0.998RvdW. This result is derived from the well-known analytical solutions (Mott and Massey, 1965) for the zero-energy scattering wave function in a van der Waals potential. Adapted from Tiesinga et al., 1996.

The bound state has a finite linewidth Γtot=Γnat +Γb(E, ℓ)+Γo. The first term is due to spontaneous emission [introduced in Eq. (2) and Fig. 1], which sets the natural linewidth of the excited state |b⟩. The second term is due to stimulated decay back into the entrance
$$
\hbar\Gamma_b(E,\ell)=2\pi\left|V_b(E,\ell)\right|^2 \tag{19}
$$
The third term Γo is due to any other processes that leads to decay of the bound state, such as molecular predissociation (Cline et al., 1994; Machholm et al., 2001; Bergeman et al., 2002).

In experiments there will be a detection channel. For example, in the experiment which produced Fig. 2, the detection channel was ionization of molecules out of level |b⟩ by an auxiliary laser. Ionization detection is characterized by a rate Γd, which adds to the width Γo although in practice it is usually made small in comparison to Γnat. Other experiments detect total atom loss, for which Γd=Γnat+Γo. The event rate coefficient for transferring atoms from the entrance channel to the detection channel for collisions with energy E and partial wave ℓ is given by the product of vrelπ/k2 and the squared S-matrix element for the process, where vrel= ℏk/μ is the relative velocity. The total event rate coefficient has the following form (Napolitano et al., 1994; Bohn and
$$
K_d(E)=v_{\mathrm{rel}}\frac{\pi}{k^2}\sum_{\ell}(2\ell+1)\frac{\hbar\Gamma_d\,\hbar\Gamma_b(E,\ell)}{\left[E+h\nu-h\nu_0-S_b(E)\right]^2+\left(\hbar\Gamma_{\mathrm{tot}}/2\right)^2} \tag{20}
$$
where ν is the PA laser frequency, hν0=Eat−Eb (defined in Fig. 1) is the energy of the bound excited state relative to two ground-state atoms at rest, and Sb is the light shift of the resonance position given by Sb(E) = ∑ ℓ′ P ∫|Vb(E′,ℓ′)|2 E −E′
$$
S_b(E)=\sum_{\ell\prime}\mathcal{P}\int \frac{\left|V_b(E\prime,\ell\prime)\right|^2}{E-E\prime}\,dE\prime \tag{21}
$$
Here P implies a principal part integral over the continuum E′>0 and a summation over discrete bound states for E′<0. In experiments designed to make accurate measurements of line positions (i.e., ν0), this intensity-dependent shift must be kept small.

The detection rate constant for an experiment at temperature T is found by averaging Kd(E) over a thermal
$$
K_d(T)=\frac{2}{\sqrt{\pi}}\int_0^\infty \sqrt{E}\,dE\,e^{-E/k_BT}K_d(E) \tag{22}
$$
The experimentally observed signal per unit volume per unit time in a gas of uniform density n is Kd(T)n2, and the number of atoms lost per detection is twice this.

Equations (20) and (22) provide the basis for understanding the line shapes observed in PA spectroscopy.

The lines are asymmetric and the peaks of the lines are shifted slightly from the resonance position ν0. These features are present even at low laser intensity, where Sb is negligible and Γb(E, ℓ)≪Γnat, as we shall assume from here on. The line shape results from the interplay between the energy dependence of Γb(E, ℓ), the prefactor vrelπ/k2 ∝1/E1/2, the exponential thermal energy distribution, and the resonance denominator. In the previous section we noted that the s-wave scattering wave function at moderate separations (around $R_{\mathrm{vdW}}$) has an energy-dependent amplitude proportional to √k as E→0. It is a general feature of low-energy collisional wave functions that the amplitude must go to zero as E→0 and, further, that the way in which it does so depends on the angular momentum. This “Wignerthreshold-law” behavior dictates that Γb(E, ℓ) will be proportional to Eℓ+1/2 as E→0. While this behavior is only guaranteed in the limit that E→0, in many cases of interest the range of validity of this scaling is larger than $k_B T$. This limiting behavior ensures that (vrelπ/k2)Γb(E, ℓ)∝Eℓ, so that this factor in the numerator of Kd(E) vanishes as E→0 for all partial waves with ℓ>0, but is a nonvanishing energy-independent constant as E→0 for s waves.

Figure 17 shows a line shape calculated from Eqs. (20) and (22) assuming that only s-wave collisions contribute and that the Wigner threshold law scaling of the wave function holds for all relevant collision energies. If only a single collision energy were present, the line shape would be a Lorentzian centered at ν=ν0−E/h. Different collision energies contribute other Lorentzians, with a height ∝√E exp(−E/$k_B T$). The largest contribution to the line comes from E=(1/2)$k_B T$. The peak of the integrated line is red of both the resonance position ν0 and v0−(1/2)$k_B T$.

> [!figure]
> ![[Fig. 17.png|center|500]]
> **Figure 17.** The photoassociation line shape vs detuning ν−ν0 (red is negative, blue positive) approximated by summing the contribution from 20 discrete collision energies in Eqs. (20) and (22). For each collision energy the line shape is a Lorentzian, with width Γnat=(2π)×5 MHz and a height proportional to √E exp(−E/$k_B T$). The heavy line is the sum, and the lighter lines are, right to left, the contributions from E/h =2,6,10,14,...,50 MHz with the height multiplied by 2 for clarity. Adapted from Jones et al., 2000.

Contributions arising from other partial waves will similarly be shifted red of the resonance position by an amount that increases with ℓ. In some cases a particular spectral line is dominated by contributions from a single partial wave. Figure 18 shows closeups of the J=2 and J=4 rotational lines shown previously in Fig. 2. The excited molecular state here has Ω=0. As discussed in Sec.

II.I the even rotational lines arise from even ℓ. In particular, the J=2 line arises mostly from s-wave scattering and the J=4 line (which cannot be reached from an s-wave collision) arises mostly from d-wave scattering.

The theoretical fits in Fig. 18 assume that the Wignerthreshold-law scaling Γb(E, ℓ)∝Eℓ+1/2 holds over the entire range of collision energies. This may not be entirely valid, particularly for the d-wave line, hence for purposes of extracting resonance positions ν0 it is best to use data from the blue side of the line. The resonance position ν0 is extracted from the fit and the overall height is adjusted to match the data. More information on fitting PA lines may be found in the article by Jones et al. (2000).

This discussion has been entirely for single-color PA or two-color PA in which the second color simply leads to additional loss from the excited state as in the ionization detection used in Fig. 2. This description, however, breaks down when the second color drives a transition to an additional narrow bound state. The resulting line shapes in that case can be quite complex, but are well described by an extended version of this theory (Bohn and Julienne, 1996, 1999). Examples are given in Sec.

VII.A.

### D. Approximate calculations of line strengths

A very useful approximation for Γb(E, ℓ) can be found by using the stationary phase approximation as is often done in line-shape theory (Jablonski, 1945). In this picture the primary contribution to the integral in Eq. (18) that determines Γb(E, ℓ) comes from the region near the Condon point RC, where the difference between the excited-and ground-state potentials equals the photon energy hν. In photoassociation the Condon point is typically near $R_{\mathrm{vdW}}$ or larger where the groundstate potential is flat (see Fig. 14). In many cases the excited-state potential is a much longer range 1/R3 resonant dipole potential, which is still changing rapidly at the Condon point. In this case the Condon point is essentially the same as the classical outer turning point Rv+ of the excited-state vibration as defined in Figs. 1 and 3.

Since the molecular electric dipole operator d ⃗ is a slowly varying function in the region around RC, the stimulated decay width Γb(E, ℓ) can be simplified from Eqs. (18) and (19) to 2π|VC|2 |⟨b|E, ℓ⟩|2, where VC is evaluated at RC. The Franck-Condon factor |⟨b|E, ℓ⟩|2 is, in the stationary phase approximation, given by (Julienne, 1996; Boisseau et al., 2000)

> [!figure]
> ![[Fig. 18.png|center|500]]
> **Figure 18.** (Color online) Comparison of observed line shapes for two rotational lines in the 0g −(3/2) v=1 vibrational level shown in Fig. 2. For each line the zero frequency is the fitted resonance position ν0. In the fit the linewidth and temperature were held constant while the position and height were fit to the data in a limited region covering the blue side and peak of the line (approximately the region −50 to 50 MHz). The J=2 line is assumed to arise from an initial, free atom, s-wave collision and the J=4 line from a d-wave collision. Note that in comparison to the J=2 line, the J=4 line is broader and peaks further to the red of its threshold.

> [!figure]
> ![[Fig. 19.png|center|500]]
> **Figure 19.** The quantity |⟨b|E, ℓ⟩|2 (∂Eb/∂b)−1 vs RC for s-, p-, and d-wave collisions at E/$k_B$=200 μK using a model potential with a scattering length of 690a0 and using the reduced mass of $^{23}$Na. The lines show the reflection approximation and points show the exact results evaluated for every tenth vibrational level in the excited potential. From Boisseau et al., 2000.

$$
\left|\left\langle b\middle|E,\ell\right\rangle\right|^2=\frac{\partial E_b}{\partial b}\frac{1}{\left|D_C\right|}\left|f_\ell(R_C,E)\right|^2 \tag{23}
$$
Here ∂Eb/∂b is the interval between excited-state vibrational levels b at energy Eb (the inverse density of states), DC is the derivative with respect to R of the difference between excited-and ground-state potentials evaluated at RC, and fℓ(RC,E) is the wave function for the ground-state partial wave ℓ at the Condon point.

This is called the reflection approximation, since the Franck-Condon factor is just a mapping (reflection) of the square of the ground-state wave function at the Condon point.

The reflection approximation has been verified to be an excellent approximation for a wide range of detunings, collision energies, and partial waves in the ultracold domain. Figure 19 shows one example of the high quality of this approximation (Boisseau et al., 2000). As RC decreases, Γb(ℓ,E) and consequently Kb(T) decreases. Thus photoassociation is favored at large Condon points. Figure 19 also shows how the oscillatory behavior of the Franck-Condon factor maps out the nodal structure of the ground-state wave function fℓ(RC,E).

The p-and d-wave contributions are much less than the s-wave at small RC due to the need to tunnel through the centrifugal barrier.

The reflection approximation can also be used to calculate the shift Sb(E), although with less accuracy than the width Γb(E, ℓ) (Bohn and Julienne, 1999). All that is necessary is to replace |fℓ(RC,E)|2 in Eq. (23) by fℓ(RC,E)gℓ(RC,E)/2, where gℓ(R,E) is a linearly independent solution of the Schrödinger equation that satisfies the asymptotic boundary condition in Eq. (15), with sin replaced by −cos. Shifts can also be evaluated by direct calculation of Eq. (21) (Simoni et al., 2002).

Power broadening and light shifts become important if the laser intensity I is sufficiently large. Figure 20 shows how the calculated PA line for a transition in the $\mathrm{Li}_2$ molecule shifts and begins to saturate as I increases in a two-level model. In general, a theoretical understanding of spectra at high intensity requires treating the coupling among several different ground and excited levels and has not yet been fully developed (Simoni et al., 2002; Ribeiro et al., 2004). See Sec. IX.B for a discussion of experimental attempts to investigate high-power effects in Bose condensates.

## IV. Experimental Considerations

### A. Laser cooling and trapping

Critical to the development of PA as a technique for high-resolution spectroscopy was the invention of techniques for cooling a gas of atoms to mK or lower temperatures and the ability to trap or hold a sample of atoms in some way (Chu, 1998; Cohen-Tannoudji, 1998; Phillips, 1998). The first suggestion that spectroscopy could be done via the PA of cold atoms was made by Thorsheim et al. (1987) shortly after the advent of optical molasses and magnetic and optical trapping of neutral atoms.

The prototypical photoassociation experiment starts with ~108 atoms held in a magneto-optical trap (MOT) at a temperature on the order of 0.1 to 1 mK and at a density on the order of 1010 –1011 atoms/cm3 (Weiner et al., 1999). Densities as low as 109 atoms/cm3 have been used for metastable He and as high as 1016 atoms/cm3 for H. Typically the magneto-optical trap is continuously loaded while it is being probed by the PA laser. Under these conditions the maximum possible PA rate, estimated by multiplying the prefactor vrelπ/k2 in Eq. (20) times the density, is ≲1 per second per atom. While this may seem like a low rate, even rates lower than this are quite sufficient for many experiments. Experiments have even been done in a laser-cooled and compressed beam without trapping the atoms (Ramirez-Serrano and Weiner, 2002).

In other experiments, atoms are first transferred from the magneto-optical trap to another “sample holder,” such as a far-off-resonance laser trap (FORT) or a magnetic trap. In these traps the atoms are often spin polarized. In such traps it is possible to achieve higher densities and lower temperatures than in a magneto-optical trap. In particular, experiments with Bose condensates achieve temperatures below 100 nK and densities of 1014 atoms/cm3. Under these conditions the maximum PA rate, estimated as before, is now 105 per atom per second, although in practice such high rates are not actually reached (see Sec. IX.B).

### B. Detection techniques

The simplest technique for detecting that a PA transition has occurred is to monitor the number of atoms remaining in a MOT. This number is a balance between the loading rate and losses. The PA of atoms introduces an additional loss mechanism: the excited molecules formed by PA quickly decay by spontaneous emission to hot atoms that are not recaptured by the trap or to stable molecules that are not trapped. A convenient way to monitor the number of trapped atoms in a MOT is by observing the level of the fluorescence emitted by the atoms as they are continuously bathed in the nearresonant light which forms the MOT. The variation in atom number with the photoassociation laser frequency gives the spectral information. This is referred to as “trap-loss” spectroscopy. One of the strengths of trap loss is that it not only provides frequency positions of PA resonances, but it also carries information about relative transition strengths (Tiesinga et al., 2005), information that is not always available with other techniques such as ionization. A disadvantage of the technique is that the response time of the MOT to a change in the PA loss rate is typically rather slow (~1 s) which requires that the PA laser frequency be scanned slowly. It is also difficult to distinguish weak PA lines from other fluctuations in the atom number.

> [!figure]
> ![[Fig. 20.png|center|500]]
> **Figure 20.** Calculated PA line at 1 mK for the v=64 3 Σg + excited state of $\mathrm{Li}_2$. From Bohn and Julienne, 1999.

Figure 21 is an example of a trap-loss spectrum taken in a MOT containing Ca atoms at 3 mK. The weak PA line strengths led to a variation in atom number of 1% or less. Detecting these small changes required great care to achieve stable MOT conditions and the use of a separate, detection laser to monitor the atom number (Zinner et al., 2000). An interesting variation on the trap-loss technique was demonstrated by Schlöder et al. (2002). In a dual-species MOT containing a large number of $^{6}$Li and a small number of $^{7}$Li atoms, PA to heteronuclear $^{6}$Li-$^{7}$Li dimers was selectively detected. The absorption of a probe laser, slightly detuned from a $^{7}$Li atomic resonance line, was used to monitor the population of $^{7}$Li atoms in the trap as a function of PA laser detuning.

Trap-loss detection can also be used in experiments in FORTs or magnetic traps. In such experiments atoms are loaded into the trap either to a predetermined level or the number of atoms is measured after loading by off-resonant phase-contrast imaging, which only “slightly” disturbs the sample (Hope and Close, 2004).

The photoassociation laser is then introduced for a fixed period, and finally a measurement is made of the number of remaining atoms, often by illuminating atoms with an auxiliary laser tuned to the atomic resonance.

For a PA experiment on a Bose-Einstein condensate (BEC) held in a magnetic trap, the cycle time to produce a condensate and measure the loss rate at one PA frequency is about 30 s, greatly limiting the spectral range over which it is practical to scan. Since the trap is not continuously loaded it is possible to detect weak PA lines by illuminating the trap for a long period of time.

A very sensitive means of detecting molecule formation is ionization detection. Once an excited molecule is formed by photoassociation one can add a second laser, to either resonantly or nonresonantly ionize this molecule before it decays. Molecular ions can be easily counted with high efficiency using a microchannel plate or other ion detector. An example of a spectrum taken this way was shown in Fig. 2. In PA of Na it happens that a single laser can provide both the PA and ionization photons and this single color (but two-photon) ionization process was important in much of the early PA work on Na (Lett et al., 1995). The main advantages of ion detection are that it is a zero background signal and ions are produced promptly so that scan rates can be high. Also, one can take advantage of molecular selection rules in the ionization step to simplify or help identify observed PA resonances. On the other hand, the ionization path complicates the interpretation of the signal. The observed line strengths depend on the (unknown) ionization probability, making a comparison of the intrinsic PA transition strengths of different lines difficult. Some of the problems associated with determining the transition strengths can be reduced by choosing to ionize into a relatively structureless ionization continuum.

Photoassociation to an excited state usually leads to trap loss, however, it is possible that the excited molecule decays mostly back to atoms that are recaptured by the trap. This can occur if the excited potential is very shallow so that the kinetic energy of the bound vibration is small. For the $\mathrm{Na}_2$ 0g −(3/2) purely long-range excited state shown in Fig. 2 for example, the lowest few vibrational levels (including the v=1 level shown) are not detectable by trap loss in a MOT even though higher vibrational levels are readily detected this way. One clever variation on the trap-loss technique gets around this limitation by looking, not at the loss of atoms, but at heating of the atomic cloud. This “bolometric” detection of the PA rate was used by Leonard et al. (2004) to detect PA transitions in a gas of metastable (1s2s 3 S) helium. Their sample was a cloud of about 106 metastable helium atoms held in a magnetic trap at about 5 μK and a density of 1012 –1013 atoms/cm3, just above conditions required to Bose condense the gas. The excited potential investigated (see also Sec. V.E) was so shallow that decay did not lead to any significant trap loss but there was a small heating of the cloud. In a magnetic trap, unlike a magneto-optical trap, there is no active cooling mechanism, which allows this heating to be detected. In practice, after a period of PA, absorption images of the cloud were taken. From the images the temperature and density of the cloud were determined and changes in these quantities as a function of the PA laser tuning produced the spectrum shown in Fig. 22.

> [!figure]
> ![[Fig. 21.png|center|500]]
> **Figure 21.** (Color online) Trap-loss spectrum in ultracold Ca. The fractional trap loss vs the detuning of the PA laser from the atomic dissociation limit. The loss is quite small, ≲1%. The PA lines are vibrational levels in the B 1 Σu + state of $\mathrm{Ca}_2$ near the 4s2 1 S+4s4p 1 P dissociation limit. The nonlinear frequency scale is chosen to give equally spaced vibrational levels. Inset: An enlarged view of the v′=55 resonance. The label v′ counts vibrational levels down from the dissociation limit rather than up from the bottom of the well. From Zinner et al., 2000.

Finally, in some cases it is possible to detect PA transitions by looking for production of excited-state atoms.

Under certain circumstances the molecules produced by PA can, in addition to spontaneous emission, fall apart into one ground-state atom and one excited-state atom, a process known as predissociation. The presence of this excited-state atom can then be selectively detected. Figure 23 shows such a scheme for detecting PA in K to molecular states connected to the 4 2 S1/2+4 2 P3/2 asymptote. If the vibrational level lies higher in energy than the 4 2 S1/2+4 2 P1/2 asymptote, the molecule can predissociate and produce a 4 2 P1/2 atom, which is detected by ionization with an auxiliary laser. A sample spectrum is shown later in Sec. V.C.

## V. Results on Singly Excited States

With this section we begin a “sampler” of experimental results to illustrate the major types of PA experiments done thus far. As noted before, the number of papers is now sufficiently large that complete coverage of all noteworthy work is no longer possible. In particular, we have omitted some of the important early work, much of which can be found in other reviews (Lett et al., 1995; Stwalley and Wang, 1999; Weiner et al., 1999; Masnou-Seeuws and Pillet, 2001). The first three sections of our sampler are primarily concerned with PA as a spectroscopic tool and are organized by the degree of electronic excitation within the molecule. In this section we discuss experiments in which the primary interest is in singly excited states reached by one photon (even if subsequent photons are involved in detecting this transition). The next section discusses experiments in which doubly excited states, reached by absorbing two photons, are the primary focus. The third discusses ground electronic states, reached by two photons, but here with the first driving an upward transition while the second drives a downward transition back to a ground electronic state. Following these three sections, all involving essentially continuous-wave (cw) experiments, we briefly discuss time-resolved experiments. Then we turn to applications of PA that are not, strictly speaking, spectroscopy: formation of ground-state molecules, modification of scattering lengths, and limits on PA rates in a Bose condensate. In the final section we speculate on possible future developments.

### A. A brief note on the early days of photoassociation

The first theoretical discussion of ultracold photoassociation (Thorsheim et al., 1987) brought out the unique features of the problem. The earliest experimental studies (Gould et al., 1988, Lett et al., 1991) grew out of room-temperature associative ionization experiments in sodium (Weiner et al., 1989). At high collision energies the time scales are such that a good description of the associative ionization process is that two Na(3S) atoms are excited to the 3P state by two laser photons, these atoms collide, eject an electron, and remain bound as an excited molecular ion [Na(3S)+γ+Na(3S)+γ→Na(3P) +Na(3P)→$\mathrm{Na}_2$ + +e−]. At the energies associated with laser cooling, however, such a description is not valid. The lifetime of the Na(3P) state is now shorter than the time scale for collisions. Instead, slowly approaching atoms can be directly excited to a molecular state (photoassociation), which in turn, upon absorption of a second photon, produces the molecular ion. Some of the earliest experiments with laser-cooled sodium (Bagnato et al., 1993; Wagshul et al., 1993) concentrated on laser detunings very close to the atomic resonance, where it is hard to distinguish the underlying molecular character, although power-broadened spectra were observed (Lett et al., 1991). Later work, at larger detunings, demonstrated clear molecular spectra in Na ionization (Lett et al., 1993), and independently and by a very different approach, in Rb (Miller et al., 1993), and the field of ultracold photoassociation spectroscopy was born.

> [!figure]
> ![[Fig. 22.png|center|500]]
> **Figure 22.** Bolometric detection of PA in He* held in a magnetic trap at 5 μK. (a) The atom number, (b) the temperature in μK, and (c) the peak optical density, all plotted as a function of the PA laser detuning from the atomic D0 line. Each point represents measurements on a new evaporated cloud after PA pulse illumination, thermalization, and ballistic expansion. Strong heating of the atomic cloud is observed when the PA laser is resonant with a molecular transition. The curve in (b) is a Lorentzian fit to the data with a width of 2.8 MHz. From Leonard et al., 2004.

> [!figure]
> ![[Fig. 23.png|center|500]]
> **Figure 23.** Excitation scheme for fragmentation detection of PA in K. One laser photoassociates atoms to an excited vibrational level above the curve crossing. This state predissociates to form a 4 2 P1/2 atom, which is subsequently ionized and detected. From Wang et al., 1998.

Early work concentrated on identifying the molecular potentials that were seen in PA spectra and extracting $C_3$ coefficients for these potentials. Most of the earliest spectra were of $\mathrm{Li}_2$, $\mathrm{Na}_2$, and $\mathrm{Rb}_2$ molecules and were explored by groups at Rice, NIST, and the University of Texas at Austin, respectively. The observed spectra were assigned to the various attractive molecular potentials discussed in Sec. II.E. An appreciation of the limitations of existing semiclassical tools for extracting long-range coefficients was developed (see Sec. V.F). The theoretical tools necessary for understanding the particular features of PA spectroscopy and for obtaining an accurate description of weakly bound excited vibrational levels were developed. Later additions to the field included the spectroscopy of $\mathrm{K}_2$ by the group at Connecticut and $\mathrm{Cs}_2$ by the group in Orsay (see Stwalley and Wang, 1999 and Masnou-Seeuws and Pillet, 2001).

### B. Measurement of the depth of a molecular potential

As a first example of a PA measurement, and the results which can be derived therefrom, we discuss an experiment in which a simple trap-loss PA measurement can help solve a difficult problem in molecular spectroscopy. Using bound→bound spectroscopy one can measure the relative positions of levels within the molecule but, as noted in Sec. I.C, it is difficult to determine the absolute binding energy of any molecular level relative to the energy of two free atoms at rest. PA spectroscopy of ultracold colliding atoms naturally measures the binding energy of molecular levels relative to free atoms very nearly at rest. When combined with bound→bound measurements of the relative positions of bound molecular levels, a single PA measurement of the binding energy of one of these levels can fix the energy scale for all.

A nice example of this is the precise determination of the dissociation energy (Herzberg, 1950) D0 or the strength of the chemical bond of the $\mathrm{Na}_2$ X 1 Σg + molecular potential as described by Jones, Maleki, et al. (1996).

Figure 24 shows the principle of the measurement.

Bound→bound spectroscopy determines the energy of the v′=165 level of the A 1 Σu + potential relative to the lowest, v=0 level of the ground X 1 Σg + potential. PA spectroscopy, shown in Fig. 25, determines the energy of the v′=165 level of the A 1 Σu + potential relative to two free 3S atoms. The PA part of this measurement was later further improved [see footnote 14 in the paper by de Araujo et al. (2003)] and yielding a dissociation energy D0 of the $\mathrm{Na}_2$ X 1 Σg + state of 5942.6881(48) cm−1.

Note that the uncertainty is quite small, of order 1 part in 106. Combining this measurement with previous spectroscopy of the X state, the depth of the potential De was also determined (Jones, Maleki, et al., 1996; de Araujo et al., 2003).

> [!figure]
> ![[Fig. 24.png|center|500]]
> **Figure 24.** Actual scheme for measuring the dissociation energy D0 of the ground X 1 Σg + potential of $^{23}\mathrm{Na}_2$. The line labeled PA is the free→bound photoassociation measurement, the other lines, 1, 2, and XA, represent bound→bound transitions. From Jones, Maleki, et al., 1996.

> [!figure]
> ![[Fig. 25.png|center|500]]
> **Figure 25.** Trap-loss PA spectrum (Sec. IV.B) showing the transition labeled PA in Fig. 24. The arrow indicates the fitted resonance position of the J=1 rotational line of this v′=165 vibrational level of the $^{23}\mathrm{Na}_2$ A 1 Σu + state using the theory discussed in Sec. III.C. The fitted line shape is for a temperature of $k_B T$/h=6 MHz and a natural linewidth Γnat/(2π)=24 MHz. The fit assumes s-wave scattering and the validity of the Wigner threshold law. Zero frequency is an etalon fringe at 16 954.8749 cm−1. From Jones et al., 1996.

In light of the discussion in Sec. II.E, the v′=165 level of the A 1 Σu + state is more properly denoted by its Hund’s case (c) label 0u + (1/2) as it lies only ≈40 GHz below the 3 2 S+3 2 P1/2 dissociation limit. As shown in Fig. 9, the A 1 Σu + state connects only with the 0u + (1/2) state, and hence experimentally there is no clear distinction between these two. Thus the A-state label is often used for the entire potential. To make a precise measurement of the binding energy it is necessary to consider several details. The rotational structure of this A-state vibrational level is apparent in Fig. 25 and one needs to ensure that the bound→bound and PA spectroscopy are measured to the same rotational line.

Reaching the low rotational levels accessible to PA spectroscopy is actually somewhat of a challenge for the bound→bound part of the experiment. As discussed in Sec. II.H, to first approximation an Ω=0 state does not have hyperfine structure and none is apparent in the spectrum. The J′=1 line dominates the spectrum because it arises from s-wave collisions as discussed in Sec.

II.I. The actual v′=165 J′=1 line position is found by fitting the line shape as described in Sec. III.C. This fitting procedure corrects for the small residual shift in the line position due to the fact that the atoms do not start at rest but instead at energies of order $k_B$×300 μK.

In principle, the experiment could be done more simply by measuring just the indicated PA transition and a single bound→bound transition (X 1 Σg + v=0→A 1 Σu + v′=165). In practice this is not practical since this latter transition is very weak. Likewise it is not practical to photoassociate to a much lower vibrational level in the A state, which could be directly reached from the X-state v=0 level since the strength of PA transitions drops with detuning from atomic resonance (see Fig. 19).

In general, vibrational states which are easily accessible by PA spectroscopy tend not to be easily accessible from the X-state v=0 level. This is a consequence of the very different character of the free-atom collisional wave function and the tightly bound X-state v=0 level. Details such as these complicate the practical realization of the experiment, but the principle of the measurement is quite simple.

### C. Broad spectral maps

Our first example relied on measurement of a single PA line and many of our other examples will depend on close-up examination of a few lines. This presupposes that one has a broad “map” which assigns lines to the correct molecular states. In the study of any new system this is always the first task facing the spectroscopist. Examples of alkali-metal spectra and their identification can be found in earlier reviews (Lett et al., 1995; Stwalley and Wang, 1999; Weiner et al., 1999). Here, in Fig. 26, we show one example of a broad-ranging spectrum in $^{39}$K, which starts with the PA laser tuned to the atomic dissociation limit and then scans down through a long series of vibrational levels (Wang et al., 1998). We shall not go through the process of how one could definitively assign the observed lines, but the example provides a picture of the broad-ranging maps that lie behind some of the other close-up examples we shall show later.

> [!figure]
> ![[Fig. 26.png|center|500]]
> **Figure 26.** Fragmentation (lower) and trap-loss (upper) spectra of the predissociated longrange 1g and 0u + states of $^{39}\mathrm{K}_2$. The fragmentation spectrum is produced using the scheme shown in Fig. 23. The inset in (c) details the line broadening of the eight vibrational levels in the dashed rectangle. From Wang et al., 1998.

The top trace in each panel of Fig. 26 shows a traploss spectrum. Near the atomic dissociation limit [bottom panel (c), right side] the vibrational levels become very dense. In the last ≈1 cm−1 the PA laser pushes atoms out of the trap distorting the signal. Two different molecular states contribute to this trap-loss signal, as can be inferred from the pattern of alternating weak and strong lines in the lower panel. The authors assign these as the attractive 1g(3/2) and 0u + (3/2), respectively (see Fig. 8).

The lower trace in each panel of Fig. 26 is a record of 4 2 P1/2 atom production detected using the ionization scheme shown earlier in Fig. 23. This fragmentation spectroscopy identifies molecular states which predissociate. Having this second detection method clearly distinguishes between the two vibrational series. In panel (c) it can clearly be seen that only one of the two states, the 0u +, predissociates. Actually the full story is more complicated as can be seen in the other panels. In the middle panel both states show predissociation for part of the scan while in panel (a), only the 1g predissociates.

The abrupt onset of the fragmentation signal for 1g levels at v=91 (top panel) gives information about the location of the curve crossing, which gives rise to the predissociation. The observed linewidths of the 0u + levels [inset of panel (c)] provide information on the strength of the interactions giving rise to the predissociation of the 0u +.

### D. Modeling of observed spectra

The spectra of vibrational levels near the dissociation limits often show an extraordinary complexity. An example was shown in Fig. 13. A simple vibrational line is split by the hyperfine interaction and further complicated by the rotation of the molecule. The resulting “tulip field” of lines with different splittings and intensities in the data is quite daunting, although in its way quite beautiful. Theoretical progress in matching such spectra, however, has actually been rather astonishing. The stick figure indicating the theoretical line positions in the third panel of Fig. 13 reproduces the observed line positions remarkably well.

The line positions, of course, are not the only quantities that need to be reproduced in order to fully model the spectra. Line intensities must also be reproduced.

These depend on the ground-state scattering wave function, the excited bound-state wave function, and the dipole moment between the ground and electronic states.

While a single-channel approximation is sometimes adequate, state-of-the-art calculations use multichannel wave functions, which include all relevant spin couplings [see, for example, Tiesinga et al. (2005)].

Figure 27 shows a PA spectrum of one vibrational level in each of the $\mathrm{Na}_2$ 1g(1/2) and 0g −(1/2) potentials (see Fig. 8) just below the S1/2+P1/2 dissociation limit.

Detection is by means of ionization. The 1g(1/2) state shows mixed hyperfine/rotation structure while the 0g −(1/2) state shows a simple Hund’s case (e) rotational progression as indicated in the figure. The accompanying theoretical spectrum has been calculated by a full multichannel treatment of the ground and excited states.

Once line positions and transition dipoles have been calculated, the thermally averaged line shape is calculated using Eq. (22). The overall vibrational position of the theory has been adjusted to match the observed position since this position depends on details of the chemically bound portion of the well, which is not known with high accuracy. The line intensities and relative positions depend almost exclusively on the long-range parts of the potentials, which are accurately known.

Modeling is made more complex by the extent to which individual states are coupled to neighboring states. The sheer number of levels in the small spectral region near the dissociation limit often forces the theoretical model to take account of couplings between states. An example of this is shown in Fig. 28 for PA of Na, detected by trap loss, approximately 42 GHz below the 3 2 S+3 2 P3/2 dissociation limit. In this spectral region there are three vibrational levels, one each in the 0u + (3/2), 1g(3/2), and 0g −(3/2) potentials (Fig. 10). This latter is the v=2 level; an ionization spectrum of the v =1 level of the 0g −(3/2) potential was shown earlier in Fig. 2. While the 0g −(3/2) level has a simple Hund’s case (c) rotational pattern dominated by a single strong line, the other two states exhibit complex patterns not easily deciphered.

> [!figure]
> ![[Fig. 27.png|center|500]]
> **Figure 27.** (Color online) PA spectrum of $^{23}$Na in a dark-spot MOT at 300 μK. One vibrational level of each of the 1g(1/2) and 0g −(1/2) potentials is shown. The zero frequency is at the 3 2 S(f=2)+32 P1/2(f=2) atomic dissociation limit. The detection is via ionization by a second color laser, which modifies the relative heights of the 1g(1/2) and 0g −(1/2) features. The overall height of each piece—the 1g(1/2) and the 0g −(1/2)—has been separately scaled to match the theory. The lower trace is a theoretical calculation using a full many-channel treatment for the calculation of the transition dipole moments.

Two calculated spectra are shown in traces (b) and (c) of Fig. 28. Note that in trace (c) the 0u + (3/2) feature is predicted to have a rotational pattern, while in trace (b) it has a set of nearly equally spaced lines. In (c) the line strength of the 1g(3/2) and 0u + (3/2) features are comparable, while in (b) the 0u + (3/2) is much stronger. Despite the dramatic difference in the predictions, the only adjustment between the two calculations is the vibrational position of the 0u + (3/2) and 1g(3/2) vibrational levels. In (c) the 1g sits below the 0u + while in (b) they are reversed.

That this small change in placement has a dramatic effect on the pattern is a consequence of the direct hyperfine coupling between these states and the fact that the potentials (see Fig. 10) are nearly degenerate, ensuring a good wave-function overlap. The calculation in (b) is a good match to the experiment. Since the spectrum is taken by trap loss, no correction is required for relative ionization probabilities.

The models which are able to fully reproduce these kinds of complex spectral patterns are themselves quite complex. Still, the basic starting point is the physicists’ molecule picture, that is, the view of the molecule as a pair of essentially unperturbed atoms that only interact by long-range forces, at least over the distance ranges primarily responsible for the observed PA spectra.

Short-range effects are taken into account by a few parameters: adjustable vibrational defects and scattering lengths. The complexity of the models lies in the necessity of describing all of the coupled angular momenta— electron orbit, spin, nuclear spin, and rotation—in a multichannel treatment.

### E. Purely long-range states

Perhaps the single most interesting application of PA spectroscopy has been the detailed investigation of purely long-range molecular states. As discussed in Sec.

II.E, vibrational levels in these molecular states have both inner and outer turning points at much larger internuclear separations than typical chemically bound potentials. Particularly for lighter alkali-metal atoms, the atoms stay sufficiently far apart that electron-cloud overlap between the atoms plays essentially no role in the binding. Thus they are almost ideal examples of what we have called the physicists’ molecule in which molecular properties are traceable, with high accuracy, to a few properties of the two constituent atoms. The study of these purely long-range potentials grew out of detailed studies of small asymmetries in the wings of atomic absorption lines. The intriguing possibility of observing the spectra of bound levels in these potentials (Movre and Pichler, 1977) was anticipated by Stwalley et al. (1978).

Resolved spectra of these bound states came only with the development of laser cooling and PA spectroscopy.

Figure 29 shows the purely long-range 0g −(3/2) potential for all of the alkali metals, whose origin was discussed in Sec. II.E. The figure shows the wells computed at two levels of approximation. For heavier atoms, terms beyond the $C_3$/R3 resonant dipole interaction are significant and electron-cloud overlap also plays an increasing role.

Figure 30 shows a PA spectrum of the lowest, v=0, vibrational level of the 23 Na20g −(3/2) state. The spectrum shows a simple Hund’s case (c) rotational progression with a rotational constant of ≈0.030 GHz, roughly 0.6% of that of the v=0 level of the X state of $\mathrm{Na}_2$. This small rotational constant is a consequence of the large (≈70a0) equilibrium position of the potential well. PA spectroscopy permits a precise determination of the binding energies, for example, the measured binding energy of the J=2 rotational level is 54.208(5) GHz below the atomic 3 2 S(f=2)+3 2 P3/2(f=3) asymptote. Despite the simplicity of the spectrum, it carries a great deal of information, which we discuss in the following.

> [!figure]
> ![[Fig. 28.png|center|500]]
> **Figure 28.** (Color online) (a) PA spectrum of $^{23}$Na in a dark-spot MOT at 450 μK detected by trap loss. The zero frequency is at the 3 2 S(f=2)+32 P3/2(f=3) atomic dissociation limit. (b) A theoretical calculation where the vibrational defects have been adjusted to match the experiment. (c) A calculation using the same model but with slightly different vibrational defects so that the 1g and 0u + features switch positions. From Tiesinga et al., 2005.

> [!figure]
> ![[Fig. 29.png|center|500]]
> **Figure 29.** The 0g −(3/2) potential curve for various alkali-metal dimers calculated using the Movre-Pichler model (Sec. II.E) describing the electrostatic interaction with R−3, R−6, and R−8 terms. For $\mathrm{Rb}_2$ and $\mathrm{Cs}_2$, the curves obtained by including only the R−3 term are also shown (closed circles). No such differences are visible for $\mathrm{Na}_2$ or $\mathrm{K}_2$ on the scale of the figure. From Fioretti et al., 1999.

The first interesting feature of the spectrum in Fig. 30 is the position of the lines. In the simplest picture, the 0g −(3/2) state is determined by two parameters, the atomic P3/2–P1/2 fine-structure splitting Δ which, for present purposes, is known exactly, and the $C_3$ coefficient which, in turn, is inversely proportional to the radiative lifetime of the Na 3P state, as noted in Eq. (6).

The calculation of Sec. II.E shows that the depth of the 0g −(3/2) state is independent of $C_3$ and is given by Δ/9.

The $C_3$ coefficient determines the curvature of the well and thus the zero-point energy of the v=0 level, but even a moderately accurate value of $C_3$ suffices to accurately predict the expected binding energy of the v=0 level. This does not agree with the observed position. To explain the observed line position in Fig. 30 it is necessary to include several corrections (Jones, Julienne, et al., 1996). The most interesting, and unexpected, was the importance of retardation corrections to the resonant dipole interaction, that is, the modification of the interatomic potential due to the finite propagation speed of light.

The retardation corrections to the resonant dipole interaction can be understood from the simple classical model invoked in Sec. II.C. Picture two electric dipoles separated by a distance R, oscillating in phase at frequency ν, let us say in a direction perpendicular to the molecular axis. Thus configured the interaction between the dipoles is repulsive, +$C_3$/R3. If the dipoles are oscillating 180° out of phase, the interaction is attractive, −$C_3$/R3. These two classical orientations correspond to the two Π states in the Movre-Pichler model (Sec. II.E).

The effect of the finite speed of light is to introduce a phase delay of φ=2πν(R/c) in the signal passing between the two dipoles, where c is the speed of light.

Although at the equilibrium position of the $\mathrm{Na}_2$ 0g −(3/2) potential the time R/c is a mere ≈10−17 s, the atomic oscillation frequency is sufficiently high that φ is of order 0.04 rad. The naive expectation is that this phase delay will make the in-phase (repulsive) state look slightly more like the out-of-phase (attractive) state and vice versa. This is indeed the case and the actual resonant dipole interactions, with retardation included, become (to lowest order in φ) ±($C_3$/R3)(1−φ2 /2). When applied to two dipoles oscillating along the internuclear axis (Σ states in the Movre-Pichler model) the naive argument gives the right magnitude correction but the wrong sign. A straightforward classical calculation, correctly accounting for the retarded Coulomb interaction, near-field, and radiation terms, shows that the actual interaction (to lowest order in φ) is ±(2C3/R3)(1+φ2 /2).

The effects of retardation are easily included in the Movre-Pichler model for the 0g −potentials [Eq. (11)] by replacing the resonant dipole interaction used there with the corrected form including retardation. Subsequent calculation of the 0g −(3/2) potential shows that the depth of the potential is increased by retardation. The magnitude of the correction near the equilibrium position of the $\mathrm{Na}_2$ 0g −(3/2) potential is 123 MHz, as shown in Fig.

30 by the dashed curve. Clearly such a large shift is readily detected and, in retrospect, this is an almost ideal system for detecting retardation corrections to molecular bonding. The key to detecting this retardation correction is not that the effect is particularly large, but rather that we are able to calculate quite precisely just where the level would be if c were infinite.

When the spectrum of Fig. 30 is compared with that of the next few higher levels (the spectrum of the v=1 level was shown earlier in Fig. 2), an interesting difference becomes apparent. In the spectrum of the v=0 level the odd rotational lines—which arise from p-wave scattering (see Sec. II.I)—are suppressed relative to those lines in the higher vibrational levels. This indicates that the ground-state p-wave wave function happens to have a node at about the equilibrium position of the 0g −(3/2) potential. As discussed briefly in Sec. I.E and in more detail in Sec. V.I, locating a node in the scattering wave function allows determination of the scattering length.

Finally, a careful measurement of the vibrational level spacing in the 0g −(3/2) potential yields the value of the $C_3$ coefficient and thus the atomic radiative lifetime.

What is perhaps surprising is that the accuracy with which the atomic lifetime can be determined from this molecular measurement is quite high, exceeding or matching that of other more obvious experimental techniques. For sodium, the 3P3/2 lifetime as determined by this technique is 16.230(16) ns.

The 0g −(3/2) purely long-range state becomes “less pure” for the heavier alkali-metal dimers. As the well moves towards shorter range (Fig. 29), effects of electron-cloud overlap become more important. While this complicates the picture somewhat, the same basic experimental and theoretical strategies have been successfully applied to explore the 0g −(3/2) states of alkali dimers from $\mathrm{Na}_2$ through $\mathrm{Cs}_2$. For $\mathrm{Cs}_2$, the effects of chemical bonding are particularly pronounced and lead to an interesting double-well structure, features of which have proved useful for producing ground-state molecules (see Sec. IX.A). Experiments and analysis may be found in the articles of Wang, Wang, et al. (1997) for $^{39}$K, Gutterres et al. (2002) for $^{87}$Rb, and Masnou-Seeuws and Pillet (2001) and Amiot et al. (2002) for $^{133}$Cs. Precise (≤0.3%) lifetimes for the lowest P state of the atoms are determined.

> [!figure]
> ![[Fig. 30.png|center|500]]
> **Figure 30.** (Color online) PA spectrum of the lowest level, v=0, of the 0g −(3/2) purely long-range potential of $^{23}\mathrm{Na}_2$ detected by ionization. The solid curve through the experimental points applies the theory of Sec. III.C. The dashed line shows the fit shifted to simulate what would happen if retardation were not present. Adapted from Jones, Julienne, et al., 1996.

Figure 10 shows that there is a purely long-range 1u(3/2) state, which is even longer range than the 0g −(3/2) state. Spectra have been obtained for $^{39}$K (Williams et al., 1999) and $^{133}$Cs (Comparat et al., 2000).

These states show complicated patterns of hyperfine/ rotation lines, but analysis using an extended Movre-Pichler model has been quite fruitful. The longest-range purely long-range state observed to date is not in an alkali-metal dimer, but in a metastable helium dimer; see Sec. V.H.

### F. Determining Cn coefficients and atomic lifetimes

A feature of PA spectroscopy that is at first curious is its use to extract precise atomic lifetimes from molecular spectra taken near dissociation. Accurate spectroscopy of vibrational progressions in diatomic molecules, coupled with a good value of the dissociation limit for the potential in question, can be used to extract longrange Cn coefficients. In the case of the resonant dipole interaction, a determination of $C_3$ leads directly to the atomic lifetime value using Eq. (6), as illustrated in the previous section. It is not necessary to use a purely longrange state for this. For example, McAlexander et al. (1996) determined an extremely accurate (0.03%) value for the lifetime of the $^{7}$Li (2P) state from an analysis of levels in the deeply bound A 1 Σu + state. This is, in fact, the most accurate atomic lifetime determination from PA spectroscopy and resolved a lingering discrepancy between theory and experiment. Such lifetime determinations provide a useful check on more conventional atomic experiments since potential systematic errors are quite different.

An accurate determination of an atomic lifetime requires an accurate determination of $C_3$. In the examples cited in the previous section on purely long-range states, the authors constructed molecular potentials such that a quantum-mechanical determination of the bound levels reproduced the observed data. For deeper potentials, constructing a model potential which covers the entire range of internuclear separation is more difficult, although possible as shown by McAlexander et al. (1996).

An appealing, simpler, alternative for extracting longrange coefficients is to use the well-known semiclassical LeRoy-Bernstein analysis (LeRoy and Bernstein, 1970; Stwalley, 1970). This approach is very useful for initial analysis of data to check for consistency, but can lead to an overly optimistic estimate of the uncertainty in a $C_3$ determination if not used carefully. For a potential, given at long range by
$$
V(R)=D-\frac{C_3}{R^3} \tag{24}
$$
where D is the dissociation limit, a semiclassical analysis leads to an expression relating the binding energy, D−Ev, and quantum number v of each vibrational level,
$$
v-v_D=H_3^{-1}(D-E_v)^{1/6} \tag{25}
$$
where vD is the effective (noninteger) vibrational quantum number at dissociation and H3 is a known numerical factor proportional to $C_3$ −1/3. This formula can then be used to extract $C_3$ from the binding energies and, by Eq. (6), the atomic lifetime.

Comparat (2004) has performed an analysis of the accuracy of this simple LeRoy-Bernstein formula, as well as extensions to this formula. For the particular example he has considered, use of Eq. (25) can easily give discrepancies of 5% or more in determining $C_3$. This may be an extreme case but suggests that care must be taken.

This is consistent with our own tests on a different potential. Creating a potential with only a $C_3$/R3 term at long range, extracting bound-state energies, and putting them into Eq. (25) reproduces the input $C_3$ only to about 1%, even when the statistical fit to Eq. (25) was apparently better than this. In addition, splitting the energy range into, say, upper and lower half ranges and doing the extraction separately on these two pieces can lead to “statistically” different $C_3$ values from the two parts. In addition, higher-order corrections to Eq. (24) are a further complication that must be considered. These calculations suggest that error bounds derived from application of Eq. (25) are likely to be unrealistically small when applied to analysis of precise PA spectroscopy. A quantum-mechanical integration of the most accurate potentials, with corrections such as retardation (which are not simple power-law corrections) included, is the only real check on the accuracy of such lifetime extractions, although reasonable extensions of semiclassical methods may be applicable over some parameter ranges (Comparat, 2004).

### G. Mixed alkalis

Photoassociation in a gas containing a single species of atoms inevitably produces a homonuclear molecule.

PA in a gas with two species of atoms allows one to produce heteronuclear molecules. Cooling and trapping two species simultaneously is more technically challenging than working with a single species. Typically, each atomic species requires a separate laser system and optics. Early mixed alkali-metal PA experiments concentrated on developing the technology of dual species magneto-optical traps (MOTs) and detected molecules produced by PA induced by MOT lasers. Early examples of such experiments included the production of NaK (Santos et al., 1995) and of NaCs (Shaffer et al., 1999).

Molecules formed by PA are typically ionized and mass analyzed by time-of-flight techniques to positively identify heteronuclear molecules. Subsequently many other pairs of alkali-metal dimers have been produced in this way (Weiner et al., 1999).

The driving interest behind most mixed-species experiments appears to be the promise of producing samples of cold molecules with permanent dipole moments, which can be manipulated with external fields.

Such molecules might be used to investigate limits on the electric dipole moment of the electron, to investigate novel quantum degenerate gases in which dipole-dipole forces act between the molecules, or possibly, when held in an optical lattice, be used as qubits in a quantum computer.

One general feature of homonuclear diatomic molecules is that singly excited states are generally 1/R3 in character at long range. On the other hand, for heteronuclear diatomic molecules excited states are generally 1/R6 in character at long range. Since in this case both ground and excited states are 1/R6 in character, the Franck-Condon overlap between the collisional and bound excited-state wave functions tends to be larger than for homonuclear systems. Typically, the reflection approximation for the Franck-Condon factor discussed in Sec. III.D breaks down for PA of heteronuclear systems and thus mapping of nodal patterns to extract a scattering length as in Sec. V.I is not straightforward.

The difference in long-range behavior also implies much smaller internuclear separations for the outer turning points of excited vibrational wave functions in heteronuclear transitions when compared to homonuclear ones. Further, heteronuclear dimers have a much lower density of states than homonuclear dimers.

Several mixed-alkali experiments have generated spectra of excited molecular states. Schlöder et al. (2002) performed very high signal-to-noise trap-loss spectroscopy on a mixed-isotope sample of fermionic $^{6}$Li and bosonic $^{7}$Li, thereby producing fermionic $^{6}$Li-$^{7}$Li molecules. Due to the large transition moments, the system is also a candidate for coherent control experiments aimed toward the formation of particular target states of the molecule. The spectroscopy was performed in overlapped MOTs containing a large amount of the $^{6}$Li isotope and a small amount of the $^{7}$Li isotope. The large asymmetry in the populations allows for an analytic solution of the rate equations for the loss. $^{6}$Li is seen as a relatively constant background, and $^{7}$Li-$^{7}$Li collisions are rare, so that the PA rate is easily extracted from the signal. The authors performed absorption measurements with a lock-in amplifier on the $^{7}$Li sample, seeing relatively large changes in its population as the modulated PA laser is scanned. The authors found that the transition rate saturates with intensity (see Sec. IX.B). Saturation intensities around 40 W/cm2 were observed for several transitions—low enough to perhaps encourage coherent control experiments in such samples.

The most extensive PA spectroscopy of a mixedspecies system has been that done on KRb (Wang et al., 2004). The potential curves for this molecule are shown in Fig. 31 and have the interesting feature, common to all mixed alkali-metal systems, that the potentials that asymptotically approach the lower two asymptotes are attractive, while those that approach the upper two are (with a few exceptions) repulsive. As a result these systems do not have the purely long-range states found in single-species systems. The authors have identified vibrational levels in all eight attractive potentials; see Fig.

32. In addition, they have formed and trapped stable KRb molecules in the a 3 Σ+ state. The molecules were formed from spontaneous decay after PA and were trapped in the magnetic-field gradient of the MOT. This heteronuclear molecule has quickly become one of the most completely studied species in the PA field.

In another promising experimental effort in mixed alkalis, RbCs has been photoassociated by Kerman et al.

(2004a), and high signal-to-noise trap-loss spectra of RbCs* have been reported. Polar RbCs molecules are considered for tests of fundamental symmetries (electric dipole moment), and a ~100 μK $^{85}$Rb-$^{133}$Cs dual MOT was used as it is a colder source than currently available from buffer gases or Stark slowing. RbCs* spectral lines appear as dips that occur simultaneously in independent monitors of Rb and Cs fluorescence. In addition, large dc Stark shifts have been observed in the spectra. Splittings and shifts on the order of 100 MHz in size have been measured for fields of 390 V/cm, confirming the highly polar nature of these molecules. These experiments take advantage of the strong transitions (favorable Franck-Condon factors) available in heteronuclear systems to produce copious numbers of molecules. Molecule production in the lowest triplet state and the spectroscopy of these molecules was also investigated and is discussed in the article by Kerman et al. (2004b).

> [!figure]
> ![[Fig. 31.png|center|500]]
> **Figure 31.** The 16 excited relativistic adiabatic potential curves of the KRb molecule, showing that all eight of the potentials that dissociate to the lower two asymptotes are attractive and all eight of those dissociating to the upper two asymptotes are repulsive (1 Å=0.1 nm). From Wang and Stwalley, 1998.

> [!figure]
> ![[Fig. 32.png|center|500]]
> **Figure 32.** Photoassociation spectrum for 39 K85 Rb showing eight vibrational bands from seven electronic states. A preliminary state number and Ω± symmetry is given for each band. Also given above each symmetry label is 103 Bv in cm−1. From Wang et al., 2004.

### H. Other atoms

Recent years have seen a growing variety of species other than alkali metals successfully laser cooled, and atoms such as Yb and Cr have even been Bose condensed. Group-II species are of special interest because they have extremely narrow intercombination lines with potential for application in ultraprecise opticalfrequency atomic clocks (Wilpers et al., 2002). Spin-zero isotopes are of particular interest as optical transitions are, to first order, independent of magnetic fields. Thus it is natural that the PA technique is being extended to these atoms. Calcium is one example (Zinner et al., 2000; Degenhardt et al., 2003) that we have already discussed in Sec. IV.B and a spectrum was shown in Fig. 21.

Group-II species like Ca can be photoassociated from the 1 Σg + molecular ground state on a strongly allowed transition to the excited 1 Σu + state with a long-range potential varying as $C_3$/R3.

While alkali-metal atoms often have spectra that are dominated by complex hyperfine structure, alkalineearth (group-II) elements like Ca have spin-zero isotopes that have no hyperfine structure. While this limits their ability to be laser cooled using polarizationgradient cooling techniques, narrow intercombination transitions can be used to bring samples to low temperatures with simple Doppler cooling. While the lack of spin prevents these isotopes from being magnetically trapped, optical trapping is still a viable option, and techniques like evaporative cooling are not limited by the lack of spin.

Machholm et al. (2001) surveyed key issues for group-II PA spectroscopy and calculated model PA spectra for several group-II species and Yb, although the absence of molecular data prevented quantitative calculations. The PA lines going to the 1 Σu + (1 P1+1 S0) state can be broadened due to predissociation caused by a variety of curve crossings with other molecular states.

Ciuryło et al. (2004) have predicted extremely narrow PA transitions to 1u and 0u + (3 P1+1 S0) states just to the red of the atomic intercombination line. These excited potentials have dominant 1/R6 van der Waals character at large R and thus many fewer lines, and they are excited at much shorter distances than for transitions to the allowed 1 Σu + state. The narrow lines are Doppler broadened. These authors have developed the generalization of the line-shape expression in Eq. (20) to incorporate effects of Doppler broadening and the recoil of the atom due to photon scattering. Ciuryło et al. (2005) have showed how group-II intercombination lines offer good prospects for optical control of ground-state scattering properties, as discussed in Sec. IX.D.

Recently PA of another alkaline-earth element, $^{88}$Sr, has been reported by Nagel et al. (2005). By performing PA in a MOT operating on a narrow intercombination line, Doppler temperatures of about 5 μK have been achieved. PA transitions to the 1 Σu + (1S0+1 P1) potential in the detuning range 0.6–2.4 GHz have been observed.

Their analysis includes retardation shifts on the order of 100 MHz and they have obtained a radiative lifetime for the atomic 5p 1 P1 state of 5.22(3) ns. Yasuda et al. (2006) have also reported PA in $^{88}$Sr and have extracted a lifetime of 5.263(4) ns for this state based on a Leroy-Bernstein analysis (see Sec. V.F) of a series of molecular energy levels observed by PA spectroscopy. In addition, Mickelson et al. (2005) have reported PA spectra of both 86 Sr and $^{88}$Sr to determine bounds on the s-wave scattering lengths of 610a0<a86<2300a0 for 86 Sr and −1a0 <a88<13a0 for $^{88}$Sr.

Another example of a spin-zero system for which PA spectroscopy has been reported is 174 Yb (Takasu et al., 2004). Yb is a lanthanide rare-earth atom whose structure is similar to that of an alkaline-earth atom, and the spinless isotope 174 Yb has been shown to undergo Bose-Einstein condensation using all-optical methods of cooling and trapping. One interesting feature of Yb is that five bosonic and two fermionic isotopes exist with reasonable abundances. This allows one to contemplate mixed Bose-Fermi gas samples and efficient sympathetic cooling. Takasu et al. (2004) have used an allowed transition at 399 nm for slowing 174 Yb and an intercombination line at 556 nm for trapping in a MOT. Using a PA laser at ≈399 nm, they have measured a series of approximately 80 vibrational levels in the lowest 1 Σu + state of 174 $\mathrm{Yb}_2$, over a range of 490 GHz. The PA transitions have been detected by observing the loss of atoms held in a far-off-resonance laser trap (FORT). Rather broad linewidths (~2.2 GHz) have been observed. These PA data were used to make a determination of the radiative lifetime of the atomic (6s6p) 1 P1 state using the LeRoy-Bernstein approach (see Sec. V.F).

Other “exotic” species, such as hydrogen and metastable helium, have their own special features. Hydrogen, of course, is the simplest system to calculate—but far from the simplest to deal with experimentally. PA spectroscopy of magnetically trapped, spin-polarized H was reported by Mosk et al. (1999). The laser cooling of H has not been possible up to now because of the ex-

treme difficulty of creating the 121-nm radiation required. In this case the sample was buffer-gas cooled by He in a magnetic trap. Large samples with densities of 1016 atoms/cm3 and temperatures of 0.15 K were used.

Detection of the PA transitions was by both lightinduced fluorescence and direct absorption of the light near 121 nm, as shown in Fig. 33. Three vibrational states in the excited a 3 Σg + potential were observed.

Two groups have obtained PA spectra of metastable He (Herschbach et al., 2000; Leonard et al., 2004). Laser cooling of metastable noble gases is similar to laser cooling of alkali atoms even though the atoms carry a large amount of internal energy (20 eV for He). Making high density samples of metastable He requires that atoms be spin polarized to prevent release of this internal energy by collisions. PA of metastable helium forms the longestrange purely long-range molecular states of any species yet investigated. Figure 34 shows potentials calculated by an extension of the Movre-Pichler model of Sec. II.E.

Herschbach et al. (2000) investigated PA resonances lying to the red of the 2 3 S1→2 3 P2 transition using an unpolarized sample in a MOT at ≈1 mK with densities of ≈5×109 atoms/cm3. Molecules formed by PA readily autoionize and result in an increase in ion counts coming out of their MOT. The mechanism for the increased ion production is not known, but the authors speculated on a possible state-mixing mechanism near a curve crossing.

Three series of resonances were observed.

Leonard et al. (2004) have developed the bolometric detection method discussed in Sec. IV.B for a spinpolarized sample held in a magnetic trap, near to the phase transition to a Bose condensate. A PA spectrum of one vibrational level in the purely long-range 0u + potential dissociating to 2 3 S1+2 3 P0 was shown in Fig. 22.

The v=4, J=1 level of this potential has a binding energy of 18 MHz and an outer turning point of 1122a0. A detailed quantitative theory of this unusual state, including retardation effects, has been given by Leonard et al. (2004) and Venturi et al. (2003).

### I. Determining scattering lengths from nodes

A knowledge of the s-wave scattering length A is fundamental to understanding the properties of cold quantum gases and their applications. Determining accurate scattering lengths has taken a sustained theoretical and experimental effort. The magnitudes and signs of scattering lengths were not known when the early work towards Bose-Einstein condensation of alkali-metal atoms began in the 1990s. The first accurate determinations of scattering lengths came from PA spectroscopy. This section will discuss how this was done using one-color PA spectroscopy, for which the line shapes and intensity patterns are sensitive to the ground-state wave function (see Sec. III.D). Section VII.B will describe how scattering lengths are determined from two-color PA spectroscopy measurements of binding energies of the vibrational levels in ground electronic states. Although magnetically tunable Feshbach resonance spectroscopy has become an excellent method for measuring nearthreshold bound states (Leo et al., 2000; Marte et al., 2002), PA spectroscopy is the method to use in systems in which there are no magnetic Feshbach resonances available.

> [!figure]
> ![[Fig. 33.png|center|500]]
> **Figure 33.** Transmission and light-induced fluorescence PA spectra of H held in a 6-T magnetic trap. The feature at Δ =−134 GHz is a PA line. The large structure in the fluorescence spectrum around Δ=−80 GHz is the atomic transition. Inset: The PA line shape with a theoretical fit that accounts for the large magnetic-field gradient. The vertical line denotes the inferred position of the unbroadened line. From Mosk et al., 1999.

> [!figure]
> ![[Fig. 34.png|center|500]]
> **Figure 34.** Ungerade electronic potential curves for excited states reached in PA of metastable He. The curves result from an extended Movre-Pichler model taking account of the three fine-structure levels of the atomic 2s2p 3 P state. Three arrows indicate the purely long-range potential wells. From Leonard et al., 2004.

Generally, it is not possible to calculate scattering lengths accurately from ab initio or semiempirical potentials, except for the very lightest elements. Nevertheless, good estimates of A can be obtained experimentally by locating the nodes in the scattering wave function by examining PA intensities. In Sec. III.B we have discussed a scattering wave function for the case of a single channel. If the ground-state atom has hyperfine structure, each s-wave scattering channel can have a different A. Using a multichannel calculation it is possible to express all of these scattering lengths in terms of a few parameters. For alkali-metal atoms these are the van der Waals coefficient $C_6$ and the scattering lengths for the X 1 Σg + and a 3 Σu + potentials. Accurate theoretical values of $C_6$ are often available (see Table I) but the scattering lengths must be determined experimentally.

Abraham, McAlexander, Gerton, et al. (1996) used the pattern of PA line intensities, such as those shown in Fig.

35, to obtain the singlet scattering lengths for $^{6}$Li and $^{7}$Li with error bars on the order of 10%. The oscillatory pattern of the PA line intensity versus v is due to the changing Franck-Condon factor for absorption as the outer turning point of the vibrational level is changed.

According to the reflection approximation in Eq. (23), the oscillatory pattern maps out the ground-state wave function.

Gardner et al. (1995) used PA spectra of a doubly spinpolarized (f=2, m=2) sample of $^{85}$Rb along with the PA threshold line-shape expressions from, Napolitano et al. (1994) to estimate bounds on the scattering length for the a 3 Σu + state of $^{85}$Rb. The spin polarization of atoms restricts the collisions to be purely triplet. They found −1000a0<AT<−60a0, consistent with current values given by van Kempen et al. (2002). They also found the scattering length by analyzing the relative strength of rotational lines of a single vibrational level of the 0g −(1/2) potential. Since this potential satisfies Hund’s case (e) coupling, J=ℓ (see Sec. II.F). Thus J=0 lines correspond to absorption from s waves, J=2 lines to d waves, etc. By applying mass scaling, the bounds on AT for $^{87}$Rb were found to be +85a0<AT< +140a0. These bounds suggested that Bose-Einstein condensation is possible for spin-polarized $^{87}$Rb, but not for $^{85}$Rb at small magnetic fields, as is now well established.

Tiesinga et al. (1996) were the first to determine an accurate scattering length for Na atoms in the ground state f=1, m=−1 hyperfine level, which had already been Bose condensed. They used a sample of unpolarized Na atoms in a 450-μK MOT and analyzed the line shapes of PA spectra to the excited purely long-range 0g −(3/2) state (see Figs. 2 and 30). Because of the selection rules for this case (see Sec. II.I), s-wave collisions give rise to the J=0 and 2 features, d waves give rise to the J=2 and 4 features, and p waves give rise to the J =1 and 3 features. The shapes and relative intensities of the 0g −(3/2) features probe the ground-state wave function for internuclear separations near the 70a0 minimum of this potential. It happens that there is a node in the ground-state p-wave wave function in this region. By using a full multichannel model the authors were able to reproduce this nodal position and other features of the observed line intensities. Within the calculation the detailed shape of the X 1 Σg + and a 3 Σu + potentials was adjusted, while keeping the known long-range part fixed.

> [!figure]
> ![[Fig. 35.png|center|500]]
> **Figure 35.** Relative PA signal strengths (dots) for transitions to vibrational levels of the A1 Σu + state of $^{6}\mathrm{Li}_2$ detected by trap loss. The binding energies vary from 220 GHz for v=79 to 3.5 THz for v=62, and the PA strength is averaged over the three hyperfine features. Results of calculations of the signal strengths for three different values of the scattering length are shown. From Abraham, McAlexander, Gerton, et al., 1996.

> [!figure]
> ![[Fig. 36.png|center|500]]
> **Figure 36.** Square of ℓ=2 partial-wave ground-state wave function for $^{87}$Rb in the presence and absence of a shape resonance at a collision energy E/$k_B$=0.3 mK. The classically forbidden region of the d-wave barrier (see Fig. 14) is shown by the dashed vertical lines. Inset: A blowup of the shorter-range behavior relevant for PA. From Boesten et al., 1999.

Tiesinga et al. (1996) found the scattering length of the f=1, m=−1 state to be 52(5)a0. This value is consistent with later determinations by magnetic Feshbach spectroscopy (van Abeelen and Verhaar, 1999) or boundstate analysis (Crubellier et al., 1999; Samuelis et al., 2001).

Photoassociation spectra are not only sensitive to nodal patterns but also to other features of the scattering wave functions. In particular, the presence of a scattering resonance for partial wave ℓ near threshold can have a strong effect on the PA spectrum due to the enhanced amplitude of the wave function for R<$R_{\mathrm{vdW}}$.

Figure 36 shows calculated wave functions for two possible ground-state potentials. One has a quasibound shape resonance behind the angular momentum barrier (see Fig. 14) and shows a greatly enhanced amplitude at internuclear separations, which can contribute to PA signals. Based on the observation of a g-wave shape resonance in PA of spin-polarized $^{85}$Rb, Boesten et al. (1999) refined their scattering-length bounds. The broad quasibound g-wave resonance level near 0.7 mK leads to an unexpectedly large intensity for the 0g −(1/2) J=4 rotational line and was examined in the time-dependent experiment discussed in Sec. VIII. Similarly, a d-wave shape resonance was observed in $^{87}$Rb.

Burke et al. (1999) and Williams et al. (1999) analyzed spectra for the purely long-range 0g −(3/2) and 1u(3/2) states of $^{39}\mathrm{K}_2$, respectively. Both found a consistent set of bounds on the X 1 Σg + and a 3 Σu + scattering lengths. The triplet scattering length is relatively small, having a magnitude less than $R_{\mathrm{vdW}}$, so that the node in the triplet wave function near $R_{\mathrm{vdW}}$ is not very sensitive to the scattering length (see Figs. 15 and 16). This resulted in rather large error bars on the small triplet scattering length, such that even the sign was not determined. A d-wave shape resonance at quite low collision energy prominently affects the spectrum as shown in Fig. 37, which shows the strong asymmetry and broadening in the J=2 0g −(3/2) feature due to the d-wave contribution.

A similar effect was seen in sodium but is less pronounced. Section IX.C discusses detection of magnetically induced resonances using PA spectroscopy.

More recently, Takasu et al. (2004), discussed above, have used the intensity pattern of PA lines to estimate the scattering length for 174 Yb. Having determined the $C_3$ coefficient for an excited state, and observed a transition frequency where the PA intensity drops, they have deduced the existence of a node in the ground-state wave function near 56a0. In order to convert this to a scattering length (see Fig. 16), it is necessary to know the van der Waals coefficient $C_6$ for the long-range potential, which they could only estimate. Combining this information with bounds on the scattering length from the observed expansion of a Bose-Einstein condensate, they have estimated a scattering length for 174 Yb between about 20a0 and 60a0. When an accurate value of $C_6$ has been established, the experimental data should be reanalyzed with the help of Fig. 16.

> [!figure]
> ![[Fig. 37.png|center|500]]
> **Figure 37.** Comparison of experimental (closed circles) and theoretical (solid line) line shapes for the J=2 0g −(3/2) line of several vibrational levels of $^{39}\mathrm{K}_2$. The synthetic spectra were calculated assuming a cloud temperature of 400 μK. The asymmetric line results from the separate contributions from s and d waves. The latter are enhanced because of the presence of a low-lying d-wave shape resonance. From Burke et al., 1999.

## VI. Doubly Excited States and Continua

Two- (or more) color spectroscopy is a common technique, and its extension to the world of PA spectroscopy is natural. In this section we discuss experiments in which a second photon promotes the molecule formed by PA to a more highly excited state. The exploration of highly excited potentials has most often been for the explicit purpose of spectroscopy, for exploring stateselective detection, or for more efficient detection of the PA transitions.

Doubly excited states in Na are interesting, in particular, for their use in state-selective detection. A number of states near the 3P+3P asymptote autoionize (Amelink et al., 2000b) and thus provide a convenient state-selective route to an ion signal. Structures observed in the earliest PA spectra (Lett et al., 1991) within a few GHz of the atomic line were complicated and not well understood. Bagnato et al. (1993) in an early twocolor experiment also saw complicated structures near the atomic line. The features observed by Lett et al. (1991) were eventually understood as a combination of structure on both the first and second steps of the twophoton but single-color transition to autoionizing bound states (Amelink et al., 2000a). This work relied on results from Molenaar et al. (1996), who used a two-color technique to observe a clear vibrational progression of singly excited states within this spectral region.

States near the 3S+3D3/2 and 3S+3D5/2 asymptotes of $\mathrm{Na}_2$ were studied by Shaffer et al. (1999). They used MOT lasers, tuned about 20 MHz red of the atomic line, to create long-range molecules near the 3S+3P3/2 asymptote, as shown in the inset to Fig. 38. A second laser excited these molecules to higher states which fragmented, resulting in Na+ ions that were collected and counted. Since the initial excitation of the colliding atoms was at long range (~80 nm), angular momentum barriers were not important. High angular momentum states were produced, unlike in more conventional PA spectroscopy. The spectra showed rotational quantum numbers as high as J=22, compared to J=4 as is usually seen in PA in a Na MOT. The complex, overlapping, spectral patterns seen in the figure can be assigned to two vibrational series. High-resolution spectra allowed a detailed analysis of these potentials.

In Fig. 5 we have shown an example of a vibrational level of a high-lying molecular Rydberg state in $\mathrm{Na}_2$.

The spectrum shows a rotational progression and each rotational line exhibits Λ-type doubling (Herzberg, 1950). An interesting feature of the spectrum is that both parity components are observed. Both s-and p-wave collisions contribute to the PA transition to the intermediate 1g state and thus PA produces a sample of intermediate 1g molecules with both parities. In the intermediate 1g state the levels of different parity are degenerate. Each of these two intermediate states gives rise to one of the observed lines in the Rydberg state.

In addition to spectroscopy of high-lying bound states, it is possible to use two-color PA spectroscopy to observe transitions to ionizing continua as illustrated in Fig. 39. For each trace, a PA laser was fixed to produce a known rovibrational level in the purely long-range 0g −(3/2) potential in $\mathrm{Na}_2$. A second laser excited these molecules either to bound states just below the 3P3/2 +3P3/2 asymptote, or to continua just above that asymptote. The bound states were examined in more detail by Amelink et al. (2000b). The limited energy range over which transitions to the continua are observed is a result of the limited kinetic energy available in the intermediate molecule. As the vibrational energy of the intermediate state also increases, the range over which ionization is observed increases. If the intermediate state is shifted to be a vibrational level in a deep chemically bound state, transitions much higher in the continuum are observed. The extent and overall structure of the oscillations in the continuum can be well understood by a simple model, which considers the overlap of a harmonic-oscillator wave function with continuum states of a flat potential.

> [!figure]
> ![[Fig. 38.png|center|500]]
> **Figure 38.** Photoassociative spectrum of the 2 3 Πg and 2 1 Πu states of $\mathrm{Na}_2$ below the 3S+3D asymptote located at 29 173 cm−1. Inset shows the excitation scheme used in the experiment. From Shaffer et al., 1999.

> [!figure]
> ![[Fig. 39.png|center|500]]
> **Figure 39.** Two-color $\mathrm{Na}_2$ + ion production in a MOT at 450 μK. For each trace a PA laser is fixed to produce a steady population of molecules in a specific level (J=2, v=0, 1, or 4) of the 0g −(3/2) purely long-range state. A second laser is scanned and resulting ions counted and plotted as a function of the total energy of two photons. The zero is the 3 2 P3/2(f=0)+3 2 P3/2(f =0) atomic dissociation limit. The traces are offset vertically for clarity. Below threshold the three traces show the same pattern of transitions to bound autoionizing levels; the extent of the above-threshold “Condon internal diffraction” spectrum depends on the available kinetic energy of the vibrational level. From Jones et al., 1997.

The ionization continua and bound states shown in Fig. 39 have played an important role in experiments by providing a sensitive detection channel. In fact, the PA spectra shown in Figs. 2 and 30 took advantage of the presence of the continua. In that experiment, in addition to the scanning PA laser there was an additional fixedfrequency ionization laser tuned so that the total energy of the PA and ionization lasers remained slightly above the 3 2 P3/2+3 2 P3/2 asymptote (i.e., the zero of Fig. 39).

Other experiments have used bound autoionizing states like those shown [for example, de Araujo et al. (2003)].

In their work on two-color PA spectroscopy of $^{39}$K, Wang, Wang, et al. (1997) emphasized the idea that using the purely long-range 0g −(3/2) state as the first step in a double-resonance scheme provides a “Franck-Condon window” for achieving simple assignable spectra of states at higher asymptotes such as the 4S+ (6S, 4D, 5D, 6D, and 7S) that they studied. They were able to determine long-range van der Waals coefficients for a number of 1u states near these asymptotes. Some of the observed levels do not show significant autoionization broadening even though they are well above the energy threshold to do so. Stwalley and Wang (1999) discussed the theory and motivations behind work at higher asymptotes, including the investigation of scaling laws for such dispersion coefficients.

We close this section by noting that it is possible to observe PA followed by a stimulated transition back down to a ground-state continuum of hot free atoms (Jones et al., 1997). Such transitions are modulated by the bound → free Franck-Condon factors and the structure (nodes) in the ground-state scattering wave functions. Such investigations lead naturally, by scanning past the energy of the PA photon, to the detection of bound states in the ground-state potentials, as discussed in the following section.

## VII. Ground Electronic States

The previous section discussed multicolor experiments in which the transitions are upward to higher energy. Here we discuss experiments in which the PA step is followed by a downward transition back to a level in one of the ground electronic states. This section concerns spectroscopy of these ground states; production of cold ground-state molecules is discussed in Sec. IX.A.

### A. Autler-Townes spectroscopy

Figure 40 shows the basic Λ scheme for two-photon PA spectroscopy of the ground electronic state. As in usual PA experiments, laser L1 is tuned to a PA resonance producing a steady population in state |1⟩, which can be detected by trap loss or ionization as before. The addition of laser L2, tuned to the bound→bound transition |1⟩ to |2⟩, can disrupt the PA process and reduce this steady-state population giving a “loss of loss.” This occurs when the |1⟩ to |2⟩ transition is strongly driven, mixing these two levels. This is thus a kind of quantum interference rather than simply a population transfer. If L2 is held fixed on the |1⟩ to |2⟩ transition, while L1 is scanned over the PA resonance, the PA line is observed to be split into two components. This technique has come to be called Autler-Townes spectroscopy (Autler and Townes, 1955). The three-level physics here is closely related to electromagnetically induced transparency observed in atomic Λ systems (Li and Xiao, 1995), although in the present case one “level” is a continuum.

The power of the Autler-Townes method in cold-atom PA spectroscopy was first demonstrated by Abraham et al. (1995), who measured the binding energy of the last bound state, v=10, in the $^{7}\mathrm{Li}_2$ a 3 Σu + potential and thereby determined that the scattering length of $^{7}$Li (in the f=2, mf=2 state) is negative (see Sec. VII.B). Subsequent work has seen much more extensive application of this technique with refined attention to details of the line shapes. The theory of these two-color line shapes was developed by Bohn and Julienne (1996, 1999). A careful experimental investigation was conducted by Lisdat et al. (2002) as shown in Fig. 41. The detection of the population in |1⟩ is by way of observing the decay products produced by spontaneous decay. In particular, cold ground-state molecules produced by the decay are ionized with a pulsed laser. The observed line shape depends on the detuning of L1 from the PA resonance.

> [!figure]
> ![[Fig. 40.png|center|500]]
> **Figure 40.** (Color online) Two-photon PA scheme for probing the structure of the electronic ground state(s), here labeled with quantum numbers appropriate for Cs. The two laser fields are denoted Li; Δ is the detuning of L1 with respect to level |1⟩. The vibrational level at the ground-state asymptote with its rotational structure is called |2⟩. The gray shaded area above the lowest hyperfine asymptote 3+3 indicates the thermal distribution of atoms in the MOT (|0⟩). Loss channels with rates γi are shown as well. Typically, γ1, due to spontaneous decay or ionization by auxiliary lasers, is much larger than γ2. From Lisdat et al., 2002.

Figure 41(a) shows sharp decreases in the ionization yield when L2 is tuned to drive each of the three bound→bound transitions in this spectral region. Figure 41(b), where L1 is intentionally detuned from the peak of the PA line, shows peaks associated with each of the same three transitions. For spectroscopic purposes, the first configuration is preferred. Following this line-shape study, Vanhaecke et al. (2004) have used the technique to study weakly bound (<3.5 cm−1) singlet and triplet levels in $\mathrm{Cs}_2$ and have derived a value for the $C_6$ dispersion constant.

The experimental data shown earlier in Fig. 12 were also obtained by Autler-Townes spectroscopy (de Araujo et al., 2003). That work measured the highest eight vibrational levels of the $^{23}\mathrm{Na}_2$ a 3 Σu + potential, going down some 27 cm−1 into the potential. Vogels et al. (2000) measured and analyzed levels in $\mathrm{Rb}_2$ with binding energies <0.6 cm−1. Schlöder et al. (2003) have measured a line in $^{6}$Li and, from the observed Autler-Townes splitting, have determined coupling parameters of interest to molecule production experiments.

### B. Determining scattering lengths

In Sec. V.I we have discussed how modeling the intensity patterns and line shapes from one-color PA spectroscopy can be used to determine bounds on scattering lengths. A more precise way to determine the scattering length is available if the binding energies of weakly bound levels of the dimer molecule can be measured. In particular, the binding energy EN of the last (Nth) bound state of the potential is closely related to the scattering length if the van der Waals $C_6$ coefficient is known. For the special case A≫$R_{\mathrm{vdW}}$, the relationship is especially simple (Gribakin and Flambaum, 1993):
$$
E_N=\frac{\hbar^2}{2\mu(A-\bar A)^2} \tag{26}
$$
For smaller values of A, the relationship is more complex, but can be calculated numerically from the potential (Crubellier et al., 1999) or by using the analytic properties of a van der Waals potential (Gao, 2000).

The previous section discussed how binding energies of near-threshold bound states can be measured by twocolor PA spectroscopy. Abraham et al. (1995) measured the binding energy of 12.47(4) GHz for the last bound state of the a 3 Σu + potential to determine that the triplet scattering length of $^{7}$Li was −27.3(8)a0. This determination was possible because a relatively accurate potential for the $\mathrm{Li}_2$ dimer molecule was available for its whole range and, in particular, the long-range potential was very accurately known. The most recent values are found in the paper by Bartenstein et al. (2005).

Tsai et al. (1997) measured the energies of 12 molecular levels near the dissociation limit of $^{85}\mathrm{Rb}_2$ and used these to refine their coupled-channels model for $^{85}$Rb scattering. Vogels et al. (1997) used this information along with data from other cold $^{85}$Rb experiments to obtain scattering lengths for the a 3 Σu + and X 1 Σg + states of $^{85}$Rb and $^{87}$Rb. This paved the way for Courteille et al. (1998) to precisely locate a broad $^{85}$Rb magnetic resonance (see Sec. IX.C) that could be used to tune its scattering length to a positive value where Bose-Einstein condensation is feasible. Later, van Kempen et al. (2002) combined previous data with the very precise measurements of Wynar et al. (2000) (see Sec. VII.C) to obtain an accurate predictive model for scattering properties of both Rb isotopes, consistent with the magnetic Feshbach spectroscopy of Marte et al. (2002).

Wang et al. (2000) used two-color PA spectroscopy on $^{39}$K to measure the binding energies of ten bound levels within about 5 GHz of threshold. Modeling these data gave a a 3 Σu + scattering length of −33(5)a0, a much tighter constraint than the wide bounds obtained from onecolor PA spectroscopy (see Sec. V.I). This analysis also permitted a 3 Σu + scattering lengths to be predicted for other isotopic combinations of K. Crubellier et al. (1999) used seven near-threshold bound states for the $\mathrm{Na}_2$ dimer measured from conventional beam spectroscopy methods to obtain an improved scattering length of 55(1.6)a0 for Na in the f=1, m=−1 level.

> [!figure]
> ![[Fig. 41.png|center|500]]
> **Figure 41.** Line shapes observed in Autler-Townes PA spectroscopy of Cs as a function of the frequency of laser L2 (see Fig. 40). The rotational series of a vibrational level 0.6 cm−1 below the (f=3)+(f=3) hyperfine asymptote is shown. In (a) laser L1 is tuned to the PA transition to |1⟩, while in (b) laser L1 is tuned about 20 MHz higher. The frequency scales are the same for (a) and (b). From Lisdat et al., 2002.

### C. Probing mean-field effects in a Bose condensate

When Wynar et al. (2000) applied the Autler-Townes technique to atoms in a Bose condensate interesting new effects were observed. Not only was this experiment at a much lower temperature than those discussed in Sec.

VII.A but the loss mechanism and laser tunings were different as well. In this work L1 was significantly detuned (Δ≫γ1 in Fig. 40). Losses are due to destruction of ground-state molecules by spontaneous Raman scattering of laser photons and possibly inelastic collisions of ground-state molecules with the remaining atoms in the condensate, summarized as the width γ2 in Fig. 40. Figure 42 shows some of their observations. The linewidths are orders of magnitude narrower than those observed in a MOT (or a FORT loaded from a MOT) permitting a precise determination of the binding energy. The four panels show the effect of increasing density on the shape and position of the line. The variation in line position is a result of mean-field shifts from elastic scattering between the molecules and atoms, as well as among the atoms themselves. The two laser intensities are sufficiently low that the linewidth is predominantly due to inhomogeneous broadening from the spatial variation of the mean-field shift within the condensate.

### D. Photoassociation in an optical lattice

An atom placed in a standing wave of light created by two counterpropagating laser beams, well detuned in frequency from any optical transitions, experiences a spatially dependent Stark shift and thus a spatially dependent potential. This situation is analogous to an electron in a crystal lattice and such “optical lattices” have been extensively studied (Jessen and Deutsch, 1996). Of particular interest for our purposes is a recent experiment on photoassociation of atoms held in such a lattice (Rom et al., 2004) based on theoretical proposals by Jaksch et al. (2002) and Damski et al. (2003).

The experiment starts with a Bose condensate of 3×105 |f=1, mf=−1⟩ $^{87}$Rb atoms. The condensate is transfered to a three-dimensional optical lattice created by three optical standing waves along three orthogonal axes. Under the proper conditions, the atomic system undergoes a phase transition to a Mott insulator state with a definite number of atoms per lattice site. For the present purposes the key feature of this new phase is that there are either 2, 1, or 0 atoms per lattice site.

When a PA laser is added, the sites with 1 or 0 atom play no role and thus the system offers an opportunity to observe PA of just two isolated atoms. The two atoms see only each other and the confining lattice potential, and hence there are no mean-field shifts of the sort shown in Sec. VII.C.

> [!figure]
> ![[Fig. 42.png|center|500]]
> **Figure 42.** Trap-loss spectra of two-photon PA transitions to ground-state molecules in a Bose condensate of $^{87}$Rb for four different peak condensate densities n0. The intermediate excited state was a vibrational level in the 0g −(1/2) state with a binding energy of 23 cm−1. The peak densities are for (A) n0 =0.77×1014, (B) 1.22×1014, (C) 1.75×1014, and (D) 2.60 ×1014 atoms/cm3. Each spectrum shows the fraction of atoms remaining in the condensate after illumination by two laser fields as a function of the laser-frequency difference. The resonant decrease in atom number arises from the formation of molecules by stimulated Raman transitions, followed by their subsequent loss from the trap. The increase in width and center frequency of the resonance with density arises from atomatom and molecule-atom mean-field interactions. From Wynar et al., 2000.

> [!figure]
> ![[Fig. 43.png|center|500]]
> **Figure 43.** (Color online) Two-color PA of two atoms in a single lattice site of an optical lattice. (a) The transitions in terms of the internuclear separation. (b) The same process viewed in terms of the center-of-mass coordinate of the pair. The Raman transition shown can affect both the relative motion (i.e., the rovibrational state) and the center-of-mass motion. In (b) two possible transitions are shown; in the upper graph the centerof-mass motion is not affected while in the lower it is changed by one quantum. From Rom et al., 2004.

Figure 43 shows the interaction potential for the pair of Rb atoms in a lattice site. Since the atoms are spatially confined, the extreme long-range part of the relative potential is not flat but is determined by the external confining potential as shown in Fig. 43(a). The PA transition is a two-color, off-resonant Raman transition from a pair of trapped atoms to a weakly bound vibrational level in the $\mathrm{Rb}_2$ electronic ground states. Under the conditions of the experiment, the quantization of the atomic and molecular motion due to the lattice is observable. In that sense, a lattice experiment differs from those discussed earlier in that the PA transition is a bound→bound transition rather than a free→bound transition. Still, it is reasonable to describe this as a PA experiment, as the length scales of the molecular binding and the optical lattice are quite different.

Figure 44 shows the observed trap-loss spectrum. The appearance of multiple lines, spaced by ≈30 kHz, is a consequence of the quantization of the center-of-mass motion of the molecules by the lattice. The molecules have almost the same trap energy-level spacing as the initial atoms since, for the weakly bound vibrational levels considered here, the molecular polarizability is approximately the sum of those of the two constituent atoms. Linewidths as narrow as 1.1 kHz were observed.

The authors interpret this as evidence that no mean-field shifts are present, despite the high on-site atomic density (2×1015 cm−3).

## VIII. Time-Resolved Photoassociation

Studies of time-resolved wave-packet dynamics in small molecules using femtosecond lasers have been a subject of tremendous interest (Zewail, 1996). It seems natural to consider combining such time-resolved techniques with laser cooling and PA spectroscopy, but there are relatively few experimental results that fit this category. The vibrational spacing of the high vibrational levels accessed by PA spectroscopy is very much smaller than the spacing of more deeply bound levels typically used for wave-packet dynamics. This inverse of this spacing defines the time scale for the dynamics and thus defines the range of interesting pulse lengths. Vibrational spacings in the GHz range imply laser-pulse durations of ns or ps. There may not be much advantage in using cold atoms and femtosecond lasers since the broad spectrum of the laser pulse will excite a great many vibrational levels.

Pulsed experiments can reveal dynamical information about the molecule not accessible in cw experiments.

Model calculations by Machholm et al. (1994) suggested that pulsed PA experiments with ultracold Na atoms could distinguish various ionization mechanisms that might contribute to the molecular ionization signal seen in cw PA experiments. One experiment along these lines has been reported (Fatemi et al., 2001). The experiment worked with ~15-ps pulses and Na atoms in a MOT to photoassociate to $\mathrm{Na}_2$ near dissociation. A pump-probe experiment investigating vibrational wave packets was envisioned, however, the usable signal was limited to a region where many vibrational levels were excited in a very anharmonic region of the potential. Although a time-delay-dependent pump-probe signal on a several ns time scale was observed, the “wave packet” dephased and decayed before showing more interesting wavepacket dynamics. An issue in short-pulse experiments is the high peak intensities of the lasers, which can drive unintended multiphoton processes, e.g., three-photon ionization of atoms.

> [!figure]
> ![[Fig. 44.png|center|500]]
> **Figure 44.** Two-photon PA of a weakly bound ℓ=0 level just below the ground electronic 1+1 hyperfine dissociation limit in $^{87}\mathrm{Rb}_2$. This state, located at δ/2π≈636 MHz, is of mixed singlet/triplet character. Transitions to this state were also shown in Fig. 42. The center-of-mass motion is resolved and leads to the observation of nearly equally spaced lines, consistent with quantized, nearly harmonic motion. The detuning is Δ=−2π×900 MHz and the lattice depth is 27Er. From Rom et al., 2004.

> [!figure]
> ![[Fig. 45.png|center|500]]
> **Figure 45.** Example of time-dependent PA for the investigation of a shape resosance. (a) The timing of laser pulses in a timedependent PA experiment. All traces are spectra of the 0g −(1/2) vibrational level at 12 573.04 cm−1. (b), (e) Single-pulse PA [timing case (a)]. (c), (f) Two-pulse PA [timing case (b)]. (d), (g) The differences between the single-and double-pulse spectra with delay time T=0 and 0.9 μs, respectively. The absence of a J=4 signal in (d) shows that the population behind the g-wave barrier has been depleted. This signal recovers with delay time as shown in (g). From Boesten et al., 1999.

Working on a much slower time scale one can spectroscopically resolve individual PA lines but still observe time-dependent collision physics. Boesten et al. (1999) examined the tunneling time associated with a shape resonance through an angular momentum barrier; see Sec. V.I. Working with spin-polarized $^{85}$Rb atoms in a FORT, they observed the growth of one rotation line in a spectrum as a function of delay time between a pair of 0.45-μs duration pulses, as shown in Fig. 45. This rotational line in the 0g −(1/2) state, when observed in a spinpolarized sample, arises solely from g-wave scattering on the triplet a 3 Σu + potential. The excited state (see Fig. 53) has an outer turning point of ~40a0, which lies well inside the g-wave barrier, Fig. 14, at ~100a0. The first pulse depletes the population behind the g-wave barrier, the second pulse probes the recovery of this population on the μs time scale. They used the measured tunneling time, coupled with cw spectroscopy, to extract the resonance energy and, in much the same way as locating the last true bound state, the triplet scattering length.

More recently, coherent control experiments have been proposed for the purposes of producing groundstate molecules. In this context, the high-intensity behavior of the PA process becomes interesting (see Sec.

IX.B) and needs to be understood. Vardi et al. (1997) proposed applying stimulated Raman adiabatic passage techniques to form molecules. Issues related to the continuum nature of the initial collisional state have been raised and debated (Mackie et al., 2004) but there is no experimental resolution. Luc-Koenig et al. (2004) have analyzed the use of chirped pulses and optimal control theory for maximizing the transfer of molecules to specified low vibrational states.

## IX. Applications of Photoassociation Beyond Spectroscopy

### A. Ground-state molecule production

The experiments described in Sec. VII.A involve producing ground-state molecules at least transiently. In the case of PA in a Bose condensate, interactions of those molecules with the remaining atoms was observed. As described in the Introduction (Sec. I.G), there is great interest in producing samples of stable or metastable molecules for further study. Here we consider PA-based schemes for producing a sample of cold ground electronic state molecules. The most common approach is to make use of the spontaneous emission from the excited molecular state to transfer population into a bound state of the ground electronic potential. The challenge is to find an excited level which can be populated by PA from cold atoms and which has a significant probability of decaying into the desired ground-state level(s). This is an active and growing area of research requiring its own review to do justice to all of the work in the field. A collection of recent papers on the theme of producing polar molecules may be found in the articles of Doyle et al. (2004) and accompanying papers. We mention here a few representative examples.

One of the early demonstrations of cold-molecule production was made possible by a fortuitous coincidence that enhanced the production of molecules compared to hot atoms in Cs (Vanhaecke et al., 2002). Figure 46 explains this happenstance. The top panel shows the typical relation between the vibrational wave function of an excited state produced by PA, the initial scattering state describing the cold atoms, and a bound vibrational level of the ground potential. The overlap between the bound excited and bound ground wave functions is poor and thus it is unlikely that the excited molecule will spontaneously decay to the bound ground level. Figure 46(b) shows a wave function in the $\mathrm{Cs}_2$ 0g −(3/2) potential.

As mentioned in Sec. V.E, this state has an unusual double-well structure. The inner turning points of vibrational levels in the outer well of the potential happen to lie at about the same internuclear separation as the outer turning points of vibrational levels in the ground potential, enhancing the overlap between these two wave functions compared to Fig. 46(a). This coincidence significantly enhances the probability of producing ground bound molecules by spontaneous emission.

> [!figure]
> ![[Fig. 46.png|center|500]]
> **Figure 46.** Creation of bound ground molecules by spontaneous emission from an excited bound state formed by PA. (a) The generic relation between a highly excited vibrational level of the excited state and bound states in the ground potential. The excited state has a good overlap with the initial collisional state but not with a bound ground state. Arrow (1) is the PA step, (2) is spontaneous decay back to hot atoms, and (3) is the desired molecule formation process. (b) The special situation which occurs for levels in the 0g −(3/2) potential of $\mathrm{Cs}_2$. This potential has a “bump” at a range of internuclear separations where ground bound levels have outer turning points. Adapted from Dion et al., 2001.

Experimental results for production of $\mathrm{Cs}_2$ a 3 Σu + molecules are shown in Fig. 47. A Cs vapor-cell MOT holds ≈107 atoms at 25 μK. Molecules are produced by a 150-ms PA pulse. Up to 2×105 ground-state molecules are produced at a temperature of 30 μK and are held in a weak magnetic trap for ≈1 s, limited by the background gas pressure. The molecules are detected by photoionization by a high-intensity pulsed dye laser and the resulting $\mathrm{Cs}_2$ + ions are collected and counted. This type of detection is very convenient but, due to the bandwidth of the pulsed laser, does not resolve the rotational or hyperfine state of the molecules.

An example of an experiment which shows a highspectral-resolution identification of $\mathrm{Na}_2$ molecules produced by spontaneous emission is shown in Fig. 48. The figure compares a “dip” spectrum of the sort discussed in Sec. VII.A to one which directly detects ground-state molecules. The lines shown belong to the ℓ=0 rotational level of the highest, v=15, vibrational state of the a3 Σu + potential. Lines which appear at negative detunings represent states which are above the lowest 1+1 asymptote and thus are only quasibound. In this figure the only truly bound level is the one which occurs at +293 MHz and is thus bound by 293 MHz below the 1+1 asymptote (the slightly bluer line is an artifact). This state can be shown to have a nuclear spin of I=3 and a total angular momentum of F=2. Thus from such high-resolution spectra with cw lasers it is possible to determine precisely which ground molecular states are being produced down to the level of individual hyperfine states.

We close this brief survey of cold-molecule production with a recent example in which PA is used to produce heteronuclear alkali-metal dimers. Kermen et al. (2004a) have investigated a scheme for producing and detecting ground-state Rb-Cs molecules ultimately destined to be used in a search for an electron dipole moment. The $^{85}$Rb and $^{133}$Cs atoms were collected in a dual-species, dark-spot MOT. The trap holds 2×108 Rb and 8×108 Cs atoms at densities of 7×1011 atoms/cm3 for Rb and 1×1012 atoms/cm3 for Cs at a temperature of ≈75 μK for both species. They have confirmed the production of RbCs molecules by detecting RbCs+ ions in a time-offlight spectrum. In addition, the experimenters were able to observe a bound→bound molecular spectrum originating from ground triplet a 3 Σ+ molecules produced by PA. From this spectrum they were able to infer information about the vibrational distribution of ground-state molecules produced.

In a similar followup experiment, this group photoassociated Rb+Cs, which spontaneously decayed to produce molecules in the lowest triplet state. They then used a “pump and dump” scheme to make molecules in the lowest X 1 Σ+ vibrational state of the molecule, v=0, and distributed over only a few J levels (Sage et al., 2005). It would be an important achievement if the ab- solute ground state v=0, J=0 could be produced with significant population, since such molecules will presumably be much less susceptible to quenching by collisions with atoms or other molecules. These molecules would then be stable enough for use in a number of other experiments, such as in quantum information processing applications. Low vibrational states have been produced in the X 1 Σg + state of $\mathrm{K}_2$ (Nikolov et al., 2000), and progress toward production of such v=0, J=0 molecules in a number of systems is proceeding rapidly. Other recent examples of experiments on production of heteronuclear molecules can be found in the papers by Mancini et al. (2004) and Wang et al. (2004).

> [!figure]
> ![[Fig. 47.png|center|500]]
> **Figure 47.** Cold $\mathrm{Cs}_2$ molecule production and trapping. (a) The same schematics of the PA process shown in Fig. 46. (b) The number of $\mathrm{Cs}_2$ + detected as a function of time after the PA laser is turned off. The initial drop is due to molecules leaving the small focal spot of the ionization laser. That some ions are detected long afterwards shows that molecules are trapped in the weak magnetic trap. Curves (1) and (2) are with and without MOT light present, showing that MOT light influences the lifetime of the molecules. (c) The same as (b) curve (2) but with a higher background gas pressure. (d) The molecular yield for various length PA pulses. The number is measured 60 ms after the end of the PA process [arrow in (b)]. From Vanhaecke et al., 2002.

> [!figure]
> ![[Fig. 48.png|center|500]]
> **Figure 48.** (Color online) Ground-state molecule production from ultracold Na atoms in a dark-spot MOT with most atoms in the f=1 hyperfine state. The upper trace (and upper-level diagram) shows an Autler-Townes “dip” spectrum as discussed in Sec. VII.A. The dips indicate tunings of L2 which connect ground-state levels to the excited-state level |e1⟩. Laser L1 is fixed to PA atoms to this same |e1⟩ level. Peaks occur when L2 acts as the PA laser. In the lower trace laser L2 is tuning over the same region as before, but now laser L1 is set to a different PA line, producing excited-state molecules in level |e2⟩, which decay by spontaneous emission producing ground-state molecules which laser L2 excites to |e1⟩. The peaks in the lower trace which line up with dips in the upper trace represent molecule formation peaks. From Fatemi et al., 2002.

### B. PA rates in a BEC

The extremely low-temperature and high-density conditions found in a Bose condensate suggest that one might be able to achieve very high PA rates. This follows from the discussion in Secs. III.C and IV.A, where it was noted that the maximum achievable two-body PA rate is ≈nvrelπ/k2 ~n/√T, where n is the atom density. This possibility has raised the question of what the actual limits on PA rates in a Bose condensate are, both in principle and in practice. Of particular interest are possible manifestations of many-body effects in the condensate.

Further, the fact that a condensate is describable in terms of a single spatial wave function suggests that it may be possible to observe Rabi oscillations between atom and molecule states or perform other kinds of ‘‘coherent control’’ experiments designed to produce particular target molecular states.

Equations (20) and (22) form the starting point for our discussion. These expressions are derived under the assumption that only two-body collisions are important, i.e., that the collision between a pair of atoms is not influenced by the presence of other atoms in the sample.

In the present section trap-loss experiments are discussed and the detection width Γd in Eq. (20) is taken to be Γnat. To simplify the discussion, we present a “cartoon” calculation of the rate coefficient that would be observed in a hypothetical experiment in which collisions occur with only a single collision energy given by E=$k_B T$ so that no thermal averaging is required. Using Eq. (20) we calculate the on-resonance PA rate, i.e., the rate which would be observed when the PA laser is tuned to the peak of the line [E+hν−hν0−Sb(E)=0].

Further, we assume that the Wigner threshold law for Γb holds for all E so that Γb∝√E. Figure 49 shows the behavior of the on-resonance rate coefficient as a function of laser intensity under these assumptions. The units are scaled with the energy-independent quantities T0 = ℏΓnat/$k_B$, K0=4πℏ2 /(√2μ3/2√ℏΓnat), and I0=√ℏΓnat/B, where B is defined through Γb(E)=B√EI. Figure 49 shows that, at low intensities, the rate rises linearly with laser intensity K=K0(I/I0) and the slope is independent of the temperature. The latter is a consequence of the competing energy dependence of the prefactor vrelπ/k2 ∝1/√E and Γb∝√E. The curves turn over at an intensity which depends on the temperature. This deviation from linear behavior occurs when the stimulated rate Γb(E) becomes comparable to the natural linewidth Γnat, i.e., the line becomes power broadened. The higher the temperature, the lower the intensity at which the curve turns over, and the smaller the maximum achievable rate. The upper limit to the on-resonant rate, for a given temperature, is known in scattering parlance as the “unitarity” limit as it follows from the requirement that the S matrix be unitary. At extremely high intensity the on-resonance rate coefficient decreases. The implications for experiments are that in a Bose condensate it is much harder to power broaden the line than in a MOT, and thus it is much harder to reach the maximum PA rate. On the other hand, the maximum achievable rate in a BEC will be much higher than in a MOT.

Experiments in magneto-optical traps—which for present purposes represent the “high temperature” dilute gas limit—appear to be consistent with the twobody theory represented by the expressions in Sec. III.C.

Drag et al. (2000) made an effort to compare measured and calculated PA rates in a Cs MOT. While fairly good agreement was achieved, measurement of the absolute rates remains challenging. More recently, Schlöder et al. (2002) have measured PA rates in a $^{6}$Li-$^{7}$Li mixture and have demonstrated saturation of PA rates with the expected dependence on intensity with fitted parameter values that appear reasonable.

One might expect that in a Bose condensate, which requires a many-body wave-function description, the PA process will deviate from the behavior predicted for a thermal gas. Before discussing many-body effects we note that even in the two-body theory there is a factor of 2 difference in the PA rate in a pure Bose condensate compared to a thermal gas. The discussion in Sec. III.C implicitly assumes that the gas follows Boltzmann statistics in which it is very unlikely that two atoms are in the same momentum state. In a Bose condensate all of the atoms are in the same zero-momentum state. This has consequences for creating properly symmetrized wave functions and leads to a factor of 2 reduction in the rate coefficient for the Bose condensate (Stoof et al., 1989).

> [!figure]
> ![[Fig. 49.png|center|500]]
> **Figure 49.** (Color online) On-resonance PA rate coefficient as a function of laser intensity in a simplified model in which all collisions have a single energy E=$k_B T$. All parameters are scaled by units defined in the text. The solid curves show the rate coefficient for three different finite temperatures. The T =0 line is given by K/K0=I/I0. The horizontal dashed line is the unitarity limit for collisions at T=T0. This upper limit is reached at I=I0 for this temperature.

The measured, low-intensity PA rate in a Na condensate confirms that it is important to take this factor of 2 into account in theoretical calculations (McKenzie et al., 2002).

There are several many-body theoretical predictions for how the PA rate in a condensate predicted by the two-body theory will break down at high laser intensities. At the present time there is no clear consensus but several themes appear; see, for example, Javanainen and Mackie (2002), Naidon and Masnou-Seeuws (2003), and Gasenzer (2004). One is that the maximum rate coefficient is lower than that predicted by two-body theories.

In fact, the PA process for high laser intensities may not be well characterized by a rate coefficient at all but may have a more complicated dependence on atom density and on the details of how the laser intensity varies as a function of time. A second theme is that photodissociation of excited molecules to noncondensed atom pairs is important and must be properly accounted for. Javanainen and Mackie (2002) emphasized the important role of photodissociation and predicted a densitydependent maximum PA rate that varied as n2/3. Gasenzer (2004) has argued that the loss rate of atoms from the BEC does not saturate but other processes are limited. Naidon and Masnou-Seeuws (2003) have stressed the importance of a full treatment of the nontrivial time evolution of the system.

The only experiment to investigate the maximum PA rate in a BEC is that of McKenzie et al., (2002). They started with a Na condensate of ≈4×106 atoms at a density of ≈4×1014 atoms/cm3 and photoassociated to the J=1, v=135 level of the A 1 Σu + state (see Fig. 25).

Figure 50 shows the observed light shift and Fig. 51 shows the on-resonance PA rate coefficient. All of the observations are consistent with the predictions of the two-body scattering theory. The large light shift complicated the experiment as small variations in light intensity across the atom cloud led to an apparent broadening of the line, limiting the intensities which could be used.

This experiment approached the intensity regime where many-body effects might have been expected and provided a limit on how large these many-body effects can be. New experiments are required to investigate the effects contemplated in the theories mentioned above. It is interesting to note that this experiment clearly demonstrated that a classical picture of collisions is inadequate for this temperature regime even though such an approach is reasonable at MOT temperatures. A simple estimate of the maximum possible PA rate based on classical particles drifting together at the typical collision velocity of ≈0.6 mm/s leads to an upper limit some four orders of magnitude lower than that observed. While it is not surprising that atoms are governed by quantum mechanics, it is a reminder that classical pictures are dangerous in this ultracold temperature range.

Prodan et al. (2003) have investigated the maximum PA rates in a Bose gas at the transition temperature to a BEC and this bridges the gap between MOT experiments and those in a BEC. They took advantage of the particular scattering properties of $^{7}$Li to be able to produce a sample with a well-defined density distribution and temperature and thus were able to place relatively tight error bars on the PA rate coefficient. Their measured rate coefficient for PA to the v=83 of the 1 3 Σg + state is shown in Fig. 52. The temperature of the sample is 600 nK and the peak density is 4×1012 atoms/cm3. At this temperature and density the limit of the semiclassical theory, the unitarity limit of the quantum-mechanical two-body theory, and the density-dependent limit predicted by the many-body theory of Javanainen and Mackie (2002) all predict about the same upper limits, consistent with those observed in the experiment. Again, all observations are consistent with the two-body theory of Sec. III.C, including the large linear intensity shift of the line.

> [!figure]
> ![[Fig. 50.png|center|500]]
> **Figure 50.** (Color online) Light shift Sb of a PA resonance in a Na Bose-Einstein condensate (BEC) as a function of laser intensity. The dotted line is a straight-line fit to the data as expected from the intensity dependence in Eq. (21). The solid line is a straight line with slope predicted by a theoretical calculation of the dipole matrix elements. Even though the strength of this PA line is almost entirely due to s-wave collisions, a major portion of the shift comes from the presence of a nearby d-wave shape resonance. Adapted from McKenzie et al., 2002.

> [!figure]
> ![[Fig. 51.png|center|500]]
> **Figure 51.** (Color online) On-resonance photoassociation rate constant as a function of intensity in a Na BEC. The corrected data have been adjusted to account for inhomogeneous broadening. The theory line is again due to a coupled-channel calculation of the dipole matrix elements with no adjustable parameters. It includes the factor of 2 reduction in the rate as compared to a noncondensed gas, as described in the text. Adapted from McKenzie et al., 2002.

### C. PA as a monitor of magnetic-field-induced changes to the initial scattering state

Magnetically tunable scattering resonances known as Feshbach resonances have proven to be an extremely fruitful tool for manipulating and controlling the properties and dynamics of ultracold quantum gases (Tiesinga et al., 1993). These resonances appear when a bound state of the molecule is tuned across the collision threshold by application of a static magnetic field. A schematic diagram for $^{85}$Rb is shown in Fig. 53. At zero magnetic field, a bound state in the ground electronic potential dissociating to f=3+f=3 lies just above (~200 MHz) the energy of two scattering f=2 atoms.

Application of a magnetic field (≈160 G, where 1 G =10−4 T) Zeeman shifts this bound state into resonance with the scattering energy. The basic physics—the embedding of a bound state in a continuum—is similar to that of PA, as illustrated by the dressed-level picture of Fig. 4. In fact, in the next section we will pursue this analogy further. Here we concentrate on PA as a tool for detecting magnetic Feshbach resonances.

> [!figure]
> ![[Fig. 52.png|center|500]]
> **Figure 52.** On-resonance photoassociation rate coefficient in a $^{7}$Li gas near the transition to Bose condensation as a function of laser intensity. The open circles are experimental data, obtained from trap-loss analysis. The solid line is the theoretical prediction, with no adjustable parameters. The dashed line is an extrapolation of the theoretical result in the low-intensity limit. From Prodan et al., 2003.

> [!figure]
> ![[Fig. 53.png|center|500]]
> **Figure 53.** Photoassociation method for detecting a magnetic Feshbach resonance in collisions of ultracold $^{85}$Rb atoms in the (f=2, mf=−2) state. The three ground-state 5 2 S1/2+5 2 S1/2 potentials are similar to those shown for Na in Fig. 11. The initial scattering wave function uinit(R) couples to a quasibound resonance state with wave function ures(R). The energy of the bound state can be shifted into resonance by application of a static magnetic field. A laser field induces PA to an excited, rovibrational level (v,J) in the 0g −(1/2) potential, which then decays by spontaneous emission back to free atoms. The PA is detected by trap loss from a FORT. As the quasibound level tunes through zero energy the scattering wave function is modified, changing the PA rate. From Courteille et al., 1998.

> [!figure]
> ![[Fig. 54.png|center|500]]
> **Figure 54.** Photoassociation trap-loss spectra showing the J=0, MF=−4 peak in a vibrational level of the 0g −(1/2) state ≈6 cm−1 below the 5 2 S1/2+5 2 P1/2 dissociation limit for a succession of magnetic-field values, with a laser intensity of 0.1 W/cm2. This peak arises only from s-wave scattering between two 5 2 S (f=2, mf=−2) atoms. The loss of atoms is plotted as a positive signal. The relative Zeeman shift of successive peaks is removed so that they appear at the same laser tuning. From Courteille et al., 1998.

Figure 54 shows a series of experimental trap-loss spectra taken in a FORT holding ≈104 $^{85}$Rb atoms at T≈100 μK and a density of order 1011 –1012 atoms/cm3.

The PA rate changes rapidly over a range of about 10 G near a field of 165 G signaling that the bound state has been swept into resonance with the scattering state. A similar experiment has been performed in Cs (Laburthe Tolra et al., 2003). PA to many vibrational levels of the purely long-range 0g −(3/2) state was used to detect the Feshbach resonance. Figure 55 shows the signal strength of PA lines of two different vibrational levels as a function of the applied magnetic field. One shows a peak, one a dip, for the range shown in the figure. Although the goal of the two experiments is the same—to measure the magnetic field which shifts the bound state into resonance with the continuum—the interpretation of the signals are somewhat different. In the Rb experiment, the signal is primarily sensitive to the population in the bound state while in the Cs experiment the signal reflects changes in the nodal pattern of the initial scattering state. Hence in the Rb experiment the signal shows up as a peak at a particular magnetic field, while in the Cs experiment the signal does not start from zero, depends on the particular 0g −(3/2) vibrational level being monitored, and can have a more complex shape. This latter picture of a changing scattering wave function will be explored further in the next section.

Chin et al. (2004) have employed a related technique to detect extremely weak Feshbach resonances in Cs.

They have used photoexcitation to an unbound state of a repulsive potential to induce trap loss. This experiment is similar to the Rb experiment in that the signal derives largely from the population in the bound state.

### D. PA as an optical Feshbach resonance

Fedichev et al. (1996) proposed that PA resonances could be used to change the collision properties of atoms in much the same way as magnetic Feshbach resonances.

By tuning the frequency of the PA laser the excited bound state, as viewed in a dressed-state picture (see Fig. 4), is swept through the collision threshold. This induces a rapid change in the s-wave scattering length thus potentially permitting control of ultracold collisions. Potential advantages to using optical rather than magnetic Feshbach resonances are that the optical coupling can be quickly turned on and off and can be applied to systems which do not have a convenient magnetic resonance available, such as metastable He (Koelemeij and Leduc, 2004). The major disadvantage of the optical resonances is that spontaneous decay of the excited state leads to loss of atoms. At present, magnetic Feshbach techniques have seen wider application; optical techniques are in the early stages of development.

Using the scattering formulation that gave Eq. (20) for inelastic-scattering losses, Bohn and Julienne (1996, 1999) obtained an expression for the modification of the scattering length by a PA laser. To describe both elastic and inelastic processes it is convenient to define a complex s-wave scattering length A−iB, where the imaginary part B describes the inelastic loss of atoms. Equation (20), with Γd replaced by Γnat, gives the loss rate Kloss. Then B=(μ/2h)Kloss. The real and imaginary parts
$$
A=A_{\mathrm{bg}}+A_{\mathrm{opt}}\frac{(\delta-S_b)\hbar\Gamma_{\mathrm{nat}}}{(\delta-S_b)^2+(\hbar\Gamma_{\mathrm{nat}}/2)^2} \tag{27}
$$
B = 1 2 Aopt (ℏΓnat)2
$$
B=\frac{1}{2}A_{\mathrm{opt}}\frac{(\hbar\Gamma_{\mathrm{nat}})^2}{(\delta-S_b)^2+(\hbar\Gamma_{\mathrm{nat}}/2)^2} \tag{28}
$$
where δ=E+hν−hν0 is the detuning, Abg is the background scattering length in the absence of light, and the “optical length” Aopt=Γb(E,0)/2kΓnat is independent of collision energy in the Wigner threshold law regime as E→0. In order to be practical, it is necessary that the change in scattering length A−Abg be large in comparison with B. This requires large detuning compared to Γnat.

Optical Feshbach resonances were first demonstrated by Fatemi et al. (2000). They worked with Na atoms at <1 mK in a MOT. In order to detect changes in the ground-state collisional wave function, they first set two fixed-frequency lasers to create and then ionize a vibrational level in the 0g −(1/2) state. The resulting $\mathrm{Na}_2$ + ions were collected and counted. This ion signal monitored the amplitude of the ground-state wave function in a particular region of internuclear separation. A third, strong laser was introduced to change the scattering length. This laser was tuned over PA resonances in the $\mathrm{Cs}_2$. The excited vibrational level is detected by ionizing ground-state molecules formed by spontaneous emission from 0g −(3/2). The rapid variation in signal strength with magnetic field reflects variations in the ground-state scattering. From Laburthe Tolra et al., 2003.

> [!figure]
> ![[Fig. 55.png|center|500]]
> **Figure 55.** Photoassociation line strength as a function of applied magnetic field for the J=2 rotational line in two different vibrational levels of the purely long-range 0g −(3/2) potential in

0u + (1/2) potential producing a variation in the ion signal, reflecting changes in the ground-state wave function.

Results from a more recent experiment (Theis et al., 2004) in a Bose condensate of ≈106 $^{87}$Rb atoms are shown in Fig. 56. A ≈70 μs pulse of PA laser light with intensity of ≈500 W/cm2 was tuned to the v=1, J=2 level of the 0g −(3/2) potential and induced changes in the scattering length. In a Bose condensate, the scattering length determines the effective interaction between atoms and thus the shape of the atom cloud in the magnetic trap. Using two-photon Bragg spectroscopy this effective mean-field interaction can be measured as a shift in the frequency of the Bragg resonance condition. Figure 56 shows the measured atom number after the 70-μs PA pulse, the frequency of the Bragg resonance, and the scattering length which was derived from these two measurements. The scattering length was tuned from 10a0 to 190a0 as the PA laser scanned over the resonance. In an even more recent experiment, Thalhammer et al. (2005) have extended this work by adding a second color laser, which couples the excited bound state to a stable ground electronic state. This Raman configuration is similar to that discussed in Sec. VII.A.

The change in the scattering length depends on the detuning from two-photon resonance.

Experiments on the Rb condensate show significant loss of atoms due to spontaneous emission from the excited molecular state. For optical Feshbach resonances to be useful, one must tune off from the line center and yet still maintain a significant change in scattering length. This was the motivation for the investigation of the Raman configuration by Thalhammer et al. (2005) in which it is possible to be tuned off of the one-photon resonance with the excited state, but still be on twophoton resonance for the Raman transition. A careful analysis, and the experiment, showed that this does not reduce the losses. It has been proposed (Ciuryło et al., 2005) that alkaline-earth elements present a particularly favorable case for changing scattering properties by optical means. This follows from the existence of extremely narrow intercombination lines in the atom.

## X. Prospects for Future Developments

Ultracold photoassociation spectroscopy is an outgrowth of the development of laser-cooling and trapping techniques. As those techniques are applied to an increasing number of atomic species, and combinations of species, PA spectroscopy will continue to be a very powerful tool for probing interactions and understanding collisional properties. The exquisite sensitivity and high precision of PA spectroscopy have been amply demonstrated. Theoretical modeling has kept pace with experimental advances, giving new insights into the physicists’ molecule, whose properties can be largely predicted from atomic parameters. Unusual purely long-range molecular states, first probed at high precision only with the advent of PA spectroscopy, are near perfect examples of such molecules.

While PA spectroscopy of ultracold atoms is very good at what it does, PA requires a sample of cold atoms and thus is not applicable to all atomic species at this time. While the number of species that can be cooled is growing, it is difficult for any one laboratory to apply PA techniques to a whole series of systems. Instead, it is most likely to be applied to cases of special interest and used to provide calibration points for other techniques that are more widely applicable. It is simplest to work with a single species of atoms, and hence formation of homonuclear molecules has dominated early work. On the other hand, recent progress in the simultaneous cooling and trapping of mixed species has been dramatic. A better understanding of those systems will stimulate further work. For example, mixed-species PA offers the option of creating cold polar molecules, which can be used to improve studies of fundamental symmetries.

It is almost certain that any species which is laser cooled will eventually be studied by PA spectroscopy. As other cooling techniques are developed, the scope of PA spectroscopy will expand. Early work was, naturally, done on species of atoms that were easiest to laser cool.

Experiments have moved on now to more challenging species such as the alkaline earths, Cr and Fr. PA near the narrow intercombination lines in alkaline earths will be interesting for understanding collisional effects relevant to optical frequency atomic clocks.

> [!figure]
> ![[Fig. 56.png|center|500]]
> **Figure 56.** Optical Feshbach resonance in a $^{87}$Rb Bose condensate. (a) The atom number remaining after an intense PA pulse as a function of the detuning of this laser from line center. (b) The measured Bragg resonance frequencies, which are sensitive to the mean-field interaction in the condensate. (c) The values for the scattering length obtained from the data in (a) and (b) along with a fit by Eq. (27). The background scattering length of ≈100a0, shown by the horizontal line in (c), is consistent with other determinations. From Theis et al., 2004.

So far, PA has combined two atoms to form a diatomic molecule. In a sufficiently dense sample it may be possible to combine three atoms to form a trimer. As samples of cold dimers become available it is interesting to contemplate the possibility of forming trimers or tetramers by PA, as dimers collide with either atoms or other dimers. Some systems of colliding dimers are predicted to have long-range states similar to the ones already observed in diatomics and they may be accessible by infrared PA.

Photoassociation in Bose-Einstein condensates is relatively new. The extremely low spread in collision energies allows for high-precision spectroscopy. The high densities promise rapid molecule formation rates as well as an opportunity to investigate many-body effects. In practice producing a condensate is, in and of itself, still a significant experimental challenge but improved production techniques (such as all-optical methods) and improved detection techniques (such as ionizaton detection) may ease the process of doing spectroscopy in a condensate. The extremely low temperature of a Bose condensate may make direct rf or microwave PA possible.

Magnetic Feshbach resonances have proven to be a very useful tool for modifying the collisional properties of atoms. The optical analog has been demonstrated, but has not yet emerged as a practical tool due to the associated large loss of atoms. There are prospects for finding systems where the optical control of scattering properties may be feasible and the alkaline earths are promising candidates.

Time-dependent PA has seen limited applications.

There has been increasing interest in time-dependent coherent control methods for producing ground-state molecules. While a fair amount of theoretical discussion has appeared there are no experimental demonstrations.

We expect this to change in the near future.

Optical traps, of which lattices are one variety, will also play a large part in the future of PA spectroscopy.

Lower temperatures than MOTs, tight confinement (high densities), and the ability to spin polarize the sample will continue to make this an attractive option.

The optical trap’s ability to hold arbitrary species of both atoms and molecules makes the investigation of atommolecule and molecule-molecule collisions likely.

Photoassociation in optical lattices is in the early stages but will obviously have a large impact in the field, particularly when the lattice is loaded from a Bose condensate. The presence of clearly resolvable motional bound states in a lattice adds a new dimension that will make PA in such systems extremely interesting. The isolation of the atoms provided by the lattice cell prevents destructive collisions with other atoms. PA of two atoms in a lattice cell has already been demonstrated. Theory suggests that PA could be a first step in creating a lattice of molecules, which could be “melted” to produce a molecular Bose condensate. PA of mixed species could produce a lattice of molecular dipoles with very interesting properties.

The possibility of creating a quantum computer has driven much work on cold atoms in lattices. Initialization of a quantum computer may depend on the ability to prepare an optical lattice with only one atom per site.

PA might be used to “clean out” any doubly occupied sites and the optical Feshbach resonance provided by PA may possibly be of use in gate operations. Quantum computing with “qubits” made from heteronuclear dipolar molecules has also been proposed.

The field of ultracold PA spectroscopy is only a little over a decade old. Without a doubt, the next ten years will see more surprises and delights.

## Acknowledgments

We would like to thank the U.S. Office of Naval Research for their support of our work over the years.

K.M.J. acknowledges generous support from NIST while visiting. We also wish to thank all of our colleagues around the world for their input to this manuscript.

## References

Abraham, E. R. I., W. I. McAlexander, J. M. Gerton, R. G. Hulet, R. Coté, and A. Dalgarno, 1996, “Singlet s-wave scattering lengths of $^{6}$Li and $^{7}$Li,” Phys. Rev. A 53, R3713–R3715.

Abraham, E. R. I., W. I. McAlexander, C. A. Sackett, and R. G. Hulet, 1995, “Spectroscopic determination of the s-wave scattering length of lithium,” Phys. Rev. Lett. 74, 1315–1318.

Abraham, E. R. I., W. I. McAlexander, H. T. C. Stoof, and R. G. Hulet, 1996, “Hyperfine structure in photoassociative spectra of $^{6}\mathrm{Li}_2$ and $^{7}\mathrm{Li}_2$,” Phys. Rev. A 53, 3092–3097.

Amelink, A., K. M. Jones, P. D. Lett, P. van der Straten, and H. G. M. Heideman, 2000a, “Single-color photoassociative ionization of ultracold sodium: the region from 0 to −5 GHz,” Phys. Rev. A 62, 013408.

Amelink, A., K. M. Jones, P. D. Lett, P. van der Straten, and H. G. M. Heideman, 2000b, “Spectroscopy of autoionizing doubly excited states in ultracold $\mathrm{Na}_2$ molecules produced by photoassociation,” Phys. Rev. A 61, 042707.

Amiot, C., O. Dulieu, R. F. Gutterres, and F. Masnou-Seeuws, 2002, “Determination of the $\mathrm{Cs}_2$ 0g −(P3/2) potential curve and of Cs 6P1/2,3/2 atomic radiative lifetimes from photoassociation spectroscopy,” Phys. Rev. A 66, 052506.

Autler, S. H., and C. H. Townes, 1955, “Stark effect in rapidly varying fields,” Phys. Rev. 100, 703–722.

Bagnato, V., L. Marcassa, C. Tsao, Y. Wang, and J. Weiner, 1993, “Two-color spectroscopy of colliding ultracold atoms,” Phys. Rev. Lett. 70, 3225–3228.

Bartenstein, M., A. Altmeyer, S. Riedl, R. Geursen, S. Jochim, C. Chin, J. Hecker Denschlag, R. Grimm, A. Simoni, E. Tiesinga, C. Williams, and P. S. Julienne, 2005, “Precise determination of $^{6}$Li cold collision paramters by radiofrequency spectroscopy on weakly bound molecules,” Phys. Rev. Lett. 94, 103201.

Bergeman, T., P. S. Julienne, C. J. Williams, E. Tiesinga, M. R. Manaa, H. Wang, P. L. Gould, and W. C. Stwalley, 2002, “Predissociations in 0u + and 1g states of $\mathrm{K}_2$,” J. Chem. Phys. 117, 7491–7505.

Bethlem, H. L., G. Berden, F. M. H. Crompvoets, R. T. Jongma, A. J. A. van Roij, and G. Meijer, 2000, “Electrostatic trapping of ammonia molecules,” Nature (London) 406, 491– 494.

Birge, R. T., and H. Sponer, 1926, “The heat of dissociation of non-polar molecules,” Phys. Rev. 28, 259–283.

Boesten, H. M. J. M., C. C. Tsai, D. J. Heinzen, A. J. Moonen, and B. J. Verhaar, 1999, “Time-independent and timedependent photoassociation of spin-polarized rubidium,” J. Phys. B 32, 287–308.

Bohn, J. L., and P. S. Julienne, 1996, “Semianalytic treatment of two-color photoassociation spectroscopy and control of cold atoms,” Phys. Rev. A 54, R4637–R4640.

Bohn, J. L., and P. S. Julienne, 1999, “Semianalytic theory of laser-assisted resonant cold collisions,” Phys. Rev. A 60, 414– 425.

Boisseau, C., E. Audouard, J. Vigue, and P. S. Julienne, 2000, “Reflection approximation in photoassociation spectroscopy,” Phys. Rev. A 62, 052705.

Burke, J. P., Jr., C. H. Greene, J. L. Bohn, H. Wang, P. L. Gould, and W. C. Stwalley, 1999, “Determination of $^{39}$K scattering lengths using photoassociation spectroscopy of the 0g −state,” Phys. Rev. A 60, 4417–4426.

Chin, C., V. Vuletic, A. J. Kerman, S. Chu, E. Tiesinga, P. J. Leo, and C. J. Williams, 2004, “Precision Feshbach spectroscopy of ultracold $\mathrm{Cs}_2$,” Phys. Rev. A 70, 032701.

Chu, S.,1998, “Nobel Lecture: The manipulation of neutral particles,” Rev. Mod. Phys. 70, 685–706.

Ciuryło, R., E. Tiesinga, and P. S. Julienne, 2005, “Optical tuning of the scattering length of cold alkaline-earth-metal atoms,” Phys. Rev. A 71, 030701(R).

Ciuryło, R., E. Tiesinga, S. Kotochigova, and P. S. Julienne, 2004, “Photoassociation spectroscopy of cold alkaline-earthmetal atoms near the intercombination line,” Phys. Rev. A 70, 062710.

Cline, R., J. Miller, and D. Heinzen, 1994, “Study of $\mathrm{Rb}_2$ long range states by high-resolution photoassociation spectroscopy,” Phys. Rev. Lett. 73, 632–635.

Cohen-Tannoudji, C., 1998, “Nobel Lecture: Manipulating atoms with photons,” Rev. Mod. Phys. 70, 707–719.

Comparat, D., 2004, “Improved LeRoy-Bernstein neardissociation expansion formula, and prospect for photoassociation spectroscopy,” J. Chem. Phys. 120, 1318–1329.

Comparat, D., C. Drag, B. L. Tolra, A. Fioretti, P. Pillet, A. Crubellier, O. Dulieu, and F. Masnou-Seeuws, 2000, “Formation of cold $\mathrm{Cs}_2$ ground state molecules through photoassociation in the 1u pure long-range state,” Eur. Phys. J. D 11, 59–71.

Courteille, P., R. S. Freeland, D. J. Heinzen, F. A. van Abeelen, and B. J. Verhaar, 1998, “Observation of a Feshbach resonance in cold atom scattering,” Phys. Rev. Lett. 81, 69– 72.

Crubellier, A., O. Dulieu, F. Masnou-Seeuws, M. Elbs, H. Knöckel, and E. Tiemann, 1999, “Simple determination of $\mathrm{Na}_2$ scattering lengths using observed bound levels at the ground state asymptote,” Eur. Phys. J. D 6, 211–220.

Damski, B., L. Santos, E. Tiemann, M. Lewenstein, S. Kotochigova, P. S. Julienne, and P. Zoller, 2003, “Creation of a dipolar superfluid in optical lattices,” Phys. Rev. Lett. 90, 110401.

de Araujo, L. E. E., J. D. Weinstein, S. D. Gensemer, F. K. Fatemi, K. M. Jones, P. D. Lett, and E. Tiesinga, 2003, “Twocolor photoassociation spectroscopy of the lowest triplet potential of $\mathrm{Na}_2$,” J. Chem. Phys. 119, 2062–2074.

de Carvalho, R., J. M. Doyle, B. Friedrich, T. Guillet, J. Kim, D. Patterson, and J. D. Weinstein, 1999, “Buffer-gas loaded magnetic traps for atoms and molecules: A primer,” Eur. Phys. J. D 7, 289–309.

Degenhardt, C., T. Binnewies, G. Wilpers, U. Sterr, F. Riehle, C. Lisdat, and E. Tiemann, 2003, “Photoassociation spectroscopy of cold calcium atoms,” Phys. Rev. A 67, 043408.

Derevianko, A., J. F. Babb, and A. Dalgarno, 2001, “Highprecision calculations of van der Waals coefficients for heteronuclear alkali-metal dimers,” Phys. Rev. A 63, 052704.

Derevianko, A., W. R. Johnson, M. S. Safronova, and J. F. Babb, 1999, “High-precision calculations of dispersion coefficients, static dipole polarizabilities, and atom-wall interaction constants for alkali-metal atoms,” Phys. Rev. Lett. 82, 3589– 3592.

Derevianko, A., S. G. Porsev, S. Kotochigova, E. Tiesinga, and P. S. Julienne, 2003, “Ultracold collision properties of metastable alkaline-earth atoms,” Phys. Rev. Lett. 90, 063002.

Dion, C., C. Drag, O. Dulieu, B. Laburthe Tolra, F. Masnou-Seeuws, and P. Pillet, 2001, “Resonant coupling in the formation of ultracold ground state molecules via photoassociation,” Phys. Rev. Lett. 86, 2253–2256.

Doery, M. R., E. J. D. Vredenbregt, S. S. Op de Beek, H. C. W. Beijerinck, and B. J. Verhaar, 1998, “Limit on suppression of ionization in metastable neon traps due to long-range anisotropy,” Phys. Rev. A 58, 3673–3682.

Doyle, J. M., B. Friedrich, R. V. Krems, and F. Masnou-Seeuws, 2004, “Quo vadis, cold molecules?,” Eur. Phys. J. D 31, 149–164 (special issue on ultracold polar molecules).

Drag, C., B. L. Tolra, O. Dulieu, D. Comparat, M. Vatasescu, S. Boussen, S. Guibal, A. Crubellier, and P. Pillet, 2000, “Experimental versus theoretical rates for photoassociation and for formation of ultracold molecules,” IEEE J. Quantum Electron. 36, 1378–1388.

Fano, U., 1961, “Effects of configuration interaction on intensities and phase shifts,” Phys. Rev. 124, 1866–1878.

Fatemi, F. K., K. M. Jones, and P. D. Lett, 2000, “Observation of optically induced Feshbach resonances in collisions of cold atoms,” Phys. Rev. Lett. 85, 4462–4465.

Fatemi, F. K., K. M. Jones, P. D. Lett, and E. Tiesinga, 2002, “Ultracold ground-state molecule production in sodium,” Phys. Rev. A 66, 053401.

Fatemi, F. K., K. M. Jones, H. Wang, I. A. Walmsley, and P. D. Lett, 2001, “Dynamics of photoinduced collisions of cold atoms probed with picosecond laser pulses,” Phys. Rev. A 64, 033421.

Fedichev, P. O., Y. Kagan, G. V. Shlyapnikov, and J. T. M. Walraven, 1996, “Influence of nearly resonant light on the scattering length in low-temperature atomic gases,” Phys. Rev. Lett. 77, 2913–2916.

Fioretti, A., D. Comparat, C. Drag, C. Amiot, O. Dulieu, F. Masnou-Seeuws, and P. Pillet, 1999, “Photoassociative spectroscopy of the $\mathrm{Cs}_2$ 0g −long-range state,” Eur. Phys. J. D 5, 389–403.

Gao, B., 1996, “Theory of slow-atom collisions,” Phys. Rev. A 54, 2022–2039.

Gao, B., 2000, “Zero-energy bound or quasibound states and their implications for diatomic systems with an asymptotic van der Waals interaction,” Phys. Rev. A 62, 050702.

Gardner, J., R. Cline, J. Miller, D. J. Heinzen, H. M. J. M. Boesten, and B. J. Verhaar, 1995, “Collisions of doubly spinpolarized, ultracold $^{85}$Rb atoms,” Phys. Rev. Lett. 74, 3764– 3767.

Gasenzer, T., 2004, “High light intensity photoassociation in a Bose-Einstein condensate,” Phys. Rev. A 70, 021603.

Gould, P. L., P. D. Lett, P. S. Julienne, W. D. Phillips, H. R. Thorsheim, and J. Weiner, 1988, “Observation of associative ionization of ultracold laser-trapped sodium atoms,” Phys. Rev. Lett. 60, 788–791.

Greiner, M., C. A. Regal, and D. S. Jin, 2003, “Emergence of a molecular Bose-Einstein condensate from a Fermi gas,” Nature (London) 426, 537–540.

Gribakin, G. F., and V. V. Flambaum, 1993, “Calculation of the scattering length in atomic collisions using the semiclassical approximation,” Phys. Rev. A 48, 546–553.

Gutterres, R. F., C. Amiot, A. Fioretti, C. Gabbanini, M. Mazzoni, and O. Dulieu, 2002, “Determination of the $^{87}$Rb 5p state dipole matrix element and radiative lifetime from the photoassociation spectroscopy of the $\mathrm{Rb}_2$ 0g −(P3/2) longrange state,” Phys. Rev. A 66, 024502.

Heinzen, D. J., 2005, private communication.

Herschbach, N., P. J. J. Tol, W. Vassen, W. Hogervorst, G. Woestenenk, J. W. Thomsen, P. van der Straten, and A. Niehaus, 2000, “Photoassociation spectroscopy of cold He(23 S) atoms,” Phys. Rev. Lett. 84, 1874–1877.

Herzberg, G., 1950, Molecular Spectra and Molecular Structure: I. Spectra of Diatomic Molecules, 2nd ed. (van Nostrand Reinhold, New York).

Hope, J., and J. Close, 2004, “Limit to minimally destructive optical detection of atoms,” Phys. Rev. Lett. 93, 180402.

Hougen, J. T., 1970, “The calculation of rotational energy levels and rotational line intensities in diatomic molecules,” NBS Monograph 115, available online at http:// physics.nist.gov/Pubs/Mono115/cover.html Hund, F., 1927, “Zur Deutung der Molekelspektren. II.,” Z. Phys. 42, 93–120.

Jablonski, A., 1945, “General theory of pressure broadening of spectral lines,” Phys. Rev. 68, 78–93.

Jaksch, D., V. Venturi, J. I. Cirac, C. J. Williams, and P. Zoller, 2002, “Creation of a molecular condensate by dynamically melting a Mott insulator,” Phys. Rev. Lett. 89, 040402.

Javanainen, J., and M. Mackie, 2002, “Rate limit for photoassociation of a Bose-Einstein condensate,” Phys. Rev. Lett. 88, 090403.

Jessen, P. S., and I. H. Deutsch, 1996, “Optical lattices,” Adv. At., Mol., Opt. Phys. 37, 95–138.

Jones, K. M., P. S. Julienne, P. D. Lett, W. D. Phillips, E. Tiesinga, and C. J. Williams, 1996, “Measurement of the atomic Na(3P) lifetime and of retardation in the interaction between two atoms bound in a molecule,” Europhys. Lett. 35, 85–90.

Jones, K. M., P. D. Lett, E. Tiesinga, and P. S. Julienne, 2000, “Fitting line shapes in photoassociation spectroscopy of ultracold atoms: A useful approximation,” Phys. Rev. A 61, 012501.

Jones, K. M., S. Maleki, S. Bize, P. D. Lett, C. J. Williams, H. Richling, H. Knöckel, E. Tiemann, H. Wang, P. L. Gould, and W. C. Stwalley, 1996, “Direct measurement of the groundstate dissociation energy of $\mathrm{Na}_2$,” Phys. Rev. A 54, R1006– R1009.

Jones, K. M., S. Maleki, L. P. Ratliff, and P. D. Lett, 1997, “Two-colour photoassociation spectroscopy of ultracold sodium,” J. Phys. B 30, 289–308.

Jones, R. B., J. H. Schloss, and J. G. Eden, 1993, “Excitationspectra for the photoassociation of Kr-F and Xe-I collision pairs in the ultraviolet (208–258 nm),” J. Chem. Phys. 98, 4317–4334.

Julienne, P. S., 1996, “Cold binary atomic collisions in a light field,” J. Res. Natl. Inst. Stand. Technol. 101, 487–503.

Julienne, P. S., and F. H. Mies, 1989, “Collisions of ultracold trapped toms,” J. Opt. Soc. Am. B 6, 2257–2269.

Kerman, A. J., J. M. Sage, S. Sainis, T. Bergeman, and D. DeMille, 2004a, “Production and state-selective detection of ultracold RbCs molecules,” Phys. Rev. Lett. 92, 153001.

Kerman, A. J., J. M. Sage, S. Sainis, T. Bergeman, and D. DeMille, 2004b, “Production of ultracold, polar RbCs* molecules via photoassociation,” Phys. Rev. Lett. 92, 033004.

Koelemeij, J. C. J., and M. Leduc, 2004, “Prospects for measurement and control of the scattering length of metastable helium using photoassociation techniques,” Eur. Phys. J. D 31, 263–271.

Kokoouline, V., O. Dulieu, and F. Masnou-Seeuws, 2000, “Theoretical treatment of channel mixing in excited $\mathrm{Rb}_2$ and $\mathrm{Cs}_2$ ultracold molecules: Perturbations in 0u + photoassociation and fluorescence spectra,” Phys. Rev. A 62, 022504. Laburthe Tolra, B., N. Hoang, B. T’Jampens, N. Vabhaecke, C.

Drag, A. Crubellier, D. Comparat, and P. Pillet, 2003, “Controlling the formation of cold molecules via a Feshbach resonance,” Europhys. Lett. 64, 171–177.

Lefebvre-Brion, H., and R. W. Field, 1986, Perturbations in the Spectra of Diatomic Molecules (Academic, London).

Leo, P., C. J. Williams, and P. S. Julienne, 2000, “Collision properties of ultracold $^{133}$Cs atoms,” Phys. Rev. Lett. 85, 2721–2724.

Leonard, J., A. P. Mosk, M. Walhout, P. van der Straten, M. Leduc, and C. Cohen-Tannoudji, 2004, “Analysis of photoassociation spectra for giant helium dimers,” Phys. Rev. A 69, 032702.

LeRoy, R. J., 1973, Molecular Spectroscopy (Chemical Society, London), Vol. 1.

LeRoy, R. J., and R. B. Bernstein, 1970, “Dissociation energy and long-range potential of diatomic molecules from vibrational spacings of higher levels,” J. Chem. Phys. 52, 3869– 3879.

Lett, P. D., K. Helmerson, W. D. Phillips, L. P. Ratliff, S. L. Rolston, and M. E. Wagshul, 1993, “Spectroscopy of $\mathrm{Na}_2$ by photoassociation of ultracold Na,” Phys. Rev. Lett. 71, 2200– 2203.

Lett, P. D., P. S. Jessen, W. D. Phillips, S. L. Rolston, C. I. Westbrook, and P. L. Gould, 1991, “Laser modification of ultracold collisions: Experiment,” Phys. Rev. Lett. 67, 2139– 2142.

Lett, P. D., P. S. Julienne, and W. D. Phillips, 1995, “Photoassociative spectroscopy of laser-cooled atoms,” Annu. Rev. Phys. Chem. 46, 423–452.

Li, Y.-Q., and M. Xiao, 1995, “Electromagnetically induced transparency in a three-level Λ-type system in rubidium atoms,” Phys. Rev. A 51, R2703–R2706.

Lisdat, C., N. Vanhaecke, D. Comparat, and P. Pillet, 2002, “Line shape analysis of two-colour photoassociation spectra on the example of the $\mathrm{Cs}_2$ ground state,” Eur. Phys. J. D 21, 299–309.

Luc-Koenig, E., M. Vatasescu, and F. Masnou-Seeuws, 2004, “Optimizing the photoassociation of cold atoms by use of chirped laser pulses,” Eur. Phys. J. D 31, 239–262.

Machholm, M., A. Giusti-Suzor, and F. H. Mies, 1994, “Photoassociation of atoms in ultracold collisions probed by wavepacket dynamics,” Phys. Rev. A 50, 5025–5036.

Machholm, M., P. S. Julienne, and K.-A. Suominen, 2001, “Calculations of collisions between cold alkaline-earth-metal atoms in a weak laser field,” Phys. Rev. A 64, 033425.

Mackie, M., K. Harkonen, A. Collin, K.-A. Suominen, and J. Javanainen, 2004, “Improved efficiency of stimulated Raman adiabatic passage in photoassociation of a Bose-Einstein condensate,” Phys. Rev. A 70, 013614.

Magnier, S., P. Millié, O. Dulieu, and F. Masnou-Seeuws, 1993, “Potential curves for the ground and excited states of the $\mathrm{Na}_2$ molecule up to the (3s+5p) dissociation limit: Results of two different effective potential calculations,” J. Chem. Phys. 98, 7113–7125.

Mancini, M. W., G. D. Telles, A. R. L. Caires, V. S. Bagnato, and L. G. Marcassa, 2004, “Observation of ultracold groundstate heteronuclear molecules,” Phys. Rev. Lett. 92, 133203.

Marte, A., T. Volz, J. Schuster, S. Dürr, G. Rempe, E. G. M. van Kempen, and B. J. Verhaar, 2002, “Feshbach resonances in rubidium 87: Precision measurement and analysis,” Phys. Rev. Lett. 89, 283202.

Masnou-Seeuws, F., and P. Pillet, 2001, “Formation of ultracold molecules (T≤200 μK) via photoassociation in a gas of lasercooled atoms,” Adv. At., Mol., Opt. Phys. 47, 53–127.

McAlexander, W. I., E. R. I. Abraham, and R. G. Hulet, 1996, “Radiative lifetime of the 2P state of lithium,” Phys. Rev. A 54, R5–R8.

McKenzie, C., et al., 2002, “Photoassociation of sodium in a Bose-Einstein condensate,” Phys. Rev. Lett. 88, 120403.

Metcalf, H. J., and P. van der Straten, 2003, “Laser cooling and trapping of atoms,” J. Opt. Soc. Am. B 20, 887–908.

Mickelson, P., Y. Martinez, A. Saenz, S. Nagel, Y. Chen, and T. Killian, 2005, “Spectroscopic determination of the s-wave scattering lengths of 86 Sr and $^{88}$Sr,” Phys. Rev. Lett. 95, 223002.

Mies, F. H., and M. Raoult, 2000, “Analysis of threshold effects in ultracold atomic collisions,” Phys. Rev. A 62, 012708.

Mies, F. H., C. J. Williams, P. S. Julienne, and M. Krauss, 1996, “Estimating bounds on collisional relaxation rates of spinpolarized $^{87}$Rb atoms at ultracold temperatures,” J. Res. Natl. Inst. Stand. Technol. 101, 521–535.

Miller, J. D., R. A. Cline, and D. J. Heinzen, 1993, “Photoassociation spectrum of ultracold Rb atoms,” Phys. Rev. Lett. 71, 2204–2207.

Molenaar, P. A., P. van der Straten, and H. G. M. Heideman, 1996, “Long-range predissociation in two-color photoassociation of ultracold Na atoms,” Phys. Rev. Lett. 77, 1460–1463.

Mosk, A. P., M. W. Reynolds, T. W. Hijmans, and J. T. M. Walraven, 1999, “Photoassociation of spin-polarized hydrogen,” Phys. Rev. Lett. 82, 307–310.

Mott, N. F., and H. S. W. Massey, 1965, Theory of Atomic Collisions, 3rd ed. (Oxford University Press, London).

Movre, M., and G. Pichler, 1977, “Resonance interaction and self-broadening of alkali resonance lines. I. Adiabatic potential curves,” J. Phys. B 10, 2631–2638.

Nagel, S., P. Mickelson, A. Saenz, Y. Martinez, Y. Chen, T. Killian, P. Pellegrini, and R. Cote, 2005, “Photoassociative spectroscopy at long range in ultracold strontium,” Phys. Rev. Lett. 94, 083004.

Naidon, P., and F. Masnou-Seeuws, 2003, “Pair dynamics in the formation of molecules in a Bose-Einstein condensate,” Phys. Rev. A 68, 033612.

Napolitano, R. J., J. Weiner, C. J. Williams, and P. S. Julienne, 1994, “Line-shape of high-resolution photoassociation spectra of optically cooled atoms,” Phys. Rev. Lett. 73, 1352–1355.

Nikolov, A., J. Ensher, E. Eyler, H. Wang, W. Stwalley, and P. Gould, 2000, “Efficient production of ground-state potassium molecules at sub-mK temperatures by two-step photoassociation,” Phys. Rev. Lett. 84, 246–249.

Phillips, W. D., 1998, “Nobel Lecture: Laser cooling and trapping of neutral atoms,” Rev. Mod. Phys. 70, 721–741.

Pichler, G., S. Milsošević, D. Veža, and R. Beuc, 1983, “Diffuse bands in the visible absorption spectra of dense alkali vapours,” J. Phys. B 16, 4619–4632.

Pillet, P., A. Crubellier, A. Bleton, O. Dulieu, P. Nosbaum, I. Mourachko, and F. Masnou-Seeuws, 1999, “Photoassociation in a gas of cold alkali atoms. 1. Perturbative quantum approach,” J. Phys. B 30, 2801–2820.

Porsev, S. G., and A. Derevianko, 2002, “High-accuracy relativistic many-body calculations of van der Waals coefficients $C_6$ for alkaline-earth-metal atoms,” Phys. Rev. A 65, 020701(R).

Porsev, S. G., and A. Derevianko, 2003, “Coefficients $C_8$ and $C_{10}$ for alkaline-earth-metal atoms,” J. Chem. Phys. 119, 844– 850.

Prodan, I. D., M. Pichler, M. Junker, R. G. Hulet, and J. L. Bohn, 2003, “Intensity dependence of photoassociation in a quantum degenerate atomic gas,” Phys. Rev. Lett. 91, 080402.

Ramirez-Serrano, J., and J. Weiner, 2002, “Polarizationdependent spectra in the photoassociative ionization of cold atoms in a bright sodium beam,” Phys. Rev. A 65, 052719.

Ribeiro, E. M. S., A. L. M. Zanelatto, and R. J. Napolitano, 2004, “High-intensity and ground-state influence on photoassociation line shapes of $^{88}$Sr,” Chem. Phys. Lett. 390, 89–93.

Rom, T., T. Best, O. Mandel, A. Widera, M. Greiner, T. Hänsch, and I. Bloch, 2004, “State selective production of molecules in optical lattices,” Phys. Rev. Lett. 93, 073002.

Sage, J. M., S. Sainis, T. Bergeman, and D. DeMille, 2005, “Optical production of ultracold polar molecules,” Phys. Rev. Lett. 94, 203001.

Samuelis, C., E. Tiesinga, T. Laue, M. Elbs, H. Knöckel, and E. Tiemann, 2001, “Cold atomic collisions studied by molecular spectroscopy,” Phys. Rev. A 63, 012710.

Santos, M. S., P. Nussenzveig, L. G. Marcassa, K. Helmerson, J. Flemming, S. C. Zilio, and V. S. Bagnato, 1995, “Simultaneous trapping of two different atomic species in a vapor-cell magnetooptical trap,” Phys. Rev. A 52, R4340–R4343.

Santra, R., K. V. Christ, and C. H. Greene, 2004, “Properties of metastable alkaline-earth-metal atoms calculated using an accurate effective core potential,” Phys. Rev. A 69, 042510.

Schlöder, U., T. Deuschle, C. Silber, and C. Zimmermann, 2003, “Autler-Townes splitting in two-color photoassociation of $^{6}$Li,” Phys. Rev. A 68, 051403.

Schlöder, U., C. Silber, T. Deuschle, and C. Zimmermann, 2002, “Saturation in heteronuclear photoassociation of 6 Li7 Li,” Phys. Rev. A 66, 061403.

Schloss, J. H., R. B. Jones, and J. G. Eden, 1993, “Photoassociation of Kr-F collision pairs in the ultraviolet,” J. Chem. Phys. 99, 6483–6494.

Shaffer, J. P., W. Chalupczak, and N. P. Bigelow, 1999, “Highly excited states of ultracold molecules: Photoassociative spectroscopy of $\mathrm{Na}_2$,” Phys. Rev. Lett. 83, 3621–3624.

Simoni, A., P. S. Julienne, E. Tiesinga, and C. J. Williams, 2002, “Intensity effects in ultracold photoassociation line shapes,” Phys. Rev. A 66, 063406.

Steinfeld, J. I., 1985, Molecules and Radiation (MIT, Cambridge, MA).

Stoof, H. T. C., A. M. L. Janssen, J. M. V. A. Koelman, and B. J. Verhaar, 1989, “Decay of spin-polarized atomic hydrogen in the presence of a Bose condensate,” Phys. Rev. A 39, 3157–3169.

Stoof, H. T. C., J. M. V. A. Koelman, and B. J. Verhaar, 1988, “Spin-exchange and dipole relaxation rates in atomic hydrogen: Rigorous and simplified calculations,” Phys. Rev. B 38, 4688–4697.

Stwalley, W. C., 1970, “The dissociation energy of the hydrogen molecule using long-range forces,” Chem. Phys. Lett. 6, 241–244.

Stwalley, W. C., 1978, “Long range molecules,” Contemp. Phys. 19, 65–80.

Stwalley, W. C., Y.-H. Uang, and G. Pichler, 1978, “Pure longrange molecules,” Phys. Rev. Lett. 41, 1164–1167.

Stwalley, W. C., and H. Wang, 1999, “Special review lecture— Photoassociation of ultracold atoms: A new spectroscopic technique,” J. Mol. Spectrosc. 195, 194–228.

Takasu, Y., K. Komori, K. Honda, M. Kumakura, T. Yabuzaki, and Y. Takahashi, 2004, “Photoassociation spectroscopy of laser-cooled ytterbium atoms,” Phys. Rev. Lett. 93, 123202.

Thalhammer, G., M. Theis, K. Winkler, R. Grimm, and J. H. Denschlag, 2005, “Inducing an optical Feshbach resonance via stimulated Raman coupling,” Phys. Rev. A 71, 033403.

Theis, M., G. Thalhammer, K. Winkler, M. Hellwig, G. Ruff, R. Grimm, and J. H. Denschlag, 2004, “Tuning the scattering length with an optically induced Feshbach resonance,” Phys. Rev. Lett. 93, 123001.

Thorsheim, H. R., J. Weiner, and P. S. Julienne, 1987, “Laserinduced photoassociation of ultracold sodium atoms,” Phys. Rev. Lett. 58, 2420–2423.

Tiesinga, E., K. M. Jones, P. D. Lett, U. Volz, C. J. Williams, and P. S. Julienne, 2005, “Measurement and modeling of hyperfine-and rotation-induced state mixing in large weaklybound sodium dimers,” Phys. Rev. A 71, 052703.

Tiesinga, E., B. J. Verhaar, and H. T. C. Stoof, 1993, “Threshold and resonance phenomena in ultracold ground-state collisions,” Phys. Rev. A 47, 4114–4122.

Tiesinga, E., C. J. Williams, P. S. Julienne, K. M. Jones, P. D. Lett, and W. D. Phillips, 1996, “A spectroscopic determination of scattering lengths for sodium atom collisions,” J. Res. Natl. Inst. Stand. Technol. 101, 505–520.

Tsai, C. C., R. S. Freeland, J. M. Vogels, H. Boesten, B. J. Verhaar, and D. J. Heinzen, 1997, “Two-color photoassociation spectroscopy of ground state $\mathrm{Rb}_2$,” Phys. Rev. Lett. 79, 1245–1248.

van Abeelen, F. A., and B. J. Verhaar, 1999, “Determination of collisional properties of cold Na atoms from analysis of bound-state photoassociation and Feshbach resonance field data,” Phys. Rev. A 59, 578–584.

Vanhaecke, N., W. de Souza Melo, B. Laburthe Tolra, D. Comparat, and P. Pillet, 2002, “Accumulation of cold cesium molecules via photoassociation in a mixed atomic and molecular trap,” Phys. Rev. Lett. 89, 063001.

Vanhaecke, N., C. Lisdat, B. T’Jampens, D. Comparat, A. Crubellier, and P. Pillet, 2004, “Accurate asymptotic ground state potential curves of $\mathrm{Cs}_2$ from two-colour photoassociation,” Eur. Phys. J. D 28, 351–360.

van Kempen, E., S. Kokkelmans, D. J. Heinzen, and B. J. Verhaar, 2002, “Interisotope determination of ultracold rubidium interactions from three high-precision experiments,” Phys. Rev. Lett. 88, 093201.

Vardi, A., D. Abrashkevich, E. Frishman, and M. Shapiro, 1997, “Theory of radiative recombination with strong laser pulses and the formation of ultracold molecules via stimulated photo-recombination of cold atoms,” J. Chem. Phys. 107, 6166–6174.

Venturi, V., P. Leo, E. Tiesinga, C. Williams, and I. Whittingham, 2003, “Purely-long-range bound states of He(2s3 S) +He(2s3 P),” Phys. Rev. A 68, 022706.

Vogels, J. M., R. S. Freeland, C. C. Tsai, B. J. Verhaar, and D. J. Heinzen, 2000, “Coupled singlet-triplet analysis of twocolor cold atom photoassociation spectra,” Phys. Rev. A 61, 043407.

Vogels, J. M., C. C. Tsai, R. S. Freeland, S. Kokkelmans, B. J. Verhaar, and D. J. Heinzen, 1997, “Prediction of Feshbach resonances in collisions of ultracold rubidium atoms,” Phys. Rev. A 56, R1067–R1070.

Wagshul, M. E., K. Helmerson, P. D. Lett, S. L. Rolston, W. D. Phillips, R. Heather, and P. S. Julienne, 1993, “Hyperfine effects on associative ionization of ultracold sodium,” Phys. Rev. Lett. 70, 2074–2077.

Wang, D., J. Qi, M. F. Stone, O. Nikolayeva, B. Hattaway, S. D. Gensemer, H. Wang, W. T. Zemke, P. L. Gould, E. E. Eyler, and W. C. Stwalley, 2004, “The photoassociative spectroscopy, photoassociative molecule formation, and trapping of ultracold 39 K85 KRb,” Eur. Phys. J. D 31, 165–177.

Wang, H., P. L. Gould, and W. C. Stwalley, 1997, “Long-range interaction of the $^{39}$K(4s)+$^{39}$K(4p) asymptote by photoassociative spectroscopy. I. The 0g −pure long-range state and the long-range potential constants,” J. Chem. Phys. 106, 7899– 7912.

Wang, H., P. L. Gould, and W. C. Stwalley, 1998, “Finestructure predissociation of ultracold photoassociated $^{39}\mathrm{K}_2$ molecules observed by fragmentation spectroscopy,” Phys. Rev. Lett. 80, 476–479.

Wang, H., J. Li, X. T. Wang, C. J. Williams, P. L. Gould, and W. C. Stwalley, 1997, “Precise determination of the dipole matrix element and radiative lifetime of the $^{39}$K 4p state by photoassociative spectroscopy,” Phys. Rev. A 55, R1569–R1572.

Wang, H., A. N. Nikolov, J. R. Ensher, P. L. Gould, E. E. Eyler, W. C. Stwalley, J. P. Burke, J. L. Bohn, C. H. Greene, E. Tiesinga, C. J. Williams, and P. S. Julienne, 2000, “Groundstate scattering lengths for potassium isotopes determined by double-resonance photoassociative spectroscopy of ultracold $^{39}$K,” Phys. Rev. A 62, 052704.

Wang, H., and W. C. Stwalley, 1998, “Ultracold photoassociative spectroscopy of heteronuclear alkali-metal diatomic molecules,” J. Chem. Phys. 108, 5767–5771.

Wang, H., X. T. Wang, P. L. Gould, and W. C. Stwalley, 1997, “Optical-optical double resonance photoassociative spectroscopy of ultracold $^{39}$K atoms near highly excited asymptotes,” Phys. Rev. Lett. 78, 4173–4176.

Weiner, J., 2003, Cold and Ultracold Collisions in Quantum Microscopic and Mesoscopic Systems (Cambridge University Press, Cambridge, UK).

Weiner, J., V. S. Bagnato, S. Zilio, and P. S. Julienne, 1999, “Experiments and theory in cold and ultracold collisions,” Rev. Mod. Phys. 71, 1–85.

Weiner, J., F. Masnou-Seeuws, and A. Giusti-Suzor, 1989, “Associative ionization: Experiments, potentials and dynamics,” Adv. At., Mol., Opt. Phys. 26, 209–296.

Williams, C. J., E. Tiesinga, and P. S. Julienne, 1996, “Hyperfine structure of the $\mathrm{Na}_2$ 0g −long-range molecular state,” Phys. Rev. A 53, R1939–R1942.

Williams, C. J., E. Tiesinga, P. S. Julienne, H. Wang, W. C. Stwalley, and P. L. Gould, 1999, “Determination of the scattering lengths of $^{39}$K from 1u photoassociation line shapes,” Phys. Rev. A 60, 4427–4438.

Wilpers, G., T. Binnewies, C. Degenhardt, U. Sterr, J. Helmcke, and F. Riehle, 2002, “Optical clock with ultracold neutral atoms,” Phys. Rev. Lett. 89, 230801; 90, 089901(E) (2003).

Wynar, R., R. S. Freeland, D. J. Han, C. Ryu, and D. J. Heinzen, 2000, “Molecules in a Bose-Einstein condensate,” Science 287, 1016–1019.

Yan, Z.-C., J. F. Babb, A. Dalgarno, and G. W. F. Drake, 1996, “Variational calculations of dispersion coefficients for interactions among H, He, and Li atoms,” Phys. Rev. A 54, 2824– 2833.

Yasuda, M., T. Kishimoto, M. Takamoto, and H. Katori, 2006, “Photoassociation spectroscopy of $^{88}$Sr: Reconstruction of the wave function near the last node,” Phys. Rev. A 73, 011403.

Zare, R. N., 1988, Angular Momentum (Wiley, New York).

Zewail, A. H., 1996, “Femtochemistry: recent progress in studies of dynamics and control of reactions and their transition states,” J. Chem. Phys. 100, 12701–12724.

Zinner, G., T. Binnewies, F. Riehle, and E. Tiemann, 2000, “Photoassociation of cold Ca atoms,” Phys. Rev. Lett. 85, 2292–2295.
