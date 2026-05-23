# Scattering Theory VI - Low-Energy Scattering, Effective Range, and Scattering Length

The previous notes developed scattering from a channel-resolved and partial-wave point of view. In that language the fundamental object is not first a phase shift, but a partial-wave block of the scattering matrix,

$$
S^l_{ba}(E),
$$

where $a$ labels the prepared incoming channel and $b$ labels an outgoing open channel. In the special case of a single open elastic channel, this block becomes a one-dimensional unitary number,

$$
S_l(E)=e^{2i\delta_l(E)}.
$$

Only in that one-channel elastic reduction does it make sense to replace the partial-wave $S$ matrix by a single real phase shift $\delta_l$.

The subject of this note is the low-energy limit of that story. At first this sounds like a return to Sakurai's single-channel problem, but the logical relation is more precise:

1. The general theory still begins with channel-resolved amplitudes and partial-wave $S$-matrix blocks.
2. At sufficiently low collision energy, ordinary short-range scattering is dominated by the $l=0$ partial wave.
3. If only one entrance channel is open, or if we focus on one elastic entrance-channel amplitude, the relevant low-energy observable is the zero-energy elastic s-wave amplitude.
4. The scattering length is the negative of that amplitude at threshold.

Thus the single-channel formulas are not being introduced as a replacement for the multichannel viewpoint. They are the simplest threshold reduction of it.

---

## 1. Low energy means that the wave cannot resolve the interaction region

Let $R$ denote the characteristic range of the interaction. For example, $R$ may be the radius beyond which a short-range potential is negligible. Low-energy scattering means

$$
kR\ll 1,
$$

where $k$ is the relative wave number in the incoming open channel.

This condition has a direct physical meaning. The de Broglie wavelength is much larger than the size of the region where the particles interact. The wave therefore cannot resolve detailed angular structure on the scale of the potential. The mathematical version of this statement is the threshold suppression of higher partial waves.

For a central single-channel problem, the free radial functions are spherical Bessel functions. Near the origin,

$$
j_l(kr)\sim \frac{(kr)^l}{(2l+1)!!}
\qquad
(kr\ll 1).
$$

The interaction acts mainly inside $r\lesssim R$. In this region the regular $l$th partial wave carries a factor $(kr)^l$. A transition amplitude in the $l$th partial wave contains an incoming regular wave sampled inside the interaction region and an outgoing projection onto the same angular-momentum sector. Thus the short-distance overlap has the threshold scaling

$$
\text{short-range overlap in the } l\text{th partial wave}
\sim k^l k^l
=
k^{2l}.
$$

This is the origin of the threshold law for the partial-wave amplitude,

$$
f_l(k)\sim k^{2l}.
$$

The corresponding relation to the phase shift follows from the one-channel elastic identity

$$
f_l(k)
=
\frac{e^{2i\delta_l(k)}-1}{2ik}.
$$

For small $k$, away from a threshold singularity, the phase shift is small, so

$$
e^{2i\delta_l}-1\simeq 2i\delta_l.
$$

Therefore

$$
f_l(k)\simeq \frac{\delta_l(k)}{k}.
$$

Combining this with $f_l(k)\sim k^{2l}$ gives

$$
\delta_l(k)\sim k^{2l+1}.
$$

Hence

$$
\delta_0(k)\sim k,
\qquad
\delta_1(k)\sim k^3,
\qquad
\delta_2(k)\sim k^5,
\qquad
\ldots
$$

The partial elastic cross section is

$$
\sigma_l
=
\frac{4\pi}{k^2}(2l+1)\sin^2\delta_l.
$$

Using $\sin\delta_l\simeq\delta_l$, one obtains

$$
\sigma_l\sim k^{4l}.
$$

Thus

$$
\sigma_0\sim k^0,
\qquad
\sigma_1\sim k^4,
\qquad
\sigma_2\sim k^8,
\qquad
\ldots
$$

The s wave survives at threshold, while all higher partial waves are suppressed for an ordinary finite-range interaction.

This is also visible from the effective radial potential. After separating variables, the $l$th reduced radial wave function sees

$$
V_{\mathrm{eff},l}(r)
=
V(r)+\frac{\hbar^2 l(l+1)}{2\mu r^2}.
$$

