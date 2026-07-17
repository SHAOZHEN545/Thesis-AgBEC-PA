This note develops the minimal theory of a coherently driven three-level system: a single quantum system with three relevant internal states, coupled pairwise by two near-resonant classical fields. This is the structural skeleton behind two-photon photoassociation, dark-state and STIRAP transfer, electromagnetically induced transparency, and optical Feshbach resonances with a second control field. Here we deliberately stay at the level of the bare three-level Hamiltonian. We build the rotating-frame Hamiltonian, identify the physically meaningful detunings, diagonalize to obtain the dressed states (including the dark state), and finally eliminate the excited state to expose an effective two-level description. No molecular physics, continuum, or spontaneous decay is introduced yet; those enter in later notes.

The guiding picture is simple:

$$
\text{two long-lived states}
\quad \longleftrightarrow \quad
\text{one shared, short-lived intermediate state}
\quad \longleftrightarrow \quad
\text{two fields that address the two legs}.
$$

Everything below is a controlled way of asking what coherent superpositions this ladder of couplings supports, and what happens when the intermediate state is only virtually populated.

---

## 1. The three configurations

Label the three states $|1\rangle$, $|2\rangle$, $|3\rangle$ with bare energies $E_1$, $E_2$, $E_3$. Two classical fields drive two of the three possible pairs; the third pair is left uncoupled (either by selection rules or by being far off resonance). Which two legs are driven, and how the energies are ordered, defines three canonical topologies:

- **$\Lambda$ (lambda) system.** Two low-lying states $|1\rangle,|2\rangle$ share a single high-lying state $|3\rangle$. A *pump* field drives $|1\rangle\!\leftrightarrow\!|3\rangle$ and a *Stokes* (or *coupling*) field drives $|2\rangle\!\leftrightarrow\!|3\rangle$. The $|1\rangle\!\leftrightarrow\!|2\rangle$ transition is dipole-forbidden or unaddressed. This is the configuration relevant to two-photon photoassociation and to dark-state physics, and it is our default below.

- **Ladder ($\Xi$) system.** The energies are ordered $E_1<E_3<E_2$: one field climbs $|1\rangle\!\to\!|3\rangle$, a second climbs $|3\rangle\!\to\!|2\rangle$. Typical of stepwise excitation to a Rydberg or highly excited state.

- **V system.** One low-lying state $|1\rangle$ shares two high-lying states; both fields originate from $|1\rangle$.

The algebra is nearly identical in all three cases; only the sign conventions for detunings and the interpretation of the states differ. We carry out the derivation for the $\Lambda$ system and comment on sign changes where relevant.

---

## 2. Bare Hamiltonian and the two driving fields

Write the bare (field-free) Hamiltonian as

$$
H_0 = E_1\,|1\rangle\langle 1| + E_2\,|2\rangle\langle 2| + E_3\,|3\rangle\langle 3|.
$$

Two classical fields act on the dipole. Denote them by their carrier frequencies $\omega_p$ (pump, on the $1$–$3$ leg) and $\omega_s$ (Stokes, on the $2$–$3$ leg):

$$
\mathbf{E}(t) = \boldsymbol{\mathcal{E}}_p\cos(\omega_p t) + \boldsymbol{\mathcal{E}}_s\cos(\omega_s t).
$$

In the dipole approximation the interaction is $V(t) = -\hat{\mathbf d}\cdot\mathbf E(t)$. We assume each field addresses only its intended leg (the $1$–$2$ leg stays dark), so the only nonzero couplings are $\langle 3|\hat{\mathbf d}|1\rangle$ and $\langle 3|\hat{\mathbf d}|2\rangle$. Define the **Rabi frequencies**

$$
\Omega_p \equiv -\frac{\langle 3|\hat{\mathbf d}|1\rangle\cdot\boldsymbol{\mathcal E}_p}{\hbar},
\qquad
\Omega_s \equiv -\frac{\langle 3|\hat{\mathbf d}|2\rangle\cdot\boldsymbol{\mathcal E}_s}{\hbar}.
$$

