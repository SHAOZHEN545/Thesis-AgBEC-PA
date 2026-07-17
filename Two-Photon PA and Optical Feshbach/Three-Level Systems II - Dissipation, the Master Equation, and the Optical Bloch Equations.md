Note I treated the three-level $\Lambda$ system as closed: the excited state $|1\rangle$ was a bookkeeping level through which population made a virtual excursion, and probability was conserved. That picture is incomplete in exactly the way that matters for photoassociation. The excited molecular state $|1\rangle$ is short-lived — it decays by spontaneous emission at a rate $\gamma_1$, and in a trap that decay overwhelmingly removes atoms from the system (they leave as hot atoms or as untrapped molecules). Two-photon photoassociation is *measured* as this loss. The coherent Schrödinger equation cannot describe loss, incoherent repopulation, or the finite lifetime of the dark state; for that we need the density matrix and a master equation. This note builds that machinery in the same $|0\rangle,|1\rangle,|2\rangle$ convention as Note I, derives the optical Bloch equations, and shows how dissipation converts the real light shift and real two-photon coupling of Note I into **complex** quantities whose imaginary parts are precisely the two-photon photoassociation loss rate and the width of an optical Feshbach resonance.

Two limits organize the whole note:

$$
\text{atoms lost after excitation}
\;\;\Longrightarrow\;\;
\text{non-Hermitian shortcut (decaying norm)},
$$

$$
\text{atoms recycled / coherences repopulated}
\;\;\Longrightarrow\;\;
\text{full Lindblad master equation}.
$$

The first is quicker and is enough for loss rates and complex shifts; the second is required for coherent population trapping, electromagnetically induced transparency (EIT), and any steady state.

---

## 1. Where the dissipation comes from

Two qualitatively different dissipative processes act on the $\Lambda$ system.

**(a) Spontaneous emission from $|1\rangle$**, at the total rate $\gamma_1$ (the natural linewidth of the excited molecular state, of order the atomic $P$-state linewidth). This depopulates $|1\rangle$. Where the population goes matters:

- A fraction may return to the initial manifold $|0\rangle$ (elastic-like return to the continuum) or to the target $|2\rangle$ (a genuine radiative-decay pathway into bound ground levels — the mechanism by which one-photon PA actually makes cold molecules).
- The remainder decays to *other* states — deeply bound levels, untrapped hyperfine states, hot free atoms — that leave the three-level system entirely.

In most two-photon PA and optical-Feshbach settings the branching back into $|0\rangle$ or $|2\rangle$ is small, so to a good approximation **decay of $|1\rangle$ is pure loss**. This is what justifies the non-Hermitian shortcut of Section 3.

**(b) Dephasing of the $|0\rangle$–$|2\rangle$ coherence**, at a rate $\gamma_{20}$. Unlike $\gamma_1$ this transfers no population; it destroys the *phase* relation between $|0\rangle$ and $|2\rangle$ that the dark state relies on. Its physical sources are the relative linewidth / frequency jitter of the two laser arms, magnetic-field noise, and — specific to PA — the fact that $|0\rangle$ is a thermal continuum, so different collision energies accumulate phase at different rates (Doppler and thermal dephasing). Because the dark state $|D\rangle$ is a coherence of $|0\rangle$ and $|2\rangle$, $\gamma_{20}$ is what gives it a finite lifetime and sets the ultimate width of the two-photon feature. In the EOM scheme, where the two arms are the carrier and a sideband of *one* laser, the common-mode laser phase noise cancels and $\gamma_{20}$ can be very small — a central experimental advantage, taken up in the EOM note.

---

## 2. The Lindblad master equation

The density operator $\rho$ evolves under the Gorini–Kossakowski–Sudarshan–Lindblad (GKSL, "Lindblad") equation

$$
\dot\rho = -\frac{i}{\hbar}\,[H,\rho] \;+\; \sum_k \mathcal{D}[L_k]\rho,
\qquad
\mathcal{D}[L]\rho \equiv L\rho L^\dagger - \tfrac{1}{2}\big\{L^\dagger L,\rho\big\}.
$$

