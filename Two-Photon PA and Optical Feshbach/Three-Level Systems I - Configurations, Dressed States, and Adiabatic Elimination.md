This note develops the minimal theory of a coherently driven three-level system: a single quantum system with three relevant internal states, coupled pairwise by two near-resonant classical fields. This is the structural skeleton behind two-photon photoassociation, dark-state and STIRAP transfer, electromagnetically induced transparency, and optical Feshbach resonances with a second control field. Here we deliberately stay at the level of the bare three-level Hamiltonian. We build the rotating-frame Hamiltonian, identify the physically meaningful detunings, diagonalize to obtain the dressed states (including the dark state), and finally eliminate the excited state to expose an effective two-level description. No spontaneous decay or continuum is introduced yet; dissipation is the subject of Note II, and the molecular continuum enters when the two legs are specialized to free–bound and bound–bound transitions.

Throughout we adopt from the outset the labelling natural to two-photon photoassociation:

$$
|0\rangle \;=\; \text{initial state (colliding atom pair / scattering state)},
$$

$$
|1\rangle \;=\; \text{intermediate electronically excited molecular state},
$$

$$
|2\rangle \;=\; \text{final target: a bound level of the ground molecular potential}.
$$

The two fields are the two photoassociation arms: $L_1$ drives the free–bound leg $|0\rangle\!\leftrightarrow\!|1\rangle$, and $L_2$ drives the bound–bound leg $|2\rangle\!\leftrightarrow\!|1\rangle$. The $|0\rangle\!\leftrightarrow\!|2\rangle$ transition is not directly driven. This is a $\Lambda$ configuration, with the lossy excited state $|1\rangle$ as the shared apex.

![[Lambda system two-photon PA schematic.svg]]

The guiding picture is simple:

$$
\text{initial pair }|0\rangle
\quad \xrightarrow{\;L_1\;} \quad
\text{excited molecule }|1\rangle
\quad \xrightarrow{\;L_2\;} \quad
\text{bound molecule }|2\rangle .
$$

Everything below is a controlled way of asking what coherent superpositions this ladder of couplings supports, and what happens when the intermediate state $|1\rangle$ is only virtually populated.

---

## 1. The three configurations

Two classical fields drive two of the three possible pairs among $|0\rangle,|1\rangle,|2\rangle$; the third pair is left uncoupled (by selection rules or by being far off resonance). Which two legs are driven, and how the energies are ordered, defines three canonical topologies:

- **$\Lambda$ (lambda) system.** Two low-lying states share a single high-lying state. In our convention $|0\rangle$ and $|2\rangle$ are the low-lying states and the excited $|1\rangle$ is the shared apex; $L_1$ drives $|0\rangle\!\leftrightarrow\!|1\rangle$ and $L_2$ drives $|2\rangle\!\leftrightarrow\!|1\rangle$. The $|0\rangle\!\leftrightarrow\!|2\rangle$ transition is unaddressed. **This is the configuration relevant to two-photon photoassociation and to dark-state physics, and it is our default.**

- **Ladder ($\Xi$) system.** The energies are ordered so that one field climbs from the lowest to a middle state and a second climbs from the middle to the highest. Typical of stepwise excitation to a Rydberg or highly excited state.

- **V system.** One low-lying state shares two high-lying states; both fields originate from the same lower state.

The algebra is nearly identical in all three cases; only the sign conventions for detunings and the interpretation of the states differ. We carry out the derivation for the $\Lambda$ system and comment on sign changes where relevant.

A note on the state energies in the photoassociation context. Measured from the two-atom dissociation threshold, the initial scattering state $|0\rangle$ sits just above threshold (energy $\approx +k_BT$, essentially zero on molecular scales); the final bound state $|2\rangle$ lies *below* threshold by its binding energy; and the excited state $|1\rangle$ lies far above, near an atomic $S+P$ asymptote. Energetically $|1\rangle$ is therefore the apex, exactly as drawn.

---

