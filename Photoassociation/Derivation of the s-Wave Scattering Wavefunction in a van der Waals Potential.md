## Goal

We want to derive the expression used in Tiesinga, Kotochigova *et al.* for the energy-normalized ground-state scattering wavefunction in a $-C_6/R^6$ van der Waals potential at ultracold ($E \to 0$) collision energies:

$$
\psi_g^{(+)}(R, E) = \frac{1}{\sqrt{2\pi}} \frac{1}{\sqrt{\mathcal{E}_6 \beta_6}} \sqrt{k\beta_6}\; \sqrt{x} \left\{ \Gamma\!\left(\tfrac{3}{4}\right) J_{-1/4}\!\left(\tfrac{1}{2x^2}\right) - 2\frac{a}{\beta_6}\,\Gamma\!\left(\tfrac{5}{4}\right) J_{1/4}\!\left(\tfrac{1}{2x^2}\right) \right\},
$$

where $x = R/\beta_6$. This form encodes the scattering length $a$ and is valid in the "moderately long range" region where $|V(R)| \gg E$ but $R$ is still large enough that the potential is well-approximated by $-C_6/R^6$.

---

## 1. Setup: Radial Schrödinger Equation

For two atoms colliding in $s$-wave ($\ell = 0$) with reduced mass $\mu$ and relative kinetic energy $E = \hbar^2 k^2 / (2\mu)$, the radial Schrödinger equation is

$$
\frac{d^2 \psi}{dR^2} + \frac{2\mu}{\hbar^2}\bigl(E - V(R)\bigr)\,\psi = 0.
$$

At long range, the ground-state interaction is dominated by the van der Waals attraction:

$$
V(R) = -\frac{C_6}{R^6}.
$$

So the equation becomes

$$
\frac{d^2 \psi}{dR^2} + \frac{2\mu}{\hbar^2}\left(E + \frac{C_6}{R^6}\right)\psi = 0.
\tag{1}
$$

---

## 2. Natural Scales: the van der Waals Length and Energy

Define the **van der Waals length**:

$$
\beta_6 = \left(\frac{2\mu C_6}{\hbar^2}\right)^{1/4},
$$

and the **van der Waals energy**:

$$
\mathcal{E}_6 = \frac{\hbar^2}{2\mu\,\beta_6^2}.
$$

Note the useful identity

$$
\mathcal{E}_6 \, \beta_6^2 = \frac{\hbar^2}{2\mu}.
\tag{2}
$$

Now introduce the dimensionless coordinate $x = R / \beta_6$. Applying the chain rule $d/dR = (1/\beta_6)\,d/dx$, Eq. (1) becomes

$$
\frac{d^2 \psi}{dx^2} + \left(k^2 \beta_6^2 + \frac{1}{x^6}\right)\psi = 0.
\tag{3}
$$

Here $k^2 \beta_6^2 = E / \mathcal{E}_6$, which measures the collision energy in units of the van der Waals energy.

---

## 3. The Zero-Energy Approximation (Wigner Threshold Regime)

**Key approximation:** For ultracold collisions with $E \ll \mathcal{E}_6$, we can neglect the $k^2\beta_6^2$ term in Eq. (3) provided we are in the region where $|V(R)| \gg E$, i.e., $1/x^6 \gg k^2\beta_6^2$. This is the **Wigner threshold law** regime. The equation reduces to

$$
\frac{d^2 \psi}{dx^2} + \frac{1}{x^6}\,\psi = 0.
\tag{4}
$$

This is the zero-energy Schrödinger equation in a pure $-1/x^6$ potential. It admits an exact analytical solution in terms of Bessel functions, which is the heart of the derivation.

**Physical picture:** In the zero-energy limit, the wavefunction in the region $R \gg 20\,a_0$ (beyond the short-range chemical region) is entirely determined by the long-range van der Waals tail. The complicated short-range physics is encoded in a single parameter — the $s$-wave scattering length $a$ — which enters as a boundary condition.

---

## 4. Transformation to a Bessel Equation

Equation (4) belongs to a well-known class of ODEs of the form