Each $\Omega$ measures the strength of one leg in angular-frequency units. We take them real for now; a relative phase between the fields can be reinstated by $\Omega_p,\Omega_s \to |\Omega_p|,|\Omega_s|e^{i\phi}$ and matters only when a closed loop of couplings exists.

The full time-dependent Hamiltonian is then

$$
H(t) = H_0
- \frac{\hbar}{2}\Big(\Omega_p\,e^{-i\omega_p t}|3\rangle\langle 1| + \Omega_s\,e^{-i\omega_s t}|3\rangle\langle 2| + \text{h.c.}\Big)
\;+\;(\text{counter-rotating terms}).
$$

The counter-rotating terms carry factors $e^{+i(\omega+ \omega_{ij})t}$ that oscillate at roughly twice the optical frequency; they are dropped in the rotating-wave approximation (RWA), justified whenever $|\Omega|,|\Delta| \ll \omega_p,\omega_s$.

---

## 3. Rotating frame and the elimination of time dependence

The RWA Hamiltonian still depends on time through the factors $e^{-i\omega_p t}$ and $e^{-i\omega_s t}$. We remove this by moving to a rotating frame — a state-dependent phase rotation that co-rotates with the fields. Define the unitary

$$
U(t) = \exp\!\Big[\,i\big(\eta_1 t\,|1\rangle\langle 1| + \eta_2 t\,|2\rangle\langle 2| + \eta_3 t\,|3\rangle\langle 3|\big)\Big],
$$

and transform $|\tilde\psi\rangle = U(t)|\psi\rangle$, so that

$$
\tilde H = U H U^\dagger + i\hbar\,\dot U U^\dagger.
$$

The phases $\eta_i$ are chosen so that the explicit time dependence cancels on each driven leg. For the $\Lambda$ system this requires

$$
\eta_3-\eta_1 = \omega_p,\qquad \eta_3-\eta_2 = \omega_s.
$$

One convenient gauge is $\eta_3 = E_3/\hbar$, giving $\eta_1 = E_3/\hbar-\omega_p$ and $\eta_2 = E_3/\hbar-\omega_s$. With this choice the transformed Hamiltonian is time-independent. Its diagonal entries are the *field-dressed* energies measured relative to the driven states, which we now name.

---

## 4. Detunings and the working Hamiltonian

Introduce the atomic transition frequencies $\omega_{31} = (E_3-E_1)/\hbar$ and $\omega_{32} = (E_3-E_2)/\hbar$, and define the two detunings

$$
\Delta_p \equiv \omega_p - \omega_{31}
\qquad(\text{one-photon / pump detuning}),
$$

$$
\Delta_s \equiv \omega_s - \omega_{32}
\qquad(\text{Stokes detuning}).
$$

Two combinations are physically meaningful. The **one-photon detuning** $\Delta \equiv \Delta_p$ measures how far the pump sits from the excited state $|3\rangle$. The **two-photon (Raman) detuning**

$$
\delta \equiv \Delta_p - \Delta_s = (\omega_p-\omega_s) - (\omega_{31}-\omega_{32}) = (\omega_p-\omega_s)-\omega_{21}
$$

measures how far the *difference* of the two laser frequencies is from the $|1\rangle\!\leftrightarrow\!|2\rangle$ splitting $\omega_{21}=(E_2-E_1)/\hbar$. The two-photon resonance condition is $\delta = 0$; it does not require either field to be individually resonant.

In the rotating frame, dropping an overall energy offset, the $\Lambda$-system Hamiltonian takes the compact matrix form in the ordered basis $\{|1\rangle,|2\rangle,|3\rangle\}$:

$$
\tilde H = \hbar
\begin{pmatrix}
0 & 0 & \tfrac{1}{2}\Omega_p^{*}\\[4pt]
0 & \delta & \tfrac{1}{2}\Omega_s^{*}\\[4pt]
\tfrac{1}{2}\Omega_p & \tfrac{1}{2}\Omega_s & \Delta
\end{pmatrix}.
$$