## 2. Bare Hamiltonian and the two driving fields

Write the bare (field-free) Hamiltonian as

$$
H_0 = E_0\,|0\rangle\langle 0| + E_1\,|1\rangle\langle 1| + E_2\,|2\rangle\langle 2|.
$$

Two classical fields act on the dipole. Denote them by their carrier frequencies $\omega_1$ (arm $L_1$, on the $0$–$1$ leg) and $\omega_2$ (arm $L_2$, on the $2$–$1$ leg):

$$
\mathbf{E}(t) = \boldsymbol{\mathcal{E}}_1\cos(\omega_1 t + \varphi_1) + \boldsymbol{\mathcal{E}}_2\cos(\omega_2 t + \varphi_2).
$$

In the dipole approximation the interaction is $V(t) = -\hat{\mathbf d}\cdot\mathbf E(t)$. We assume each field addresses only its intended leg (the $0$–$2$ leg stays dark), so the only nonzero couplings are $\langle 1|\hat{\mathbf d}|0\rangle$ and $\langle 1|\hat{\mathbf d}|2\rangle$. Define the **Rabi frequencies**

$$
\Omega_1 \equiv -\frac{\langle 1|\hat{\mathbf d}|0\rangle\cdot\boldsymbol{\mathcal E}_1}{\hbar},
\qquad
\Omega_2 \equiv -\frac{\langle 1|\hat{\mathbf d}|2\rangle\cdot\boldsymbol{\mathcal E}_2}{\hbar}.
$$

Each $\Omega_i$ measures the strength of one leg in angular-frequency units. In the two-photon photoassociation context the two matrix elements are of very different character: $\langle 1|\hat{\mathbf d}|0\rangle$ is a *free–bound* (continuum-to-bound) element carrying a density-of-states normalization, while $\langle 1|\hat{\mathbf d}|2\rangle$ is an ordinary *bound–bound* element. Their magnitudes and intensity dependences differ accordingly, but the three-level algebra is blind to this distinction and treats both as Rabi frequencies.

The full time-dependent Hamiltonian is then

$$
H(t) = H_0
- \frac{\hbar}{2}\Big(\Omega_1\,e^{-i(\omega_1 t+\varphi_1)}|1\rangle\langle 0| + \Omega_2\,e^{-i(\omega_2 t+\varphi_2)}|1\rangle\langle 2| + \text{h.c.}\Big)
\;+\;(\text{counter-rotating terms}).
$$

The counter-rotating terms carry factors $e^{+i(\omega+ \omega_{ij})t}$ that oscillate at roughly twice the optical frequency; they are dropped in the rotating-wave approximation (RWA), justified whenever $|\Omega_i|,|\Delta| \ll \omega_1,\omega_2$.

---

## 3. Rotating frame and the elimination of time dependence

The RWA Hamiltonian still depends on time through the factors $e^{-i\omega_1 t}$ and $e^{-i\omega_2 t}$. We remove this by moving to a rotating frame — a state-dependent phase rotation that co-rotates with the fields. Define the unitary

$$
U(t) = \exp\!\Big[\,i\big(\eta_0 t\,|0\rangle\langle 0| + \eta_1 t\,|1\rangle\langle 1| + \eta_2 t\,|2\rangle\langle 2|\big)\Big],
$$

and transform $|\tilde\psi\rangle = U(t)|\psi\rangle$, so that

$$
\tilde H = U H U^\dagger + i\hbar\,\dot U U^\dagger.
$$

The phases $\eta_i$ are chosen so that the explicit time dependence cancels on each driven leg. For the $\Lambda$ system this requires

$$
\eta_1-\eta_0 = \omega_1,\qquad \eta_1-\eta_2 = \omega_2.
$$

One convenient gauge is $\eta_1 = E_1/\hbar$, giving $\eta_0 = E_1/\hbar-\omega_1$ and $\eta_2 = E_1/\hbar-\omega_2$. With this choice the transformed Hamiltonian is time-independent. Its diagonal entries are the *field-dressed* energies measured relative to the driven states, which we now name.