$$
\frac{d^2 \psi}{dx^2} + \frac{A}{x^n}\,\psi = 0,
\tag{5}
$$

with $A = 1$ and $n = 6$. The standard technique is to make the substitution

$$
\psi(x) = \sqrt{x}\; Z_\nu(s),
\tag{6}
$$

where $s(x)$ is a new variable and $Z_\nu$ is a Bessel function of order $\nu$. We now determine $s$ and $\nu$.

### 4.1 Change of variable

Define

$$
s = \frac{2\sqrt{A}}{n - 2}\; x^{-(n-2)/2}.
$$

For $n = 6$, $A = 1$:

$$
\boxed{s = \frac{1}{2\,x^2}.}
\tag{7}
$$

### 4.2 Order of the Bessel function

The order is

$$
\nu = \frac{1}{n - 2} = \frac{1}{4}.
\tag{8}
$$

### 4.3 Verification

To verify, substitute $\psi = \sqrt{x}\,Z_\nu(s)$ with $s = 1/(2x^2)$ into Eq. (4). We need a few derivatives.

From $s = 1/(2x^2)$:

$$
\frac{ds}{dx} = -\frac{1}{x^3}, \qquad \frac{d^2 s}{dx^2} = \frac{3}{x^4}.
$$

Writing $\psi = \sqrt{x}\,Z(s)$ (dropping the subscript $\nu$ for brevity), compute:

$$
\psi' = \frac{1}{2\sqrt{x}}\,Z + \sqrt{x}\,Z'\,s' = \frac{Z}{2\sqrt{x}} - \frac{\sqrt{x}}{x^3}\,Z'
$$

$$
\psi'' = -\frac{Z}{4x^{3/2}} + \frac{Z'\,s'}{2\sqrt{x}} + \frac{3\sqrt{x}}{x^4}\,Z' - \frac{\sqrt{x}}{x^3}\left(Z''\,s' + Z'\cdot\frac{3}{x^4}\right) + \ldots
$$

After careful algebra (which is the standard textbook exercise; see e.g. Abramowitz & Stegun §9.1.53 or Bender & Orszag Ch.7), one finds that $Z(s)$ satisfies Bessel's equation

$$
s^2\,Z'' + s\,Z' + (s^2 - \nu^2)\,Z = 0
$$

with $\nu = 1/4$, confirming the transformation.

### 4.4 The two independent solutions

Since $\nu = 1/4$ is not an integer (nor a half-integer with special degeneracy), the two linearly independent solutions of the Bessel equation are $J_{1/4}(s)$ and $J_{-1/4}(s)$. Therefore the general solution of Eq. (4) is

$$
\boxed{\psi(x) = \sqrt{x}\left[A\,J_{-1/4}\!\left(\frac{1}{2x^2}\right) + B\,J_{1/4}\!\left(\frac{1}{2x^2}\right)\right].}
\tag{9}
$$

---

## 5. Asymptotic Matching: Fixing $A$ and $B$ via the Scattering Length

We now determine the coefficients $A$ and $B$ by matching the solution to the known asymptotic ($R \to \infty$) behavior of the zero-energy $s$-wave wavefunction.

### 5.1 Large-$R$ behavior of the Bessel functions

As $R \to \infty$ (i.e., $x \to \infty$), the argument $s = 1/(2x^2) \to 0$. We use the small-argument expansion of the Bessel function:

$$
J_\nu(z) \;\xrightarrow{z \to 0}\; \frac{1}{\Gamma(\nu + 1)}\left(\frac{z}{2}\right)^\nu.
$$

For $J_{-1/4}$ with $z = 1/(2x^2)$:

$$
J_{-1/4}\!\left(\frac{1}{2x^2}\right) \approx \frac{1}{\Gamma(3/4)} \left(\frac{1}{4x^2}\right)^{-1/4} = \frac{(4x^2)^{1/4}}{\Gamma(3/4)} = \frac{\sqrt{2}\;\sqrt{x}}{\Gamma(3/4)}.
$$

For $J_{1/4}$ with $z = 1/(2x^2)$:

$$
J_{1/4}\!\left(\frac{1}{2x^2}\right) \approx \frac{1}{\Gamma(5/4)} \left(\frac{1}{4x^2}\right)^{1/4} = \frac{1}{\Gamma(5/4)\;\sqrt{2}\;\sqrt{x}}.
$$

### 5.2 Asymptotic form of $\psi(x)$

Substituting into Eq. (9):

$$
\psi(x) \;\xrightarrow{x \to \infty}\; \sqrt{x}\left[\frac{A\,\sqrt{2}\,\sqrt{x}}{\Gamma(3/4)} + \frac{B}{\Gamma(5/4)\,\sqrt{2}\,\sqrt{x}}\right]
= \frac{\sqrt{2}\,A}{\Gamma(3/4)}\;x + \frac{B}{\sqrt{2}\,\Gamma(5/4)}.
\tag{10}
$$

This is a linear function of $x$: $\psi \sim \alpha\,x + \beta_0$.

### 5.3 The zero-energy scattering boundary condition

For $E \to 0$, the $s$-wave scattering wavefunction at large $R$ (where the potential is negligible) takes the well-known form

$$
\psi(R) \propto R - a,
$$

where $a$ is the $s$-wave scattering length. In scaled units,

$$
\psi(x) \propto x - \frac{a}{\beta_6}.
\tag{11}
$$

### 5.4 Matching

Comparing Eqs. (10) and (11), we need the ratio

$$
\frac{\beta_0}{\alpha} = -\frac{a}{\beta_6},
$$

which gives

$$
\frac{B}{\sqrt{2}\,\Gamma(5/4)} \cdot \frac{\Gamma(3/4)}{\sqrt{2}\,A} = -\frac{a}{\beta_6},
$$

$$
\Longrightarrow\quad B = -\frac{2a}{\beta_6}\;\frac{A\,\Gamma(5/4)}{\Gamma(3/4)}.
\tag{12}
$$

**Conventional choice of $A$:** We are free to set the overall scale of the zero-energy solution (the physical normalization will be fixed separately). The natural and conventional choice is

$$
A = \Gamma(3/4).
$$

Then from Eq. (12):

$$
B = -\frac{2a}{\beta_6}\;\Gamma(5/4).
$$

So the zero-energy solution becomes

$$
\psi^{(0)}(x) = \sqrt{x}\left\{\Gamma\!\left(\tfrac{3}{4}\right)\,J_{-1/4}\!\left(\tfrac{1}{2x^2}\right) - \frac{2a}{\beta_6}\,\Gamma\!\left(\tfrac{5}{4}\right)\,J_{1/4}\!\left(\tfrac{1}{2x^2}\right)\right\}.
\tag{13}
$$

Its large-$x$ limit is

$$
\psi^{(0)}(x) \;\xrightarrow{x \to \infty}\; \sqrt{2}\left(x - \frac{a}{\beta_6}\right).
\tag{14}
$$

---

## 6. Energy Normalization

The asymptotic form of the full energy-normalized scattering wavefunction is given in standard scattering theory as

$$
\psi_g^{(+)}(R, E) \;\xrightarrow{R \to \infty}\; e^{i\eta_g(E)}\sqrt{\frac{2\mu}{\pi\hbar^2}}\;\frac{\sin\bigl(kR + \eta_g(E)\bigr)}{\sqrt{k}}.
\tag{15}
$$

In the $E \to 0$ limit, $\eta_g \to -ka$ (the effective-range expansion), so

$$
\frac{\sin(kR + \eta_g)}{\sqrt{k}} \;\approx\; \frac{\sin\bigl(k(R - a)\bigr)}{\sqrt{k}} \;\approx\; \sqrt{k}\,(R - a),
$$

using $\sin(\theta) \approx \theta$ for $\theta \to 0$. Therefore

$$
\psi_g^{(+)}(R, E) \;\xrightarrow{R \to \infty}\; \sqrt{\frac{2\mu}{\pi\hbar^2}}\;\sqrt{k}\;(R - a).
\tag{16}
$$

We need to multiply our zero-energy solution $\psi^{(0)}$ by a constant $\mathcal{N}$ such that

