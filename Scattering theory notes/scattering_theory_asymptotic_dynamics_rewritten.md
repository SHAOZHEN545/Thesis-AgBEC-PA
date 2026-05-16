# Scattering Theory I: Asymptotic Dynamics and the Lippmann--Schwinger Equation

This note develops the operator structure behind elementary scattering theory in a form that does not rely on a single incident plane wave plus an outgoing scattered wave. The basic objects are channel labels, asymptotic comparison maps, resolvents, and the transition operator. This is the language one needs before specializing to coordinate-space amplitudes, partial waves, cross sections, or particular multichannel models.

The guiding physical experiment is simple:

$$
\text{prepare separated fragments in an incoming channel}
\quad \longrightarrow \quad
\text{let the exact Hamiltonian act}
\quad \longrightarrow \quad
\text{detect separated fragments in an outgoing channel}.
$$

The formalism below is a precise way of removing from this experiment the trivial motion that the fragments would have had even if no scattering interaction were present. What remains is the nontrivial input-output map.

---

## 1. The two Hamiltonians

Let

$$
H=H_0+V.
$$

The exact Hamiltonian $H$ generates the true laboratory time evolution. The reference Hamiltonian $H_0$ generates the motion used to define separated asymptotic channels. In the simplest elastic one-particle problem, $H_0$ may be just $\mathbf p^2/2m$. In a multichannel problem, $H_0$ may also include internal Hamiltonians of separated fragments, threshold energies, spin labels, bound states of subsystems, and relative kinetic energies.

Write the generalized channel eigenvectors of $H_0$ as

$$
H_0|\alpha\rangle=E_\alpha|\alpha\rangle .
$$

The label $\alpha$ is collective. It may be a momentum vector in a single channel, or it may include a channel index, internal quantum numbers, angular momenta, spin projections, and continuous relative momenta. We use the schematic notation

$$
1=\int d\alpha\,|\alpha\rangle\langle\alpha|,\qquad
\langle\beta|\alpha\rangle=\delta(\beta-\alpha),
$$

where $d\alpha$ denotes both sums over discrete labels and integrations over continuous labels. Likewise, $\delta(\beta-\alpha)$ denotes a mixture of Kronecker deltas and Dirac deltas.

The word "channel" refers to this $H_0$ classification. It is an asymptotic notion. During the collision the state is not a free channel state; it is an exact state evolving under $H$. But far before and far after the collision, the separated fragments can be classified by the eigenstates of $H_0$. Thus an incoming channel $\alpha$ means an exact scattering state whose remote-past asymptote is the free channel state $|\alpha\rangle$. An outgoing channel $\beta$ means the corresponding remote-future detection label.

This distinction is important in multichannel scattering. A channel is not merely a direction of a plane wave. It is a complete asymptotic arrangement of separated degrees of freedom.

---

## 2. Laboratory amplitudes and the interaction comparison

Suppose a source prepares a normalizable incoming packet

$$
|g\rangle=\int d\alpha\,g(\alpha)|\alpha\rangle ,
$$

where the coefficient $g(\alpha)$ is concentrated near the intended incoming channel data. A detector may similarly be represented by an outgoing packet

$$
|h\rangle=\int d\beta\,h(\beta)|\beta\rangle .
$$

The symbols $|g\rangle$ and $|h\rangle$ are most conveniently understood as channel packets specified at a reference time. If preparation happens at time $t_i$ and detection at time $t_f$, then the freely transported channel packets are

$$
e^{-iH_0t_i/\hbar}|g\rangle,\qquad
e^{-iH_0t_f/\hbar}|h\rangle .
$$

The exact laboratory amplitude is therefore

$$
\mathcal A_{hg}(t_f,t_i)
=
\langle h|e^{iH_0t_f/\hbar}
e^{-iH(t_f-t_i)/\hbar}
e^{-iH_0t_i/\hbar}|g\rangle .
$$

This is not a change of physical frame. It is the laboratory amplitude written after factoring out the known free channel motion at the preparation and detection ends. The operator in the middle is called the interaction-picture evolution operator,