For $l>0$, the centrifugal term is a positive barrier near the interaction region. At very small collision energy, this barrier prevents most of the higher-$l$ wave from reaching the short-range potential. The s wave has no centrifugal barrier, so it is the only generic partial wave that remains unsuppressed as $k\to 0$.

There are exceptions, such as a near-threshold p-wave resonance, but those are special threshold-tuned situations. The ordinary low-energy, short-range case is s-wave dominated.

---

## 2. The s-wave amplitude is the low-energy object

For a single open elastic channel, the $l=0$ partial-wave block is

$$
S_0(k)=e^{2i\delta_0(k)}.
$$

The corresponding partial-wave amplitude is

$$
f_0(k)
=
\frac{S_0(k)-1}{2ik}
=
\frac{e^{2i\delta_0(k)}-1}{2ik}.
$$

It is useful to rewrite this formula as

$$
f_0(k)
=
\frac{e^{i\delta_0(k)}\sin\delta_0(k)}{k}
=
\frac{1}{k\cot\delta_0(k)-ik}.
$$

The last form separates two different kinds of information:

$$
f_0(k)^{-1}
=
k\cot\delta_0(k)-ik.
$$

The imaginary term $-ik$ is not a model-dependent detail. It is fixed by the outgoing-wave boundary condition and elastic unitarity. The real term $k\cot\delta_0(k)$ contains the low-energy information about the short-range dynamics.

At ultralow energy the full scattering amplitude is approximately isotropic,

$$
f(\theta;k)
=
\sum_{l=0}^{\infty}(2l+1)f_l(k)P_l(\cos\theta)
\approx f_0(k).
$$

Therefore the threshold behavior of scattering is controlled by the single complex number $f_0(k)$.

---

## 3. The scattering length from the zero-energy amplitude

The scattering length is defined by

$$
a
=
-\lim_{k\to 0} f_0(k),
$$

or equivalently,

$$
f_0(0)=-a.
$$

This definition is not arbitrary. It is the amplitude version of a simple zero-energy coordinate-space statement.

At large distance, the scattering state has the form

$$
\psi^{(+)}_{\mathbf k}(\mathbf r)
\sim
e^{i\mathbf k\cdot \mathbf r}
+
f(\theta;k)\frac{e^{ikr}}{r}.
$$

In the s-wave dominated zero-energy limit,

$$
e^{i\mathbf k\cdot \mathbf r}\to 1,
\qquad
e^{ikr}\to 1,
\qquad
f(\theta;k)\to f_0(0).
$$

Thus the outside wave function becomes

$$
\psi(\mathbf r)
\sim
1+\frac{f_0(0)}{r}.
$$

Using $f_0(0)=-a$,

$$
\psi(\mathbf r)
\sim
1-\frac{a}{r}.
$$

For the reduced s-wave radial function $u(r)=rR_0(r)$, this is

$$
u(r)\propto r-a
\qquad
(r>R,\ E=0).
$$

So $a$ is the point at which the extrapolated zero-energy outside radial wave function crosses the $r$ axis.

This explains both words in the name:

- it is a length because it is an intercept in the zero-energy radial wave function;
- it is a scattering length because it is defined from the zero-energy scattering amplitude.

The sign convention $f_0(0)=-a$ is chosen so that the outside zero-energy wave takes the simple form $1-a/r$, or equivalently $u(r)\propto r-a$.

The same definition follows from the phase-shift formula. If $a$ is finite, then

$$
f_0(k)
=
\frac{1}{k\cot\delta_0(k)-ik}
\longrightarrow
-a.
$$

Therefore

$$
\lim_{k\to 0} k\cot\delta_0(k)
=
-\frac{1}{a}.
$$

For small $k$ with $|ka|\ll 1$,

$$
\delta_0(k)\simeq -ka.
$$

Thus the scattering length may be read equivalently from the zero-energy amplitude, the zero-energy radial intercept, or the leading low-energy phase shift. The amplitude definition is the most portable one, because it generalizes directly to a chosen elastic channel in a multichannel problem.

---

## 4. Effective-range expansion

The s-wave amplitude can be inverted as

$$
f_0(k)^{-1}
=
k\cot\delta_0(k)-ik.
$$