---

## 4. Detunings and the working Hamiltonian

Introduce the transition frequencies $\omega_{10} = (E_1-E_0)/\hbar$ and $\omega_{12} = (E_1-E_2)/\hbar$, and define the two single-arm detunings

$$
\Delta_1 \equiv \omega_1 - \omega_{10}
\qquad(\text{one-photon detuning of the free--bound arm }L_1),
$$

$$
\Delta_2 \equiv \omega_2 - \omega_{12}
\qquad(\text{detuning of the bound--bound arm }L_2).
$$

Two combinations are physically meaningful. The **one-photon detuning** $\Delta \equiv \Delta_1$ measures how far $L_1$ sits from the excited state $|1\rangle$ — this is the $\Delta$ drawn between the dashed laser level and the solid $|1\rangle$ in the schematic. The **two-photon (Raman) detuning**

$$
\delta \equiv \Delta_1 - \Delta_2 = (\omega_1-\omega_2) - (\omega_{10}-\omega_{12}) = (\omega_1-\omega_2)-\omega_{20}
$$

measures how far the *difference* of the two laser frequencies is from the $|0\rangle\!\leftrightarrow\!|2\rangle$ splitting $\omega_{20}=(E_2-E_0)/\hbar$ (the binding energy of the target level below the initial-state energy). The two-photon resonance condition is $\delta = 0$; it does not require either arm to be individually resonant, and it is the condition that locates a two-photon photoassociation line.

In the rotating frame, dropping an overall energy offset, the $\Lambda$-system Hamiltonian takes the compact matrix form in the ordered basis $\{|0\rangle,|2\rangle,|1\rangle\}$ (initial and final states first, excited apex last):

$$
\tilde H = \hbar
\begin{pmatrix}
0 & 0 & \tfrac{1}{2}\Omega_1^{*}\\[4pt]
0 & \delta & \tfrac{1}{2}\Omega_2^{*}\\[4pt]
\tfrac{1}{2}\Omega_1 & \tfrac{1}{2}\Omega_2 & \Delta
\end{pmatrix}.
$$

This is the central object of the note. Read it as follows: the initial and final states $|0\rangle$ and $|2\rangle$ are split only by the two-photon detuning $\delta$; the excited state $|1\rangle$ sits at the one-photon detuning $\Delta$; the off-diagonal blocks are the two Rabi arms. All fast optical timescales have been removed. (For a ladder system one instead places $+\Delta$ on state $|2\rangle$ and keeps the same structure; the sign of $\delta$ follows from the energy ordering.)

The absolute laser phases $\varphi_1,\varphi_2$ have dropped out of the diagonal and appear only as phases on $\Omega_1,\Omega_2$. Because the $\Lambda$ system has **no closed loop of couplings** (the $0$–$2$ leg is dark), a single global rephasing of $|0\rangle,|2\rangle$ removes the relative phase entirely: it is a gauge artifact and cannot affect populations here. This is *not* the same statement as saying the two arms are independent — when the two arms are generated as **carrier and sideband of one laser through an electro-optic modulator (EOM)**, they are mutually phase-coherent, and that coherence becomes physical the moment a third pathway or loop is present (e.g. multiple sidebands, or the closed loop formed when $|0\rangle$–$|2\rangle$ acquires an effective coupling). The EOM implementation and its phase structure are taken up in a dedicated later note; here we simply keep the $\Omega_i$ complex and remember that their relative phase is available and controlled, not arbitrary.

---

## 5. Dressed states and the dark state

The eigenstates of $\tilde H$ are the **dressed states** — the true stationary states of the atom-plus-field system in the rotating frame. Their most transparent feature appears on exact two-photon resonance, $\delta = 0$.

Define the total Rabi frequency and the mixing angle $\theta$ by

$$
\Omega \equiv \sqrt{|\Omega_1|^2+|\Omega_2|^2},
\qquad
\tan\theta \equiv \frac{|\Omega_1|}{|\Omega_2|}.
$$