$$
U_I(t_f,t_i)
=
e^{iH_0t_f/\hbar}
e^{-iH(t_f-t_i)/\hbar}
e^{-iH_0t_i/\hbar}.
$$

The interaction picture is useful here because a scattering measurement compares the exact evolution with the reference channel evolution. The measured probabilities are unchanged: if one wants the Schrödinger-picture state at a laboratory time, one restores the free channel phases that were removed. The interaction-picture kernel is simply the clean object that maps incoming channel coefficients to outgoing channel coefficients.

For ideal channel labels define

$$
A_{\beta\alpha}(t_f,t_i)
=
\langle\beta|U_I(t_f,t_i)|\alpha\rangle .
$$

For continuum labels this kernel is distribution-valued. Physical amplitudes are obtained only after smearing it with normalizable packets $g$ and $h$.

The operator $U_I$ satisfies

$$
i\hbar\frac{\partial}{\partial t}U_I(t,t_i)
=
V_I(t)U_I(t,t_i),
$$

where

$$
V_I(t)=e^{iH_0t/\hbar}Ve^{-iH_0t/\hbar}.
$$

Equivalently,

$$
U_I(t,t_i)
=
1-\frac{i}{\hbar}\int_{t_i}^{t}dt'\,V_I(t')U_I(t',t_i).
$$

Taking channel matrix elements and inserting the channel identity gives

$$
A_{\beta\alpha}(t,t_i)
=
\delta(\beta-\alpha)
-\frac{i}{\hbar}\int_{t_i}^{t}dt'\int d\gamma\,
V_{\beta\gamma}
e^{i(E_\beta-E_\gamma)t'/\hbar}
A_{\gamma\alpha}(t',t_i),
$$

where

$$
V_{\beta\gamma}=\langle\beta|V|\gamma\rangle .
$$

This equation is the time-dependent starting point. It says that the channel transition amplitude is built from insertions of $V$, with free channel phases between them.

---

## 3. The asymptotic input-output map

**A scattering experiment does not ask for the detailed state during the collision.** It asks what a packet prepared in the remote past becomes when compared with channel detectors in the remote future. On the scattering subspace one defines
$$
S_{\beta\alpha}
=
\langle\beta|S|\alpha\rangle
=
\lim_{t_f\to+\infty,\;t_i\to-\infty}
\langle\beta|U_I(t_f,t_i)|\alpha\rangle ,
$$

with the limit understood through wave packets, adiabatic switching, or Møller operators. Thus $S$ is the asymptotic input-output operator in the channel basis.

The identity contribution in $S$ represents the part of the packet that passes through with no transition in the channel labels. Everything else is produced by the interaction. Since $H$ and $H_0$ are time independent, the nontrivial asymptotic process is invariant under a simultaneous time translation of the entire collision history. This invariance is what produces total channel-energy conservation.

The origin of the energy delta function can be seen directly from the Dyson series. The first-order term is

$$
S^{(1)}_{\beta\alpha}
=
-\frac{i}{\hbar}
\int_{-\infty}^{+\infty}dt\,
\langle\beta|V_I(t)|\alpha\rangle .
$$

Since

$$
\langle\beta|V_I(t)|\alpha\rangle
=
e^{i(E_\beta-E_\alpha)t/\hbar}V_{\beta\alpha},
$$

one obtains

$$
S^{(1)}_{\beta\alpha}
=
-2\pi i\,\delta(E_\beta-E_\alpha)V_{\beta\alpha}.
$$

At second order,

$$
S^{(2)}_{\beta\alpha}
=
\left(-\frac{i}{\hbar}\right)^2
\int_{-\infty}^{+\infty}dt_1
\int_{-\infty}^{t_1}dt_2
\int d\gamma\,
V_{\beta\gamma}V_{\gamma\alpha}
e^{i(E_\beta-E_\gamma)t_1/\hbar}
e^{i(E_\gamma-E_\alpha)t_2/\hbar}.
$$

Set $\tau=t_1-t_2\geq 0$. The phase separates as

$$
e^{i(E_\beta-E_\alpha)t_1/\hbar}
e^{i(E_\alpha-E_\gamma)\tau/\hbar}.
$$

The integral over the overall time $t_1$ gives the same universal factor

$$
2\pi\hbar\,\delta(E_\beta-E_\alpha).
$$

The remaining ordered time interval is convergent after the usual infinitesimal damping and gives

$$
-\frac{i}{\hbar}
\int_0^{+\infty}d\tau\,
e^{i(E_\alpha-E_\gamma)\tau/\hbar}e^{-\eta\tau/\hbar}
=
\frac{1}{E_\alpha-E_\gamma+i\eta}.
$$

Therefore

$$
S^{(2)}_{\beta\alpha}
=
-2\pi i\,\delta(E_\beta-E_\alpha)
\int d\gamma\,
V_{\beta\gamma}
\frac{1}{E_\alpha-E_\gamma+i0}
V_{\gamma\alpha}.
$$

The same structure persists to all orders. One overall time integral gives energy conservation, while the ordered time differences give the energy denominators of intermediate channel propagation. This motivates the definition

$$
S_{\beta\alpha}
=
\delta(\beta-\alpha)
-
2\pi i\,\delta(E_\beta-E_\alpha)T_{\beta\alpha}(E_\alpha).
$$

This equation is a definition of the reduced transition amplitude $T_{\beta\alpha}$, but it is not an arbitrary convention. The Dyson expansion shows that $T$ is precisely the coefficient that remains after removing the identity term and the universal on-shell energy-conservation delta function.

The first terms are

$$
T_{\beta\alpha}(E)
=
V_{\beta\alpha}
+
\int d\gamma\,
V_{\beta\gamma}
\frac{1}{E-E_\gamma+i0}
V_{\gamma\alpha}
+\cdots .
$$

Thus the first Born approximation is

$$
T_{\beta\alpha}(E)\simeq V_{\beta\alpha}.
$$

It is the leading term of the same transition operator that later satisfies an exact integral equation.

Only the on-shell part of $T$ appears in $S$, because $S$ contains $\delta(E_\beta-E_\alpha)$. The operator $T(E)$ is nevertheless defined as a function of a spectral parameter $E$ because the integral equation that sums repeated interactions naturally depends on that parameter. Off-shell matrix elements are useful inside the equation; the physical asymptotic transition uses the on-shell value.

---

## 4. Resolvents and boundary prescriptions

The free resolvent is the operator-valued function

$$
G_0(z)=\frac{1}{z-H_0}
$$

away from the spectrum of $H_0$. Scattering requires approaching the continuous spectrum from one side of the complex energy plane. The two boundary values are

$$
G_0^{(+)}(E)=\frac{1}{E-H_0+i0},
\qquad
G_0^{(-)}(E)=\frac{1}{E-H_0-i0}.
$$

The signs are not decorative. They encode a time boundary condition. With the convention that Schrödinger phases are $e^{-iEt/\hbar}$,

$$
G_0^{(+)}(E)
=
-\frac{i}{\hbar}
\lim_{\eta\downarrow0}
\int_0^{+\infty}d\tau\,
e^{i(E-H_0)\tau/\hbar}
e^{-\eta\tau/\hbar}.
$$

This representation is just the elementary half-line integral

$$
-\frac{i}{\hbar}
\int_0^{+\infty}d\tau\,
e^{i(E-E_\gamma)\tau/\hbar}
e^{-\eta\tau/\hbar}
=
\frac{1}{E-E_\gamma+i\eta}.
$$

Thus $+i0$ appears whenever an intermediate free channel propagates through a positive time interval after an earlier interaction. This is the same half-line integral that arose from the time ordering in the Dyson expansion.

The opposite prescription is

$$
G_0^{(-)}(E)
=
\frac{i}{\hbar}
\lim_{\eta\downarrow0}
\int_0^{+\infty}d\tau\,
e^{-i(E-H_0)\tau/\hbar}
e^{-\eta\tau/\hbar}.
$$

Equivalently, it is the boundary value appropriate to the opposite time orientation.

The distribution identity

$$
\frac{1}{x\pm i0}
=
\operatorname{P}\frac{1}{x}
\mp i\pi\delta(x)
$$

is often useful, but it should not be mistaken for the primary meaning of the prescription. The primary meaning is the selection of a boundary condition. In coordinate space, for the usual kinetic-energy Hamiltonian, $G_0^{(+)}$ produces outgoing spherical waves and $G_0^{(-)}$ produces incoming spherical waves. In the abstract channel language, the same distinction is expressed by whether the scattering solution is selected by remote-past preparation or by remote-future testing.

The phrase "incoming state" can therefore be slightly misleading if it is attached too literally to the sign. A state prepared in the remote past and allowed to scatter forward in time is represented by a $+$ scattering vector. That $+$ vector has an incoming free asymptote in the past and outgoing scattered behavior in the future. The $+i0$ prescription is the analytic trace of that forward-in-time construction.

---

## 5. The transition operator

The Born series suggested by the Dyson expansion can be summed by the operator equation

$$
T(E)=V+VG_0^{(+)}(E)T(E).
$$

In the channel basis,

$$
T_{\beta\alpha}(E)
=
V_{\beta\alpha}
+
\int d\gamma\,
V_{\beta\gamma}
\frac{1}{E-E_\gamma+i0}
T_{\gamma\alpha}(E).
$$

This equation says that a transition from $\alpha$ to $\beta$ is either a single interaction $V_{\beta\alpha}$, or an interaction from an intermediate channel $\gamma$ into $\beta$ after the system has already accumulated the full transition amplitude from $\alpha$ into $\gamma$ at the same total energy.

Iterating the equation gives

$$
T(E)
=
V
+
VG_0^{(+)}(E)V
+
VG_0^{(+)}(E)VG_0^{(+)}(E)V
+\cdots .
$$

For multichannel scattering the integration over $\gamma$ includes all intermediate channel labels. Open channels and closed channels are treated in the same operator equation. Closed channels do not appear as asymptotic final states at a given energy, but they can still contribute virtually through the resolvent.

The transition operator is the reduced dynamical part of the scattering matrix. Once the universal identity and energy-conservation factors have been separated, the remaining physics is encoded in $T$.

---

## 6. Stationary scattering vectors

The stationary scattering vector associated with an incoming channel $\alpha$ is defined by

$$
|\psi_\alpha^{(+)}\rangle
=
|\alpha\rangle
+
G_0^{(+)}(E_\alpha)V|\psi_\alpha^{(+)}\rangle .
$$

This is the Lippmann--Schwinger equation. It is not a separate postulate added after the time-dependent construction. It is the fixed-energy form of the same asymptotic preparation problem. The free vector $|\alpha\rangle$ gives the remote channel data; the resolvent supplies the boundary prescription for the scattered part.

Multiplying by $V$ gives

$$
V|\psi_\alpha^{(+)}\rangle
=
V|\alpha\rangle
+
VG_0^{(+)}(E_\alpha)V|\psi_\alpha^{(+)}\rangle .
$$

Comparing with

$$
T(E_\alpha)|\alpha\rangle
=
V|\alpha\rangle
+
VG_0^{(+)}(E_\alpha)T(E_\alpha)|\alpha\rangle
$$

shows that

$$
T(E_\alpha)|\alpha\rangle
=
V|\psi_\alpha^{(+)}\rangle .
$$

Therefore

$$
T_{\beta\alpha}(E_\alpha)
=
\langle\beta|T(E_\alpha)|\alpha\rangle
=
\langle\beta|V|\psi_\alpha^{(+)}\rangle .
$$

This formula has one channel vector and one exact scattering vector because $T$ is the reduced amplitude between an asymptotic label and a fully dressed collision state. The interaction history is contained in $|\psi_\alpha^{(+)}\rangle$; the detector label is supplied by $\langle\beta|$.

The Lippmann--Schwinger equation also implies the exact stationary eigenvalue equation. Apply $E_\alpha-H_0$ to both sides:

$$
(E_\alpha-H_0)|\psi_\alpha^{(+)}\rangle
=
(E_\alpha-H_0)|\alpha\rangle
+
(E_\alpha-H_0)G_0^{(+)}(E_\alpha)V|\psi_\alpha^{(+)}\rangle .
$$

Since $H_0|\alpha\rangle=E_\alpha|\alpha\rangle$, the first term vanishes. Since $(E_\alpha-H_0)G_0^{(+)}(E_\alpha)$ is the identity in the distributional sense appropriate to the chosen boundary value, the second term gives

$$
(E_\alpha-H_0)|\psi_\alpha^{(+)}\rangle
=
V|\psi_\alpha^{(+)}\rangle .
$$

Equivalently,

$$
H|\psi_\alpha^{(+)}\rangle
=
E_\alpha|\psi_\alpha^{(+)}\rangle .
$$

Thus $|\psi_\alpha^{(+)}\rangle$ is a generalized eigenvector of the exact Hamiltonian, not of $H_0$. What makes it a scattering state labelled by $\alpha$ is its asymptotic boundary condition.

There is a companion solution

$$
|\psi_\beta^{(-)}\rangle
=
|\beta\rangle
+
G_0^{(-)}(E_\beta)V|\psi_\beta^{(-)}\rangle .
$$

It is selected by the opposite boundary prescription. For Hermitian interactions, the same on-shell transition amplitude can be written in either form,

$$
T_{\beta\alpha}(E)
=
\langle\beta|V|\psi_\alpha^{(+)}\rangle
=
\langle\psi_\beta^{(-)}|V|\alpha\rangle,
\qquad
E=E_\alpha=E_\beta.
$$

The two forms are often called prior and post forms. They are equal on shell because they describe the same reduced input-output amplitude using opposite asymptotic comparisons.

---

## 7. Møller operators

The time-dependent and stationary descriptions are tied together by the Møller operators. With the convention used here,

$$
\Omega^{(+)}
=
\operatorname{s-}\lim_{t\to-\infty}
e^{iHt/\hbar}e^{-iH_0t/\hbar},
$$

and

$$
\Omega^{(-)}
=
\operatorname{s-}\lim_{t\to+\infty}
e^{iHt/\hbar}e^{-iH_0t/\hbar}.
$$

The superscript refers to the boundary prescription of the corresponding scattering vector, not simply to the sign of the time limit.

The strong limit means convergence on vectors, not uniform convergence of operators. More explicitly, for every normalizable channel packet $|g\rangle$ in the scattering subspace,

$$
\left\|
e^{iHt/\hbar}e^{-iH_0t/\hbar}|g\rangle
-
\Omega^{(+)}|g\rangle
\right\|
\to0
\qquad
(t\to-\infty),
$$

and similarly for $\Omega^{(-)}$ as $t\to+\infty$. This is weaker than convergence in operator norm, but it is exactly the kind of convergence needed for physical wave packets. The restriction to the scattering subspace excludes states that are not described by asymptotic free channels, such as bound states of the full Hamiltonian not included among the channel states.

The Møller operators generate the exact scattering vectors:

$$
|\psi_\alpha^{(+)}\rangle=\Omega^{(+)}|\alpha\rangle,
\qquad
|\psi_\beta^{(-)}\rangle=\Omega^{(-)}|\beta\rangle .
$$

They also give the scattering operator

$$
S=\Omega^{(-)\dagger}\Omega^{(+)} .
$$

This formula is the clean asymptotic comparison between the exact state determined by remote-past preparation and the exact state associated with remote-future detection. It is also the same $S$ that appeared in the interaction-picture limit. Indeed, formally,

$$
\Omega^{(-)\dagger}\Omega^{(+)}
=
\lim_{t_f\to+\infty,\;t_i\to-\infty}
e^{iH_0t_f/\hbar}
e^{-iH(t_f-t_i)/\hbar}
e^{-iH_0t_i/\hbar},
$$

which is exactly the limiting form of $U_I(t_f,t_i)$. Therefore

$$
S_{\beta\alpha}
=
\langle\beta|S|\alpha\rangle
=
\langle\psi_\beta^{(-)}|\psi_\alpha^{(+)}\rangle .
$$

The stationary overlap, the Møller-operator expression, and the interaction-picture limit are three descriptions of the same asymptotic input-output map.

---

## 8. Probabilities and rates

For continuum labels, $S_{\beta\alpha}$ is not an ordinary number but a distribution. Physical probabilities require wave packets or integration over finite final bins. After separating out the identity term and the energy-conserving delta function, the standard transition-rate expression is

$$
dW_{\alpha\to\beta}
=
\frac{2\pi}{\hbar}
|T_{\beta\alpha}(E_\alpha)|^2
\delta(E_\beta-E_\alpha)d\mu(\beta),
$$

where $d\mu(\beta)$ includes the appropriate sums over discrete final labels and integrations over continuous final labels.

This is the scattering version of Fermi's golden rule with the first-order interaction matrix element replaced by the exact transition matrix element. Cross sections are then obtained by dividing the appropriate final transition rate by the incoming flux of the prepared beam. The detailed expression for the flux depends on the representation and belongs naturally to the coordinate-space or partial-wave formulation.

---

## 9. Logical summary

The channel basis is defined by the reference Hamiltonian,

$$
H_0|\alpha\rangle=E_\alpha|\alpha\rangle .
$$

Exact scattering is described by comparing true evolution with free channel evolution at the initial and final ends,

$$
U_I(t_f,t_i)
=
e^{iH_0t_f/\hbar}
e^{-iH(t_f-t_i)/\hbar}
e^{-iH_0t_i/\hbar}.
$$

The scattering operator is the asymptotic limit of this comparison,

$$
S_{\beta\alpha}
=
\lim_{t_f\to+\infty,\;t_i\to-\infty}
\langle\beta|U_I(t_f,t_i)|\alpha\rangle .
$$

Time-translation invariance of the infinite-time collision gives energy conservation, and the reduced transition operator is defined by

$$
S_{\beta\alpha}
=
\delta(\beta-\alpha)
-
2\pi i\,\delta(E_\beta-E_\alpha)T_{\beta\alpha}(E_\alpha).
$$

The time-ordered construction yields the resolvent prescription

$$
G_0^{(+)}(E)=\frac{1}{E-H_0+i0}
$$

and the exact transition equation

$$
T(E)=V+VG_0^{(+)}(E)T(E).
$$

Equivalently, the stationary scattering vector satisfies

$$
|\psi_\alpha^{(+)}\rangle
=
|\alpha\rangle
+
G_0^{(+)}(E_\alpha)V|\psi_\alpha^{(+)}\rangle ,
$$

and the physical on-shell transition amplitude is

$$
T_{\beta\alpha}(E_\alpha)
=
\langle\beta|V|\psi_\alpha^{(+)}\rangle .
$$

The opposite boundary prescription gives

$$
|\psi_\beta^{(-)}\rangle
=
|\beta\rangle
+
G_0^{(-)}(E_\beta)V|\psi_\beta^{(-)}\rangle ,
$$

and on shell,

$$
T_{\beta\alpha}(E)
=
\langle\beta|V|\psi_\alpha^{(+)}\rangle
=
\langle\psi_\beta^{(-)}|V|\alpha\rangle .
$$

Finally, the Møller operators provide the invariant bridge between the time-dependent and stationary pictures,

$$
\Omega^{(+)}
=
\operatorname{s-}\lim_{t\to-\infty}
e^{iHt/\hbar}e^{-iH_0t/\hbar},
\qquad
\Omega^{(-)}
=
\operatorname{s-}\lim_{t\to+\infty}
e^{iHt/\hbar}e^{-iH_0t/\hbar},
$$

with

$$
S=\Omega^{(-)\dagger}\Omega^{(+)} .
$$

This is the operator-level entrance to scattering theory. Coordinate-space outgoing waves, scattering amplitudes, partial waves, and differential cross sections are later representations of the same asymptotic structure.