For elastic scattering, unitarity fixes the imaginary part of $f_0(k)^{-1}$ to be $-k$. The remaining real part,

$$
k\cot\delta_0(k),
$$

is the part controlled by the short-range potential.

For an ordinary finite-range potential, this real quantity is smooth near $k=0$ as a function of the energy, and the energy is proportional to $k^2$. Therefore one expands it in powers of $k^2$:

$$
k\cot\delta_0(k)
=
-\frac{1}{a}
+
\frac{1}{2}r_e k^2
+
O(k^4).
$$

This is the effective-range expansion.

The coefficient $r_e$ is called the effective range because it measures the first correction to the zero-range approximation. If the entire low-energy interaction were captured only by $a$, then

$$
k\cot\delta_0(k)\approx -\frac{1}{a}.
$$

Keeping $r_e$ tells us how the finite spatial extent of the interaction begins to matter once $k$ is small but nonzero.

There is also a coordinate-space way to see why $r_e$ is a range-like quantity. Let $u_0(r)$ be the zero-energy s-wave reduced radial solution normalized so that outside the potential,

$$
u_0(r)=1-\frac{r}{a}
\qquad
(r>R).
$$

For a finite-range potential, one can express the effective range as

$$
r_e
=
2\int_0^\infty
\left[
\left(1-\frac{r}{a}\right)^2
-
u_0(r)^2
\right]dr,
$$

under the usual assumptions for the effective-range formula. The integrand vanishes outside the region where the true zero-energy solution differs from its free extrapolation. Thus $r_e$ is naturally of order the size of the region where the interaction distorts the wave function, unless the system is tuned close to a singular threshold situation.

Substituting the effective-range expansion into the amplitude gives

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

The leading scattering-length approximation is obtained by dropping the $r_e k^2$ term:

$$
f_0(k)
\simeq
\frac{1}{-1/a-ik}
=
-\frac{a}{1+ika}.
$$

At exactly zero energy,

$$
\sigma_0(0)
=
4\pi |f_0(0)|^2
=
4\pi a^2
$$

for real $a$.

At small but nonzero $k$,

$$
\sigma_0(k)
\simeq
4\pi |f_0(k)|^2
=
\frac{4\pi a^2}{1+k^2a^2}.
$$

This expression is especially important when $|a|$ is large. If $|a|\to\infty$ at fixed nonzero $k$, then

$$
\sigma_0(k)\to \frac{4\pi}{k^2}.
$$

This is the s-wave unitarity limit. A very large scattering length does not make the cross section infinite at fixed collision energy; the outgoing-wave term $-ik$ enforces the unitarity bound.

---
## 5. Bound states as poles of the s-wave amplitude

The scattering length is not only a parameter in the low-energy cross section. It also knows about the nearest s-wave pole of the analytically continued scattering amplitude. This is the generic reason why scattering length and shallow bound states are connected.

For a single-channel central potential, write the s-wave reduced radial equation as

$$
-\frac{d^2u}{dr^2}
+
U(r)u
=
k^2u,
\qquad
U(r)=\frac{2\mu}{\hbar^2}V(r).
$$

The physical radial wave function is $R_0(r)=u(r)/r$, and regularity at the origin requires

$$
u(0)=0.
$$

For a short-range potential, $U(r)=0$ outside the interaction region. Thus, for $r>R$, the scattering solution is a linear combination of free incoming and outgoing radial waves. In the one-channel elastic case this is equivalently written as

$$
u_k(r)
\propto
\sin(kr+\delta_0(k)).
$$

The s-wave amplitude is

$$
f_0(k)
=
\frac{1}{k\cot\delta_0(k)-ik}.
$$

For real positive $k$, this formula describes ordinary scattering states. But the expression also has an analytic continuation to complex $k$. The poles of that analytic continuation have physical meaning.

A bound state has negative energy relative to the scattering threshold,

$$
E
=
-\frac{\hbar^2\kappa^2}{2\mu},
\qquad
\kappa>0.
$$

This corresponds to

$$
k=i\kappa.
$$

Outside the potential, the bound-state radial equation is

$$
-u''=-\kappa^2u,
$$

so the outside solution is a combination of

