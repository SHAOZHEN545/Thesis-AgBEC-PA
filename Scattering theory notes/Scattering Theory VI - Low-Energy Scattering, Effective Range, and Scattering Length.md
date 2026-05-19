The previous note introduced partial waves as angular-momentum blocks of the scattering matrix. In the single-channel elastic case each block is a number,

$$
S_l(k)=e^{2i\delta_l(k)},
$$

and the corresponding partial-wave amplitude is

$$
f_l(k)
=
\frac{S_l(k)-1}{2ik}
=
\frac{e^{2i\delta_l(k)}-1}{2ik}
=
\frac{1}{k\cot\delta_l(k)-ik}.
$$

This note studies the low-energy limit of this expression. The goal is not only to reproduce Sakurai's single-channel discussion of scattering length and effective range, but also to state the version needed for Feshbach resonances. In that setting the relevant scattering length is not an abstract geometric length. It is the zero-energy limit of a chosen entrance-channel elastic s-wave amplitude.

To avoid a notational collision, this note often denotes the entrance open channel by $o$. The scattering length itself is still denoted by $a$ in the single-channel case and by $a_o$ when the entrance channel must be specified.

---

## 1. Low-energy means long wavelength compared with the interaction range

Let $R$ denote the **characteristic range** of a short-range interaction. Low-energy scattering means

$$
kR\ll 1,
$$

or equivalently that the de Broglie wavelength is much longer than the region where the interaction is appreciable.

In this regime the incoming wave cannot resolve fine angular structure in the potential region. 

>[!mythoughts] what is this

This is why the angular-momentum expansion becomes especially simple. The centrifugal barrier for the $l$th partial wave is

$$
\frac{\hbar^2}{2\mu}\frac{l(l+1)}{r^2}.
$$

For $l>0$, this barrier suppresses penetration into the short-range interaction region. Unless there is a near-threshold resonance or bound state in a higher partial wave, the higher partial waves become increasingly unimportant as $k\to 0$.

---

## 2. Threshold behavior of partial waves

For a short-range single-channel potential, the regular free radial function behaves at small argument as

$$
j_l(kr)\sim \frac{(kr)^l}{(2l+1)!!}.
$$

Inside the range of the potential, where $r\lesssim R$ and $kR\ll 1$, this gives one factor of $k^l$ from the incoming regular partial wave and another factor of $k^l$ from the outgoing projection. In Sakurai's partial-wave integral equation this appears schematically as

$$
f_l(k)
=
\frac{e^{i\delta_l}\sin\delta_l}{k}
\sim
k^{2l}.
$$

>[!mythoughts] what is this

For small phase shift,

$$
f_l(k)\simeq \frac{\delta_l(k)}{k},
$$

so the threshold behavior is

$$
\boxed{
\delta_l(k)\sim k^{2l+1}
}
\qquad
(k\to 0).
$$

Thus

$$
f_l(k)\sim k^{2l},
$$

and the $l$th partial contribution to the elastic cross section behaves as

$$
\sigma_l
=
\frac{4\pi}{k^2}(2l+1)\sin^2\delta_l
\sim
k^{4l}.
$$

The $l=0$ term is special:

$$
\delta_0(k)\sim k,
\qquad
f_0(k)\sim k^0,
\qquad
\sigma_0\sim k^0.
$$

All higher partial waves vanish at threshold for an ordinary finite-range potential:

$$
\sigma_1\sim k^4,\qquad
\sigma_2\sim k^8,\qquad
\ldots
$$

This is the mathematical content of the statement that ultralow-energy scattering is s-wave dominated.

---

## 3. Why s-wave scattering dominates at ultralow energy

The s wave has $l=0$, so it has no centrifugal barrier. Its effective radial potential is just the true interaction potential,

$$
V_{\mathrm{eff},0}(r)=V(r).
$$

For $l>0$,

$$
V_{\mathrm{eff},l}(r)
=
V(r)+\frac{\hbar^2}{2\mu}\frac{l(l+1)}{r^2}.
$$

At very small collision energy, the centrifugal term prevents most of the higher-$l$ wave from reaching the region where $V(r)$ acts. Physically, the incoming long-wavelength particle sees the scatterer as almost pointlike, so the outgoing wave is almost isotropic.

Therefore, for distinguishable particles in an ordinary short-range potential and away from special higher-partial-wave resonances,

$$
f(\theta;k)
=
\sum_{l=0}^{\infty}(2l+1)f_l(k)P_l(\cos\theta)
\approx
f_0(k).
$$

The leading scattering is independent of $\theta$. This isotropy is one of the practical signatures of s-wave dominance.

---

## 4. The s-wave amplitude

For $l=0$,