$H$ is the coherent rotating-frame Hamiltonian of Note I (Section 4). The dissipators $\mathcal D[L_k]$ encode the processes of Section 1 through **collapse (jump) operators** $L_k$:

- **Spontaneous emission** $|1\rangle\to|f\rangle$ into each final channel $f$:
$$
L_{1\to f} = \sqrt{\gamma_{1\to f}}\;|f\rangle\langle 1|,
\qquad
\sum_f \gamma_{1\to f} = \gamma_1 .
$$
For decay into the tracked states, $f\in\{0,2\}$; decay to untracked states is a leak whose collapse operator maps $|1\rangle$ onto a "reservoir" not represented in the $3\times3$ block (it removes trace, i.e. atom number).

- **Ground-state dephasing**:
$$
L_\phi = \sqrt{2\gamma_{20}}\;\Big(\tfrac{1}{2}|2\rangle\langle 2| - \tfrac{1}{2}|0\rangle\langle 0|\Big),
$$
which damps the coherence $\rho_{02}$ at rate $\gamma_{20}$ while leaving populations untouched. (Any operator diagonal in $\{|0\rangle,|2\rangle\}$ with unequal entries generates pure dephasing; this symmetric choice fixes the rate cleanly.)

The action of $\mathcal D[L]$ is read off from its two pieces: $L\rho L^\dagger$ is the **refilling** term (population *arriving* in the jump's target state, coherences rebuilt), while $-\tfrac12\{L^\dagger L,\rho\}$ is the **damping** term (population and coherence *leaving* the jump's source). The non-Hermitian shortcut of the next section keeps only the damping term and drops the refilling.

---

## 3. The non-Hermitian shortcut and complex light shifts

When decay from $|1\rangle$ is pure loss (Section 1a) and we do not need to track where the lost atoms go, the refilling terms $L\rho L^\dagger$ can be dropped. What remains is equivalent to evolving a pure state under a **non-Hermitian effective Hamiltonian** obtained by giving $|1\rangle$ a complex energy:

$$
\tilde H_{\rm eff} = \hbar
\begin{pmatrix}
0 & 0 & \tfrac{1}{2}\Omega_1^{*}\\[4pt]
0 & \delta & \tfrac{1}{2}\Omega_2^{*}\\[4pt]
\tfrac{1}{2}\Omega_1 & \tfrac{1}{2}\Omega_2 & \Delta - \tfrac{i}{2}\gamma_1
\end{pmatrix}
\qquad(\text{basis }\{|0\rangle,|2\rangle,|1\rangle\}).
$$

The replacement $\Delta \to \tilde\Delta \equiv \Delta - \tfrac{i}{2}\gamma_1$ is the Wigner–Weisskopf prescription: the excited level acquires a width $\gamma_1$. Because $\tilde H_{\rm eff}$ is not Hermitian, the norm $\langle\psi|\psi\rangle$ decays — and the decay rate *is* the physical loss rate of atoms from the system.

Now repeat the adiabatic elimination of Note I (Section 6) with the complex detuning. Setting $\dot c_1 = 0$,

$$
c_1 \simeq -\frac{\Omega_1 c_0 + \Omega_2 c_2}{2\,\tilde\Delta},
\qquad
\tilde\Delta = \Delta - \tfrac{i}{2}\gamma_1,
$$

and the effective two-level Hamiltonian in $\{|0\rangle,|2\rangle\}$ becomes complex:

$$
\boxed{\;
H_{\rm eff} = -\frac{\hbar}{4\tilde\Delta}
\begin{pmatrix}
|\Omega_1|^2 & \Omega_1^{*}\Omega_2\\[4pt]
\Omega_1\Omega_2^{*} & |\Omega_2|^2
\end{pmatrix}
+\hbar
\begin{pmatrix}
0 & 0\\ 0 & \delta
\end{pmatrix}.
\;}
$$