$$
e^{-\kappa r}
\qquad
\text{and}
\qquad
e^{+\kappa r}.
$$

Normalizability requires the growing piece to vanish. Therefore a bound state is exactly the situation in which the analytically continued scattering solution becomes a purely decaying outside solution,

$$
u_{\mathrm{bound}}(r)\propto e^{-\kappa r}.
$$

Since an outgoing scattering wave has outside dependence $e^{ikr}$, the substitution $k=i\kappa$ gives

$$
e^{ikr}
=
e^{-\kappa r}.
$$

Thus a bound state appears as a pole of the s-wave amplitude on the positive imaginary $k$ axis.

Using the effective-range expansion,

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
},
$$

a pole at $k=i\kappa$ satisfies

$$
-\frac{1}{a}
-\frac{1}{2}r_e\kappa^2
+\kappa
+
O(\kappa^4)
=
0.
$$

Equivalently,

$$
\kappa
=
\frac{1}{a}
+
\frac{1}{2}r_e\kappa^2
+
O(\kappa^4).
$$

If the bound state is shallow, then its size $1/\kappa$ is much larger than the potential range $R$. In that case

$$
\kappa R\ll 1,
$$

and the effective-range correction is subleading. The leading relation is therefore

$$
\kappa\simeq \frac{1}{a}.
$$

A shallow bound state close to threshold therefore requires

$$
a>0,
\qquad
a\gg R,
$$

and its binding energy is

$$
E_{\mathrm{bind}}
=
\frac{\hbar^2\kappa^2}{2\mu}
\simeq
\frac{\hbar^2}{2\mu a^2}.
$$

This derivation is generic. It did not use a square well. It only used the short-range nature of the potential, the one-channel elastic s-wave amplitude, and the fact that a bound state must be a normalizable pole of the analytically continued scattering solution.

There is also a useful coordinate-space way to see the same result. At zero energy and outside the potential,

$$
u_0(r)=C(r-a).
$$

For a shallow bound state, the outside bound-state wave is

$$
u_{\mathrm{bound}}(r)=A e^{-\kappa r}.
$$

Because the state is shallow, there is an intermediate region

$$
R\ll r\ll \frac{1}{\kappa},
$$

where the particle is already outside the potential but the exponential tail has not yet decayed much. In this region,

$$
e^{-\kappa r}
=
1-\kappa r+O(\kappa^2r^2).
$$

Up to an irrelevant normalization,

$$
1-\kappa r
=
-\kappa\left(r-\frac{1}{\kappa}\right).
$$

Comparing with the zero-energy outside form $r-a$ gives

$$
a\simeq \frac{1}{\kappa}.
$$

This is the same result as the pole derivation, but now it has a direct spatial interpretation: a shallow bound state has a very long tail, and the zero-energy scattering solution extrapolates to a node at approximately the size of that tail.

Now consider the opposite sign. If $a<0$ and $|a|\gg R$, the leading low-energy amplitude

$$
f_0(k)
\simeq
-\frac{a}{1+ika}
$$

has a pole at

$$
k=\frac{i}{a}
=
-\frac{i}{|a|}.
$$

This pole lies on the negative imaginary $k$ axis. The outside factor is then

$$
e^{ikr}
=
e^{+r/|a|},
$$

which grows at infinity. Therefore this pole is not a normalizable bound state.

Nevertheless, it is still a genuine pole of the analytically continued s-wave amplitude. It is called a virtual state, or sometimes an antibound state. A virtual state is not a hidden normalizable state of the Hamiltonian. It is a near-threshold pole on the non-bound side of the analytic continuation. Because it is close to $k=0$, it can strongly affect low-energy scattering even though it is not a physical bound state.

Thus, in the simplest one-channel s-wave situation,

$$
a\gg R
\quad
\Longleftrightarrow
\quad
\text{near-threshold bound-state pole},
$$

whereas

$$
a\ll -R
\quad
\Longleftrightarrow
\quad
\text{near-threshold virtual-state pole}.
$$

The magnitude $|a|$ tells us that an s-wave pole is close to threshold. The sign tells us on which side of the threshold pole structure the system lies.

---

## 6. How attraction changes the sign of the scattering length