$$
S_0(k)=e^{2i\delta_0(k)}
$$

and

$$
f_0(k)
=
\frac{S_0(k)-1}{2ik}.
$$

Equivalently,

$$
\boxed{
f_0(k)
=
\frac{e^{i\delta_0(k)}\sin\delta_0(k)}{k}
=
\frac{1}{k\cot\delta_0(k)-ik}
}
$$

This formula is the main bridge between phase-shift language and low-energy amplitude language.

The denominator has two parts:

$$
k\cot\delta_0(k)
\quad
\text{and}
\quad
-ik.
$$

The term $-ik$ is fixed by outgoing-wave boundary conditions and elastic unitarity. The real threshold information about the short-range potential is contained in $k\cot\delta_0(k)$.

---

## 5. Defining the scattering length through the low-energy amplitude

The scattering length is defined from the zero-energy limit of the s-wave scattering amplitude:

$$
\boxed{
a
\equiv
-\lim_{k\to 0} f_0(k)
}
$$

Equivalently,

$$
\boxed{
f_0(k\to 0)=-a
}
$$

This is the definition that will generalize most directly to Feshbach resonances.

>[!mythoughts] why can we do this? What's the meaning of scattering length in this definition? Is this definition universally accepted by the community?

Using

$$
f_0(k)
=
\frac{1}{k\cot\delta_0(k)-ik},
$$

a finite nonzero scattering length implies

$$
\lim_{k\to 0} k\cot\delta_0(k)
=
-\frac{1}{a}.
$$

Thus the same quantity may also be read from the small-$k$ phase shift:

$$
\delta_0(k)
\simeq
-ka
\qquad
(k\to 0,\ |ka|\ll 1).
$$

The sign in $f_0(0)=-a$ is important. A positive scattering length gives a negative zero-energy s-wave amplitude, while a negative scattering length gives a positive zero-energy s-wave amplitude.

---

## 6. Effective-range expansion

For a short-range single-channel potential, $k\cot\delta_0(k)$ is regular near $k=0$ as a function of $k^2$, apart from special singular cases. The low-energy expansion is

$$
\boxed{
k\cot\delta_0(k)
=
-\frac{1}{a}
+
\frac{1}{2}r_e k^2
+
O(k^4)
}
$$

Here $r_e$ is the effective range. Sakurai writes this parameter as $r_0$; this note uses $r_e$ to avoid confusion with the radial coordinate or the potential range $R$.

Substituting into the s-wave amplitude gives

$$
\boxed{
f_0(k)
=
\frac{1}{
-\dfrac{1}{a}
+
\dfrac{1}{2}r_e k^2
-ik
+
O(k^4)
}
}
$$

The leading approximation, obtained by dropping the effective-range term, is

$$
f_0(k)
\simeq
\frac{1}{-1/a-ik}
=
-\frac{a}{1+ika}.
$$

The corresponding s-wave elastic cross section is

$$
\sigma_0
=
4\pi |f_0(k)|^2.
$$

At strictly zero energy, for finite real $a$,

$$
\boxed{
\sigma_0(k\to 0)=4\pi a^2.
}
$$

If $|a|$ is very large, the finite-$k$ unitarity term $-ik$ cannot be ignored. In the leading approximation,

$$
\sigma_0(k)
\simeq
\frac{4\pi a^2}{1+k^2a^2}.
$$

For $|a|\to\infty$ at fixed nonzero $k$,

$$
\sigma_0(k)\to \frac{4\pi}{k^2},
$$

the s-wave unitarity limit.

---

## 7. Coordinate-space interpretation after the amplitude definition

The scattering length can be visualized in coordinate space, but this interpretation should come after the amplitude definition.

At zero energy and outside the range of a short-range potential, the $l=0$ reduced radial wave function $u(r)=rR_0(r)$ obeys

$$
\frac{d^2u}{dr^2}=0
\qquad
(r>R,\ k=0).
$$

Therefore

$$
u(r)=C(r-a).
$$

The number $a$ is the point where the extrapolated zero-energy outside wave function crosses the $r$ axis. This is why it is called a length.

This picture agrees with the phase-shift formula. At small but nonzero $k$, the outside s-wave radial function has the form

$$
u(r)\propto \sin(kr+\delta_0).
$$

When $k\to 0$,

$$
\sin(kr+\delta_0)
\simeq
k\left(r+\frac{\delta_0}{k}\right).
$$

Using $\delta_0\simeq -ka$, one obtains

$$
u(r)\propto r-a.
$$

Thus the intercept picture is useful, but it is not the primary definition in the scattering-amplitude viewpoint. The primary low-energy statement is

$$
f_0(0)=-a.
$$