Separating real and imaginary parts using $\dfrac{1}{\tilde\Delta} = \dfrac{\Delta + \tfrac{i}{2}\gamma_1}{\Delta^2+\tfrac14\gamma_1^2}$ gives, for the initial state $|0\rangle$,

$$
E_0' = \underbrace{-\,\frac{\hbar|\Omega_1|^2\,\Delta}{4\big(\Delta^2+\tfrac14\gamma_1^2\big)}}_{\text{AC Stark shift }\hbar s_0}
\;-\;\frac{i}{2}\,\hbar\,\underbrace{\frac{|\Omega_1|^2\,\gamma_1}{4\big(\Delta^2+\tfrac14\gamma_1^2\big)}}_{\displaystyle \Gamma_0\;(\text{loss rate})} .
$$

Two real observables have emerged from one complex number:

- **Real part — the AC Stark (light) shift** $s_0$. In the far-detuned limit $\Delta\gg\gamma_1$ it reduces to the $-|\Omega_1|^2/4\Delta$ of Note I. When $|0\rangle$ is the scattering continuum, this shift of the collision energy is what an **optical Feshbach resonance** exploits to tune the scattering length: $|1\rangle$ plays the role of a closed-channel resonance whose position is set optically.

- **Imaginary part — the loss rate** $\Gamma_0$. In the far-detuned limit $\Gamma_0 \to |\Omega_1|^2\gamma_1/4\Delta^2$, the familiar off-resonant photon-scattering rate. As a scattering-length effect it is the **inelastic width** of the optical Feshbach resonance — the price paid in atom loss for a given change in $a$. The single-arm ($L_2$ off) version of $\Gamma_0$ is exactly the one-photon PA loss rate.

The off-diagonal element likewise becomes a complex effective coupling

$$
\Omega_{\rm eff} = \frac{\Omega_1\Omega_2^{*}}{2\tilde\Delta}
= \frac{\Omega_1\Omega_2^{*}}{2}\,\frac{\Delta + \tfrac{i}{2}\gamma_1}{\Delta^2+\tfrac14\gamma_1^2},
$$

whose real part is the coherent two-photon coupling of Note I and whose imaginary part is a **two-photon loss** channel. The interplay of the diagonal loss $\Gamma_0$ and this off-diagonal loss is what produces the characteristic two-photon PA lineshape — including the dark resonance discussed next, where the two interfere destructively.

The shortcut is quantitatively correct whenever repopulation of $|0\rangle,|2\rangle$ by spontaneous emission is negligible. When it is not — or when one wants the true steady state — one must go back to the full master equation, which is the optical Bloch equations.

---

## 4. The optical Bloch equations

Writing $\rho$ in the $\{|0\rangle,|1\rangle,|2\rangle\}$ basis and inserting the Note I Hamiltonian and the dissipators of Section 2 gives the **optical Bloch equations** (OBEs) — the equations of motion for the nine density-matrix elements (three populations, and three coherences with their conjugates). The populations obey

$$
\dot\rho_{11} = -\gamma_1\rho_{11} + \frac{i}{2}\Big(\Omega_1\rho_{01} + \Omega_2\rho_{21} - \Omega_1^{*}\rho_{10} - \Omega_2^{*}\rho_{12}\Big),
$$

$$
\dot\rho_{00} = +\gamma_{1\to 0}\,\rho_{11} + \frac{i}{2}\Big(\Omega_1^{*}\rho_{10} - \Omega_1\rho_{01}\Big),
\qquad
\dot\rho_{22} = +\gamma_{1\to 2}\,\rho_{11} + \frac{i}{2}\Big(\Omega_2^{*}\rho_{12} - \Omega_2\rho_{21}\Big),
$$

where the $\gamma_{1\to f}\rho_{11}$ terms are the refilling from spontaneous emission (absent in the non-Hermitian shortcut, which is why that shortcut does not conserve trace). The coherences obey damped, driven equations:

$$
\dot\rho_{10} = -\Big(\tfrac{\gamma_1}{2} + i\Delta\Big)\rho_{10}
+ \frac{i}{2}\Omega_1(\rho_{00}-\rho_{11}) + \frac{i}{2}\Omega_2\rho_{20},
$$