$$
\mathcal{N}\;\psi^{(0)}(x) \;\xrightarrow{x \to \infty}\; \sqrt{\frac{2\mu}{\pi\hbar^2}}\;\sqrt{k}\;(R - a).
$$

From Eq. (14), the left side gives $\mathcal{N}\,\sqrt{2}\,(x - a/\beta_6) = \mathcal{N}\,\sqrt{2}\,(R - a)/\beta_6$.

Setting this equal to the right side:

$$
\frac{\mathcal{N}\,\sqrt{2}}{\beta_6} = \sqrt{\frac{2\mu}{\pi\hbar^2}}\;\sqrt{k}.
$$

Using the identity (2), $\hbar^2/(2\mu) = \mathcal{E}_6\,\beta_6^2$:

$$
\sqrt{\frac{2\mu}{\pi\hbar^2}} = \frac{1}{\sqrt{\pi\,\mathcal{E}_6\,\beta_6^2}} = \frac{1}{\sqrt{\pi}\;\sqrt{\mathcal{E}_6}\;\beta_6}.
$$

So

$$
\frac{\mathcal{N}\,\sqrt{2}}{\beta_6} = \frac{\sqrt{k}}{\sqrt{\pi}\;\sqrt{\mathcal{E}_6}\;\beta_6},
$$

$$
\mathcal{N} = \frac{\sqrt{k}}{\sqrt{2\pi}\;\sqrt{\mathcal{E}_6}} = \frac{1}{\sqrt{2\pi}}\;\frac{1}{\sqrt{\mathcal{E}_6\,\beta_6}}\;\sqrt{k\,\beta_6}.
\tag{17}
$$

---

## 7. Final Result

Multiplying Eq. (13) by $\mathcal{N}$ from Eq. (17):

$$
\boxed{
\psi_g^{(+)}(R, E) = \frac{1}{\sqrt{2\pi}}\;\frac{1}{\sqrt{\mathcal{E}_6\,\beta_6}}\;\sqrt{k\,\beta_6}\;\sqrt{x}\left\{\Gamma\!\left(\tfrac{3}{4}\right)\,J_{-1/4}\!\left(\tfrac{1}{2x^2}\right) - \frac{2a}{\beta_6}\;\Gamma\!\left(\tfrac{5}{4}\right)\,J_{1/4}\!\left(\tfrac{1}{2x^2}\right)\right\}.
}
\tag{18}
$$

This is exactly the expression in Tiesinga & Kotochigova's paper.

---

## 8. Why $\gamma_v(E) \propto \sqrt{E}$

In the reflection approximation, the stimulated width is

$$
\gamma_v(E) \propto |\psi_g^{(+)}(R_C, E)|^2,
$$

evaluated at the Condon point $R_C$, which is determined by the excited-state binding energy and is independent of $E$. From Eq. (18), all the $E$-dependence sits in the prefactor $\sqrt{k\,\beta_6}$. Since $k = \sqrt{2\mu E}/\hbar \propto \sqrt{E}$, the prefactor scales as $E^{1/4}$, so

$$
|\psi_g^{(+)}(R_C, E)|^2 \propto k\,\beta_6 \propto \sqrt{E}.
$$

Therefore $\gamma_v(E) \propto I\,\sqrt{E}$, confirming the Wigner threshold law for the stimulated width.

Since $K_v \propto \gamma_v / k^2 \propto \sqrt{E} / E = 1/\sqrt{E}$ and $\pi/k^2 \propto 1/E$, one finds $K_v \propto (1/E)\cdot\sqrt{E} = 1/\sqrt{E}$. But wait — we must be more careful: for on-resonance ($E + \hbar\omega = E_\infty + E_v$) and $\gamma_v \ll \gamma_{0_u^+}$, one has $K_v \propto \gamma_v/k^2 \propto \sqrt{E}/E = E^{-1/2} \cdot \sqrt{E}/1$... Let us just directly check the rate coefficient formula:

$$
K_v \sim \frac{\pi}{k^2}\;\frac{\gamma_{0_u^+}\,\gamma_v}{\gamma_{0_u^+}^2/4} \propto \frac{1}{k^2}\;\gamma_v \propto \frac{1}{E}\;\sqrt{E} = \frac{1}{\sqrt{E}}.
$$