---

## 8. Interpreting positive and negative scattering length

The scattering length is not simply the physical radius of the potential. It can be much smaller than, comparable to, or much larger than the potential range $R$.

### Positive scattering length

If

$$
a>0,
$$

then

$$
f_0(0)=-a<0.
$$

In the zero-energy coordinate-space picture, the extrapolated outside wave function crosses zero at a positive radius $r=a$.

A positive scattering length can arise from a repulsive potential. It can also arise from an attractive potential strong enough to support, or nearly support, an s-wave bound state near threshold. These two cases can have the same sign of $a$ but very different microscopic origins.

A large positive scattering length,

$$
a\gg R,
$$

is especially important. It usually signals a pole of the s-wave amplitude close to threshold on the bound-state side.

### Negative scattering length

If

$$
a<0,
$$

then

$$
f_0(0)=-a>0.
$$

In the coordinate-space picture, the extrapolated zero of the outside wave function lies at negative $r$. For an attractive potential, this often means that the attraction is not quite strong enough to support an s-wave bound state.

A large negative scattering length,

$$
|a|\gg R,
$$

also indicates a pole close to threshold, but on the non-bound side. In single-channel language this is often described as a virtual state rather than a normalizable bound state.

Thus the magnitude $|a|$ tells us how close the system is to a threshold pole, while the sign tells us on which side of threshold the pole lies in the simplest single-channel situation.

---

## 9. Large positive scattering length and a shallow bound state

A bound state has negative energy relative to the scattering threshold. Write

$$
E_{\mathrm{bound}}
=
-\frac{\hbar^2\kappa^2}{2\mu},
\qquad
\kappa>0.
$$

Its large-distance s-wave radial behavior is

$$
u_{\mathrm{bound}}(r)\propto e^{-\kappa r}.
$$

A bound state corresponds to a pole of the analytically continued s-wave amplitude at

$$
k=i\kappa.
$$

Using the effective-range form,

$$
f_0(k)
=
\frac{1}{
-\dfrac{1}{a}
+
\dfrac{1}{2}r_e k^2
-ik
},
$$

the pole condition at $k=i\kappa$ is

$$
-\frac{1}{a}
-\frac{1}{2}r_e\kappa^2
+\kappa
=
0.
$$

Equivalently,

$$
\kappa
=
\frac{1}{a}
+
\frac{1}{2}r_e\kappa^2.
$$

If the bound state is shallow compared with the range scale, then

$$
\kappa R\ll 1,
\qquad
a\gg R,
$$

and the effective-range correction is subleading. Therefore

$$
\kappa\simeq \frac{1}{a}
$$

and

$$
\boxed{
E_{\mathrm{bound}}
\simeq
-\frac{\hbar^2}{2\mu a^2}
\qquad
(a>0,\ a\gg R).
}
$$

Equivalently, the binding energy measured as a positive number is

$$
\boxed{
E_{\mathrm{bind}}
\simeq
\frac{\hbar^2}{2\mu a^2}.
}
$$

This is the key physical meaning of a large positive scattering length: the system has a very shallow s-wave bound state whose size is of order $a$, much larger than the microscopic interaction range.

---

## 10. Sakurai's single-channel limit

Sakurai's discussion is recovered by making the following reductions:

1. keep only one asymptotic channel;
2. assume a central, short-range potential;
3. work in a spinless elastic partial wave;
4. write the one-dimensional unitary partial-wave block as $S_l=e^{2i\delta_l}$.

Then

$$
f_l(k)
=
\frac{e^{2i\delta_l}-1}{2ik}
=
\frac{e^{i\delta_l}\sin\delta_l}{k}
=
\frac{1}{k\cot\delta_l-ik}.
$$

At low energy, the threshold law gives

$$
\delta_l(k)\sim k^{2l+1}.
$$

Thus the s wave dominates:

$$
f(\theta;k)\approx f_0(k).
$$

For the s wave,

$$
\lim_{k\to 0}k\cot\delta_0(k)
=
-\frac{1}{a},
$$

and therefore

$$
f_0(k\to 0)=-a.
$$

The zero-energy cross section becomes

$$
\sigma_{\mathrm{tot}}(k\to 0)
=
\sigma_0(k\to 0)
=
4\pi a^2.
$$

Keeping the next term gives Sakurai's effective-range correction:

$$
k\cot\delta_0
=
-\frac{1}{a}
+
\frac{1}{2}r_e k^2.
$$

Finally, a shallow bound state appears as a pole of $S_0(k)$, or equivalently of $f_0(k)$, at $k=i\kappa$. For $a\gg R$,