This is the central object of the note. Read it as follows: the two ground states $|1\rangle$ and $|2\rangle$ are nearly degenerate on the scale of optical frequencies, split only by the two-photon detuning $\delta$; the excited state sits at the one-photon detuning $\Delta$; the off-diagonal blocks are the two Rabi legs. All fast optical timescales have been removed. (For a ladder system one instead has $+\Delta$ on state $|2\rangle$ and the same structure otherwise; the sign of $\delta$ follows from the energy ordering.)

---

## 5. Dressed states and the dark state

The eigenstates of $\tilde H$ are the **dressed states** — the true stationary states of the atom-plus-field system in the rotating frame. Their most transparent feature appears on exact two-photon resonance, $\delta = 0$.

Define the total Rabi frequency and the mixing angle $\theta$ by

$$
\Omega \equiv \sqrt{|\Omega_p|^2+|\Omega_s|^2},
\qquad
\tan\theta \equiv \frac{|\Omega_p|}{|\Omega_s|}.
$$

At $\delta=0$ one linear combination of the two ground states decouples completely from the excited state:

$$
\boxed{\;|D\rangle = \cos\theta\,|1\rangle - \sin\theta\,|2\rangle,
\qquad
\tilde H\,|D\rangle = 0.\;}
$$

This is the **dark state**. Because it has no projection onto $|3\rangle$, the two excitation amplitudes $1\!\to\!3$ and $2\!\to\!3$ interfere destructively: the system driven into $|D\rangle$ neither absorbs nor scatters, regardless of how strong the fields are. It is the microscopic origin of coherent population trapping, electromagnetically induced transparency, and — when $\theta$ is swept adiabatically by ramping the two Rabi frequencies — STIRAP population transfer between $|1\rangle$ and $|2\rangle$ without ever populating the lossy state $|3\rangle$.

The orthogonal **bright state**

$$
|B\rangle = \sin\theta\,|1\rangle + \cos\theta\,|2\rangle
$$

does couple to $|3\rangle$, with strength $\tfrac{1}{2}\hbar\Omega$. On resonance the bright and excited states mix into the two **bright dressed states**

$$
|\pm\rangle = \tfrac{1}{\sqrt2}\big(|B\rangle \pm |3\rangle\big),
\qquad
E_\pm = \frac{\hbar}{2}\Big(\Delta \pm \sqrt{\Delta^2+\Omega^2}\Big),
$$

split by the generalized Rabi frequency $\sqrt{\Delta^2+\Omega^2}$. The dark state sits between them at zero energy. This three-level splitting — one uncoupled dark level flanked by two bright levels repelled by the coupling — is the structure probed spectroscopically as the Autler–Townes doublet and the transparency window.

Away from $\delta\neq 0$ the dark state acquires a small admixture of $|3\rangle$ and is no longer perfectly dark; the width of the transparency window in $\delta$ is set by $\Omega^2/\Delta$ (or by the excited-state linewidth once decay is included, in a later note).

---

## 6. Adiabatic elimination of the excited state

When the pump is far detuned, $|\Delta| \gg |\Omega_p|,|\Omega_s|,|\delta|$, the excited state $|3\rangle$ is never appreciably populated: it is only *virtually* excited. It can then be removed to yield an effective two-level Hamiltonian acting in the $\{|1\rangle,|2\rangle\}$ subspace. This adiabatic elimination is the step that turns a three-level ladder into an effective coupling between the two long-lived states, and it is the formal heart of two-photon photoassociation and of two-color optical Feshbach control.

Write the state as $|\psi\rangle = c_1|1\rangle + c_2|2\rangle + c_3|3\rangle$. The Schrödinger equation $i\hbar\dot{\mathbf c} = \tilde H\mathbf c$ gives, for the excited amplitude,

$$
i\dot c_3 = \Delta\,c_3 + \tfrac{1}{2}\Omega_p\,c_1 + \tfrac{1}{2}\Omega_s\,c_2 .
$$

