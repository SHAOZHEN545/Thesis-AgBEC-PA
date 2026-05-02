# Body-Frame Angular Factor for Photoassociation

A tutorial derivation, with the cesium
$0_g^-(6s+6p_{3/2})$, $f+f=4+4$, even-$\ell$ channel as a worked example.

---

## 1. What quantity are we calculating?

In photoassociation, two ground-state atoms collide on a ground molecular potential and absorb a photon into a bound excited molecular state. For a specific entrance/final channel $\nu$, the laser coupling is

$$
V_{b,\nu}
=
\frac{\mathcal E_0}{2}
\langle f,\nu|
\boldsymbol\epsilon\cdot\mathbf d
|i,\nu\rangle.
$$

Here $\mathcal E_0$ is the electric-field amplitude, $\boldsymbol\epsilon$ is the laser polarization, and $\mathbf d$ is the molecular electric-dipole operator.

The stimulated width depends on the square of this coupling. Using energy-normalized continuum states,

$$
\Gamma_b(E,\ell)
=
\frac{2\pi}{\hbar}|V_b(E,\ell)|^2.
$$

Therefore the object we ultimately need is not just the amplitude $V_{b,\nu}$, but the summed/averaged line strength built from $|V_{b,\nu}|^2$.

After factoring out the radial free-bound overlap and the reduced atomic dipole, the coupling is usually written as

$$
V_{b,\nu}(E,\ell)
=
\frac{\mathcal E_0 d_{\rm at}}{2}
\langle \psi_v|\chi_{E\ell}\rangle
\,a_\nu.
$$

The dimensionless amplitude $a_\nu$ contains the angular, rotational, polarization, electronic, hyperfine, exchange-symmetry, and body-frame projection algebra.

The experimentally relevant angular factor is a line strength,

$$
A(g,e,\boldsymbol\epsilon)
=
\sum_{\rm final}
\overline{|a_\nu|^2}_{\rm initial},
$$

where the bar means an average over the statistically populated entrance channels, including symmetry constraints.

For the cesium channel

$$
0_g^-(6s+6p_{3/2}),
\qquad
f+f=4+4,
\qquad
\text{even }\ell,
$$

the tabulated factor is

$$
A
=
\frac{1}{3}
\times
\frac{45}{81}
\times
\frac{25}{144}
=
\frac{125}{3888}.
$$

The three factors have different origins:

- $1/3$: rotational, orientation, and polarization average;
- $45/81$: bosonic exchange-symmetry weight for the entrance hyperfine channel;
- $25/144$: body-fixed internal electronic/hyperfine line strength after the correct molecular symmetry projection.

The most delicate point is the last one. In particular, the value $25/144$ is obtained only after excluding the body-frame $q=0$ dipole component. That exclusion is not an atomic Clebsch--Gordan rule. It is a molecular reflection-symmetry filter.

---

## 2. Frames, coordinates, and Hilbert spaces

After separating the center of mass, the nuclear relative coordinate is

$$
\mathbf R=\mathbf r_2-\mathbf r_1.
$$

Its magnitude is $R=|\mathbf R|$. Its orientation specifies the molecular body frame.

Throughout this note, we use the following axis convention:

$$
(X,Y,Z):\quad \text{space-fixed/lab-frame axes},
$$

$$
(x,y,z):\quad \text{body-fixed/molecular-frame axes},
$$

with

$$
z\parallel \mathbf R.
$$

Lab-frame spherical components carry labels $p=0,\pm1$. Body-frame spherical components carry labels $q=0,\pm1$.

The total Hilbert space is organized as

$$
\mathcal H
=
\mathcal H_R
\otimes
\mathcal H_{\rm orient}
\otimes
\mathcal H_{\rm int}.
$$

Here:

- $\mathcal H_R$ contains the radial nuclear motion;
- $\mathcal H_{\rm orient}$ contains the orientation of the molecular frame relative to the lab frame;
- $\mathcal H_{\rm int}$ contains electronic, spin, nuclear-spin, hyperfine, and molecular-symmetry labels.

This separation is the cleanest way to keep track of which operator acts where.

---

## 3. Rotational states as abstract kets

A molecular rotational state should first be viewed as an abstract ket in $\mathcal H_{\rm orient}$:

$$
|J M \Omega\rangle_{\rm orient}.
$$

Here:

- $J$ is the total rotational angular momentum of the molecule, or more generally the angular momentum associated with rotation of the molecular frame;
- $M$ is its projection on the lab-frame $Z$ axis;
- $\Omega$ is the projection of the relevant body-fixed angular momentum on the molecular $z$ axis.

For an entrance scattering channel, the analogous orientation ket may be written

$$
|\ell m_\ell \Omega_i\rangle_{\rm orient},
$$

where $\ell$ is the partial wave and $m_\ell$ is its lab-frame projection. In the simplest central-potential limit one often thinks of this as a spherical harmonic state, but for molecular body-frame algebra it is better to keep the full symmetric-top notation until the end.

Only when we want a coordinate representation do we insert the orientation identity

$$
\mathbf 1_{\rm orient}
=
\int d\eta\,|\eta\rangle\langle \eta|,
$$

where

$$
\eta=(\alpha,\beta,\gamma),
\qquad
 d\eta=d\alpha\,\sin\beta\,d\beta\,d\gamma.
$$

Then

$$
\langle \eta|J M\Omega\rangle
=
\sqrt{\frac{2J+1}{8\pi^2}}
D^{J*}_{M\Omega}(\eta).
$$

Equivalently,

$$
|J M\Omega\rangle
=
\sqrt{\frac{2J+1}{8\pi^2}}
\int d\eta\,
D^{J*}_{M\Omega}(\eta)|\eta\rangle.
$$

This is not a new physical assumption. It is just the coordinate representation of the abstract orientation ket.

For $\Omega=0$, the Wigner $D$ function reduces to the familiar spherical-harmonic description, up to normalization and phase conventions.

---

## 4. Abstract channel states before any wavefunctions

Before projecting into coordinate space, write the initial and final channel states as tensor-product states:

$$
|i,\nu\rangle
=
|\chi_{E\ell}\rangle_R
\otimes
|\ell m_\ell \Omega_i\rangle_{\rm orient}
\otimes
|\lambda_i\rangle_{\rm int},
$$

and

$$
|f,\nu\rangle
=
|\psi_v\rangle_R
\otimes
|J M \Omega_f\rangle_{\rm orient}
\otimes
|\lambda_f\rangle_{\rm int}.
$$

Here $\lambda_i$ and $\lambda_f$ are placeholders for internal labels. They may include:

- atomic electronic angular momenta $j_g,j_e$;
- electronic projection quantum numbers $\omega$;
- nuclear spin projections $m_I$;
- coupled hyperfine labels $f,m_f,F_t,M_F$;
- molecular labels such as $g/u$, $0^\pm$, and $\Omega$;
- exchange-symmetrized combinations for identical atoms.

The point of this notation is that no wavefunction has been introduced yet. We only project into $R$ or $\eta$ coordinate space when doing so is useful.

---

## 5. Starting from the physical interaction

The channel coupling is

$$
V_{b,\nu}
=
\frac{\mathcal E_0}{2}
\langle f,\nu|
\boldsymbol\epsilon\cdot\mathbf d
|i,\nu\rangle.
$$

At this stage the interaction is simply $\boldsymbol\epsilon\cdot\mathbf d$. There is no need yet to rotate the dipole operator. The rotation becomes necessary only after we ask how to evaluate the electronic molecular matrix element.

Using the abstract tensor-product structure, the matrix element has the schematic form

$$
\langle f|
\boldsymbol\epsilon\cdot\mathbf d
|i\rangle
=
\langle \psi_v|\,
\langle J M\Omega_f|\,
\langle \lambda_f|
\boldsymbol\epsilon\cdot\mathbf d
|\chi_{E\ell}\rangle
|\ell m_\ell\Omega_i\rangle
|\lambda_i\rangle.
$$

In photoassociation, the free-bound overlap is dominated by a relatively long range of internuclear separations. Under the Condon approximation, the electronic dipole matrix element is taken to vary slowly with $R$ over the important region. Therefore the radial part factors out:

$$
\langle \psi_v|\chi_{E\ell}\rangle
=
\int_0^\infty dR\,\psi_v^*(R)\chi_{E\ell}(R).
$$

Then

$$
V_{b,\nu}
=
\frac{\mathcal E_0}{2}
\langle \psi_v|\chi_{E\ell}\rangle
\,
\langle J M\Omega_f,\lambda_f|
\boldsymbol\epsilon\cdot\mathbf d
|\ell m_\ell\Omega_i,\lambda_i\rangle.
$$

Now we have separated the radial free-bound Franck--Condon factor from the angular/internal matrix element.

---

## 6. Why the body-frame dipole appears

The laser polarization is specified in the lab frame. Therefore the scalar product is naturally written using lab-frame spherical components:

$$
\boldsymbol\epsilon\cdot\mathbf d
=
\sum_{p=-1}^{1}
(-1)^p
\epsilon_p^{\rm lab}
d_{-p}^{\rm lab}.
$$

However, molecular electronic states are naturally labeled in the body frame. Hund-case molecular labels such as $\Omega$, $0_g^-$, and $0_u^+$ refer to projections and symmetries with respect to the internuclear axis.

There is one important subtlety. In a rotational state such as $|JM\Omega\rangle$, the molecular orientation is not a fixed classical angle. The molecule is in a quantum state over possible orientations. Therefore we should not immediately write a fixed-angle rotation formula as if the molecule had a definite orientation.

Instead, first project onto the orientation-coordinate basis:

$$
\mathbf 1_{\rm orient}
=
\int d\eta\,|\eta\rangle\langle\eta|.
$$

For a basis state $|\eta\rangle=|\alpha,\beta,\gamma\rangle$, the molecule has a definite orientation. At that fixed orientation, the lab and body frames are related by the rotation $R(\eta)$. For a rank-$k$ spherical tensor, a fixed rotation gives