$$
\dot\rho_{12} = -\Big(\tfrac{\gamma_1}{2} + i(\Delta-\delta)\Big)\rho_{12}
+ \frac{i}{2}\Omega_2(\rho_{22}-\rho_{11}) + \frac{i}{2}\Omega_1\rho_{02},
$$

$$
\dot\rho_{20} = -\Big(\gamma_{20} + i\delta\Big)\rho_{20}
+ \frac{i}{2}\Omega_2^{*}\rho_{10} - \frac{i}{2}\Omega_1\rho_{12}.
$$

The structure is worth reading off. Each coherence relaxes at a rate set by *which* states it connects: the optical coherences $\rho_{10},\rho_{12}$ decay at $\gamma_1/2$ (they involve the lossy $|1\rangle$), while the **ground coherence** $\rho_{20}$ decays only at the small $\gamma_{20}$ (it does not involve $|1\rangle$). This asymmetry — one long-lived coherence among the driven levels — is the entire basis of dark-state physics: it is why a superposition of $|0\rangle$ and $|2\rangle$ can survive while anything touching $|1\rangle$ is rapidly damped.

---

## 5. Steady state: coherent population trapping and EIT with decay

Take the experimentally common regime of a weak free–bound probe $\Omega_1$ and a strong bound–bound coupling $\Omega_2$, and solve for the steady state $\dot\rho = 0$ to lowest order in $\Omega_1$ (so $\rho_{00}\approx 1$, $\rho_{11},\rho_{22}\approx0$). Eliminating $\rho_{20}$ from the $\rho_{10}$ equation gives the probe coherence

$$
\rho_{10}^{\rm ss} = \frac{i\,\Omega_1/2}
{\;\big(\tfrac{\gamma_1}{2} + i\Delta\big) + \dfrac{|\Omega_2|^2/4}{\;\gamma_{20} + i\delta\;}\;}.
$$

This single expression contains the whole story of the dissipative $\Lambda$ system:

- The atom-loss / absorption rate on the probe arm is $\propto \operatorname{Im}\rho_{10}^{\rm ss}$. With $\Omega_2=0$ it is a single Lorentzian in $\Delta$ of width $\gamma_1$ — the ordinary one-photon PA line.

- Turning on $\Omega_2$ adds the second term in the denominator. On two-photon resonance $\delta=0$ it becomes $|\Omega_2|^2/(4\gamma_{20})$, which is *large* when $\gamma_{20}$ is small. The probe coherence — and with it the loss — is **suppressed**: a transparency window opens at $\delta=0$. This is electromagnetically induced transparency; equivalently, the system is pumped into the dark state $|D\rangle$ of Note I, which no longer couples to $|1\rangle$. In PA language, the one-photon loss is quenched exactly where the second arm brings $|2\rangle$ into two-photon resonance — the **dark resonance**, and the primary signal of two-photon PA / bound-state spectroscopy.

- The width of the transparency window is not zero but is set by $\gamma_{20}$ (broadened by power to $\sim |\Omega_2|^2/\gamma_1$). Its depth is limited by the ratio $\gamma_{20}\gamma_1/|\Omega_2|^2$: a perfectly dark resonance requires $\gamma_{20}\to 0$, which is why suppressing ground dephasing (Section 1b, and the EOM common-mode cancellation) is decisive. The *position* of the dip measures the binding energy $\omega_{20}$, shifted by the light shifts of Section 3 — the quantity one is usually after.

The two bright dressed states of Note I reappear here as the two absorption peaks flanking the dip: the **Autler–Townes doublet**, split by $\sim|\Omega_2|$ when $\Omega_2$ is strong. EIT (interference, weak probe) and Autler–Townes (splitting, strong fields) are the same denominator viewed in two limits.

---

## 6. Connection to the optical Feshbach resonance

Sections 3 and 5 are two views of one object. Reinterpret the initial state $|0\rangle$ as the two-atom **scattering continuum** rather than a discrete level. The complex light shift of $|0\rangle$,