The previous section explains why a large positive scattering length signals a shallow bound state. It remains to understand how this fits with the intuitive statement that weak attraction often gives negative scattering length, while strong attraction can give positive scattering length.

The key point is that the scattering length is not the sign of the potential. It is the intercept of the zero-energy outside solution,

$$
u_0(r)=C(r-a),
\qquad
r>R.
$$

The potential determines how the regular solution starting from the origin joins onto this outside straight line.

At zero energy, the s-wave equation is

$$
u_0''(r)
=
U(r)u_0(r),
\qquad
U(r)=\frac{2\mu}{\hbar^2}V(r).
$$

Suppose first that the potential is weakly attractive. In the interaction region, $V(r)<0$, so where $u_0(r)>0$,

$$
u_0''(r)<0.
$$

The zero-energy wave is bent downward relative to the free solution. When the outside solution is extrapolated backward, its zero typically lies at negative $r$. Therefore a weak attractive potential usually gives

$$
a<0.
$$

This statement is not saying that attraction always means $a<0$. It only describes the first stage before an s-wave bound state has appeared.

Now imagine increasing the strength of an attractive potential continuously. For example, write

$$
V_g(r)=gV(r),
\qquad
V(r)<0,
\qquad
g\geq 0.
$$

As $g$ increases, the s-wave spectrum changes continuously. At first there may be no bound state. Eventually, at a critical strength $g=g_c$, the first s-wave bound state appears exactly at threshold.

At that threshold point, the bound-state wave number is

$$
\kappa=0.
$$

The outside zero-energy solution is no longer a line with nonzero slope. It is the limiting case of a bound-state tail whose decay length has gone to infinity. Equivalently, in the outside zero-energy form

$$
u_0(r)=A+Br,
$$

the threshold state has

$$
B=0.
$$

Since

$$
u_0(r)=C(r-a)
=
Cr-Ca,
$$

we have

$$
a=-\frac{A}{B}.
$$

Therefore, when $B\to 0$, the scattering length diverges:

$$
|a|\to\infty.
$$

This is the generic reason why the scattering length blows up when an s-wave bound state crosses threshold.

On the weak-attraction side, before the bound state is created, the near-threshold pole is a virtual-state pole and the scattering length is large and negative:

$$
a\to -\infty.
$$

At the critical coupling, the pole reaches threshold:

$$
k=0.
$$

After the coupling is increased slightly beyond the critical value, the pole moves to the positive imaginary $k$ axis and becomes a true shallow bound state:

$$
k=i\kappa,
\qquad
\kappa>0.
$$

Then the scattering length is large and positive:

$$
a\simeq \frac{1}{\kappa}>0.
$$

Thus the sign flip is not an accidental feature of the square well. It is the generic s-wave pole crossing threshold.

Schematically, as an attractive potential is deepened,

$$
\text{no bound state, virtual pole near threshold}
\quad
\Longrightarrow
\quad
a<0,
$$

then

$$
\text{pole at threshold}
\quad
\Longrightarrow
\quad
|a|=\infty,
$$

then

$$
\text{shallow bound state}
\quad
\Longrightarrow
\quad
a>0.
$$

The same pattern repeats whenever another s-wave bound state is pulled through threshold. This is why an attractive potential can give either sign of scattering length. The sign is controlled not by whether the potential is attractive or repulsive in a naive sense, but by the location of the nearest s-wave pole relative to threshold.

Repulsive potentials are different. For a purely repulsive short-range potential, the zero-energy wave is excluded from the interaction region. Its outside line usually extrapolates to a zero at a positive radius. A hard sphere of radius $R$ is the limiting example:

$$
u_0(R)=0,
\qquad
u_0(r)\propto r-R
\quad
(r>R),
$$

so

$$
a=R.
$$

Thus positive scattering length has two physically distinct origins:

1. repulsion can produce a positive intercept by excluding the wave from the interaction region;
2. attraction can produce a positive scattering length after an s-wave bound state has crossed below threshold.

The same sign of $a$ can therefore correspond to very different microscopic physics.

---

## 7. The square well as an explicit model

The attractive square well is useful because every step above can be seen analytically. Consider

$$
V(r)=
\begin{cases}
-V_0, & r<R,\\
0, & r>R,
\end{cases}
\qquad
V_0>0.
$$