Adiabatic elimination is the statement that $c_3$ follows the ground amplitudes instantaneously: set $\dot c_3 \approx 0$ (equivalently, $c_3$ is slaved to its quasi-steady value on the slow timescale of the ground dynamics), so that

$$
c_3 \simeq -\frac{1}{2\Delta}\big(\Omega_p\,c_1 + \Omega_s\,c_2\big).
$$

Substituting back into the equations for $c_1$ and $c_2$ removes state $|3\rangle$ and leaves an effective $2\times 2$ Hamiltonian:

$$
\boxed{\;
H_{\rm eff} = -\frac{\hbar}{4\Delta}
\begin{pmatrix}
|\Omega_p|^2 & \Omega_p^{*}\Omega_s\\[4pt]
\Omega_p\Omega_s^{*} & |\Omega_s|^2
\end{pmatrix}
\;+\;
\hbar
\begin{pmatrix}
0 & 0\\ 0 & \delta
\end{pmatrix}.
\;}
$$

Three ingredients emerge, and each has a clear physical name:

- **Light shifts (AC Stark shifts).** The diagonal terms $-\hbar|\Omega_p|^2/4\Delta$ and $-\hbar|\Omega_s|^2/4\Delta$ shift states $|1\rangle$ and $|2\rangle$ in proportion to the intensity of the field that connects them to $|3\rangle$. They shift the two-photon resonance and must be tracked in any precision measurement of the $|1\rangle$–$|2\rangle$ splitting.

- **Effective two-photon coupling.** The off-diagonal term defines an effective Rabi frequency between the two ground states,

$$
\Omega_{\rm eff} \equiv \frac{\Omega_p\,\Omega_s^{*}}{2\Delta},
$$

a *second-order* coupling mediated by the virtual excursion through $|3\rangle$. It scales as the product of the two field amplitudes and inversely with the one-photon detuning — the signature of a two-photon (Raman) process.

- **Effective two-photon detuning.** The bare $\delta$ carries over; combined with the light shifts it sets the true resonance condition of the effective two-level system, $\delta_{\rm eff} = \delta - (|\Omega_p|^2-|\Omega_s|^2)/4\Delta = 0$.

The effective system is thus an ordinary driven two-level problem: two states, split by $\delta_{\rm eff}$, coupled by $\Omega_{\rm eff}$, with the lossy intermediate state present only as a virtual mediator. This is precisely the structure one wants for coherently linking a scattering (or ground molecular) state to a target bound state through an electronically excited molecular state — the subject of the notes that follow.

---

## 7. What has and has not been assumed

To keep the boundaries of this note explicit:

- **Closed system.** No spontaneous emission from $|3\rangle$ and no continuum have been included. Decay is what makes the far-detuned virtual excursion of Section 6 favorable (it suppresses real scattering as $1/\Delta^2$ while the coupling falls only as $1/\Delta$), and it is what gives the transparency window its finite width. It will be added as a non-Hermitian term $-i\hbar\gamma/2$ on $|3\rangle$ in a later note.
- **Discrete states.** All three states are treated as isolated levels. In photoassociation, state $|1\rangle$ is really a scattering continuum and the couplings become free–bound and bound–bound matrix elements; the three-level algebra above survives, with the continuum handled separately.
- **Classical fields, RWA.** The fields are classical and near-resonant, so counter-rotating and multi-photon-off-resonant terms are dropped.

With this scaffold in place — configurations, detunings, the dressed/dark states, and the adiabatically eliminated effective coupling — the later notes specialize the two legs to molecular transitions (two-photon photoassociation) and reinterpret $|3\rangle$ as an electronically excited molecular state used to tune the ground-state scattering length (optical Feshbach resonances).

---

### Related notes

- [[Photoassociation formula sheet]] — where the single-leg (one-photon) free–bound coupling is quantified.
- [[Feshbach Resonance I - Projection Formalism and the Origin of the Resonant Scattering Length]] — the closed-channel resonance language that optical Feshbach control mirrors optically.