$$
\mathscr R(\eta)\,
T_q^{(k)}
\mathscr R^\dagger(\eta)
=
\sum_{q'=-k}^{k}
D^k_{q'q}(\eta)\,
T_{q'}^{(k)}.
$$

For the electric dipole, $k=1$. With the phase and active/passive convention used in this note, the fixed-orientation relation between lab-frame and body-frame dipole components is written as

$$
d_p^{\rm lab}(\eta)
=
\sum_{q=-1}^{1}
D^{1*}_{pq}(\eta)\,
d_q^{\rm body}.
$$

Here $\eta$ is an ordinary number-valued orientation, not an operator. This equation says: if the molecule is known to point in the orientation specified by $\eta$, then the lab-frame component $p$ is a linear combination of the body-frame components $q$.

Now return to the quantum rotational problem. Since the orientation is not fixed, the full lab-frame dipole operator must act correctly on every orientation component of the rotational state. In the orientation-coordinate representation, this means

$$
{}_{\rm orient}\langle\eta'|
d_p^{\rm lab}
|\eta\rangle_{\rm orient}
=
\delta(\eta'-\eta)
\sum_{q=-1}^{1}
D^{1*}_{pq}(\eta)\,
d_q^{\rm body}.
$$

The object on the right is still an operator on the internal electronic Hilbert space. The delta function expresses that the electric dipole operator acts on the internal electronic coordinates and does not itself change the orientation coordinate.

Equivalently, in abstract operator form,

$$
d_p^{\rm lab}
=
\int d\eta\,
|\eta\rangle
\left[
\sum_{q=-1}^{1}
D^{1*}_{pq}(\eta)\,
d_q^{\rm body}
\right]
\langle\eta|.
$$

This motivates the compact notation

$$
D^{1*}_{pq}(\hat\eta)
=
\int d\eta\,
|\eta\rangle
D^{1*}_{pq}(\eta)
\langle\eta|,
$$

so that

$$
D^{1*}_{pq}(\hat\eta)|\eta\rangle
=
D^{1*}_{pq}(\eta)|\eta\rangle.
$$

Therefore the full operator identity is

$$
d_p^{\rm lab}
=
\sum_{q=-1}^{1}
D^{1*}_{pq}(\hat\eta)
d_q^{\rm body}.
$$

This equation should be understood as a quantum version of the fixed-orientation rotation formula. The Wigner-$D$ factor acts diagonally on the orientation Hilbert space, while $d_q^{\rm body}$ acts on the internal electronic Hilbert space:

$$
D^{1*}_{pq}(\hat\eta):
\mathcal H_{\rm orient}\rightarrow \mathcal H_{\rm orient},
\qquad
d_q^{\rm body}:
\mathcal H_{\rm int}\rightarrow \mathcal H_{\rm int}.
$$

Substituting this into the scalar product gives

$$
\boldsymbol\epsilon\cdot\mathbf d
=
\sum_{p,q}
(-1)^p
\epsilon_p^{\rm lab}
D^{1*}_{-p,q}(\hat\eta)
d_q^{\rm body}.
$$

This is the precise point where the lab-frame photon polarization is converted into body-frame molecular components. The conversion is not made by assuming a deterministic molecular orientation. Rather, it is made by resolving the rotational state into definite-orientation components, applying the ordinary fixed-angle tensor rotation in each component, and then rewriting the result as the diagonal orientation operator $D^{1*}_{pq}(\hat\eta)$.

---

## 7. Factorized expression for the angular amplitude

Substitute the rotated dipole expression into the factorized coupling:

$$
V_{b,\nu}
=
\frac{\mathcal E_0}{2}
\langle \psi_v|\chi_{E\ell}\rangle
\sum_{p,q}
(-1)^p
\epsilon_p^{\rm lab}
\langle J M\Omega_f,\lambda_f|
D^{1*}_{-p,q}(\hat\eta)d_q^{\rm body}
|\ell m_\ell\Omega_i,\lambda_i\rangle.
$$

Since $D^{1*}_{-p,q}(\hat\eta)$ acts on the orientation Hilbert space and $d_q^{\rm body}$ acts on the internal Hilbert space, the matrix element separates:

$$
\begin{aligned}
V_{b,\nu}
&=
\frac{\mathcal E_0}{2}
\langle \psi_v|\chi_{E\ell}\rangle
\sum_{p,q}
(-1)^p
\epsilon_p^{\rm lab}
\\
&\quad\times
\langle J M\Omega_f|
D^{1*}_{-p,q}(\hat\eta)
|\ell m_\ell\Omega_i\rangle
\\
&\quad\times
\langle \lambda_f|
 d_q^{\rm body}
|\lambda_i\rangle.
\end{aligned}
$$

For a homonuclear alkali molecule, the molecular dipole is the sum of the two atomic dipoles:

$$
\mathbf d=\mathbf d_1+\mathbf d_2.
$$

Pull out the reduced atomic dipole matrix element $d_{\rm at}$ by defining

$$
\mathcal M_q(\lambda_f,\lambda_i)
=
\left\langle
\lambda_f
\left|
\frac{d_{1q}^{\rm body}+d_{2q}^{\rm body}}{d_{\rm at}}
\right|
\lambda_i
\right\rangle.
$$

Then

$$
V_{b,\nu}
=
\frac{\mathcal E_0 d_{\rm at}}{2}
\langle \psi_v|\chi_{E\ell}\rangle
 a_\nu,
$$

with

$$
\boxed{
a_\nu
=
\sum_{p,q}
(-1)^p
\epsilon_p^{\rm lab}
\langle J M\Omega_f|
D^{1*}_{-p,q}(\hat\eta)
|\ell m_\ell\Omega_i\rangle
\mathcal M_q(\lambda_f,\lambda_i).
}
$$

This equation is the main structural result of the note.

---

## 8. Coordinate representation of the rotational matrix element

If desired, the orientation part can be evaluated by inserting

$$
\mathbf 1_{\rm orient}
=
\int d\eta\,|\eta\rangle\langle\eta|.
$$

Then

$$
\begin{aligned}
&\langle J M\Omega_f|
D^{1*}_{-p,q}(\hat\eta)
|\ell m_\ell\Omega_i\rangle
\\
&=
\int d\eta\,
\langle J M\Omega_f|\eta\rangle
D^{1*}_{-p,q}(\eta)
\langle \eta|\ell m_\ell\Omega_i\rangle.
\end{aligned}
$$

Using

$$
\langle \eta|J M\Omega\rangle
=
\sqrt{\frac{2J+1}{8\pi^2}}
D^{J*}_{M\Omega}(\eta),
$$

this becomes a triple-$D$ integral. Up to phase-convention details,

$$
\begin{aligned}
&\langle J M\Omega_f|
D^{1*}_{-p,q}
|\ell m_\ell\Omega_i\rangle
\\
&\propto
(-1)^{M-\Omega_f}
\sqrt{(2J+1)(2\ell+1)}
\begin{pmatrix}
J & 1 & \ell\\
-M & -p & m_\ell
\end{pmatrix}
\begin{pmatrix}
J & 1 & \ell\\
-\Omega_f & q & \Omega_i
\end{pmatrix}.
\end{aligned}
$$

This is the rotational, orientation, and Hönl--London part of the angular factor.

---

## 9. From amplitude to line strength

For one resolved channel $\nu$, the stimulated width contains

$$
|V_{b,\nu}|^2
=
\left(\frac{\mathcal E_0d_{\rm at}}{2}\right)^2
|\langle \psi_v|\chi_{E\ell}\rangle|^2
|a_\nu|^2.
$$

If the experiment does not resolve the initial and final angular subchannels, we sum over unresolved final labels and average over the populated initial labels:

$$
A(g,e,\boldsymbol\epsilon)
=
\sum_{\rm final}
\overline{|a_\nu|^2}_{\rm initial}.
$$

This step must be done only after deciding which molecular symmetry sectors are part of the transition being modeled. In particular, the allowed set of $q$ values is not determined only by atomic Clebsch--Gordan coefficients. It is also constrained by molecular symmetry.

---

## 10. Generic internal amplitude for alkali photoassociation

For an alkali atom,

$$
j_g=\frac12
$$

for the ground $nS_{1/2}$ state. For excitation to the D lines,

$$
j_e=
\begin{cases}
\frac12, & \text{D1 line},\\[2mm]
\frac32, & \text{D2 line}.
\end{cases}
$$

A one-atom body-frame dipole matrix element has the Wigner--Eckart form

$$
\frac{
\langle nP_{j_e},\omega_e|
 d_q^{\rm body}
|nS_{1/2},\omega_g\rangle
}{d_{\rm at}}
=
\langle 1q;\tfrac12\omega_g|j_e\omega_e\rangle.
$$

Thus the atomic CG coefficient enforces

$$
\omega_e=\omega_g+q.
$$

This atomic rule alone allows any $q=0,\pm1$ that satisfies the angular-momentum projection constraints. It does not by itself impose molecular reflection symmetry, $g/u$ symmetry, or exchange symmetry.

For two atoms, the internal amplitude is built from two coherent pathways:

1. atom 1 absorbs the photon;
2. atom 2 absorbs the photon.

For homonuclear molecules these pathways must be combined with the correct exchange and $g/u$ symmetry of the molecular state.

---

## 11. Symmetry filters before the final $q$ sum

Before writing the final line-strength sum, one must apply the relevant molecular symmetry filters. This is the main point that can otherwise make the $q=0$ exclusion look mysterious.

The asymptotic labels like

$$
f+f=4+4,
\qquad
\ell=0
$$

do not, by themselves, say whether the short-range body-frame entrance component is $0^+$ or $0^-$. They specify the atomic hyperfine channel and the nuclear partial wave. To decide which body-frame dipole components belong to a given molecular transition, we must also specify which molecular electronic continuum the entrance state is assumed to correlate with.

In the reference C. Drag, et al., IEEE J. Quantum Electron. 36, 1378 (2000) calculation whose table gives the cesium angular factors, this extra assumption is made explicitly: apart from the angular factor, hyperfine structure is ignored and the excited molecular states are assumed to be populated from the continua of the ground molecular potentials

$$
a^3\Sigma_u^+(6s+6s)
$$

or

$$
X^1\Sigma_g^+(6s+6s),
$$

depending on the final excited state being considered. These are both $\Sigma^+$ ground potentials. Therefore their body-frame electronic reflection character is even.

That is the missing bridge: the tabulated angular factor is not obtained from the labels $f=4$ and $\ell=0$ alone. It is obtained after combining those labels with the molecular-continuum assumption that the relevant entrance electronic state has $\Sigma^+$ reflection character.

### 11.1 Exchange symmetry

For identical atoms, the total two-atom wavefunction must have the correct exchange symmetry. For bosonic isotopes it must be symmetric under atom exchange; for fermionic isotopes it must be antisymmetric.

For two atoms with equal hyperfine angular momentum $f$, the coupled hyperfine state obeys

$$
P_{12}|f,f;F_tM_F\rangle
=
(-1)^{2f-F_t}|f,f;F_tM_F\rangle.
$$

This determines which $F_t$ values are compatible with isotope statistics, the electronic exchange symmetry, and the partial wave $\ell$.

### 11.2 Inversion symmetry

For a homonuclear molecule, electronic states carry $g/u$ inversion symmetry. The electric dipole operator is ungerade, so the molecular electric-dipole transition changes

$$
g\leftrightarrow u.
$$

Thus a $0_g^-$ final state is reached from an ungerade ground-continuum component, while a $0_u^+$ final state is reached from a gerade ground-continuum component.

In the reference-style calculation this means, schematically,

$$
a^3\Sigma_u^+
\longrightarrow
0_g^-,
$$

and

$$
X^1\Sigma_g^+
\longrightarrow
0_u^+.
$$

### 11.3 Reflection symmetry for $\Sigma^+\rightarrow 0^\pm$ transitions

The ground electronic continua just mentioned are $\Sigma^+$ states. In Hund-case language, $\Sigma$ means $\Lambda=0$, and the superscript $+$ means the electronic state is even under reflection through a plane containing the internuclear axis.

For the body-frame reflection operator $\sigma_v$, this means the relevant entrance electronic component satisfies

$$
\sigma_v|i,\Sigma^+\rangle
=
+|i,\Sigma^+\rangle.
$$

For an excited $0^-$ state,

$$
\sigma_v|f,0^-\rangle
=
-|f,0^-\rangle.
$$

For an excited $0^+$ state,

$$
\sigma_v|f,0^+\rangle
=
+|f,0^+\rangle.
$$

Now examine the body-frame dipole components. Let $\sigma_v$ be reflection through the body-frame $xz$ plane. Then

$$
x\to x,
\qquad
y\to -y,
\qquad
z\to z.
$$

Therefore

$$
\sigma_v d_x\sigma_v^{-1}=d_x,
\qquad
\sigma_v d_y\sigma_v^{-1}=-d_y,
\qquad
\sigma_v d_z\sigma_v^{-1}=d_z.
$$

The parallel body-frame component is

$$
d_0^{\rm body}=d_z.
$$

Hence

$$
\sigma_v d_0^{\rm body}\sigma_v^{-1}
=+d_0^{\rm body}.
$$

So $q=0$ is reflection even.

The transverse spherical components are

$$
d_{+1}^{\rm body}
=-\frac{1}{\sqrt2}(d_x+i d_y),
$$

$$
d_{-1}^{\rm body}
=+\frac{1}{\sqrt2}(d_x-i d_y).
$$

Under reflection,

$$
\sigma_v d_{+1}^{\rm body}\sigma_v^{-1}
=-d_{-1}^{\rm body},
$$

$$
\sigma_v d_{-1}^{\rm body}\sigma_v^{-1}
=-d_{+1}^{\rm body}.
$$

Thus the transverse $q=\pm1$ subspace contains the reflection-odd operator needed for a $\Sigma^+\rightarrow 0^-$ transition.

So, for a $\Sigma^+$ entrance component,

$$
\Sigma^+\rightarrow 0^+:
\qquad
q=0\quad\text{parallel transition},
$$

whereas

$$
\Sigma^+\rightarrow 0^-:
\qquad
q=\pm1\quad\text{perpendicular transition}.
$$

This is the precise molecular-symmetry reason why the cesium $0_g^-$ angular factor uses $q=\pm1$ and excludes $q=0$.

---

## 12. Important interpretation of the $q=0$ exclusion

The exclusion of $q=0$ is not a statement that the atomic Clebsch--Gordan coefficient for $q=0$ vanishes. It usually does not.

It is also not a consequence of only saying the entrance condition as

$$
f+f=4+4,
\qquad
\ell=0.
$$

Those labels specify the hyperfine entrance manifold and the nuclear partial wave. They do not fully specify the molecular reflection sector of the entrance electronic continuum.

The additional physical assumption, used in the reference calculation being reproduced, is that the relevant ground continuum is correlated with a $\Sigma^+$ molecular potential. For the cesium $0_g^-(6s+6p_{3/2})$ line, this is the triplet ground continuum

$$
a^3\Sigma_u^+(6s+6s).
$$

This entrance component is reflection even. The target state is reflection odd:

$$
0_g^-.
$$

Therefore the transition is a perpendicular molecular transition. In body-frame language, it lives in the $q=\pm1$ subspace.

The $q=0$ contribution would instead correspond to a reflection-even operator. It would connect a reflection-odd entrance component to the $0^-$ final state, or a reflection-even entrance component to a $0^+$ final state. That is a different molecular symmetry sector, not the $a^3\Sigma_u^+\rightarrow0_g^-$ line strength tabulated as $125/3888$.

Equivalently, decompose a hypothetical body-frame entrance state into reflection sectors:

$$
|i\rangle
=P_+|i\rangle+P_-|i\rangle,
\qquad
P_\pm=\frac{1\pm\sigma_v}{2}.
$$

For a final $0^-$ state,

$$
\sigma_v|f,0^-\rangle=-|f,0^-\rangle.
$$

Since $d_0$ is reflection even,

$$
\langle f,0^-|d_0|i\rangle
=
\langle f,0^-|d_0P_-|i\rangle.
$$

So the $q=0$ contribution samples the reflection-odd entrance sector.

But the entrance continuum used for the $0_g^-$ cesium angular factor is the reflection-even $\Sigma^+$ sector. Therefore $q=0$ is not included in that line strength.

By contrast, the reflection-odd transverse dipole component connects the reflection-even entrance sector to the reflection-odd final state:

$$
\langle f,0^-|d_\perp^{(-)}|i,\Sigma^+\rangle
\neq 0.
$$

This is why the body-fixed sum for the $25/144$ factor contains only

$$
q=\pm1.
$$

If a different calculation explicitly included a reflection-odd entrance continuum, then the $q=0$ piece could define a different molecular line strength. It should not be silently mixed into the $\Sigma^+\rightarrow0^-$ perpendicular transition.

---

## 13. Worked example: cesium $0_g^-(6s+6p_{3/2})$

Now specialize to the cesium D2 asymptote

$$
6s_{1/2}+6p_{3/2}.
$$

The angular momenta are

$$
j_g=\frac12,
\qquad
j_e=\frac32,
\qquad
I=\frac72,
\qquad
f=4.
$$

The target excited molecular state is

$$
0_g^-(6s+6p_{3/2}).
$$

The asymptotic entrance hyperfine channel is

$$
f+f=4+4,
\qquad
\ell=0\quad\text{or, more generally, even }\ell.
$$

For the molecular line strength being reproduced, this entrance hyperfine channel is understood to correlate at molecular range with the reflection-even triplet ground continuum

$$
a^3\Sigma_u^+(6s+6s).
$$

Thus the relevant electronic transition is

$$
a^3\Sigma_u^+
\longrightarrow
0_g^-.
$$

This transition has the required inversion change $u\rightarrow g$, and because it is $\Sigma^+\rightarrow0^-$, it is a perpendicular transition. Therefore the body-frame dipole sum uses

$$
q=\pm1,
$$

not $q=0$.

The calculation of $A=125/3888$ is then organized as three separate factors:

$$
A
=
\left(\text{rotational/polarization average}\right)
\left(\text{allowed entrance-state fraction}\right)
\left(\text{body-fixed internal line strength}\right).
$$

For this example:

$$
A
=
\frac13\times\frac{45}{81}\times\frac{25}{144}.
$$

---

## 14. The $0_g^-$ body-frame electronic state

For the asymptote $6s_{1/2}+6p_{3/2}$,

$$
j_g=\frac12,
\qquad
j_e=\frac32.
$$

The ground atom can only have

$$
\omega_g=\pm\frac12.
$$

For an excited $\Omega=0$ pair, the allowed projection pairs are

$$
\omega_e=+\frac12,
\qquad
\omega_g=-\frac12,
$$

and

$$
\omega_e=-\frac12,
\qquad
\omega_g=+\frac12.
$$

Define

$$
|A\rangle
=
\left|+\frac12\right\rangle_e
\left|-\frac12\right\rangle_g,
\qquad
|B\rangle
=
\left|-\frac12\right\rangle_e
\left|+\frac12\right\rangle_g.
$$

The possible coupled electronic angular momenta are

$$
j_{12}=1,2.
$$

For $\Omega=0$, the Clebsch--Gordan expansion gives

$$
|j_{12}=2,\Omega=0\rangle
=
\frac{1}{\sqrt2}(|A\rangle+|B\rangle),
$$

whereas

$$
|j_{12}=1,\Omega=0\rangle
=
\frac{1}{\sqrt2}(|A\rangle-|B\rangle).
$$

With the phase convention used here, reflection through a plane containing the molecular axis acts as

$$
\sigma_v|A\rangle=-|B\rangle,
\qquad
\sigma_v|B\rangle=-|A\rangle.
$$

Therefore

$$
\sigma_v\frac{|A\rangle+|B\rangle}{\sqrt2}
=-\frac{|A\rangle+|B\rangle}{\sqrt2},
$$

while

$$
\sigma_v\frac{|A\rangle-|B\rangle}{\sqrt2}
=+\frac{|A\rangle-|B\rangle}{\sqrt2}.
$$

Thus, in this convention,

$$
0^-:
\qquad
|j_{12}=2,\Omega=0\rangle
=
\frac{1}{\sqrt2}(|A\rangle+|B\rangle),
$$

and

$$
0^+:
\qquad
|j_{12}=1,\Omega=0\rangle
=
\frac{1}{\sqrt2}(|A\rangle-|B\rangle).
$$

For the homonuclear molecule, the gerade excited state is the exchange-symmetrized state

$$
|\Phi_{0_g^-}\rangle
=
\frac{1}{\sqrt2}
\left(
|eg;j_{12}=2,\Omega=0\rangle
+
|ge;j_{12}=2,\Omega=0\rangle
\right).
$$

Here

$$
|eg;j_{12}=2,\Omega=0\rangle
=
\sum_{\omega_e,\omega_g}
\langle \tfrac32\omega_e;\tfrac12\omega_g|2,0\rangle
|6p_{3/2},\omega_e\rangle_1
|6s_{1/2},\omega_g\rangle_2,
$$

and

$$
|ge;j_{12}=2,\Omega=0\rangle
=
\sum_{\omega_g,\omega_e}
\langle \tfrac12\omega_g;\tfrac32\omega_e|2,0\rangle
|6s_{1/2},\omega_g\rangle_1
|6p_{3/2},\omega_e\rangle_2.
$$

The important point is that the $0^-$ label is a reflection label, whereas the $g$ label is an inversion/exchange-related homonuclear label. They are distinct symmetry labels.

---

## 15. Entrance hyperfine states and bosonic exchange

The entrance hyperfine channel is two cesium atoms in

$$
f_1=f_2=4.
$$

The product basis has

$$
(2f+1)^2=9^2=81
$$

states.

Couple the two atomic hyperfine angular momenta to total $F_t$:

$$
|(ff)F_tM_F\rangle
=
\sum_{m_{f1},m_{f2}}
\langle f m_{f1};f m_{f2}|F_tM_F\rangle
|f m_{f1}\rangle_1
|f m_{f2}\rangle_2.
$$

Under exchange,

$$
P_{12}|f,f;F_t,M_F\rangle
=
(-1)^{2f-F_t}|f,f;F_t,M_F\rangle.
$$

For $f=4$,

$$
(-1)^{2f-F_t}=(-1)^{8-F_t}=(-1)^{F_t}.
$$

For bosonic $^{133}$Cs, even $\ell$, and the relevant electronic exchange symmetry, the allowed entrance hyperfine states are the even-$F_t$ states:

$$
F_t=0,2,4,6,8.
$$

Their total degeneracy is

$$
\sum_{F_t=0,2,4,6,8}(2F_t+1)
=1+5+9+13+17
=45.
$$

Therefore the entrance-state statistical weight is

$$
\frac{45}{81}.
$$

This factor is separate from the reflection filter. The factor $45/81$ tells us which hyperfine-pair states are allowed by bosonic exchange symmetry. It does not by itself decide whether the body-frame dipole sum should use $q=0$ or $q=\pm1$.

---

## 16. Internal amplitude for the Cs example

The initial hyperfine pair expands as

$$
|(ff)F_tM_F\rangle
=
\sum_{m_{I1},\omega_1,m_{I2},\omega_2}
C^{F_tM_F}_{m_{I1}\omega_1m_{I2}\omega_2}
|m_{I1}\rangle_1|6s_{1/2},\omega_1\rangle_1
|m_{I2}\rangle_2|6s_{1/2},\omega_2\rangle_2,
$$

where

$$
\begin{aligned}
C^{F_tM_F}_{m_{I1}\omega_1m_{I2}\omega_2}
&=
\langle f m_{f1};f m_{f2}|F_tM_F\rangle
\\
&\quad\times
\langle I m_{I1};\tfrac12\omega_1|f m_{f1}\rangle
\\
&\quad\times
\langle I m_{I2};\tfrac12\omega_2|f m_{f2}\rangle,
\end{aligned}
$$

with

$$
m_{f1}=m_{I1}+\omega_1,
\qquad
m_{f2}=m_{I2}+\omega_2.
$$

The one-atom reduced dipole matrix element is

$$
\frac{
\langle 6p_{3/2},\omega_e|
 d_q^{\rm body}
|6s_{1/2},\omega_g\rangle
}{d_{\rm at}}
=
\langle 1q;\tfrac12\omega_g|\tfrac32\omega_e\rangle.
$$

For the target $0_g^-$ state, define

$$
\mathcal M_q(F_t,M_F;m_{I1},m_{I2})
=
\left\langle
\Phi_{0_g^-};m_{I1},m_{I2}
\left|
\frac{d_{1q}^{\rm body}+d_{2q}^{\rm body}}{d_{\rm at}}
\right|
(ff)F_tM_F
\right\rangle.
$$

Expanding the two coherent absorption pathways gives

$$
\begin{aligned}
\mathcal M_q(F_t,M_F;m_{I1},m_{I2})
&=
\sum_{\omega_1,\omega_2}
C^{F_tM_F}_{m_{I1}\omega_1m_{I2}\omega_2}
\\
&\quad\times
\frac{1}{\sqrt2}
\Bigg[
\sum_{\omega_e,\omega_g}
\langle \tfrac32\omega_e;\tfrac12\omega_g|2,0\rangle
\delta_{\omega_g,\omega_2}
\langle 1q;\tfrac12\omega_1|\tfrac32\omega_e\rangle
\\
&\qquad+
\sum_{\omega_g,\omega_e}
\langle \tfrac12\omega_g;\tfrac32\omega_e|2,0\rangle
\delta_{\omega_g,\omega_1}
\langle 1q;\tfrac12\omega_2|\tfrac32\omega_e\rangle
\Bigg].
\end{aligned}
$$

The first term is the amplitude where atom 1 absorbs the photon. The second term is the amplitude where atom 2 absorbs the photon. Since the final state is gerade, the two pathways are added coherently.

At this purely CG level, one could evaluate $q=0,\pm1$. But that would not yet be the desired $a^3\Sigma_u^+\rightarrow0_g^-$ molecular line strength. The reflection character of the entrance continuum has to be imposed before writing the final body-fixed sum.

---

## 17. Body-fixed line strength $B=25/144$

For the cesium $0_g^-$ angular factor quoted above, the body-fixed internal line strength is

$$
\boxed{
B
=
\frac{1}{45}
\sum_{F_t=0,2,4,6,8}
\sum_{M_F=-F_t}^{F_t}
\sum_{q=\pm1}
\sum_{m_{I1},m_{I2}}
\left|
\mathcal M_q(F_t,M_F;m_{I1},m_{I2})
\right|^2.
}
$$

The sum contains only $q=\pm1$ because this line strength is the $\Sigma^+\rightarrow0^-$ perpendicular transition. For the reference cesium channel, that means

$$
a^3\Sigma_u^+
\rightarrow
0_g^-.
$$

The parallel component $q=0$ is not removed by atomic angular momentum algebra. It is excluded because it belongs to a different reflection-sector transition.

Evaluating the Clebsch--Gordan sum gives

$$
B=\frac{25}{144}.
$$

If one incorrectly includes $q=0$ in the same sum, the result changes to

$$
B_{q=-1,0,+1}=\frac{25}{48},
$$

and the $q=0$ piece alone is

$$
B_{q=0}=\frac{25}{72}.
$$

This numerical fact is a useful diagnostic: the atomic CG machinery does not automatically remove $q=0$. The molecular continuum symmetry must be imposed explicitly.

---

## 18. Rotational/polarization factor

The full amplitude is

$$
a_\nu
=
\sum_{p,q}
(-1)^p
\epsilon_p^{\rm lab}
\langle J M\Omega_f|
D^{1*}_{-p,q}(\hat\eta)
|\ell m_\ell\Omega_i\rangle
\mathcal M_q.
$$

The full line strength requires summing over unresolved final rotational quantum numbers and averaging over unresolved initial lab-frame magnetic substates and orientations.

For an isotropic ultracold sample with linear polarization and the usual unresolved orientation average, the rotational/polarization part gives the familiar vector average

$$
\frac13.
$$

This factor is independent of the internal body-frame hyperfine/electronic sum $B$.

---

## 19. Final Cs angular factor

Putting the three factors together,

$$
A
=
\left(\text{rotational/polarization average}\right)
\times
\left(\text{bosonic entrance-state fraction}\right)
\times
\left(\text{body-fixed internal line strength}\right).
$$

For the cesium
$0_g^-(6s+6p_{3/2})$,
$f+f=4+4$,
even-$\ell$ channel, with the entrance continuum correlated with
$a^3\Sigma_u^+(6s+6s)$,

$$
A
=
\frac13
\times
\frac{45}{81}
\times
\frac{25}{144}.
$$

Therefore

$$
\boxed{
A
=
\frac{125}{3888}.
}
$$

---

## 20. Cross-check: why the same logic works for $0_u^+$ examples

The same symmetry logic also explains why related table entries, such as cesium $f+f=4+4$ photoassociation to a $0_u^+$ state in the $6s+6p_{1/2}$ limit, can be reproduced by the same machinery.

For a $0_u^+$ target, the reference-style molecular continuum is the singlet ground state

$$
X^1\Sigma_g^+(6s+6s).
$$

The transition is then

$$
X^1\Sigma_g^+
\rightarrow
0_u^+.
$$

This has the required inversion change $g\rightarrow u$, and it has no change of reflection parity:

$$
\Sigma^+\rightarrow0^+.
$$

Therefore the body-frame transition is the parallel one, associated with the reflection-even $q=0$ component. This is the complementary case to

$$
a^3\Sigma_u^+\rightarrow0_g^-,
$$

which is $\Sigma^+\rightarrow0^-$ and therefore uses the perpendicular $q=\pm1$ components.

So the rule is not “always throw away $q=0$.” The rule is:

> Decide the molecular continuum symmetry first. Then choose the body-frame dipole components compatible with the target molecular symmetry.

---

## 21. Generic recipe for other alkali PA channels

The reusable calculation flow is:

1. **Specify the atomic species.**  
   Input the nuclear spin $I$ and whether the isotope is bosonic or fermionic.

2. **Specify the asymptotic entrance hyperfine channel.**  
   Choose $f_1,f_2$ and the partial wave $\ell$.

3. **Specify the ground molecular continuum used for the radial problem.**  
   For homonuclear alkalis this often means deciding whether the entrance continuum is correlated with a singlet or triplet ground potential such as
   $$
   X^1\Sigma_g^+
   \quad\text{or}\quad
   a^3\Sigma_u^+.
   $$
   This step fixes the relevant $g/u$ and reflection character of the entrance electronic state.

4. **Specify the excited asymptote.**  
   For alkalis,
   $$
   j_g=\frac12,
   \qquad
   j_e=\frac12\text{ for D1},
   \qquad
   j_e=\frac32\text{ for D2}.
   $$

5. **Specify the target molecular symmetry.**  
   Examples include $0_g^-$, $0_u^+$, $1_g$, $1_u$, etc.

6. **Build the body-frame excited molecular state.**  
   Couple $j_e$ and $j_g$ to the desired $\Omega$ and impose $g/u$ and reflection symmetry.

7. **Expand the entrance hyperfine state.**  
   Write $|(f_1f_2)F_tM_F\rangle$ in the uncoupled basis
   $|m_{I1},\omega_1;m_{I2},\omega_2\rangle$.

8. **Apply exchange symmetry.**  
   Keep only the $F_t$ sectors consistent with isotope statistics, electronic exchange symmetry, and $\ell$.

9. **Apply molecular selection rules before the $q$ sum.**  
   Use the ground-continuum symmetry and target excited symmetry to decide whether the transition is parallel or perpendicular. For $\Sigma^+$ entrance states,
   $$
   \Sigma^+\rightarrow0^+:
   \quad q=0,
   $$
   while
   $$
   \Sigma^+\rightarrow0^-:
   \quad q=\pm1.
   $$

10. **Compute the internal amplitude.**  
    Use the one-atom CG coefficient
    $$
    \langle 1q;\tfrac12\omega_g|j_e\omega_e\rangle.
    $$

11. **Square, sum, and average.**  
    Compute
    $$
    A(g,e,\boldsymbol\epsilon)
    =
    \sum_{\rm final}
    \overline{|a_\nu|^2}_{\rm initial}.
    $$

This structure keeps the generic tutorial independent of the cesium-specific number $125/3888$.

---

## 22. Summary of the logic

The derivation should be remembered in this order:

1. Start with the physical interaction:

   $$
   V_{b,\nu}
   =
   \frac{\mathcal E_0}{2}
   \langle f,\nu|\boldsymbol\epsilon\cdot\mathbf d|i,\nu\rangle.
   $$

2. Write the states abstractly in

   $$
   \mathcal H_R\otimes\mathcal H_{\rm orient}\otimes\mathcal H_{\rm int}.
   $$

3. Use the Condon approximation to factor out

   $$
   \langle \psi_v|\chi_{E\ell}\rangle.
   $$

4. Rotate the dipole only because the laser is lab-fixed but the molecular electronic states are body-fixed:

   $$
   d_p^{\rm lab}
   =
   \sum_qD^{1*}_{pq}(\hat\eta)d_q^{\rm body}.
   $$

5. Obtain

   $$
   a_\nu
   =
   \sum_{p,q}
   (-1)^p
   \epsilon_p^{\rm lab}
   \langle J M\Omega_f|
   D^{1*}_{-p,q}
   |\ell m_\ell\Omega_i\rangle
   \mathcal M_q.
   $$

6. Remember that the physical stimulated width depends on

   $$
   |a_\nu|^2,
   $$

   summed over final channels and averaged over initial channels.

7. Do not decide the $q$ sum from $f+f$ and $\ell$ alone. First specify the molecular continuum symmetry. In the reference cesium $0_g^-$ example, the entrance continuum is correlated with

   $$
   a^3\Sigma_u^+(6s+6s),
   $$

   which is reflection even.

8. Since the target is $0_g^-$, the transition is

   $$
   \Sigma^+\rightarrow0^-,
   $$

   so it is perpendicular and uses

   $$
   q=\pm1,
   $$

   not $q=0$.

9. The final angular factor is

   $$
   A
   =
   \frac13
   \times
   \frac{45}{81}
   \times
   \frac{25}{144}
   =
   \frac{125}{3888}.
   $$

---

## Appendix: Mathematica verification of $B=25/144$

```mathematica
ClearAll["Global`*"];

Ics = 7/2;
jg = 1/2;
je = 3/2;
f = 4;
J12 = 2;
Omega = 0;

mList[j_] := Range[-j, j, 1];

validM[j_, m_] := MemberQ[mList[j], m];

cg[j1_, m1_, j2_, m2_, J_, M_] :=
  If[
    validM[j1, m1] && validM[j2, m2] && validM[J, M] && m1 + m2 == M,
    ClebschGordan[{j1, m1}, {j2, m2}, {J, M}],
    0
  ];

amp[F_, M_, q_, mI1_, mI2_] :=
  FullSimplify[
    Sum[
      Module[
        {
          mf1, mf2, ci,
          me1, me2,
          term1, term2
        },

        mf1 = mI1 + mj1;
        mf2 = mI2 + mj2;

        ci =
          cg[f, mf1, f, mf2, F, M] *
          cg[Ics, mI1, jg, mj1, f, mf1] *
          cg[Ics, mI2, jg, mj2, f, mf2];

        (* Atom 1 absorbs the photon: g1 -> e1 *)
        me1 = mj1 + q;

        term1 =
          cg[1, q, jg, mj1, je, me1] *
          cg[je, me1, jg, mj2, J12, Omega] / Sqrt[2];

        (* Atom 2 absorbs the photon: g2 -> e2 *)
        me2 = mj2 + q;

        term2 =
          cg[1, q, jg, mj2, je, me2] *
          cg[jg, mj1, je, me2, J12, Omega] / Sqrt[2];

        ci * (term1 + term2)
      ],
      {mj1, mList[jg]},
      {mj2, mList[jg]}
    ]
  ];

allowedF = {0, 2, 4, 6, 8};

B =
  FullSimplify[
    (1/45) *
      Sum[
        amp[F, M, q, mI1, mI2]^2,
        {F, allowedF},
        {M, mList[F]},
        {q, {-1, 1}},
        {mI1, mList[Ics]},
        {mI2, mList[Ics]}
      ]
  ]

(* Output: 25/144 *)
```

The partial contributions by $F_t$ are obtained from

```mathematica
Table[
  {
    F,
    FullSimplify[
      Sum[
        amp[F, M, q, mI1, mI2]^2,
        {M, mList[F]},
        {q, {-1, 1}},
        {mI1, mList[Ics]},
        {mI2, mList[Ics]}
      ]
    ]
  },
  {F, allowedF}
]

(* Output:
{
  {0, 7/72},
  {2, 155/288},
  {4, 19/16},
  {6, 637/288},
  {8, 34/9}
}
*)
```

Their sum is

$$
\frac{7}{72}
+
\frac{155}{288}
+
\frac{19}{16}
+
\frac{637}{288}
+
\frac{34}{9}
=
\frac{125}{16}.
$$

Averaging over the $45$ allowed initial hyperfine states gives

$$
B
=
\frac{1}{45}\frac{125}{16}
=
\frac{25}{144}.
$$

If one incorrectly includes $q=0$ in the same line-strength sum, replacing

```mathematica
{q, {-1, 1}}
```

by

```mathematica
{q, {-1, 0, 1}}
```

gives

$$
B_{q=-1,0,+1}=\frac{25}{48},
$$

not $25/144$. The $q=0$ piece alone gives

$$
B_{q=0}=\frac{25}{72}.
$$

Thus excluding $q=0$ is essential for reproducing the quoted $125/3888$ angular factor. The reason is molecular reflection symmetry, not the one-atom angular-momentum CG rule.