Define

$$
q=\frac{\sqrt{2\mu V_0}}{\hbar}.
$$

At zero scattering energy, the inside equation is

$$
u''+q^2u=0.
$$

Regularity at the origin gives

$$
u_{\mathrm{in}}(r)=A\sin(qr).
$$

Outside the well, the zero-energy solution is

$$
u_{\mathrm{out}}(r)=C(r-a).
$$

Matching logarithmic derivatives at $r=R$ gives

$$
\frac{u_{\mathrm{out}}'(R)}{u_{\mathrm{out}}(R)}
=
\frac{u_{\mathrm{in}}'(R)}{u_{\mathrm{in}}(R)}.
$$

That is,

$$
\frac{1}{R-a}
=
q\cot(qR).
$$

Solving for $a$ gives

$$
a
=
R-\frac{\tan(qR)}{q}.
$$

This formula already contains the full sign-changing behavior.

For a weak well,

$$
qR\ll 1,
$$

and

$$
\tan(qR)
=
qR+\frac{(qR)^3}{3}+O((qR)^5).
$$

Therefore

$$
a
=
R-\left[
R+\frac{q^2R^3}{3}+O(q^4R^5)
\right],
$$

so

$$
a
\simeq
-\frac{q^2R^3}{3}
<0.
$$

Thus weak attraction gives negative scattering length.

As the well becomes deeper, $qR$ increases. When

$$
qR\to \frac{\pi}{2}^{-},
$$

we have

$$
\tan(qR)\to +\infty,
$$

so

$$
a\to -\infty.
$$

Immediately after crossing this point,

$$
qR\to \frac{\pi}{2}^{+},
$$

we have

$$
\tan(qR)\to -\infty,
$$

so

$$
a\to +\infty.
$$

This is the first s-wave threshold crossing. The square well has just become deep enough to support an s-wave bound state at zero energy.

To see this directly, consider a bound state with

$$
E=-\frac{\hbar^2\kappa^2}{2\mu},
\qquad
\kappa>0.
$$

Outside the well,

$$
u_{\mathrm{out}}(r)=C e^{-\kappa r}.
$$

Inside the well,

$$
u_{\mathrm{in}}(r)=A\sin(Kr),
$$

where

$$
K=\sqrt{q^2-\kappa^2}.
$$

Matching logarithmic derivatives at $r=R$ gives the bound-state condition

$$
K\cot(KR)=-\kappa.
$$

At the threshold where the bound state first appears,

$$
\kappa=0,
\qquad
K=q.
$$

The condition becomes

$$
q\cot(qR)=0.
$$

Therefore

$$
qR=\frac{\pi}{2},\frac{3\pi}{2},\frac{5\pi}{2},\ldots
$$

These are exactly the points where the scattering length formula

$$
a
=
R-\frac{\tan(qR)}{q}
$$

diverges.

The first divergence at $qR=\pi/2$ corresponds to the first s-wave bound state entering from threshold. The next divergence at $qR=3\pi/2$ corresponds to the next s-wave bound state entering from threshold, and so on. This is the square-well version of the general statement that each new s-wave bound state crossing threshold produces a pole at $k=0$ and a divergence of the scattering length.

The virtual-state side is also visible. A virtual state corresponds to a pole at

$$
k=-i\lambda,
\qquad
\lambda>0.
$$

The outside outgoing-wave factor is then

$$
e^{ikr}=e^{+\lambda r},
$$

so the state is not normalizable. Nevertheless, imposing the same analytic pole condition gives an outside logarithmic derivative

$$
\frac{u_{\mathrm{out}}'(R)}{u_{\mathrm{out}}(R)}
=
+\lambda.
$$

The corresponding square-well pole equation is

$$
K\cot(KR)=+\lambda,
$$

with

$$
K=\sqrt{q^2-\lambda^2},
$$

for a near-threshold virtual pole with $\lambda\ll q$.

Near threshold, the general effective-range result says

$$
\lambda\simeq \frac{1}{|a|}
$$

when

$$
a\ll -R.
$$

Thus, just before the first bound state appears, the square well has a virtual-state pole very close to threshold and a large negative scattering length. Just after the bound state appears, the pole is on the positive imaginary $k$ axis and the scattering length is large and positive.

The square well therefore illustrates the generic theory rather than replacing it. The analytic formula

$$
a
=
R-\frac{\tan(qR)}{q}
$$

is model-specific, but the pole logic is not model-specific:

$$
\text{virtual pole near } k=0
\quad
\Longleftrightarrow
\quad
a\ll -R,
$$

$$
\text{pole at } k=0
\quad
\Longleftrightarrow
\quad
|a|=\infty,
$$

$$
\text{shallow bound-state pole near } k=0
\quad
\Longleftrightarrow
\quad
a\gg R.
$$

This is the sense in which the square well's ladder of bound states has a generic meaning. The exact level spacings and threshold values depend on the potential, but the threshold crossing of an s-wave pole and the associated divergence and sign change of $a$ are general features of short-range one-channel s-wave scattering.
## 8. How this fits the multichannel viewpoint

In the channel-resolved theory, the scattering amplitude carries channel labels. If $o$ is the chosen entrance open channel, then the elastic s-wave amplitude is the $o\to o$ component of the $l=0$ amplitude:

$$
f^0_{oo}(E).
$$

The entrance-channel scattering length is defined by

$$
a_o
=
-\lim_{k_o\to 0} f^0_{oo}(E),
$$

where

$$
E
=
\epsilon_o+\frac{\hbar^2 k_o^2}{2\mu_o}.
$$

This is the direct multichannel analogue of

$$
a=-\lim_{k\to 0}f_0(k).
$$

The channel label matters. A different entrance channel can have a different elastic threshold, reduced mass, internal state, and scattering length.

If the entrance channel is the only energetically open channel at threshold, and if the dynamics is lossless, then the relevant open-channel $S$-matrix block is effectively one-dimensional at threshold. In that case one may write

$$
S^0_{oo}(E)=e^{2i\delta_o(E)}
$$

and use the same effective-range expansion,

$$
k_o\cot\delta_o(k_o)
=
-\frac{1}{a_o}
+
\frac{1}{2}r_{e,o}k_o^2
+
O(k_o^4).
$$

If other open channels are available at the same energy, the elastic element $S^0_{oo}$ need not have unit modulus. Probability can leave the entrance channel into other open channels. Then the elastic threshold parameter can be complex:

$$
a_o=\alpha_o-i\beta_o
$$

under the common convention in which $\beta_o\ge 0$ describes loss from the entrance channel. The real part controls the elastic phase-like shift, while the imaginary part encodes inelastic or reactive loss.

Closed channels require a different interpretation. A closed channel does not appear as an outgoing flux channel at infinity, because its asymptotic wave number is imaginary and its coordinate-space component decays exponentially. Nevertheless, closed channels can strongly affect the open-channel elastic amplitude through virtual propagation.

A useful way to say this is to split the Hilbert space into an open part $P$ and a closed part $Q$. Eliminating $Q$ gives an energy-dependent effective interaction in the open subspace,

$$
V_{\mathrm{eff}}(E)
=
V_{PP}
+
V_{PQ}\frac{1}{E-H_{QQ}}V_{QP},
$$

schematically, with the appropriate outgoing boundary prescription understood. If $H_{QQ}$ has a closed-channel bound state $|\phi_c\rangle$ with energy $E_c$ near the open-channel threshold, then the resolvent contains a term of the form

$$
\frac{|\phi_c\rangle\langle \phi_c|}{E-E_c}.
$$

After coupling back to the open channel, this produces a large energy-dependent contribution to the open-channel scattering amplitude. This is why a bound state in a closed channel can control the scattering length of an open channel even though the closed channel is not an asymptotic outgoing channel.

In a magnetic Feshbach resonance, the closed-channel bound-state energy depends on the magnetic field $B$. The entrance-channel scattering length is therefore

$$
a_o(B)
=
-\lim_{k_o\to 0} f^0_{oo}(E;B).
$$

The magnetic field tunes a near-threshold pole through the open-channel threshold, and the zero-energy elastic amplitude responds by becoming very large and changing sign. The familiar resonance formula for $a_o(B)$ is a later result; the definition needed for it is already contained in the threshold elastic amplitude.

---

## 9. Sakurai's single-channel discussion as a special case

Sakurai's single-channel formulas are recovered by imposing the following reductions:

1. there is only one asymptotic channel;
2. the potential is central and short-ranged;
3. the scattering is elastic;
4. the particles are treated in a spinless partial-wave basis;
5. each partial-wave block is one-dimensional.

Then

$$
S_l(k)=e^{2i\delta_l(k)}
$$

and

$$
f_l(k)
=
\frac{S_l(k)-1}{2ik}
=
\frac{e^{2i\delta_l(k)}-1}{2ik}
=
\frac{e^{i\delta_l(k)}\sin\delta_l(k)}{k}
=
\frac{1}{k\cot\delta_l(k)-ik}.
$$

The full amplitude is

$$
f(\theta;k)
=
\sum_{l=0}^{\infty}(2l+1)f_l(k)P_l(\cos\theta).
$$

At low energy,

$$
f_l(k)\sim k^{2l},
$$

so

$$
f(\theta;k)\approx f_0(k).
$$

For the s wave,

$$
k\cot\delta_0(k)
=
-\frac{1}{a}
+
\frac{1}{2}r_e k^2
+
O(k^4),
$$

and therefore

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

At leading order,

$$
f_0(k)
\simeq
-\frac{a}{1+ika}.
$$

At zero energy,

$$
f_0(0)=-a,
\qquad
\sigma_0(0)=4\pi a^2.
$$

If $a\gg R$, the analytically continued amplitude has a pole at

$$
k=i\kappa,
\qquad
\kappa\simeq \frac{1}{a},
$$

which corresponds to a shallow bound state with

$$
E_{\mathrm{bind}}
\simeq
\frac{\hbar^2}{2\mu a^2}.
$$

This is the Sakurai single-channel story, but now its place in the broader framework is clear. The phase shift is a one-channel parameterization of a partial-wave $S$-matrix block. The scattering length is the zero-energy limit of the elastic s-wave amplitude. In a multichannel problem, the same definition applies only after choosing an entrance channel and an elastic s-wave amplitude.

---

## 10. Summary

The low-energy condition

$$
kR\ll 1
$$

means that the incoming wavelength is much larger than the interaction region. For ordinary short-range scattering, the $l$th partial-wave amplitude scales as

$$
f_l(k)\sim k^{2l},
$$

and the phase shift scales as

$$
\delta_l(k)\sim k^{2l+1}.
$$

Therefore s-wave scattering dominates at threshold.

In the single-channel elastic s-wave problem,

$$
f_0(k)
=
\frac{1}{k\cot\delta_0(k)-ik}.
$$

The scattering length is

$$
a=-\lim_{k\to 0}f_0(k),
$$

so

$$
f_0(0)=-a.
$$

Equivalently, the outside zero-energy radial wave function behaves as

$$
u(r)\propto r-a.
$$

The effective-range expansion is

$$
k\cot\delta_0(k)
=
-\frac{1}{a}
+
\frac{1}{2}r_e k^2
+
O(k^4).
$$

The term $-ik$ in $f_0^{-1}$ is fixed by outgoing-wave boundary conditions and unitarity; $k\cot\delta_0$ is the real short-range part that can be expanded at low energy.

A large positive scattering length indicates, in the simplest single-channel elastic case, a shallow s-wave bound state with

$$
E_{\mathrm{bind}}
\simeq
\frac{\hbar^2}{2\mu a^2}.
$$

A large negative scattering length indicates a near-threshold virtual state rather than a normalizable bound state.

Positive $a$ can arise from repulsion because repulsion pushes the zero-energy wave outward. Positive $a$ can also arise from strong attraction after an s-wave bound state crosses threshold. Weak attraction usually gives negative $a$. These statements are consequences of the zero-energy radial equation and the pole structure of the amplitude, not independent rules to memorize.

In the multichannel setting, the scattering length must be attached to a chosen entrance channel:

$$
a_o
=
-\lim_{k_o\to 0}f^0_{oo}(E).
$$

A Feshbach resonance changes this entrance-channel scattering length by tuning a closed-channel bound state near the open-channel threshold. The observable remains the same kind of object: the zero-energy elastic s-wave amplitude in the chosen entrance channel.