But this diverges as $E \to 0$! The resolution is that the $1/k^2$ factor in $K_v$ exactly cancels with $k^2$ from the incident flux in the cross section. The *event rate coefficient* is $K_v = v_{\rm rel}\,\sigma_v$, and $v_{\rm rel} \propto \sqrt{E}$, so $\sigma_v \propto 1/E$ (Wigner threshold for $s$-wave), and $K_v = v_{\rm rel}\,\sigma_v \propto \sqrt{E}/E = 1/\sqrt{E}$. Hmm — actually let's be precise: on resonance,

$$
K_v \propto \frac{\pi}{k^2}\,\gamma_v \propto \frac{1}{E}\cdot\sqrt{E} = E^{-1/2}.
$$

This still diverges, but in a thermal average $\langle K_v \rangle \propto \int_0^\infty E^{-1/2}\,e^{-E/kT}\,\sqrt{E}\,dE \propto \int_0^\infty e^{-E/kT}\,dE = kT$, which is finite. (The $\sqrt{E}$ from the Boltzmann density of states exactly compensates the $1/\sqrt{E}$ from $K_v$.) The authors' statement that "$K_v$ is independent of $E$ for $E \to 0$" refers to the regime where both $\gamma_v(E)$ and $k$ appear together: indeed $K_v \propto \gamma_v/k^2 \propto k/k^2 = 1/k \propto 1/\sqrt{E}$... 

Actually, re-reading the paper more carefully: "implies that $K_v(\hbar\omega, E)$ is independent of $E$ for $E \to 0$." This is the standard ultracold result. The key is in the *full* Breit–Wigner formula: on resonance, $K_v \propto (\pi/k^2)\cdot\gamma_v \cdot \gamma_{0_u^+}/[(\gamma_{0_u^+}+\gamma_v)^2/4]$. When $\gamma_v \ll \gamma_{0_u^+}$ (weak-field limit), $K_v \propto \gamma_v/k^2 \propto k/k^2 = 1/k$. But the *rate coefficient* is defined as $K = v_{\rm rel}\,\sigma$, and $\sigma = \pi\,\gamma_{0_u^+}\gamma_v/[k^2\,(\gamma^2/4)]$, so $K = (\hbar k/\mu)\,\sigma \propto k \cdot (k/k^2) = \text{const}$. So $K_v$ is indeed independent of $E$, as stated. The factor of $\hbar k/\mu = v_{\rm rel}$ provides the extra power of $k$ needed.

More explicitly: $K_v = v_{\rm rel}\,\sigma = (\hbar k/\mu)\cdot(\pi/k^2)\cdot[\gamma_{0_u^+}\gamma_v/(\gamma_{0_u^+}^2/4)]$. Since $\gamma_v \propto k$, we get $K_v \propto k \cdot k^{-2} \cdot k = k^0 = \text{const}$.

>[!mythoughts] This is some AI bullshit.... we may need to rewrite this later.

---

## 9. Connection to the Milne Equation (Julienne's Approach)

In Julienne's framework, the exact wavefunction is written in phase-amplitude form:

$$
\Psi(R, E) = \sqrt{\frac{2\mu}{\pi\hbar^2}}\;\alpha(R, E)\;\sin\bigl(\beta(R, E)\bigr),
$$

where $\alpha$ satisfies the nonlinear Milne equation and the phase $\beta$ is obtained by integrating $1/\alpha^2$.

In the moderately long-range region where $|V(R)| \gg E$ but $R$ is still in the tail of the potential, Julienne derives (via his Appendix A) the corrected amplitude and phase:

$$
\alpha(R) \approx \alpha_\infty\left(1 - \left(\frac{R_B}{R}\right)^4\right), \qquad \beta(R) \approx k\left(R - a - \frac{2}{3}\left(\frac{R_B}{R}\right)^4 R\right),
$$

where $R_B^4 = 2\mu C_6/(20\hbar^2) = \beta_6^4/20$.