$$
\kappa\simeq \frac{1}{a},
\qquad
E_{\mathrm{bind}}
\simeq
\frac{\hbar^2}{2\mu a^2}.
$$

This is the single-channel story. Feshbach resonance theory keeps the same low-energy observable but changes the mechanism that makes it large.

---

## 11. Multichannel scattering length: attach it to an entrance channel

In multichannel scattering, there is no single universal scattering length unless a particular entrance channel and a particular elastic amplitude have been chosen.

Let $o$ be the entrance open channel whose threshold defines the collision energy,

$$
E
=
\epsilon_o+\frac{\hbar^2k_o^2}{2\mu_o}.
$$

The elastic channel-resolved s-wave amplitude is the $l=0$ component of the amplitude for

$$
o\to o.
$$

Denote it by

$$
f^0_{oo}(E).
$$

The entrance-channel scattering length is defined by

$$
\boxed{
a_o
\equiv
-\lim_{k_o\to 0}f^0_{oo}(E)
}
$$

with

$$
E=\epsilon_o+\frac{\hbar^2k_o^2}{2\mu_o}.
$$

Thus

$$
\boxed{
f^0_{oo}(k_o\to 0)=-a_o.
}
$$

This is the multichannel version of the single-channel definition. The channel label matters. A different entrance channel $o'$ can have a different elastic amplitude and therefore a different scattering length $a_{o'}$.

If the entrance channel is the only energetically open channel at threshold and the dynamics is lossless, $a_o$ is real. If there are open inelastic or reactive loss channels at the same energy, then the elastic element need not be a pure one-channel unitary phase. In that case the zero-energy elastic scattering length can be complex:

$$
a_o=\alpha_o-i\beta_o,
$$

with the imaginary part encoding loss from the observed elastic channel under the chosen convention.

---

## 12. Preparing for magnetic-field-dependent scattering length

The Feshbach resonance setting adds a control parameter, often a magnetic field $B$. The Hamiltonian and channel thresholds depend on $B$, so the entrance-channel elastic s-wave amplitude also depends on $B$:

$$
f^0_{oo}(E;B).
$$

The magnetic-field-dependent scattering length is therefore

$$
\boxed{
a_o(B)
\equiv
-\lim_{k_o\to 0}f^0_{oo}(E;B).
}
$$

This definition does not require a new kind of scattering observable. It is the same zero-energy entrance-channel elastic s-wave amplitude, evaluated for a Hamiltonian whose channel energies and couplings depend on $B$.

The physical mechanism is multichannel. A closed-channel bound state can be tuned near the open-channel threshold. Even though the closed channel does not appear as an outgoing flux channel at infinity, it enters the internal resolvent and can strongly modify the open-channel block

$$
S^0_{oo}(E;B).
$$

As that closed-channel state approaches threshold, the zero-energy elastic amplitude can become very large. In scattering-length language, $a_o(B)$ becomes strongly field dependent.

The familiar Feshbach-resonance formula for $a(B)$ will be derived later. For now, the essential point is only the definition:

$$
\boxed{
\text{Feshbach scattering length}
=
-\text{zero-energy entrance-channel elastic s-wave amplitude}.
}
$$

---

## 13. Logical summary

At low energy,

$$
kR\ll 1,
$$

higher partial waves are suppressed by threshold behavior:

$$
\delta_l(k)\sim k^{2l+1},
\qquad
f_l(k)\sim k^{2l}.
$$

Therefore s-wave scattering dominates:

$$
f(\theta;k)\approx f_0(k).
$$

The s-wave amplitude is

$$
f_0(k)
=
\frac{1}{k\cot\delta_0(k)-ik}.
$$

The scattering length is defined by

$$
a=-\lim_{k\to 0}f_0(k),
$$

so

$$
f_0(0)=-a.
$$

The effective-range expansion is

$$
k\cot\delta_0(k)
=
-\frac{1}{a}
+
\frac{1}{2}r_e k^2
+
O(k^4),
$$

hence

$$
f_0(k)
=
\frac{1}{
-\dfrac{1}{a}
+
\dfrac{1}{2}r_e k^2
-ik
+
O(k^4)
}.
$$

A large positive scattering length corresponds, in the simplest single-channel case, to a shallow bound state with

$$
E_{\mathrm{bind}}
\simeq
\frac{\hbar^2}{2\mu a^2}.
$$

In multichannel scattering, the scattering length must be attached to a specified entrance channel and elastic s-wave amplitude:

$$
a_o
=
-\lim_{k_o\to 0}f^0_{oo}(E).
$$

With a magnetic field,

$$
a_o(B)
=
-\lim_{k_o\to 0}f^0_{oo}(E;B).
$$

This is the low-energy observable that Feshbach resonance theory will explain.