At $\delta=0$ one linear combination of the two low-lying states decouples completely from the excited state:

$$
\boxed{\;|D\rangle = \cos\theta\,|0\rangle - \sin\theta\,|2\rangle,
\qquad
\tilde H\,|D\rangle = 0.\;}
$$

This is the **dark state**. Because it has no projection onto $|1\rangle$, the two excitation amplitudes $0\!\to\!1$ and $2\!\to\!1$ interfere destructively: a system prepared in $|D\rangle$ neither absorbs nor scatters, regardless of how strong the fields are. It is the microscopic origin of coherent population trapping, electromagnetically induced transparency, and — when $\theta$ is swept adiabatically by ramping the two Rabi frequencies — STIRAP transfer between $|0\rangle$ and $|2\rangle$ without ever populating the lossy state $|1\rangle$.

The orthogonal **bright state**

$$
|B\rangle = \sin\theta\,|0\rangle + \cos\theta\,|2\rangle
$$

does couple to $|1\rangle$, with strength $\tfrac{1}{2}\hbar\Omega$. On resonance the bright and excited states mix into the two **bright dressed states**

$$
|\pm\rangle = \tfrac{1}{\sqrt2}\big(|B\rangle \pm |1\rangle\big),
\qquad
E_\pm = \frac{\hbar}{2}\Big(\Delta \pm \sqrt{\Delta^2+\Omega^2}\Big),
$$

split by the generalized Rabi frequency $\sqrt{\Delta^2+\Omega^2}$. The dark state sits between them at zero energy. This three-level splitting — one uncoupled dark level flanked by two bright levels repelled by the coupling — is the structure probed spectroscopically as the Autler–Townes doublet and, once decay is included, as the transparency window.

Away from $\delta\neq 0$ the dark state acquires a small admixture of $|1\rangle$ and is no longer perfectly dark; the width of the transparency window in $\delta$ is set by $\Omega^2/\Delta$ (or by the excited-state linewidth once decay is included — Note II).

---

## 6. Adiabatic elimination of the excited state

When the free–bound arm is far detuned, $|\Delta| \gg |\Omega_1|,|\Omega_2|,|\delta|$, the excited state $|1\rangle$ is never appreciably populated: it is only *virtually* excited. It can then be removed to yield an effective two-level Hamiltonian acting in the $\{|0\rangle,|2\rangle\}$ subspace. This adiabatic elimination is the step that turns a three-level ladder into an effective coupling between the initial and final states, and it is the formal heart of two-photon photoassociation and of two-color optical Feshbach control.

Write the state as $|\psi\rangle = c_0|0\rangle + c_2|2\rangle + c_1|1\rangle$. The Schrödinger equation $i\hbar\dot{\mathbf c} = \tilde H\mathbf c$ gives, for the excited amplitude,

$$
i\dot c_1 = \Delta\,c_1 + \tfrac{1}{2}\Omega_1\,c_0 + \tfrac{1}{2}\Omega_2\,c_2 .
$$

Adiabatic elimination is the statement that $c_1$ follows the low-lying amplitudes instantaneously: set $\dot c_1 \approx 0$ (equivalently, $c_1$ is slaved to its quasi-steady value on the slow timescale of the ground dynamics), so that

$$
c_1 \simeq -\frac{1}{2\Delta}\big(\Omega_1\,c_0 + \Omega_2\,c_2\big).
$$

Substituting back into the equations for $c_0$ and $c_2$ removes state $|1\rangle$ and leaves an effective $2\times 2$ Hamiltonian in the basis $\{|0\rangle,|2\rangle\}$:

$$
\boxed{\;
H_{\rm eff} = -\frac{\hbar}{4\Delta}
\begin{pmatrix}
|\Omega_1|^2 & \Omega_1^{*}\Omega_2\\[4pt]
\Omega_1\Omega_2^{*} & |\Omega_2|^2
\end{pmatrix}
\;+\;
\hbar
\begin{pmatrix}
0 & 0\\ 0 & \delta
\end{pmatrix}.
\;}
$$