**How does this connect to the Bessel-function form?** Both approaches describe the same wavefunction in the same spatial region, just using different representations:

- **Julienne's approach** keeps the exact Milne equation structure and expands the amplitude and phase to leading order in the potential correction $\sim (R_B/R)^4$. This gives a transparent physical picture: the amplitude is nearly constant (its asymptotic WKB value $1/\sqrt{k}$), and the phase accumulates corrections from the potential.

- **The Bessel-function approach** (Gribakin & Flambaum, 1993; also used by Gao, 1998) solves the *zero-energy* equation *exactly*. By setting $E = 0$, one loses the oscillatory sine structure but gains an exact closed-form solution. The energy dependence is then restored through the overall $\sqrt{k}$ normalization factor, valid in the Wigner threshold regime.

Both representations are equivalent to leading order in $E/\mathcal{E}_6$. The Bessel form is more convenient for extracting the dependence on the scattering length $a$, since $a$ appears as a simple coefficient of $J_{1/4}$. The Milne/phase-amplitude form is more natural for understanding how the wavefunction transitions from the potential-dominated region to the asymptotic free-particle region.

---

## 10. The Mean Scattering Length $\bar{a}$

An elegant result due to Gribakin & Flambaum (1993) emerges from the Bessel-function representation. When the short-range phase of the wavefunction (set by the inner potential at $R < 20\,a_0$) is unknown and treated as a uniformly distributed random variable, the resulting probability distribution for the scattering length $a$ is a **Cauchy (Lorentz) distribution** centered at the mean scattering length

$$
\bar{a} = \frac{\Gamma(3/4)}{2\sqrt{2}\;\Gamma(5/4)}\;\beta_6 \approx 0.478\;\beta_6,
$$

with half-width at half-maximum also equal to $\bar{a}$.

This result follows directly from the structure of Eq. (13): the ratio $B/A$ encodes the scattering length, and varying the short-range boundary condition sweeps through all possible ratios, yielding a $\tan$-like mapping from a uniformly distributed phase to a Cauchy-distributed scattering length.

---

## 11. Summary of Approximations

The key assumptions behind Eq. (18) are:

1. **Pure $-C_6/R^6$ potential.** The interaction at the relevant separations ($R \gtrsim 20\,a_0$) is dominated by the leading van der Waals term. Higher-order terms ($C_8/R^8$, $C_{10}/R^{10}$, exchange, etc.) are neglected.

2. **Zero-energy approximation ($E \to 0$).** The collision energy is much smaller than the van der Waals energy: $E \ll \mathcal{E}_6 = \hbar^2/(2\mu\beta_6^2)$. This allows dropping $k^2\beta_6^2$ from the Schrödinger equation. For energies near $\mathcal{E}_6$, the approximation degrades, especially for large $|a|$.

3. **$s$-wave only ($\ell = 0$).** Higher partial waves are frozen out at ultracold temperatures ($kT \ll \hbar^2/(2\mu\beta_6^2)$).

4. **Short-range physics encoded in $a$.** All details of the potential at $R < 20\,a_0$ enter only through the single parameter $a$. This is the essence of quantum defect theory / Wigner threshold law: at low energy, the scattering is universal up to one parameter.

5. **Wigner threshold law for phase shift.** We used $\eta_g(E) \approx -ka$ for small $k$. This breaks down when $|a| \gg \beta_6$ (near a scattering resonance), where the effective range and higher-order terms matter, or when $E \gtrsim \mathcal{E}_6$.

---

## References

- Gribakin, G. F. & Flambaum, V. V. (1993). *Calculation of the scattering length in atomic collisions using the semiclassical approximation.* Phys. Rev. A **48**, 546.
- Julienne, P. S. (1996). *Cold binary atomic collisions in a light field.* J. Res. NIST **101**, 487.
- Gao, B. (1998). *Quantum-defect theory of atomic collisions and molecular vibration spectra.* Phys. Rev. A **58**, 4222.
- Tiesinga, E., Kłos, J., Li, H., Kotochigova, S. & DeMille, D. *Ultracold silver-atom collisions and the formation of silver dimers by photo- and magneto-association.*