$$
E_0' = \hbar s_0 - \tfrac{i}{2}\hbar\,\Gamma_0,
$$

then shifts the collision energy by a complex amount, which is equivalent to shifting the **scattering length** by a complex amount $a \to a + \delta a - i\,\beta$. Schematically, with the excited molecular state $|1\rangle$ acting as the resonance,

$$
\delta a \;\propto\; \frac{\Omega_1^2\,\Delta}{\Delta^2 + \tfrac14\gamma_1^2},
\qquad
\beta \;\propto\; \frac{\Omega_1^2\,\gamma_1}{\Delta^2 + \tfrac14\gamma_1^2},
$$

the same real/imaginary pair as the light shift and loss rate, now read as a tunable elastic scattering length ($\delta a$) accompanied by an unavoidable inelastic loss ($\beta$). This is the **optical Feshbach resonance**: a laser tuned near a free–bound transition tunes $a$, at the cost of loss that scales with the same $\Omega_1^2$. The one-photon scheme forces a fixed trade-off between tuning strength and loss, both governed by the single detuning $\Delta$.

The **second arm $L_2$** is what a three-level treatment adds to this two-level story. Coupling the excited state further to a stable bound level $|2\rangle$ — the dark-resonance interference of Section 5 — modifies the excited state's effective width seen by the continuum. Near the two-photon (dark) resonance the elastic response can be enhanced while the inelastic loss $\beta$ is suppressed by the same destructive interference that produces EIT. This is the principle behind two-color / dark-state optical Feshbach schemes and is the reason the three-level system, not the two-level one, is the right starting point for engineering interactions optically. The quantitative continuum theory — free–bound matrix elements, the reflection approximation, and the resonance's stimulated width — is developed in the photoassociation notes; here we have only located where each piece sits in the three-level algebra.

---

## 7. What has and has not been assumed

- **Markovian, RWA dissipation.** The Lindblad form assumes a memoryless reservoir and the rotating-wave approximation; both are excellent for optical transitions with $\gamma_1 \ll \omega_1,\omega_2$.
- **Loss vs. recycling.** The non-Hermitian shortcut (Section 3) assumes decay of $|1\rangle$ leaves the system; the full OBEs (Section 4) are needed if a significant fraction returns to $|0\rangle$ or $|2\rangle$, or for the true steady state and EIT depth.
- **Discrete $|0\rangle$.** Sections 2–5 treat $|0\rangle$ as a level; the continuum reinterpretation of Section 6 is where photoassociation-specific physics (free–bound couplings, thermal averaging, the collision-energy dependence of $\gamma_{20}$) enters, and is deferred to the PA notes.
- **Given rates.** $\gamma_1$ and $\gamma_{20}$ are taken as phenomenological inputs. Their microscopic origins — radiative lifetime and branching for $\gamma_1$, laser and thermal dephasing for $\gamma_{20}$ — are physics of the specific system and, for $\gamma_{20}$, of the EOM implementation.

---

## Planned notes in this series

- [[Three-Level Systems I - Configurations, Dressed States, and Adiabatic Elimination]] — the closed system: dressed and dark states, adiabatic elimination.
- **Three-Level Systems II** *(this note)* — dissipation, the master equation, optical Bloch equations, complex light shifts, and the optical Feshbach connection.
- **The EOM two-arm scheme** — carrier and sideband of one laser through an electro-optic modulator: sideband spectrum, common-mode phase-noise cancellation (small $\gamma_{20}$), and the consequences for the $\Lambda$ Hamiltonian.

---

### Related notes

- [[Three-Level Systems I - Configurations, Dressed States, and Adiabatic Elimination]] — the closed-system starting point elaborated here.
- [[Photoassociation formula sheet]] — free–bound couplings and one-photon PA loss rates that fix the scale of $\Omega_1$ and $\gamma_1$.
- [[Feshbach Resonance I - Projection Formalism and the Origin of the Resonant Scattering Length]] — the magnetic closed-channel resonance whose complex-energy structure the optical Feshbach resonance reproduces.