Three ingredients emerge, and each has a clear physical name:

- **Light shifts (AC Stark shifts).** The diagonal terms $-\hbar|\Omega_1|^2/4\Delta$ and $-\hbar|\Omega_2|^2/4\Delta$ shift $|0\rangle$ and $|2\rangle$ in proportion to the intensity of the arm that connects each to $|1\rangle$. They shift the two-photon resonance and must be tracked in any precision measurement of the binding energy $\omega_{20}$.

- **Effective two-photon coupling.** The off-diagonal term defines an effective Rabi frequency between the initial and final states,

$$
\Omega_{\rm eff} \equiv \frac{\Omega_1\,\Omega_2^{*}}{2\Delta},
$$

a *second-order* coupling mediated by the virtual excursion through $|1\rangle$. It scales as the product of the two field amplitudes and inversely with the one-photon detuning — the signature of a two-photon (Raman) process, and the coherent coupling that a bound–bound arm adds to a photoassociation scheme.

- **Effective two-photon detuning.** The bare $\delta$ carries over; combined with the light shifts it sets the true resonance condition of the effective two-level system, $\delta_{\rm eff} = \delta - (|\Omega_1|^2-|\Omega_2|^2)/4\Delta = 0$.

The effective system is thus an ordinary driven two-level problem: initial and final states, split by $\delta_{\rm eff}$, coupled by $\Omega_{\rm eff}$, with the lossy intermediate state present only as a virtual mediator. This is precisely the structure one wants for coherently linking a scattering state to a target bound state through an electronically excited molecular state. What is still missing is the *loss*: at finite $\Delta$ the excursion through $|1\rangle$ is not perfectly virtual, and $|1\rangle$ decays. Once decay is restored, $\Delta \to \Delta - i\gamma_1/2$ and $\Omega_{\rm eff}$ becomes complex — its imaginary part is the two-photon photoassociation loss rate and, reinterpreted for the scattering length, the width of an optical Feshbach resonance. That is the subject of Note II.

---

## 7. What has and has not been assumed

To keep the boundaries of this note explicit:

- **Closed system.** No spontaneous emission from $|1\rangle$ and no continuum have been included. Decay is what makes the far-detuned virtual excursion of Section 6 favorable (it suppresses real scattering as $1/\Delta^2$ while the coupling falls only as $1/\Delta$), and it is what gives the transparency window its finite width. It is added in Note II.
- **Discrete states.** All three states are treated as isolated levels. In photoassociation, $|0\rangle$ is really a scattering continuum and the $L_1$ coupling is a free–bound matrix element; the three-level algebra above survives, with the continuum handled separately.
- **Classical fields, RWA.** The fields are classical and near-resonant, so counter-rotating and multi-photon-off-resonant terms are dropped. The specific case where the two arms are the carrier and an EOM sideband of a single laser — our experimental scheme — is a refinement of the field description and is treated in its own note.

---

## Planned notes in this series

- **Three-Level Systems I** *(this note)* — configurations, dressed and dark states, adiabatic elimination; closed (non-dissipative) system.
- **Three-Level Systems II — Dissipation, the Master Equation, and the Optical Bloch Equations** — spontaneous emission and dephasing, the Lindblad master equation, the non-Hermitian shortcut, and the emergence of complex light shifts (optical Feshbach shift + width) and two-photon loss.
- **The EOM two-arm scheme** — the two arms as carrier and sideband of one laser through an electro-optic modulator: sideband spectrum, phase coherence, and its consequences for the $\Lambda$ Hamiltonian.

---

### Related notes

- [[Photoassociation formula sheet]] — where the single-arm ($L_1$) free–bound coupling is quantified.
- [[Feshbach Resonance I - Projection Formalism and the Origin of the Resonant Scattering Length]] — the closed-channel resonance language that optical Feshbach control mirrors optically.
