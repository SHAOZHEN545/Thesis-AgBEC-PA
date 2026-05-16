# Chapter 6 — Scattering Theory

This chapter is devoted to scattering processes. These are processes in which a continuum initial state is transformed into a continuum final state through the action of a potential that will be treated as a time-dependent perturbation. Such processes are central experimentally because they are a primary way of learning about mass, charge, and potential-energy distributions in molecular, atomic, and subatomic systems.

## 6.1 Scattering as a Time-Dependent Perturbation

Assume that the Hamiltonian can be written as

$$
H = H_0 + V(\mathbf{x}) . \tag{6.1}
$$

Here

$$
H_0 = \frac{\mathbf{p}^2}{2m} \tag{6.2}
$$

is the kinetic-energy operator, with eigenvalues

$$
E_k = \frac{\hbar^2 k^2}{2m}. \tag{6.3}
$$

The plane-wave eigenvectors of $H_0$ are denoted by $|\mathbf{k}\rangle$, and the scattering potential $V(\mathbf{r})$ is assumed to be time independent.

An incoming particle “sees” the scattering potential as a perturbation turned on only while the particle is near the scatterer. Thus the problem can be analyzed using time-dependent perturbation theory in the interaction picture.

Reviewing Section 5.7, the state $|\alpha,t_0;t_0\rangle_I$ evolves into $|\alpha,t_0;t\rangle_I$ according to

$$
|\alpha,t_0;t\rangle_I = U_I(t,t_0)|\alpha,t_0;t_0\rangle_I, \tag{6.4}
$$

where $U_I(t,t_0)$ satisfies

$$
i\hbar \frac{\partial}{\partial t} U_I(t,t_0)=V_I(t)U_I(t,t_0). \tag{6.5}
$$

The initial condition is $U_I(t_0,t_0)=1$, and

$$
V_I(t)=\exp\!\left(\frac{iH_0t}{\hbar}\right)V\exp\!\left(-\frac{iH_0t}{\hbar}\right).
$$

The formal solution is

$$
U_I(t,t_0)=1-\frac{i}{\hbar}\int_{t_0}^{t}V_I(t')U_I(t',t_0)\,dt'. \tag{6.6}
$$

Therefore the transition amplitude for an initial state $|i\rangle$ to transform into a final state $|n\rangle$, where both are eigenstates of $H_0$, is

$$
\langle n|U_I(t,t_0)|i\rangle
=\delta_{ni}-\frac{i}{\hbar}\sum_m \langle n|V|m\rangle
\int_{t_0}^{t}e^{i\omega_{nm}t'}\langle m|U_I(t',t_0)|i\rangle\,dt', \tag{6.7}
$$

where $\langle n|i\rangle=\delta_{ni}$ and $\hbar\omega_{nm}=E_n-E_m$.

To apply this formalism to scattering, the initial and final states must be normalized. Equation (6.7) assumes discrete states, while scattering states lie in the continuum. The standard device is to quantize the scattering states in a large cube of side $L$. In the coordinate representation,

$$
\langle \mathbf{x}|\mathbf{k}\rangle=\frac{1}{L^{3/2}}e^{i\mathbf{k}\cdot\mathbf{x}}, \tag{6.8}
$$

so that $\langle \mathbf{k}'|\mathbf{k}\rangle=\delta_{\mathbf{k}\mathbf{k}'}$, with the allowed $\mathbf{k}$ values discrete. The limit $L\to\infty$ is taken at the end.

The initial and final states exist asymptotically, so both $t\to\infty$ and $t_0\to -\infty$ must be considered. In first order, one sets $\langle m|U_I(t',t_0)|i\rangle=\delta_{mi}$ inside the integral, giving

$$
\langle n|U_I(t,t_0)|i\rangle
=\delta_{ni}-\frac{i}{\hbar}\langle n|V|i\rangle\int_{t_0}^{t}e^{i\omega_{ni}t'}\,dt'. \tag{6.9}
$$

As $t\to\infty$, this leads to a transition rate, namely Fermi’s golden rule. To also accommodate $t_0\to -\infty$, define the $T$ matrix by

$$
\langle n|U_I(t,t_0)|i\rangle
=\delta_{ni}-\frac{i}{\hbar}T_{ni}\int_{t_0}^{t}e^{i\omega_{ni}t'+\epsilon t'}\,dt', \tag{6.10}
$$

where $\epsilon>0$ and $t\ll 1/\epsilon$. These conditions make $e^{\epsilon t'}$ close to unity as $t\to\infty$ and force the integrand to vanish as $t_0\to -\infty$. The limit $\epsilon\to 0$ is taken before $t\to +\infty$.

The scattering matrix, or $S$ matrix, is defined in terms of the $T$ matrix as

$$
\begin{aligned}
S_{ni}
&\equiv \lim_{t\to\infty}\left[\lim_{\epsilon\to 0}\langle n|U_I(t,-\infty)|i\rangle\right] \\
&=\delta_{ni}-\frac{i}{\hbar}T_{ni}\int_{-\infty}^{\infty}e^{i\omega_{ni}t'}\,dt' \\
&=\delta_{ni}-2\pi i\,\delta(E_n-E_i)T_{ni}.
\end{aligned} \tag{6.11}
$$

The $S$ matrix has a no-scattering part, where final and initial states are the same, and a scattering part governed by the $T$ matrix.

### 6.1.1 Transition Rates and Cross Sections

Proceeding as in Section 5.7, define the transition rate as

$$
w(i\to n)=\frac{d}{dt}|\langle n|U_I(t,-\infty)|i\rangle|^2. \tag{6.12}
$$

For $|i\rangle\ne |n\rangle$,

$$
\langle n|U_I(t,-\infty)|i\rangle
=-\frac{i}{\hbar}T_{ni}\int_{-\infty}^{t}e^{i\omega_{ni}t'+\epsilon t'}\,dt'
=-\frac{i}{\hbar}T_{ni}\frac{e^{i\omega_{ni}t+\epsilon t}}{i\omega_{ni}+\epsilon}. \tag{6.13}
$$

Thus

$$
\begin{aligned}
w(i\to n)
&=\frac{d}{dt}\left[\frac{1}{\hbar^2}|T_{ni}|^2\frac{e^{2\epsilon t}}{\omega_{ni}^2+\epsilon^2}\right] \\
&=\frac{1}{\hbar^2}|T_{ni}|^2\frac{2\epsilon e^{2\epsilon t}}{\omega_{ni}^2+\epsilon^2}.
\end{aligned}
$$

Since

$$
\int_{-\infty}^{\infty}\frac{1}{\omega^2+\epsilon^2}\,d\omega=\frac{\pi}{\epsilon}, \tag{6.14}
$$

one has, for finite $t$,

$$
\lim_{\epsilon\to 0}\frac{\epsilon e^{2\epsilon t}}{\omega_{ni}^2+\epsilon^2}
=\pi\delta(\omega_{ni})=\pi\hbar\delta(E_n-E_i). \tag{6.15}
$$

Therefore

$$
w(i\to n)=\frac{2\pi}{\hbar}|T_{ni}|^2\delta(E_n-E_i). \tag{6.16}
$$

This resembles Fermi’s golden rule, except that $V_{ni}$ is replaced by the more general $T_{ni}$.

For elastic scattering, take $|i\rangle=|\mathbf{k}\rangle$ and $|n\rangle=|\mathbf{k}'\rangle$, with $|\mathbf{k}|=|\mathbf{k}'|\equiv k$. In the large box,

$$
E_n=\frac{\hbar^2k'^2}{2m}=\frac{\hbar^2}{2m}\left(\frac{2\pi}{L}\right)^2|\mathbf{n}|^2,
$$

so

$$
\Delta E_n=\frac{\hbar^2}{m}\left(\frac{2\pi}{L}\right)^2|\mathbf{n}|\Delta |\mathbf{n}|. \tag{6.17}
$$

The number of states in a spherical shell of radius $|\mathbf{n}|$ and thickness $\Delta |\mathbf{n}|$ is

$$
\Delta n=4\pi |\mathbf{n}|^2\Delta |\mathbf{n}|\frac{d\Omega}{4\pi}. \tag{6.18}
$$

Thus the density of final states is

$$
\rho(E_n)=\frac{\Delta n}{\Delta E_n}
=\frac{m}{\hbar^2}\left(\frac{L}{2\pi}\right)^2|\mathbf{n}|\,d\Omega
=\frac{mk}{\hbar^2}\left(\frac{L}{2\pi}\right)^3d\Omega. \tag{6.19}
$$

After integrating over final states, the transition rate becomes

$$
w(i\to n)=\frac{mkL^3}{(2\pi)^2\hbar^3}|T_{ni}|^2d\Omega. \tag{6.20}
$$

The speed of particles in the incoming beam is $v=\hbar k/m$, so the flux in the beam is $v/L^3$. The probability flux for the wave function (6.8) is

$$
\mathbf{j}(\mathbf{x},t)=\left(\frac{\hbar}{m}\right)\frac{\mathbf{k}}{L^3}=\frac{\mathbf{v}}{L^3}. \tag{6.21}
$$

The cross section $d\sigma$ is the transition rate divided by the flux, yielding

$$
\frac{d\sigma}{d\Omega}=\left(\frac{mL^3}{2\pi\hbar^2}\right)^2|T_{ni}|^2. \tag{6.22}
$$

The remaining task is to relate $T_{ni}$ to the scattering potential $V(\mathbf{r})$.

### 6.1.2 Solving for the $T$ Matrix

From (6.10) and (6.13),

$$
\langle n|U_I(t,-\infty)|i\rangle
=\delta_{ni}+\frac{1}{\hbar}T_{ni}\frac{e^{i\omega_{ni}t+\epsilon t}}{-\omega_{ni}+i\epsilon}. \tag{6.23}
$$

Returning to (6.7), with $V_{nm}=\langle n|V|m\rangle$,

$$
\langle n|U_I(t,-\infty)|i\rangle
=\delta_{ni}-\frac{i}{\hbar}\sum_m V_{nm}\int_{-\infty}^{t}e^{i\omega_{nm}t'}\langle m|U_I(t',-\infty)|i\rangle\,dt'. \tag{6.24}
$$

Insert (6.23) into the integrand. The third term is

$$
-\frac{i}{\hbar}\frac{1}{\hbar}\sum_m V_{nm}\frac{T_{mi}}{-\omega_{mi}+i\epsilon}
\int_{-\infty}^{t}e^{i\omega_{nm}t'+i\omega_{mi}t'+\epsilon t'}\,dt'. \tag{6.25}
$$

Since $\omega_{nm}+\omega_{mi}=\omega_{ni}$, comparison with (6.23) gives

$$
T_{ni}=V_{ni}+\frac{1}{\hbar}\sum_m V_{nm}\frac{T_{mi}}{-\omega_{mi}+i\epsilon}
=V_{ni}+\sum_m V_{nm}\frac{T_{mi}}{E_i-E_m+i\hbar\epsilon}. \tag{6.26}
$$

This is an inhomogeneous system of linear equations for $T_{ni}$. Define states $|\psi^{(+)}\rangle$ by

$$
T_{ni}=\sum_j\langle n|V|j\rangle\langle j|\psi^{(+)}\rangle
=\langle n|V|\psi^{(+)}\rangle. \tag{6.27}
$$

Then

$$
\langle n|V|\psi^{(+)}\rangle
=\langle n|V|i\rangle+\sum_m\langle n|V|m\rangle\frac{\langle m|V|\psi^{(+)}\rangle}{E_i-E_m+i\hbar\epsilon}. \tag{6.28}
$$

Since this holds for all $|n\rangle$,

$$
\begin{aligned}
|\psi^{(+)}\rangle
&=|i\rangle+\sum_m |m\rangle\frac{\langle m|V|\psi^{(+)}\rangle}{E_i-E_m+i\hbar\epsilon} \\
&=|i\rangle+\frac{1}{E_i-H_0+i\hbar\epsilon}V|\psi^{(+)}\rangle.
\end{aligned} \tag{6.29}
$$

This is the Lippmann-Schwinger equation. In terms of $|\psi^{(+)}\rangle$,

$$
\frac{d\sigma}{d\Omega}=\left(\frac{mL^3}{2\pi\hbar^2}\right)^2|\langle n|V|\psi^{(+)}\rangle|^2. \tag{6.30}
$$

Introduce an operator $T$ by $\langle n|T|i\rangle=T_{ni}$ and $T|i\rangle=V|\psi^{(+)}\rangle$. Acting on (6.29) with $V$ from the left gives

$$
T=V+V\frac{1}{E_i-H_0+i\hbar\epsilon}T. \tag{6.31}
$$

If the scattering potential $V$ is weak, one obtains the order-by-order expansion

$$
T=V+V\frac{1}{E_i-H_0+i\hbar\epsilon}V
+V\frac{1}{E_i-H_0+i\hbar\epsilon}V\frac{1}{E_i-H_0+i\hbar\epsilon}V+\cdots . \tag{6.32}
$$

This approximation scheme is revisited in Section 6.3.

### 6.1.3 Scattering from the Future to the Past

One may also picture scattering as evolving backward in time from a plane wave state $|i\rangle$ in the far future to a state $|n\rangle$ in the distant past. In that case the formal solution (6.6) can be written as

$$
U_I(t,t_0)=1+\frac{i}{\hbar}\int_t^{t_0}V_I(t')U_I(t',t_0)\,dt', \tag{6.33}
$$

which is suited to taking $t_0\to +\infty$. The $T$ matrix is then defined by regularizing the integral with the opposite sign exponential:

$$
\langle n|U_I(t,t_0)|i\rangle
=\delta_{ni}+\frac{i}{\hbar}T_{ni}\int_t^{t_0}e^{i\omega_{ni}t'-\epsilon t'}\,dt'. \tag{6.34}
$$

This form defines a different set of states $|\psi^{(-)}\rangle$ through $T|i\rangle=V|\psi^{(-)}\rangle$.

## 6.2 The Scattering Amplitude

Replace $\hbar\epsilon$ in the Lippmann-Schwinger equation with $\epsilon$, and take $E$ as the initial and final elastic-scattering energy. Then

$$
|\psi^{(\pm)}\rangle=|i\rangle+\frac{1}{E-H_0\pm i\epsilon}V|\psi^{(\pm)}\rangle. \tag{6.35}
$$

Multiplying by $\langle \mathbf{x}|$ and inserting position completeness gives the integral equation

$$
\langle \mathbf{x}|\psi^{(\pm)}\rangle
=\langle \mathbf{x}|i\rangle+
\int d^3x'\left\langle \mathbf{x}\left|\frac{1}{E-H_0\pm i\epsilon}\right|\mathbf{x}'\right\rangle
\langle \mathbf{x}'|V|\psi^{(\pm)}\rangle. \tag{6.36}
$$

Define

$$
G_\pm(\mathbf{x},\mathbf{x}')\equiv \frac{\hbar^2}{2m}
\left\langle \mathbf{x}\left|\frac{1}{E-H_0\pm i\epsilon}\right|\mathbf{x}'\right\rangle. \tag{6.37}
$$

Inserting complete sets of momentum states gives

$$
G_\pm(\mathbf{x},\mathbf{x}')=\frac{\hbar^2}{2m}\sum_{\mathbf{k}'}\sum_{\mathbf{k}''}
\langle \mathbf{x}|\mathbf{k}'\rangle
\left\langle \mathbf{k}'\left|\frac{1}{E-H_0\pm i\epsilon}\right|\mathbf{k}''\right\rangle
\langle \mathbf{k}''|\mathbf{x}'\rangle. \tag{6.38}
$$

Use

$$
\left\langle \mathbf{k}'\left|\frac{1}{E-\hbar^2k'^2/2m\pm i\epsilon}\right|\mathbf{k}''\right\rangle
=\frac{\delta_{\mathbf{k}'\mathbf{k}''}}{E-\hbar^2k'^2/2m\pm i\epsilon}, \tag{6.39}
$$

$$
\langle \mathbf{x}|\mathbf{k}'\rangle=\frac{e^{i\mathbf{k}'\cdot\mathbf{x}}}{L^{3/2}}, \tag{6.40}
$$

and

$$
\langle \mathbf{k}''|\mathbf{x}'\rangle=\frac{e^{-i\mathbf{k}''\cdot\mathbf{x}'}}{L^{3/2}}. \tag{6.41}
$$

Putting $E=\hbar^2k^2/2m$, one obtains

$$
G_\pm(\mathbf{x},\mathbf{x}')=\frac{1}{L^3}\sum_{\mathbf{k}'}\frac{e^{i\mathbf{k}'\cdot(\mathbf{x}-\mathbf{x}')}}{k^2-k'^2\pm i\epsilon}. \tag{6.42}
$$

Taking $L\to\infty$ converts the sum to an integral:

$$
G_\pm(\mathbf{x},\mathbf{x}')=\frac{1}{(2\pi)^3}\int d^3k'\frac{e^{i\mathbf{k}'\cdot(\mathbf{x}-\mathbf{x}')}}{k^2-k'^2\pm i\epsilon}. \tag{6.43}
$$

In spherical coordinates, with angles measured relative to $\mathbf{x}-\mathbf{x}'$,

$$
\begin{aligned}
G_\pm(\mathbf{x},\mathbf{x}')
&=\frac{1}{(2\pi)^2}\int_0^\infty k'^2\,dk'\int_{-1}^{+1}d\mu\,
\frac{e^{ik'|\mathbf{x}-\mathbf{x}'|\mu}}{k^2-k'^2\pm i\epsilon} \\
&=\frac{1}{8\pi^2}\frac{1}{i|\mathbf{x}-\mathbf{x}'|}
\int_{-\infty}^{\infty}k'\,dk'
\left[\frac{e^{ik'|\mathbf{x}-\mathbf{x}'|}-e^{-ik'|\mathbf{x}-\mathbf{x}'|}}{k^2-k'^2\pm i\epsilon}\right].
\end{aligned} \tag{6.44}
$$

Complex contour integration is used to evaluate the integral. The Cauchy integral formula is

$$
\oint_C \frac{f(z)}{z-z_0}\,dz=2\pi i f(z_0), \tag{6.45}
$$

with $C$ counterclockwise.[^1]

> [!figure]
> ![[Fig. 6.1.png|center|500]]
> **Figure 6.1.** Integrating the two terms in (6.44) using complex contours. The dots (crosses) mark the positions of the two poles for the $+$ ($-$) form of $G_\pm(\mathbf{x},\mathbf{x}')$. We replace the integral over a real-valued $k'$ in (6.44) with one of the two contours in the figure, choosing the one on which the factor $e^{\pm ik'|\mathbf{x}-\mathbf{x}'|}$ tends to zero along the semicircle at large $\operatorname{Im}(k')$. Thus, the only contribution to the contour integral is along the real axis.

The denominator can be written as $-(k'-k_0)(k'+k_0)$, where $k_0\equiv k\pm i\epsilon$. The poles are at $\pm k_0$. Closing the contour in the appropriate half-plane gives

$$
\frac{2\pi i(\pm k)e^{i(\pm k)|\mathbf{x}-\mathbf{x}'|}}{-(\pm 2k)}
=-\pi i e^{\pm ik|\mathbf{x}-\mathbf{x}'|}, \tag{6.46}
$$

and hence

$$
G_\pm(\mathbf{x},\mathbf{x}')=-\frac{1}{4\pi}\frac{e^{\pm ik|\mathbf{x}-\mathbf{x}'|}}{|\mathbf{x}-\mathbf{x}'|}. \tag{6.47}
$$

This is Green’s function for the Helmholtz equation:

$$
(\nabla^2+k^2)G_\pm(\mathbf{x},\mathbf{x}')=\delta^{(3)}(\mathbf{x}-\mathbf{x}'). \tag{6.48}
$$

Using (6.47), the integral equation becomes

$$
\langle \mathbf{x}|\psi^{(\pm)}\rangle
=\langle \mathbf{x}|i\rangle-\frac{2m}{\hbar^2}\int d^3x'\frac{e^{\pm ik|\mathbf{x}-\mathbf{x}'|}}{4\pi|\mathbf{x}-\mathbf{x}'|}
\langle \mathbf{x}'|V|\psi^{(\pm)}\rangle. \tag{6.49}
$$

The wave function in the presence of the scatterer is the incident wave plus a scattering term. At large $r$, the latter has spatial dependence $e^{\pm ikr}/r$ for a finite-range potential. Thus $\psi^{(+)}$ is a plane wave plus an outgoing spherical wave, while $\psi^{(-)}$ is a plane wave plus an incoming spherical wave.

For a local potential,

$$
\langle \mathbf{x}'|V|\mathbf{x}''\rangle=V(\mathbf{x}')\delta^{(3)}(\mathbf{x}'-\mathbf{x}''). \tag{6.50}
$$

Thus

$$
\langle \mathbf{x}'|V|\psi^{(\pm)}\rangle
=\int d^3x''\langle \mathbf{x}'|V|\mathbf{x}''\rangle\langle \mathbf{x}''|\psi^{(\pm)}\rangle
=V(\mathbf{x}')\langle \mathbf{x}'|\psi^{(\pm)}\rangle. \tag{6.51}
$$

Then

$$
\langle \mathbf{x}|\psi^{(\pm)}\rangle
=\langle \mathbf{x}|i\rangle-\frac{2m}{\hbar^2}\int d^3x'\frac{e^{\pm ik|\mathbf{x}-\mathbf{x}'|}}{4\pi|\mathbf{x}-\mathbf{x}'|}V(\mathbf{x}')\langle \mathbf{x}'|\psi^{(\pm)}\rangle. \tag{6.52}
$$

For a finite-range potential, observations are made at $r$ much larger than the range of the potential, so

$$
|\mathbf{x}|\gg |\mathbf{x}'|. \tag{6.53}
$$

> [!figure]
> ![[Fig. 6.2.png|center|500]]
> **Figure 6.2.** Finite-range scattering potential. The observation point $P$ is where the wave function $\langle \mathbf{x}|\psi^{(\pm)}\rangle$ is to be evaluated, while the contribution to the integral in (6.52) is for $|\mathbf{x}'|$ less than the range of the potential, as depicted by the shaded region of the figure.

Writing $r=|\mathbf{x}|$, $r'=|\mathbf{x}'|$, and $\alpha=\angle(\mathbf{x},\mathbf{x}')$, for $r\gg r'$,

$$
|\mathbf{x}-\mathbf{x}'|
=\sqrt{r^2-2rr'\cos\alpha+r'^2}
=r\left(1-\frac{2r'}{r}\cos\alpha+\frac{r'^2}{r^2}\right)^{1/2}
\approx r-\hat{\mathbf{r}}\cdot\mathbf{x}', \tag{6.54}
$$

where

$$
\hat{\mathbf{r}}\equiv \frac{\mathbf{x}}{|\mathbf{x}|}. \tag{6.55}
$$

With $\mathbf{k}'\equiv k\hat{\mathbf{r}}$,

$$
e^{\pm ik|\mathbf{x}-\mathbf{x}'|}\approx e^{\pm ikr}e^{\mp i\mathbf{k}'\cdot\mathbf{x}'} \tag{6.56}
$$

for large $r$, and $1/|\mathbf{x}-\mathbf{x}'|$ may be replaced by $1/r$.

Taking the initial state as $|i\rangle=|\mathbf{k}\rangle$ gives

$$
\begin{aligned}
\langle \mathbf{x}|\psi^{(+)}\rangle
&\underset{r\,\mathrm{large}}{\longrightarrow}
\langle \mathbf{x}|\mathbf{k}\rangle
-\frac{1}{4\pi}\frac{2m}{\hbar^2}\frac{e^{ikr}}{r}
\int d^3x'\,e^{-i\mathbf{k}'\cdot\mathbf{x}'}V(\mathbf{x}')\langle \mathbf{x}'|\psi^{(+)}\rangle \\
&=\frac{1}{L^{3/2}}\left[e^{i\mathbf{k}\cdot\mathbf{x}}+\frac{e^{ikr}}{r}f(\mathbf{k}',\mathbf{k})\right].
\end{aligned} \tag{6.57}
$$

The scattering amplitude is

$$
\begin{aligned}
f(\mathbf{k}',\mathbf{k})
&\equiv -\frac{1}{4\pi}\frac{2m}{\hbar^2}L^3
\int d^3x'\frac{e^{-i\mathbf{k}'\cdot\mathbf{x}'}}{L^{3/2}}V(\mathbf{x}')\langle \mathbf{x}'|\psi^{(+)}\rangle \\
&=-\frac{mL^3}{2\pi\hbar^2}\langle \mathbf{k}'|V|\psi^{(+)}\rangle.
\end{aligned} \tag{6.58}
$$

The negative solution corresponds to the original plane wave plus an incoming spherical wave with spatial dependence $e^{-ikr}/r$ and amplitude $-(mL^3/2\pi\hbar^2)\langle -\mathbf{k}'|V|\psi^{(-)}\rangle$.

Comparing (6.58) with (6.30) gives

$$
\frac{d\sigma}{d\Omega}=|f(\mathbf{k}',\mathbf{k})|^2. \tag{6.59}
$$

> [!figure]
> ![[Fig. 6.3.png|center|500]]
> **Figure 6.3.** (a) Incident wave packet approaching scattering center initially. (b) Incident wave packet continuing to move in the original direction plus spherical outgoing wave front (after a long time duration).

### 6.2.1 Wave Packet Description

The plane wave used above is infinite in extent in both space and time. A more realistic description uses a wave packet approaching the scattering center.[^2] After a long time, the system consists of the original wave packet moving in the original direction plus a spherical wave front. The use of a plane wave is satisfactory when the wave-packet dimension is much larger than the size of the scatterer, or the range of $V$.

### 6.2.2 The Optical Theorem

The optical theorem relates the imaginary part of the forward scattering amplitude $f(\theta=0)\equiv f(\mathbf{k},\mathbf{k})$ to the total cross section $\sigma_{\mathrm{tot}}\equiv\int d\Omega\,(d\sigma/d\Omega)$:[^3]

$$
\operatorname{Im} f(\theta=0)=\frac{k\sigma_{\mathrm{tot}}}{4\pi}. \tag{6.60}
$$

Starting with the Lippmann-Schwinger equation (6.35) and $|i\rangle=|\mathbf{k}\rangle$,

$$
\begin{aligned}
\langle \mathbf{k}|V|\psi^{(+)}\rangle
&=\left(\langle \psi^{(+)}|-\langle \psi^{(+)}|V\frac{1}{E-H_0-i\epsilon}\right)V|\psi^{(+)}\rangle \\
&=\langle \psi^{(+)}|V|\psi^{(+)}\rangle
-\langle \psi^{(+)}|V\frac{1}{E-H_0-i\epsilon}V|\psi^{(+)}\rangle.
\end{aligned} \tag{6.61}
$$

The first term on the right is real because it is the expectation value of a Hermitian operator. To handle the imaginary part of the second term, use the Cauchy principal value.

> [!figure]
> ![[Fig. 6.4.png|center|500]]
> **Figure 6.4.** Contour used to integrate around a singularity located at $z_0=x_0+i\epsilon$.

For a singularity near the real axis,

$$
\int_{-\infty}^{\infty}\frac{f(x)}{x-x_0}\,dx
=\int_{-\infty}^{x_0-\delta}\frac{f(x)}{x-x_0}\,dx+
\int_c\frac{f(z)}{z-z_0}\,dz+
\int_{x_0+\delta}^{+\infty}\frac{f(x)}{x-x_0}\,dx. \tag{6.62}
$$

The principal value is

$$
P\int_{-\infty}^{+\infty}\frac{f(x)}{x-x_0}\,dx
=\lim_{\delta\to 0}\left[\int_{-\infty}^{x_0-\delta}\frac{f(x)}{x-x_0}\,dx+\int_{x_0+\delta}^{+\infty}\frac{f(x)}{x-x_0}\,dx\right]. \tag{6.63}
$$

The small semicircular contribution is

$$
\int_c\frac{f(z)}{z-z_0}\,dz
=\int_{-\pi}^{0}\frac{f(x_0)}{\delta e^{i\phi}}i\delta e^{i\phi}\,d\phi
\to i\pi f(x_0)\quad (\delta\to 0). \tag{6.64}
$$

Consequently,

$$
\int_{-\infty}^{\infty}\frac{f(x)}{x-x_0}\,dx
=P\int_{-\infty}^{+\infty}\frac{f(x)}{x-x_0}\,dx+i\pi f(x_0). \tag{6.65}
$$

This gives

$$
\lim_{\epsilon\to 0}\left(\frac{1}{E-H_0-i\epsilon}\right)
=\lim_{\epsilon\to 0}\int_{-\infty}^{+\infty}\frac{\delta(E-E')}{E'-H_0-i\epsilon}\,dE'
=i\pi\delta(E-H_0). \tag{6.66}
$$

Therefore,

$$
\operatorname{Im}\langle \mathbf{k}|V|\psi^{(+)}\rangle
=-\pi\langle \psi^{(+)}|V\delta(E-H_0)V|\psi^{(+)}\rangle
=-\pi\langle \mathbf{k}|T^\dagger\delta(E-H_0)T|\mathbf{k}\rangle. \tag{6.67}
$$

Using (6.58),

$$
\begin{aligned}
\operatorname{Im}f(\mathbf{k},\mathbf{k})
&=-\frac{mL^3}{2\pi\hbar^2}\operatorname{Im}\langle \mathbf{k}|V|\psi^{(+)}\rangle \\
&=\frac{mL^3}{2\hbar^2}\langle \mathbf{k}|T^\dagger\delta(E-H_0)T|\mathbf{k}\rangle \\
&=\frac{mL^3}{2\hbar^2}\sum_{\mathbf{k}'}|\langle \mathbf{k}'|T|\mathbf{k}\rangle|^2\delta_{E,\hbar^2k'^2/2m},
\end{aligned} \tag{6.68}
$$

where $E=\hbar^2k^2/2m$. Converting the sum to an integral yields

$$
\begin{aligned}
\operatorname{Im}f(\mathbf{k},\mathbf{k})
&=\frac{mL^3}{2\hbar^2}\left(\frac{2\pi\hbar^2}{mL^3}\right)^2
\sum_{\mathbf{k}'}|f(\mathbf{k}',\mathbf{k})|^2\delta_{E,\hbar^2k'^2/2m} \\
&\to \frac{2\pi^2\hbar^2}{m(2\pi)^3}\int d^3k'\,|f(\mathbf{k}',\mathbf{k})|^2\delta\!\left(E-\frac{\hbar^2k'^2}{2m}\right) \\
&=\frac{k}{4\pi}\int d\Omega_{\mathbf{k}'}\frac{d\sigma}{d\Omega_{\mathbf{k}'}}
=\frac{k}{4\pi}\sigma_{\mathrm{tot}}.
\end{aligned} \tag{6.69}
$$

This proves the optical theorem.

## 6.3 The Born Approximation

The task is to calculate $f(\mathbf{k}',\mathbf{k})$ for a given potential $V(\mathbf{x})$. This amounts to calculating

$$
\langle \mathbf{k}'|V|\psi^{(+)}\rangle=\langle \mathbf{k}'|T|\mathbf{k}\rangle. \tag{6.70}
$$

Since neither $\langle \mathbf{x}'|\psi^{(+)}\rangle$ nor $T$ is known in closed form, approximations are usually needed. Replacing $\hbar\epsilon$ with $\epsilon$, the expansion is

$$
T=V+V\frac{1}{E-H_0+i\epsilon}V
+V\frac{1}{E-H_0+i\epsilon}V\frac{1}{E-H_0+i\epsilon}V+\cdots. \tag{6.71}
$$

The first-order Born approximation takes $T=V$, or equivalently $|\psi^{(+)}\rangle=|\mathbf{k}\rangle$. Then

$$
f^{(1)}(\mathbf{k}',\mathbf{k})
=-\frac{m}{2\pi\hbar^2}\int d^3x'\,e^{i(\mathbf{k}-\mathbf{k}')\cdot\mathbf{x}'}V(\mathbf{x}'). \tag{6.72}
$$

Thus the first-order amplitude is, up to a constant, the three-dimensional Fourier transform of $V$ with respect to $\mathbf{q}\equiv\mathbf{k}-\mathbf{k}'$.

> [!figure]
> ![[Fig. 6.5.png|center|500]]
> **Figure 6.5.** Scattering through angle $\theta$, where $\mathbf{q}=\mathbf{k}-\mathbf{k}'$.

For a spherically symmetric potential, $f^{(1)}$ depends only on $q=|\mathbf{q}|$. Since $|\mathbf{k}'|=k$ by energy conservation,

$$
q=|\mathbf{k}-\mathbf{k}'|=2k\sin\frac{\theta}{2}. \tag{6.73}
$$

The angular integration in (6.72) gives

$$
\begin{aligned}
f^{(1)}(\theta)
&=-\frac{1}{2}\frac{2m}{\hbar^2}\frac{1}{iq}\int_0^\infty r^2\frac{1}{r}V(r)(e^{iqr}-e^{-iqr})\,dr \\
&=-\frac{2m}{\hbar^2}\frac{1}{q}\int_0^\infty rV(r)\sin(qr)\,dr.
\end{aligned} \tag{6.74}
$$

For a finite square well,

$$
V(r)=\begin{cases}
V_0, & r\le a, \\
0, & r>a,
\end{cases} \tag{6.75}
$$

and

$$
f^{(1)}(\theta)
=-\frac{2m}{\hbar^2}\frac{V_0a^3}{(qa)^2}\left(\frac{\sin qa}{qa}-\cos qa\right). \tag{6.76}
$$

The zeros of this function occur at $qa=4.49,7.73,10.9,\ldots$, and their positions together with (6.73) can be used to determine the well radius $a$.

> [!figure]
> ![[Fig. 6.6.png|center|500]]
> **Figure 6.6.** Data on elastic scattering of protons from the nuclei of four different isotopes of calcium. The angles at which the cross sections show minima, decrease consistently with increasing neutron number. Therefore, the radius of the calcium nucleus increases as more neutrons are added, as one expects. From Ray et al., *Phys. Rev. C*, **23** (1981) 828.

For a Yukawa potential,

$$
V(r)=\frac{V_0e^{-\mu r}}{\mu r}, \tag{6.77}
$$

where $1/\mu$ corresponds to the range of the potential. From (6.74),

$$
f^{(1)}(\theta)=-\left(\frac{2mV_0}{\mu\hbar^2}\right)\frac{1}{q^2+\mu^2}, \tag{6.78}
$$

using

$$
\operatorname{Im}\int_0^\infty e^{-\mu r}e^{iqr}\,dr
=-\operatorname{Im}\left(\frac{1}{-\mu+iq}\right)
=\frac{q}{\mu^2+q^2}. \tag{6.79}
$$

Also,

$$
q^2=4k^2\sin^2\frac{\theta}{2}=2k^2(1-\cos\theta). \tag{6.80}
$$

Thus, in the first Born approximation,

$$
\frac{d\sigma}{d\Omega}=\left(\frac{2mV_0}{\mu\hbar^2}\right)^2\frac{1}{[2k^2(1-\cos\theta)+\mu^2]^2}. \tag{6.81}
$$

As $\mu\to 0$, the Yukawa potential reduces to the Coulomb potential if $V_0/\mu$ is held fixed, for example $V_0/\mu=ZZ'e^2$. The first Born result becomes

$$
\frac{d\sigma}{d\Omega}=\frac{(2m)^2(ZZ'e^2)^2}{\hbar^4}\frac{1}{16k^4\sin^4(\theta/2)}. \tag{6.82}
$$

Identifying $\hbar k$ with $|\mathbf{p}|$ gives the Rutherford cross section,

$$
\frac{d\sigma}{d\Omega}=\frac{1}{16}\left(\frac{ZZ'e^2}{E_{\mathrm{KE}}}\right)^2\frac{1}{\sin^4(\theta/2)}, \tag{6.83}
$$

where $E_{\mathrm{KE}}=|\mathbf{p}|^2/2m$.

For a spherically symmetric potential in the first Born approximation:

1. $d\sigma/d\Omega$, or $f(\theta)$, is a function of $q$ only.
2. $f(\theta)$ is real.
3. $d\sigma/d\Omega$ is independent of the sign of $V$.
4. For small $k$,

$$
f^{(1)}(\theta)=-\frac{1}{4\pi}\frac{2m}{\hbar^2}\int V(r)\,d^3x,
$$

which is independent of $\theta$.

5. $f(\theta)$ is small for large $q$ due to rapid oscillation of the integrand.

To study validity, return to (6.52). The approximation $T\approx V$ means $|\psi^{(+)}\rangle$ may be replaced by $|\mathbf{k}\rangle$, so the scattered term must be much smaller than the incident term. If $V_0$ is a typical potential strength and $a$ its range, then at low energies $ka\ll 1$ the criterion is

$$
\frac{m|V_0|a^2}{\hbar^2}\ll 1. \tag{6.84}
$$

For the Yukawa potential, $a=1/\mu$, giving $m|V_0|/(\hbar^2\mu^2)\ll 1$. If the potential is strong enough to develop a bound state, the Born approximation is likely misleading.

At high energies $ka\gg 1$, the oscillatory factors cannot be replaced by unity, and the condition becomes

$$
\frac{2m}{\hbar^2}\frac{|V_0|a}{k}\ln(ka)\ll 1. \tag{6.85}
$$

Thus the Born approximation tends to improve at higher energies.

### 6.3.1 The Higher-Order Born Approximation

To second order in $V$,

$$
T=V+V\frac{1}{E-H_0+i\epsilon}V.
$$

Thus

$$
f(\mathbf{k}',\mathbf{k})\approx f^{(1)}(\mathbf{k}',\mathbf{k})+f^{(2)}(\mathbf{k}',\mathbf{k}),
$$

where

$$
\begin{aligned}
f^{(2)}
&=-\frac{1}{4\pi}\frac{2m}{\hbar^2}(2\pi)^3
\int d^3x'\int d^3x''\langle \mathbf{k}'|\mathbf{x}'\rangle V(\mathbf{x}')
\left\langle \mathbf{x}'\left|\frac{1}{E-H_0+i\epsilon}\right|\mathbf{x}''\right\rangle
V(\mathbf{x}'')\langle \mathbf{x}''|\mathbf{k}\rangle \\
&=-\frac{1}{4\pi}\frac{2m}{\hbar^2}
\int d^3x'\int d^3x''e^{-i\mathbf{k}'\cdot\mathbf{x}'}V(\mathbf{x}')
\left[\frac{2m}{\hbar^2}G_+(\mathbf{x}',\mathbf{x}'')\right]
V(\mathbf{x}'')e^{i\mathbf{k}\cdot\mathbf{x}''}.
\end{aligned} \tag{6.86}
$$

> [!figure]
> ![[Fig. 6.7.png|center|500]]
> **Figure 6.7.** Physical interpretation of the higher-order Born term $f^{(2)}(\mathbf{k}',\mathbf{k})$.

The incident wave interacts at $\mathbf{x}''$, propagates from $\mathbf{x}''$ to $\mathbf{x}'$ through the Green’s function, interacts again at $\mathbf{x}'$, and finally scatters into direction $\mathbf{k}'$. Higher orders similarly represent multi-step scattering processes.

## 6.4 Phase Shifts and Partial Waves

For a spherically symmetric potential, it is useful to examine states of definite angular momentum. This leads to the method of partial waves. Before treating scattering states, consider free-particle states that are also angular-momentum eigenstates.

### 6.4.1 Free-Particle States

For a free particle, $H_0$ commutes with the momentum operator and also with $L^2$ and $L_z$. Ignoring spin, a simultaneous eigenket of $H_0$, $L^2$, and $L_z$ is denoted $|E,l,m\rangle$ and is often called a spherical-wave state.

The spherical-wave states are normalized as

$$
\langle E',l',m'|E,l,m\rangle=\delta_{ll'}\delta_{mm'}\delta(E-E'). \tag{6.87}
$$

The momentum-space wave function has angular dependence

$$
\langle \mathbf{k}|E,l,m\rangle=g_{lE}(k)Y_l^m(\hat{\mathbf{k}}). \tag{6.88}
$$

For a plane wave along $z$,

$$
L_z|k\hat{\mathbf{z}}\rangle=(xp_y-yp_x)|k_x=0,k_y=0,k_z=k\rangle=0. \tag{6.89}
$$

Therefore

$$
|k\hat{\mathbf{z}}\rangle=\sum_{l'}\int dE'\,|E',l',m'=0\rangle\langle E',l',m'=0|k\hat{\mathbf{z}}\rangle. \tag{6.90}
$$

A general $|\mathbf{k}\rangle$ is obtained by rotation:

$$
|\mathbf{k}\rangle=D(\alpha=\phi,\beta=\theta,\gamma=0)|k\hat{\mathbf{z}}\rangle. \tag{6.91}
$$

Multiplying by $\langle E,l,m|$ gives

$$
\begin{aligned}
\langle E,l,m|\mathbf{k}\rangle
&=\sum_{l'}\int dE'\,
\langle E,l,m|D(\phi,\theta,0)|E',l',m'=0\rangle
\langle E',l',m'=0|k\hat{\mathbf{z}}\rangle \\
&=D^{(l)}_{m0}(\phi,\theta,0)\langle E,l,m=0|k\hat{\mathbf{z}}\rangle.
\end{aligned} \tag{6.92}
$$

Using the relation to spherical harmonics,

$$
\langle \mathbf{k}|E,l,m\rangle=g_{lE}(k)Y_l^m(\hat{\mathbf{k}}). \tag{6.93}
$$

Since

$$
(H_0-E)|E,l,m\rangle=0, \tag{6.94}
$$

and

$$
\langle \mathbf{k}|(H_0-E)=\left(\frac{\hbar^2k^2}{2m}-E\right)\langle \mathbf{k}|, \tag{6.95}
$$

one obtains

$$
\left(\frac{\hbar^2k^2}{2m}-E\right)\langle \mathbf{k}|E,l,m\rangle=0. \tag{6.96}
$$

Thus

$$
g_{lE}(k)=N\delta\!\left(\frac{\hbar^2k^2}{2m}-E\right). \tag{6.97}
$$

Normalization gives

$$
\begin{aligned}
\langle E',l',m'|E,l,m\rangle
&=\int d^3k''\langle E',l',m'|\mathbf{k}''\rangle\langle \mathbf{k}''|E,l,m\rangle \\
&=|N|^2\frac{mk'}{\hbar^2}\delta(E-E')\delta_{ll'}\delta_{mm'}.
\end{aligned} \tag{6.98}
$$

Comparing with (6.87) gives

$$
g_{lE}(k)=\frac{\hbar}{\sqrt{mk}}\delta\!\left(\frac{\hbar^2k^2}{2m}-E\right). \tag{6.99}
$$

Hence

$$
\langle \mathbf{k}|E,l,m\rangle
=\frac{\hbar}{\sqrt{mk}}\delta\!\left(\frac{\hbar^2k^2}{2m}-E\right)Y_l^m(\hat{\mathbf{k}}). \tag{6.100}
$$

The plane wave $|\mathbf{k}\rangle$ may therefore be written as

$$
|\mathbf{k}\rangle
=\sum_l\sum_m\int dE\,|E,l,m\rangle\langle E,l,m|\mathbf{k}\rangle
=\sum_{l=0}^{\infty}\sum_{m=-l}^{l}|E,l,m\rangle_{E=\hbar^2k^2/2m}
\left(\frac{\hbar}{\sqrt{mk}}Y_l^{m*}(\hat{\mathbf{k}})\right). \tag{6.101}
$$

A plane wave contains all possible values of $l$, corresponding semiclassically to all possible impact parameters.

In position space the free spherical wave is

$$
\langle \mathbf{x}|E,l,m\rangle=c_lj_l(kr)Y_l^m(\hat{\mathbf{r}}), \tag{6.102}
$$

where $j_l$ is the spherical Bessel function. Comparing

$$
\begin{aligned}
\langle \mathbf{x}|\mathbf{k}\rangle
&=\frac{e^{i\mathbf{k}\cdot\mathbf{x}}}{(2\pi)^{3/2}} \\
&=\sum_l\sum_m\int dE\,\langle \mathbf{x}|E,l,m\rangle\langle E,l,m|\mathbf{k}\rangle \\
&=\sum_l\frac{2l+1}{4\pi}P_l(\hat{\mathbf{k}}\cdot\hat{\mathbf{r}})\frac{\hbar}{\sqrt{mk}}c_lj_l(kr)
\end{aligned} \tag{6.103}
$$

with

$$
\frac{e^{i\mathbf{k}\cdot\mathbf{x}}}{(2\pi)^{3/2}}
=\frac{1}{(2\pi)^{3/2}}\sum_l(2l+1)i^lj_l(kr)P_l(\hat{\mathbf{k}}\cdot\hat{\mathbf{r}}), \tag{6.104}
$$

and using

$$
j_l(kr)=\frac{1}{2i^l}\int_{-1}^{+1}e^{ikr\cos\theta}P_l(\cos\theta)\,d(\cos\theta), \tag{6.105}
$$

one obtains

$$
c_l=i^l\frac{1}{\hbar}\sqrt{\frac{2mk}{\pi}}. \tag{6.106}
$$

Thus

$$
\langle \mathbf{k}|E,l,m\rangle=\frac{\hbar}{\sqrt{mk}}\delta\!\left(E-\frac{\hbar^2k^2}{2m}\right)Y_l^m(\hat{\mathbf{k}}), \tag{6.107a}
$$

and

$$
\langle \mathbf{x}|E,l,m\rangle=i^l\frac{1}{\hbar}\sqrt{\frac{2mk}{\pi}}\,j_l(kr)Y_l^m(\hat{\mathbf{r}}). \tag{6.107b}
$$

As an application, consider the decay of a parent particle of spin $j$ into two spin-zero particles:

$$
A(\text{spin }j)\to B(\text{spin }0)+C(\text{spin }0).
$$

Angular momentum conservation implies that the final momentum-space wave function has the form (6.107a), with $l$ identified with the parent spin. For example,

$$
{}^{20}\mathrm{Ne}^*\to {}^{16}\mathrm{O}+{}^4\mathrm{He}. \tag{6.108}
$$

If the magnetic quantum number of the parent nucleus is $\pm 1$, the angular distribution of the decay product is proportional to $|Y_1^{\pm 1}(\theta,\phi)|^2=(3/8\pi)\sin^2\theta$. If the magnetic quantum number is $0$, the distribution is $|Y_1^0(\theta,\phi)|^2=(3/4\pi)\cos^2\theta$.

For general spin orientation,

$$
\sum_{m=-l}^{l}w(m)|Y_{l=1}^m|^2. \tag{6.109}
$$

For an unpolarized nucleus, the $w(m)$ are all equal and the distribution is isotropic.

### 6.4.2 Partial-Wave Expansion

Assume the potential is spherically symmetric. Then $T$ commutes with $L^2$ and $\mathbf{L}$ and is a scalar operator. The Wigner-Eckart theorem gives

$$
\langle E',l',m'|T|E,l,m\rangle=T_l(E)\delta_{ll'}\delta_{mm'}. \tag{6.110}
$$

Thus $T$ is diagonal in $l$ and $m$, and its nonzero diagonal element depends on $E$ and $l$ but not on $m$.

Using (6.58),

$$
\begin{aligned}
f(\mathbf{k}',\mathbf{k})
&=-\frac{1}{4\pi}\frac{2m}{\hbar^2}L^3\langle \mathbf{k}'|T|\mathbf{k}\rangle \\
&\to -\frac{1}{4\pi}\frac{2m}{\hbar^2}(2\pi)^3
\sum_{l,m,l',m'}\int dE\int dE'
\langle \mathbf{k}'|E',l',m'\rangle
\langle E',l',m'|T|E,l,m\rangle
\langle E,l,m|\mathbf{k}\rangle \\
&=-\frac{4\pi^2}{k}\sum_l\sum_m T_l(E)\big|_{E=\hbar^2k^2/2m}Y_l^m(\hat{\mathbf{k}}')Y_l^{m*}(\hat{\mathbf{k}}).
\end{aligned} \tag{6.111}
$$

Choose $\mathbf{k}$ along $+z$, so

$$
Y_l^m(\hat{\mathbf{k}})=\sqrt{\frac{2l+1}{4\pi}}\delta_{m0}, \tag{6.112}
$$

and

$$
Y_l^0(\hat{\mathbf{k}}')=\sqrt{\frac{2l+1}{4\pi}}P_l(\cos\theta). \tag{6.113}
$$

Define the partial-wave amplitude

$$
f_l(k)\equiv -\frac{\pi T_l(E)}{k}. \tag{6.114}
$$

Then

$$
f(\mathbf{k}',\mathbf{k})=f(\theta)=\sum_{l=0}^{\infty}(2l+1)f_l(k)P_l(\cos\theta). \tag{6.115}
$$

The large-$r$ behavior of the spherical Bessel function is

$$
j_l(kr)\underset{r\,\mathrm{large}}{\longrightarrow}
\frac{e^{i(kr-l\pi/2)}-e^{-i(kr-l\pi/2)}}{2ikr},
\qquad i^l=e^{i\pi l/2}. \tag{6.116}
$$

Using the plane-wave expansion and (6.115),

$$
\begin{aligned}
\langle \mathbf{x}|\psi^{(+)}\rangle
&\underset{r\,\mathrm{large}}{\longrightarrow}
\frac{1}{(2\pi)^{3/2}}\left[e^{ikz}+f(\theta)\frac{e^{ikr}}{r}\right] \\
&=\frac{1}{(2\pi)^{3/2}}\sum_l(2l+1)\frac{P_l(\cos\theta)}{2ik}
\left([1+2ikf_l(k)]\frac{e^{ikr}}{r}-\frac{e^{-i(kr-l\pi)}}{r}\right).
\end{aligned} \tag{6.117}
$$

The scatterer changes only the coefficient of the outgoing wave:

$$
1\to 1+2ikf_l(k). \tag{6.118}
$$

The incoming wave is unaffected.

### 6.4.3 Unitarity and Phase Shifts

Probability conservation implies, in a time-independent formulation,

$$
\nabla\cdot\mathbf{j}=-\frac{\partial |\psi|^2}{\partial t}=0. \tag{6.119}
$$

By Gauss’s theorem, for a large sphere,

$$
\int_{\text{spherical surface}}\mathbf{j}\cdot d\mathbf{S}=0. \tag{6.120}
$$

The outgoing flux must equal the incoming flux, and by angular-momentum conservation this holds for each partial wave. Define

$$
S_l(k)\equiv 1+2ikf_l(k). \tag{6.121}
$$

Then

$$
|S_l(k)|=1. \tag{6.122}
$$

This is the unitarity relation for the $l$th partial wave. Write

$$
S_l=e^{2i\delta_l}, \tag{6.123}
$$

with real phase shift $\delta_l$. From (6.121),

$$
f_l=\frac{S_l-1}{2ik}. \tag{6.124}
$$

Thus

$$
f_l=\frac{e^{2i\delta_l}-1}{2ik}=\frac{e^{i\delta_l}\sin\delta_l}{k}=\frac{1}{k\cot\delta_l-ik}. \tag{6.125}
$$

The full scattering amplitude is

$$
\begin{aligned}
f(\theta)
&=\sum_{l=0}^{\infty}(2l+1)\left(\frac{e^{2i\delta_l}-1}{2ik}\right)P_l(\cos\theta) \\
&=\frac{1}{k}\sum_{l=0}^{\infty}(2l+1)e^{i\delta_l}\sin\delta_l\,P_l(\cos\theta).
\end{aligned} \tag{6.126}
$$

The total cross section is

$$
\begin{aligned}
\sigma_{\mathrm{tot}}
&=\int |f(\theta)|^2\,d\Omega \\
&=\frac{1}{k^2}\int_0^{2\pi}d\phi\int_{-1}^{+1}d(\cos\theta)
\sum_l\sum_{l'}(2l+1)(2l'+1)e^{i\delta_l}\sin\delta_l e^{-i\delta_{l'}}\sin\delta_{l'}P_lP_{l'} \\
&=\frac{4\pi}{k^2}\sum_l(2l+1)\sin^2\delta_l.
\end{aligned} \tag{6.127}
$$

The optical theorem is checked by noting that

$$
\operatorname{Im}f(\theta=0)
=\sum_l\frac{2l+1}{k}\operatorname{Im}[e^{i\delta_l}\sin\delta_l]P_l(1)
=\sum_l\frac{2l+1}{k}\sin^2\delta_l. \tag{6.128}
$$

An Argand diagram for $kf_l$ follows from

$$
kf_l=\frac{i}{2}+\frac{1}{2}e^{-i\pi/2+2i\delta_l}. \tag{6.129}
$$

> [!figure]
> ![[Fig. 6.8.png|center|500]]
> **Figure 6.8.** Argand diagram for $kf_l$. $OP$ is the magnitude of $kf_l$, while $CO$ and $CP$ are each radii of length $1/2$ on the unitary circle; angle $OCP=2\delta_l$.

For small $\delta_l$,

$$
f_l=\frac{e^{i\delta_l}\sin\delta_l}{k}\simeq \frac{(1+i\delta_l)\delta_l}{k}\simeq \frac{\delta_l}{k}. \tag{6.130}
$$

If $\delta_l$ is near $\pi/2$, $kf_l$ is nearly purely imaginary and $|kf_l|$ is maximal. The maximum partial cross section is

$$
\sigma_{\max}^{(l)}=\frac{4\pi}{k^2}(2l+1). \tag{6.131}
$$

### 6.4.4 Determination of Phase Shifts

Let $V$ vanish for $r>R$. Outside the potential range, the radial wave function is a linear combination of $j_l(kr)$ and $n_l(kr)$, or equivalently of spherical Hankel functions

$$
h_l^{(1)}=j_l+in_l,
\qquad
h_l^{(2)}=j_l-in_l. \tag{6.132}
$$

Their asymptotic behavior is

$$
h_l^{(1)}\underset{r\,\mathrm{large}}{\longrightarrow}\frac{e^{i(kr-l\pi/2)}}{ikr},
\qquad
h_l^{(2)}\underset{r\,\mathrm{large}}{\longrightarrow}-\frac{e^{-i(kr-l\pi/2)}}{ikr}. \tag{6.133}
$$

For $r>R$,

$$
\langle \mathbf{x}|\psi^{(+)}\rangle=\frac{1}{(2\pi)^{3/2}}\sum_l i^l(2l+1)A_l(r)P_l(\cos\theta). \tag{6.134}
$$

The radial function is

$$
A_l=c_l^{(1)}h_l^{(1)}(kr)+c_l^{(2)}h_l^{(2)}(kr). \tag{6.135}
$$

Comparison with the large-$r$ form

$$
\frac{1}{(2\pi)^{3/2}}\sum_l(2l+1)P_l(\cos\theta)
\left[\frac{e^{2i\delta_l}e^{ikr}}{2ikr}-\frac{e^{-i(kr-l\pi)}}{2ikr}\right] \tag{6.136}
$$

requires

$$
c_l^{(1)}=\frac{1}{2}e^{2i\delta_l},
\qquad
c_l^{(2)}=\frac{1}{2}. \tag{6.137}
$$

Thus

$$
A_l(r)=e^{i\delta_l}[\cos\delta_l\,j_l(kr)-\sin\delta_l\,n_l(kr)]. \tag{6.138}
$$

The logarithmic derivative just outside $R$ is

$$
\beta_l\equiv \left(\frac{r}{A_l}\frac{dA_l}{dr}\right)_{r=R}
=kR\left[\frac{j_l'(kR)\cos\delta_l-n_l'(kR)\sin\delta_l}{j_l(kR)\cos\delta_l-n_l(kR)\sin\delta_l}\right], \tag{6.139}
$$

where the prime denotes derivative with respect to $kr$. Solving for the phase shift gives

$$
\tan\delta_l=\frac{kRj_l'(kR)-\beta_lj_l(kR)}{kRn_l'(kR)-\beta_ln_l(kR)}. \tag{6.140}
$$

Inside the potential range, the radial equation is

$$
\frac{d^2u_l}{dr^2}+\left[k^2-\frac{2m}{\hbar^2}V-\frac{l(l+1)}{r^2}\right]u_l=0, \tag{6.141}
$$

where

$$
u_l=rA_l(r), \tag{6.142}
$$

with boundary condition

$$
u_l|_{r=0}=0. \tag{6.143}
$$

The inner solution is integrated up to $r=R$, and continuity of the logarithmic derivative gives

$$
\beta_l|_{\text{inside solution}}=\beta_l|_{\text{outside solution}}. \tag{6.144}
$$

Then (6.140) gives the phase shifts.

### 6.4.5 Hard-Sphere Scattering

For a hard sphere,

$$
V=\begin{cases}
\infty, & r<R, \\
0, & r>R.
\end{cases} \tag{6.145}
$$

The wave function must vanish at $r=R$:

$$
A_l(r)|_{r=R}=0. \tag{6.146}
$$

From (6.138),

$$
j_l(kR)\cos\delta_l-n_l(kR)\sin\delta_l=0, \tag{6.147}
$$

so

$$
\tan\delta_l=\frac{j_l(kR)}{n_l(kR)}. \tag{6.148}
$$

For $l=0$,

$$
\tan\delta_0=\frac{\sin kR/kR}{-\cos kR/kR}=-\tan kR, \tag{6.149}
$$

so $\delta_0=-kR$. With the factor $e^{i\delta_0}$ omitted,


$$
A_{l=0}(r)\propto \frac{\sin kr}{kr}\cos\delta_0+\frac{\cos kr}{kr}\sin\delta_0
=\frac{1}{kr}\sin(kr+\delta_0). \tag{6.150}
$$

> [!figure]
> ![[Fig. 6.9.png|center|500]]
> **Figure 6.9.** Plot of $rA_{l=0}(r)$ versus $r$ (with the $e^{i\delta_0}$ factor removed). The dashed curve for $V=0$ behaves like $\sin kr$, while the solid curve is for S-wave hard-sphere scattering, shifted by $R=-\delta_0/k$ from the case $V=0$.

For $kR\ll 1$, use[^4]

$$
j_l(kr)\simeq \frac{(kr)^l}{(2l+1)!!},
\qquad
n_l(kr)\simeq -\frac{(2l-1)!!}{(kr)^{l+1}}. \tag{6.151}
$$

Then

$$
\tan\delta_l=\frac{-(kR)^{2l+1}}{(2l+1)[(2l-1)!!]^2}. \tag{6.152}
$$

At low energy, only S-wave scattering is important. Since $\delta_0=-kR$,

$$
\frac{d\sigma}{d\Omega}=\frac{\sin^2\delta_0}{k^2}\simeq R^2 \qquad (kR\ll 1). \tag{6.153}
$$

The total cross section is

$$
\sigma_{\mathrm{tot}}=\int\frac{d\sigma}{d\Omega}\,d\Omega=4\pi R^2. \tag{6.154}
$$

This is four times the geometric cross section $\pi R^2$.

## 6.5 Eikonal Approximation

The eikonal approximation applies when $V(\mathbf{x})$ varies little over a wavelength $\bar\lambda$, and when $E\gg |V|$. The semiclassical wave function is

$$
\psi^{(+)}\sim e^{iS(\mathbf{x})/\hbar}. \tag{6.155}
$$

This leads to the Hamilton-Jacobi equation

$$
\frac{(\nabla S)^2}{2m}+V=E=\frac{\hbar^2k^2}{2m}. \tag{6.156}
$$

In the eikonal approximation, the classical trajectory is approximated by a straight line, suitable for small deflection at high energy.[^5]

> [!figure]
> ![[Fig. 6.10.png|center|500]]
> **Figure 6.10.** Schematic diagram of eikonal approximation scattering where the classical straight-line trajectory is along the $z$-direction, $|\mathbf{x}|=r$, and $b=|\mathbf{b}|$ is the impact parameter.

For a straight-line trajectory along $z$,

$$
\frac{S}{\hbar}=\int_{-\infty}^{z}\left[k^2-\frac{2m}{\hbar^2}V\left(\sqrt{b^2+z'^2}\right)\right]^{1/2}dz'+\text{constant}. \tag{6.157}
$$

Choose the additive constant so that

$$
\frac{S}{\hbar}\to kz \qquad \text{as } V\to 0. \tag{6.158}
$$

Then

$$
\begin{aligned}
\frac{S}{\hbar}
&=kz+\int_{-\infty}^{z}\left[\sqrt{k^2-\frac{2m}{\hbar^2}V\left(\sqrt{b^2+z'^2}\right)}-k\right]dz' \\
&\simeq kz-\frac{m}{\hbar^2k}\int_{-\infty}^{z}V\left(\sqrt{b^2+z'^2}\right)dz',
\end{aligned} \tag{6.159}
$$

where, for $E\gg V$,

$$
\sqrt{k^2-\frac{2m}{\hbar^2}V}\simeq k-\frac{mV}{\hbar^2k}.
$$

Thus

$$
\psi^{(+)}(\mathbf{x})=\psi^{(+)}(\mathbf{b}+z\hat{\mathbf{z}})
\simeq \frac{1}{(2\pi)^{3/2}}e^{ikz}
\exp\left[-\frac{im}{\hbar^2k}\int_{-\infty}^{z}V\left(\sqrt{b^2+z'^2}\right)dz'\right]. \tag{6.160}
$$

Although this is not of the exact asymptotic incident-plus-outgoing-spherical-wave form, it can be used in (6.58) to obtain an approximate scattering amplitude:[^6]

$$
\begin{aligned}
f(\mathbf{k}',\mathbf{k})
&=-\frac{1}{4\pi}\frac{2m}{\hbar^2}\int d^3x'\,e^{-i\mathbf{k}'\cdot\mathbf{x}'}V\left(\sqrt{b^2+z'^2}\right)e^{i\mathbf{k}\cdot\mathbf{x}'} \\
&\quad\times \exp\left[-\frac{im}{\hbar^2k}\int_{-\infty}^{z'}V\left(\sqrt{b^2+z''^2}\right)dz''\right].
\end{aligned} \tag{6.161}
$$

For small deflection,

$$
(\mathbf{k}-\mathbf{k}')\cdot\mathbf{x}'=(\mathbf{k}-\mathbf{k}')\cdot(\mathbf{b}+z'\hat{\mathbf{z}})\simeq -\mathbf{k}'\cdot\mathbf{b}. \tag{6.162}
$$

Choosing the scattering plane as the $xz$ plane,

$$
\mathbf{k}'\cdot\mathbf{b}=(k\sin\theta\,\hat{\mathbf{x}}+k\cos\theta\,\hat{\mathbf{z}})\cdot(b\cos\phi_b\,\hat{\mathbf{x}}+b\sin\phi_b\,\hat{\mathbf{y}})
\simeq kb\theta\cos\phi_b. \tag{6.163}
$$

Hence

$$
\begin{aligned}
f(\mathbf{k}',\mathbf{k})
&=-\frac{1}{4\pi}\frac{2m}{\hbar^2}\int_0^\infty b\,db\int_0^{2\pi}d\phi_b\,e^{-ikb\theta\cos\phi_b} \\
&\quad\times \int_{-\infty}^{+\infty}dz\,V
\exp\left[-\frac{im}{\hbar^2k}\int_{-\infty}^{z}V\,dz'\right].
\end{aligned} \tag{6.164}
$$

Use

$$
\int_0^{2\pi}d\phi_b\,e^{-ikb\theta\cos\phi_b}=2\pi J_0(kb\theta), \tag{6.165}
$$

and

$$
\int_{-\infty}^{+\infty}dz\,V\exp\left[-\frac{im}{\hbar^2k}\int_{-\infty}^{z}V\,dz'\right]
=\frac{i\hbar^2k}{m}\exp\left[-\frac{im}{\hbar^2k}\int_{-\infty}^{z}V\,dz'\right]_{z=-\infty}^{z=+\infty}. \tag{6.166}
$$

Finally,

$$
f(\mathbf{k}',\mathbf{k})=-ik\int_0^\infty db\,bJ_0(kb\theta)[e^{2i\Delta(b)}-1], \tag{6.167}
$$

where

$$
\Delta(b)\equiv -\frac{m}{2k\hbar^2}\int_{-\infty}^{+\infty}V\left(\sqrt{b^2+z^2}\right)dz. \tag{6.168}
$$

There is no contribution from $e^{2i\Delta(b)}-1$ if $b$ is larger than the range of $V$.

### 6.5.1 Partial Waves and the Eikonal Approximation

The eikonal approximation is valid at high energies, $\lambda\ll R$, so many partial waves contribute. Semiclassically, $l=bk$ because $l\hbar=bp$ and $p=\hbar k$. Let

$$
l_{\max}=kR. \tag{6.169}
$$

In (6.126), make the substitutions

$$
\sum_l^{l_{\max}=kR}\to k\int db,
\qquad
P_l(\cos\theta)\underset{l\,\mathrm{large},\,\theta\,\mathrm{small}}{\simeq}J_0(l\theta)=J_0(kb\theta),
\qquad
\delta_l\to \Delta(b)|_{b=l/k}. \tag{6.170}
$$

Since $l_{\max}=kR$,

$$
e^{2i\delta_l}-1=e^{2i\Delta(b)}-1=0\qquad (l>l_{\max}). \tag{6.171}
$$

Thus

$$
f(\theta)\to k\int db\frac{2kb}{2ik}(e^{2i\Delta(b)}-1)J_0(kb\theta)
=-ik\int db\,bJ_0(kb\theta)[e^{2i\Delta(b)}-1]. \tag{6.172}
$$

For hard-sphere scattering at high energies, many $l$ values contribute up to $l_{\max}\simeq kR$. The total cross section is

$$
\sigma_{\mathrm{tot}}=\frac{4\pi}{k^2}\sum_{l=0}^{l\simeq kR}(2l+1)\sin^2\delta_l. \tag{6.173}
$$

Using (6.148),

$$
\sin^2\delta_l=\frac{\tan^2\delta_l}{1+\tan^2\delta_l}
=\frac{[j_l(kR)]^2}{[j_l(kR)]^2+[n_l(kR)]^2}
\simeq \sin^2\left(kR-\frac{\pi l}{2}\right). \tag{6.174}
$$

where

$$
j_l(kr)\sim \frac{1}{kr}\sin\left(kr-\frac{l\pi}{2}\right),
\qquad
n_l(kr)\sim -\frac{1}{kr}\cos\left(kr-\frac{l\pi}{2}\right). \tag{6.175}
$$

Averaging $\sin^2\delta_l$ to $1/2$ gives

$$
\sigma_{\mathrm{tot}}=\frac{4\pi}{k^2}(kR)^2\frac{1}{2}=2\pi R^2. \tag{6.176}
$$

This is still not the geometric cross section $\pi R^2$. Split the amplitude into

$$
\begin{aligned}
f(\theta)
&=\frac{1}{2ik}\sum_{l=0}^{kR}(2l+1)e^{2i\delta_l}P_l(\cos\theta)
+\frac{i}{2k}\sum_{l=0}^{kR}(2l+1)P_l(\cos\theta) \\
&=f_{\mathrm{reflection}}+f_{\mathrm{shadow}}.
\end{aligned} \tag{6.177}
$$

The reflected part gives

$$
\int |f_{\mathrm{refl}}|^2d\Omega
=\frac{2\pi}{4k^2}\sum_{l=0}^{l_{\max}}\int_{-1}^{+1}(2l+1)^2[P_l(\cos\theta)]^2d(\cos\theta)
=\frac{\pi l_{\max}^2}{k^2}=\pi R^2. \tag{6.178}
$$

The shadow part is imaginary and coherently forward peaked. Using the small-angle approximation,

$$
f_{\mathrm{shad}}\simeq \frac{i}{2k}\sum(2l+1)J_0(l\theta)
\simeq ik\int_0^R b\,db\,J_0(kb\theta)
=\frac{iRJ_1(kR\theta)}{\theta}. \tag{6.179}
$$

With $\xi=kR\theta$,

$$
\begin{aligned}
\int |f_{\mathrm{shad}}|^2d\Omega
&=2\pi\int_{-1}^{+1}\frac{R^2[J_1(kR\theta)]^2}{\theta^2}d(\cos\theta) \\
&\simeq 2\pi R^2\int_0^\infty\frac{[J_1(\xi)]^2}{\xi}\,d\xi
\simeq \pi R^2.
\end{aligned} \tag{6.180}
$$

The interference vanishes:

$$
\operatorname{Re}(f_{\mathrm{shad}}^*f_{\mathrm{refl}})\simeq 0, \tag{6.181}
$$

because $f_{\mathrm{refl}}$ has an oscillating phase while $f_{\mathrm{shad}}$ is purely imaginary. Therefore

$$
\sigma_{\mathrm{tot}}=\pi R^2+\pi R^2. \tag{6.182}
$$

The second term is called the shadow contribution. It represents the diffraction required to create the shadow behind the scatterer. The optical theorem follows because

$$
\frac{4\pi}{k}\operatorname{Im}f(0)\simeq \frac{4\pi}{k}\operatorname{Im}f_{\mathrm{shad}}(0), \tag{6.183}
$$

and

$$
\frac{4\pi}{k}\operatorname{Im}f_{\mathrm{shad}}(0)
=\frac{4\pi}{k}\operatorname{Im}\left[\frac{i}{2k}\sum_{l=0}^{kR}(2l+1)P_l(1)\right]
=2\pi R^2, \tag{6.184}
$$

which equals $\sigma_{\mathrm{tot}}$.

## 6.6 Low-Energy Scattering and Bound States

At low energies, more precisely when $\lambda=1/k$ is comparable to or larger than the range $R$, higher partial waves are generally unimportant. The effective potential for the $l$th partial wave is

$$
V_{\mathrm{eff}}=V(r)+\frac{\hbar^2}{2m}\frac{l(l+1)}{r^2}. \tag{6.185}
$$

Unless the potential is strong enough to accommodate $l\ne 0$ bound states near $E\simeq 0$, the centrifugal barrier dominates the behavior of higher partial waves. The integral equation for partial waves gives

$$
\frac{e^{i\delta_l}\sin\delta_l}{k}
=-\frac{2m}{\hbar^2}\int_0^\infty j_l(kr)V(r)A_l(r)r^2\,dr. \tag{6.186}
$$

If $A_l(r)$ is close to $j_l(kr)$ and $1/k$ is much larger than the potential range, the right side varies as $k^{2l}$. For small $\delta_l$, the left side varies as $\delta_l/k$, so

$$
\delta_l\sim k^{2l+1} \tag{6.187}
$$

as $k\to 0$. This is threshold behavior. At low energy with a finite-range potential, S-wave scattering is therefore dominant.

### 6.6.1 Rectangular Well or Barrier

Consider S-wave scattering by

$$
V=\begin{cases}
V_0=\text{constant}, & r<R, \\
0, & \text{otherwise},
\end{cases}
\qquad
\begin{cases}
V_0>0, & \text{repulsive}, \\
V_0<0, & \text{attractive}.
\end{cases} \tag{6.188}
$$

The outside wave function behaves like

$$
e^{i\delta_0}[j_0(kr)\cos\delta_0-n_0(kr)\sin\delta_0]
\simeq e^{i\delta_0}\frac{\sin(kr+\delta_0)}{kr}. \tag{6.189}
$$

The inside solution for constant $V_0$ is

$$
u\equiv rA_{l=0}(r)\propto \sin k'r, \tag{6.190}
$$

where

$$
E-V_0=\frac{\hbar^2k'^2}{2m}. \tag{6.191}
$$

If $V_0>E$, the sine should be read as a hyperbolic sine:

$$
u(r)\propto \sinh(\kappa r), \tag{6.190'}
$$

with

$$
\frac{\hbar^2\kappa^2}{2m}=V_0-E. \tag{6.191'}
$$

> [!figure]
> ![[Fig. 6.11.png|center|500]]
> **Figure 6.11.** Plot of $u(r)$ versus $r$. (a) For $V=0$ (dashed line). (b) For $V_0<0$, $\delta_0>0$ with the wave function (solid line) pushed in. (c) For $V_0>0$, $\delta_0<0$ with the wave function (solid line) pulled out.

For attractive $V_0$, increasing $|V_0|$ increases curvature. If the range $[0,R]$ just accommodates one-fourth cycle in the low-energy limit, then $\delta_0=\pi/2$ and the S-wave cross section is maximal. If the well is deeper so that one-half cycle fits in the potential range, $\delta_0=\pi$, and

$$
\sigma_{l=0}=0. \tag{6.192}
$$

This occurs despite strong attraction and leads to nearly perfect transmission when higher partial waves are unimportant. This is the Ramsauer-Townsend effect, observed in electron scattering from rare gases.

### 6.6.2 Zero-Energy Scattering and Bound States

For extremely low energy, $k\simeq 0$, and $r>R$ with $l=0$, the outside radial wave function satisfies

$$
\frac{d^2u}{dr^2}=0. \tag{6.193}
$$

The solution is

$$
u(r)=\text{constant}\,(r-a). \tag{6.194}
$$

This is the infinite-wavelength limit of

$$
\lim_{k\to 0}\sin(kr+\delta_0)=\lim_{k\to 0}\sin\left[k\left(r+\frac{\delta_0}{k}\right)\right]. \tag{6.195}
$$

Also,

$$
\frac{u'}{u}=k\cot\left[k\left(r+\frac{\delta_0}{k}\right)\right]
\underset{k\to 0}{\longrightarrow}\frac{1}{r-a}. \tag{6.196}
$$

Setting $r=0$ gives

$$
\lim_{k\to 0}k\cot\delta_0=-\frac{1}{a}. \tag{6.197}
$$

The quantity $a$ is the scattering length. The zero-energy total cross section is

$$
\sigma_{\mathrm{tot}}=\sigma_{l=0}=4\pi\lim_{k\to 0}\left|\frac{1}{k\cot\delta_0-ik}\right|^2=4\pi a^2. \tag{6.198}
$$

The scattering length $a$ can differ greatly from the range $R$. For a repulsive potential, $a>0$ and is roughly of order $R$. For an attractive potential, the intercept may be on the negative side. With increased attraction, the outside wave function can again cross the $r$ axis on the positive side.

> [!figure]
> ![[Fig. 6.12.png|center|500]]
> **Figure 6.12.** Plot of $u(r)$ versus $r$ for (a) repulsive potential, (b) attractive potential, and (c) deeper attraction. The intercept $a$ of the zero-energy outside wave function with the $r$-axis is shown for each of three cases.

The sign change as attraction increases is related to the development of a bound state. For a weakly bound state near zero energy, the inner wave functions for $E=0^+$ scattering and $E=0^-$ binding are essentially the same because

$$
\frac{\hbar^2k'^2}{2m}=E-V_0\simeq |V_0| \tag{6.199}
$$

with $E$ infinitesimal. Equating logarithmic derivatives gives

$$
\left.\frac{-\kappa e^{-\kappa r}}{e^{-\kappa r}}\right|_{r=R}
=\left.\frac{1}{r-a}\right|_{r=R}. \tag{6.200}
$$

If $R\ll a$,

$$
\kappa\simeq \frac{1}{a}. \tag{6.201}
$$

The binding energy is then

$$
E_{\mathrm{BE}}=-E_{\mathrm{bound\ state}}=\frac{\hbar^2\kappa^2}{2m}\simeq \frac{\hbar^2}{2ma^2}. \tag{6.202}
$$

Thus, a loosely bound-state energy can be inferred from near-zero-energy scattering if $a$ is much larger than $R$.

For the $np$ system, the ${}^3S_1$ state has the deuteron bound state,

$$
E_{\mathrm{BE}}=2.22\ \mathrm{MeV}. \tag{6.203}
$$

The triplet scattering length is

$$
a_{\mathrm{triplet}}=5.4\times 10^{-13}\ \mathrm{cm}. \tag{6.204}
$$

This predicts

$$
\frac{\hbar^2}{2\mu a^2}=\frac{\hbar^2}{m_Na^2}
=m_Nc^2\left(\frac{\hbar}{m_Nca}\right)^2
=(938\ \mathrm{MeV})\left(\frac{2.1\times 10^{-14}\ \mathrm{cm}}{5.4\times 10^{-13}\ \mathrm{cm}}\right)^2
=1.4\ \mathrm{MeV}, \tag{6.205}
$$

where $\mu\simeq m_{n,p}/2$. Better agreement is obtained by keeping the next term in the expansion of $k\cot\delta$:

$$
k\cot\delta_0=-\frac{1}{a}+\frac{1}{2}r_0k^2, \tag{6.206}
$$

where $r_0$ is the effective range.

### 6.6.3 Bound States as Poles of $S_l(k)$

For $l=0$, the large-distance radial wave function is proportional to

$$
S_{l=0}(k)\frac{e^{ikr}}{r}-\frac{e^{-ikr}}{r}. \tag{6.207}
$$

A bound state has large-distance wave function

$$
\frac{e^{-\kappa r}}{r}. \tag{6.208}
$$

A bound state corresponds to imaginary $k=i\kappa$. In the bound-state case, the outgoing wave with imaginary $k$ exists without an incident wave, so $S_{l=0}(k)$ has a pole at $k=i\kappa$.

> [!figure]
> ![[Fig. 6.13.png|center|500]]
> **Figure 6.13.** The complex $k$-plane with bound-state pole at $k=+i\kappa$.

For real positive $k$,

$$
S_{l=0}=e^{2i\delta_0}, \tag{6.209}
$$

with real $\delta_0$. As $k\to 0$, $k\cot\delta_0$ tends to $-1/a$, so

$$
\delta_0\to 0,\ \pm\pi,\ldots . \tag{6.210}
$$

Thus $S_{l=0}\to 1$ as $k\to 0$. The simplest desired properties are

$$
\begin{gathered}
\text{pole at }k=i\kappa,\qquad |S_{l=0}|=1\text{ for real }k>0,\qquad S_{l=0}=1\text{ at }k=0.
\end{gathered} \tag{6.211}
$$

A simple function satisfying these three conditions is

$$
S_{l=0}(k)=-\frac{k+i\kappa}{k-i\kappa}. \tag{6.212}
$$

> [!note]
> **Editor’s Note.** Equation (6.212) is chosen for simplicity rather than as a physically realistic example. For reasonable potentials, not hard spheres, the phase shift vanishes as $k\to\infty$.

Using (6.124),

$$
f_{l=0}=\frac{S_{l=0}-1}{2ik}=\frac{1}{-\kappa-ik}. \tag{6.213}
$$

Comparing with

$$
f_{l=0}=\frac{1}{k\cot\delta_0-ik}, \tag{6.214}
$$

we find

$$
\lim_{k\to 0}k\cot\delta_0=-\frac{1}{a}=-\kappa, \tag{6.215}
$$

which is the relation between bound-state energy and scattering length.

## 6.7 Resonance Scattering

In atomic, nuclear, and particle physics, a given partial-wave scattering cross section may show a pronounced peak. Such behavior is called resonance scattering.

For a finite-range attractive potential, the effective potential for partial wave $l$ is $V(r)$ plus the centrifugal barrier (6.185). The centrifugal term

$$
\frac{\hbar^2}{2m}\frac{l(l+1)}{r^2}
$$

is repulsive. Thus the effective potential can have an attractive well followed by a repulsive barrier.

> [!figure]
> ![[Fig. 6.14.png|center|500]]
> **Figure 6.14.** $V_{\mathrm{eff}}=V(r)+(\hbar^2/2m)[l(l+1)/r^2]$ versus $r$. For $l\ne 0$ the barrier can be due to $(\hbar^2/2m)[l(l+1)/r^2]$; for $l=0$ barrier must be due to $V$ itself.

If the barrier were infinitely high, particles could be trapped inside and form genuine bound states with $E>0$. With a finite barrier, the trapped state has a finite lifetime due to tunneling and is called a quasi-bound state. The phase shift $\delta_l$ rises through $\pi/2$ as the incident energy crosses the quasi-bound-state energy, and the partial cross section reaches its maximum (6.131).

> [!note]
> **Editor’s Note.** Such a sharp rise in the phase shift is, in the time-dependent Schrödinger equation, associated with a delay of the emergence of trapped particles, rather than an unphysical advance, as would be the case for a sharp decrease through $\pi/2$.

For a spherical well with $2mV_0R^2/\hbar^2=5.52$ and $l=3$, numerical results show resonance behavior: the phase shift rises rapidly past $k\simeq 1/R$ and passes through $\pi/2$ at $k=1.41/R$.

For a repulsive delta-shell potential,

$$
\frac{2m}{\hbar^2}V(r)=\gamma\delta(r-R). \tag{6.216}
$$

Resonances are possible for $l=0$ because the shell can trap the particle in $0<r<R$. For $\gamma=\infty$, bound states inside the shell satisfy

$$
kR=\pi,2\pi,\ldots . \tag{6.217}
$$

Outside, the problem reduces to hard-sphere S-wave scattering,

$$
\delta_0=-kR. \tag{6.218}
$$

For finite barrier strength, the phase shift exhibits resonance whenever

$$
E_{\mathrm{incident}}\simeq E_{\mathrm{quasi\text{-}bound\ state}}. \tag{6.219}
$$

The larger $\gamma$ is, the sharper the resonance. Away from resonance, $\delta_0$ resembles the hard-sphere phase shift.

> [!figure]
> ![[Fig. 6.15.png|center|500]]
> **Figure 6.15.** Plots of (a) $\sigma_{l=3}$ versus $k$, where at resonance $\delta_3(k_{\mathrm{res}})=\pi/2$, along with the unitarity limit $4\pi(7)/k^2$ from (6.131); and (b) $\delta_3(k)$ versus $k$. The curves are for a spherical well with $2mV_0R^2/\hbar^2=5.52$.

Near a resonance energy,

$$
E\simeq E_r, \tag{6.220}
$$

assume $\cot\delta_l$ varies smoothly. Expand

$$
\cot\delta_l=\left.\cot\delta_l\right|_{E=E_r}-c(E-E_r)+O[(E-E_r)^2]. \tag{6.221}
$$

Since $\cot\delta_l=0$ at resonance, this gives

$$
f_l(k)=\frac{1}{k\cot\delta_l-ik}
=\frac{1}{k}\frac{1}{[-c(E-E_r)-i]}
=-\frac{\Gamma/2}{k[(E-E_r)+i\Gamma/2]}, \tag{6.222}
$$

where the width $\Gamma$ is defined by

$$
\left.\frac{d(\cot\delta_l)}{dE}\right|_{E=E_r}=-c\equiv -\frac{2}{\Gamma}. \tag{6.223}
$$

If a simple resonance dominates the $l$th partial-wave cross section, the Breit-Wigner form is

$$
\sigma_l=\frac{4\pi}{k^2}(2l+1)\frac{(\Gamma/2)^2}{(E-E_r)^2+\Gamma^2/4}. \tag{6.224}
$$

Thus $\Gamma$ is the full width at half maximum when the resonance is narrow enough that variation in $1/k^2$ can be ignored.

Positive pion-proton elastic scattering gives an example of a relatively isolated resonance.[^7] Pions and protons are strongly interacting particles with sizes of order $1\ \mathrm{fm}=10^{-15}\ \mathrm{m}$, and the force between them is attractive and short-ranged.

> [!figure]
> ![[Fig. 6.16.png|center|500]]
> **Figure 6.16.** Elastic cross section data for the elastic scattering reaction $\pi^+p\to\pi^+p$, as a function of momentum in the center-of-mass. Also plotted are the unitary limits for different possibilities of the dominant partial wave. Compare to the calculated cross section for a hard walled square well in Figure 6.15. There is a clear suggestion that this is a resonance with total angular momentum $j=3/2$.

For particles with spin, replace $2l+1$ by $2j+1$, but also average over initial spin states. Thus

$$
\sigma_{\max}^{(l)}=\frac{4\pi}{k^2}g,
\qquad
g\equiv \frac{2j+1}{(2s_1+1)(2s_2+1)}. \tag{6.225}
$$

The factor $g$ is the statistical factor. For $\pi^+p$ scattering, the pion has spin zero and the proton has spin $1/2$, so $g=(2j+1)/2$. The agreement with the $j=3/2$ unitary limit indicates a spin-$3/2$ resonance, known as the $\Delta(1232)$.

## 6.8 Symmetry Considerations in Scattering

For two identical spinless charged particles interacting through a central potential,[^8] the spatial wave function must be symmetric. The asymptotic wave function has the form

$$
e^{i\mathbf{k}\cdot\mathbf{x}}+e^{-i\mathbf{k}\cdot\mathbf{x}}+[f(\theta)+f(\pi-\theta)]\frac{e^{ikr}}{r}, \tag{6.226}
$$

where $\mathbf{x}=\mathbf{x}_1-\mathbf{x}_2$. Thus

$$
\frac{d\sigma}{d\Omega}=|f(\theta)+f(\pi-\theta)|^2
=|f(\theta)|^2+|f(\pi-\theta)|^2+2\operatorname{Re}[f(\theta)f^*(\pi-\theta)]. \tag{6.227}
$$

The cross section is enhanced by constructive interference near $\theta\simeq \pi/2$.

For spin-$1/2$--spin-$1/2$ scattering with an unpolarized beam and a spin-independent $V$, the spin singlet goes with a symmetric spatial function, while the spin triplet goes with an antisymmetric spatial function. The statistical weights are $1/4$ and $3/4$, so

$$
\begin{aligned}
\frac{d\sigma}{d\Omega}
&=\frac{1}{4}|f(\theta)+f(\pi-\theta)|^2+\frac{3}{4}|f(\theta)-f(\pi-\theta)|^2 \\
&=|f(\theta)|^2+|f(\pi-\theta)|^2-\operatorname{Re}[f(\theta)f^*(\pi-\theta)].
\end{aligned} \tag{6.228}
$$

This gives destructive interference near $\theta\simeq \pi/2$.

For a unitary symmetry operation $U$, if

$$
UH_0U^\dagger=H_0,
\qquad
UVU^\dagger=V, \tag{6.229}
$$

then

$$
UTU^\dagger=T. \tag{6.230}
$$

Define

$$
|\tilde{\mathbf{k}}\rangle\equiv U|\mathbf{k}\rangle,
\qquad
|\tilde{\mathbf{k}}'\rangle\equiv U|\mathbf{k}'\rangle. \tag{6.231}
$$

Then

$$
\langle \tilde{\mathbf{k}}'|T|\tilde{\mathbf{k}}\rangle
=\langle \mathbf{k}'|U^\dagger UTU^\dagger U|\mathbf{k}\rangle
=\langle \mathbf{k}'|T|\mathbf{k}\rangle. \tag{6.232}
$$

For parity,

$$
\pi|\mathbf{k}\rangle=|-\mathbf{k}\rangle,
\qquad
\pi|-\mathbf{k}\rangle=|\mathbf{k}\rangle. \tag{6.233}
$$

Thus parity invariance gives

$$
\langle -\mathbf{k}'|T|-\mathbf{k}\rangle=\langle \mathbf{k}'|T|\mathbf{k}\rangle. \tag{6.234}
$$

> [!figure]
> ![[Fig. 6.17.png|center|500]]
> **Figure 6.17.** (a) Equality of $T$ matrix elements between $\mathbf{k}\to\mathbf{k}'$ and $-\mathbf{k}\to -\mathbf{k}'$. (b) Equality of $T$ matrix elements under rotation.

Rotation invariance implies that $T$ is diagonal in the $|E,l,m\rangle$ basis and that $\langle \mathbf{k}'|T|\mathbf{k}\rangle$ depends only on the relative orientation of $\mathbf{k}$ and $\mathbf{k}'$.

For the antiunitary time-reversal operator $\Theta$,

$$
\Theta T\Theta^{-1}=T^\dagger. \tag{6.235}
$$

This is because antiunitarity changes

$$
\frac{1}{E-H_0+i\epsilon} \quad \text{into} \quad \frac{1}{E-H_0-i\epsilon} \tag{6.236}
$$

in (6.32). For an antiunitary operator,

$$
\langle \beta|\alpha\rangle=\langle \tilde{\alpha}|\tilde{\beta}\rangle, \tag{6.237}
$$

where

$$
|\tilde{\alpha}\rangle\equiv \Theta|\alpha\rangle,
\qquad
|\tilde{\beta}\rangle\equiv \Theta|\beta\rangle. \tag{6.238}
$$

Let

$$
|\alpha\rangle=T|\mathbf{k}\rangle,
\qquad
\langle \beta|=\langle \mathbf{k}'|. \tag{6.239}
$$

Then

$$
|\tilde{\alpha}\rangle=\Theta T|\mathbf{k}\rangle=\Theta T\Theta^{-1}\Theta|\mathbf{k}\rangle=T^\dagger|-\mathbf{k}\rangle,
\qquad
|\tilde{\beta}\rangle=\Theta|\mathbf{k}'\rangle=|-\mathbf{k}'\rangle. \tag{6.240}
$$

Therefore

$$
\langle \mathbf{k}'|T|\mathbf{k}\rangle=\langle -\mathbf{k}|T|-\mathbf{k}'\rangle. \tag{6.241}
$$

Combining time reversal and parity,

$$
\langle \mathbf{k}'|T|\mathbf{k}\rangle
\xrightarrow{\Theta}
\langle -\mathbf{k}|T|-\mathbf{k}'\rangle
\xrightarrow{\pi}
\langle \mathbf{k}|T|\mathbf{k}'\rangle. \tag{6.242}
$$

Thus

$$
f(\mathbf{k},\mathbf{k}')=f(\mathbf{k}',\mathbf{k}), \tag{6.243}
$$

and

$$
\frac{d\sigma}{d\Omega}(\mathbf{k}\to\mathbf{k}')=\frac{d\sigma}{d\Omega}(\mathbf{k}'\to\mathbf{k}). \tag{6.244}
$$

Equation (6.244) is detailed balance.

With spin, using time reversal,

$$
\begin{aligned}
\langle \mathbf{k}',m_s'|T|\mathbf{k},m_s\rangle
&=i^{-2m_s+2m_s'}\langle -\mathbf{k},-m_s|T|-\mathbf{k}',-m_s'\rangle \\
&=i^{-2m_s+2m_s'}\langle \mathbf{k},-m_s|T|\mathbf{k}',-m_s'\rangle.
\end{aligned} \tag{6.245}
$$

For unpolarized initial states and unobserved final polarization, detailed balance becomes

$$
\overline{\frac{d\sigma}{d\Omega}}(\mathbf{k}\to\mathbf{k}')
=\overline{\frac{d\sigma}{d\Omega}}(\mathbf{k}'\to\mathbf{k}), \tag{6.246}
$$

where the bar indicates averaging over initial spin states and summing over final spin states.

## 6.9 Inelastic Electron-Atom Scattering

Consider electron beams interacting with atoms in their ground states. Elastic scattering is

$$
e^-+\text{atom (ground state)}\to e^-+\text{atom (ground state)}. \tag{6.247}
$$

The target atom may also be excited:

$$
e^-+\text{atom (ground state)}\to e^-+\text{atom (excited state)}. \tag{6.248}
$$

In the inelastic case, the final electron has less kinetic energy, the difference being used to excite the target atom.

The initial ket for the electron plus atomic system is

$$
|\mathbf{k},0\rangle, \tag{6.249}
$$

where $\mathbf{k}$ is the incident electron wave vector and $0$ is the atomic ground state. The wave function is

$$
\frac{1}{L^{3/2}}e^{i\mathbf{k}\cdot\mathbf{x}}\psi_0(\mathbf{x}_1,\mathbf{x}_2,\ldots,\mathbf{x}_Z). \tag{6.250}
$$

For a final electron wave vector $\mathbf{k}'$, the final state ket and wave function are

$$
|\mathbf{k}',n\rangle,
\qquad
\frac{1}{L^{3/2}}e^{i\mathbf{k}'\cdot\mathbf{x}}\psi_n(\mathbf{x}_1,\ldots,\mathbf{x}_Z). \tag{6.251}
$$

Here $n=0$ for elastic scattering and $n\ne 0$ for inelastic scattering.

Using time-dependent perturbation theory,

$$
\begin{aligned}
\frac{d\sigma}{d\Omega}(0\to n)
&=\frac{1}{(\hbar k/m_eL^3)}\frac{2\pi}{\hbar}|\langle \mathbf{k}'n|V|\mathbf{k}0\rangle|^2
\left(\frac{L}{2\pi}\right)^3\left(\frac{k'm_e}{\hbar^2}\right) \\
&=\left(\frac{k'}{k}\right)L^6\left|\frac{1}{4\pi}\frac{2m_e}{\hbar^2}\langle \mathbf{k}',n|V|\mathbf{k},0\rangle\right|^2.
\end{aligned} \tag{6.252}
$$

The important difference from elastic scattering is that $k'=|\mathbf{k}'|$ need not equal $k=|\mathbf{k}|$.

The incident electron interacts with the nucleus at the origin and with each atomic electron:

$$
V=-\frac{Ze^2}{r}+\sum_i\frac{e^2}{|\mathbf{x}-\mathbf{x}_i|}. \tag{6.253}
$$

Ignoring exchange between the incident electron and bound atomic electrons for relatively fast incident electrons, the matrix element is

$$
\begin{aligned}
\langle \mathbf{k}'n|V|\mathbf{k}0\rangle
&=\frac{1}{L^3}\int d^3x\,e^{i\mathbf{q}\cdot\mathbf{x}}
\left\langle n\left|-\frac{Ze^2}{r}+\sum_i\frac{e^2}{|\mathbf{x}-\mathbf{x}_i|}\right|0\right\rangle \\
&=\frac{1}{L^3}\int d^3x\,e^{i\mathbf{q}\cdot\mathbf{x}}
\prod_i^Z\int d^3x_i\,\psi_n^*(\mathbf{x}_1,\ldots,\mathbf{x}_Z)
\left[-\frac{Ze^2}{r}+\sum_i\frac{e^2}{|\mathbf{x}-\mathbf{x}_i|}\right]
\psi_0(\mathbf{x}_1,\ldots,\mathbf{x}_Z),
\end{aligned} \tag{6.254}
$$

with $\mathbf{q}\equiv \mathbf{k}-\mathbf{k}'$.

For the nuclear term, the remaining atomic integration gives

$$
\langle n|0\rangle=\delta_{n0}. \tag{6.255}
$$

The Fourier transform of the Coulomb potential follows from the Yukawa transform:

$$
\int d^3x\frac{e^{i\mathbf{q}\cdot\mathbf{x}}}{r}
=\lim_{\mu\to 0}\int d^3x\frac{e^{i\mathbf{q}\cdot\mathbf{x}-\mu r}}{r}
=\frac{4\pi}{q^2}. \tag{6.256}
$$

For the electron term, shift $\mathbf{x}\to \mathbf{x}+\mathbf{x}_i$:

$$
\sum_i\int \frac{d^3x\,e^{i\mathbf{q}\cdot\mathbf{x}}}{|\mathbf{x}-\mathbf{x}_i|}
=\sum_i\int \frac{d^3x\,e^{i\mathbf{q}\cdot(\mathbf{x}+\mathbf{x}_i)}}{|\mathbf{x}|}
=\frac{4\pi}{q^2}\sum_i e^{i\mathbf{q}\cdot\mathbf{x}_i}. \tag{6.257}
$$

This is the Fourier transform of the Coulomb potential multiplied by the Fourier transform of the electron density

$$
\rho_{\mathrm{atom}}(\mathbf{x})=\sum_i\delta^{(3)}(\mathbf{x}-\mathbf{x}_i). \tag{6.258}
$$

Define the form factor for excitation $|0\rangle\to |n\rangle$ by

$$
ZF_n(\mathbf{q})\equiv \left\langle n\left|\sum_i e^{i\mathbf{q}\cdot\mathbf{x}_i}\right|0\right\rangle. \tag{6.259}
$$

For $n=0$, $F_n(\mathbf{q})\to 1$ as $q\to 0$. For $n\ne 0$, $F_n(\mathbf{q})\to 0$ as $q\to 0$ by orthogonality. Then

$$
\int d^3x\,e^{i\mathbf{q}\cdot\mathbf{x}}
\left\langle n\left|-\frac{Ze^2}{r}+\sum_i\frac{e^2}{|\mathbf{x}-\mathbf{x}_i|}\right|0\right\rangle
=\frac{4\pi Ze^2}{q^2}[-\delta_{n0}+F_n(\mathbf{q})]. \tag{6.260}
$$

Thus

$$
\begin{aligned}
\frac{d\sigma}{d\Omega}(0\to n)
&=\left(\frac{k'}{k}\right)\left|\frac{1}{4\pi}\frac{2m_e}{\hbar^2}\frac{4\pi Ze^2}{q^2}[-\delta_{n0}+F_n(\mathbf{q})]\right|^2 \\
&=\frac{4m_e^2}{\hbar^4}\frac{(Ze^2)^2}{q^4}\left(\frac{k'}{k}\right)|-\delta_{n0}+F_n(\mathbf{q})|^2.
\end{aligned} \tag{6.261}
$$

For inelastic scattering, the $\delta_{n0}$ term is absent. With the Bohr radius

$$
a_0=\frac{\hbar^2}{e^2m_e}, \tag{6.262}
$$

write

$$
\frac{d\sigma}{d\Omega}(0\to n)=4Z^2a_0^2\left(\frac{k'}{k}\right)\frac{1}{(qa_0)^4}|F_n(\mathbf{q})|^2. \tag{6.263}
$$

It is often useful to work with $d\sigma/dq$. Since

$$
q^2=|\mathbf{k}-\mathbf{k}'|^2=k^2+k'^2-2kk'\cos\theta, \tag{6.264}
$$

and $dq=-d(\cos\theta)kk'/q$,

$$
\frac{d\sigma}{dq}=\frac{2\pi q}{kk'}\frac{d\sigma}{d\Omega}. \tag{6.265}
$$

The inelastic cross section can be used to discuss stopping power. The energy loss per unit length is

$$
\begin{aligned}
\frac{dE}{dx}
&=N\sum_n(E_n-E_0)\int \frac{d\sigma}{dq}(0\to n)\,dq \\
&=N\sum_n(E_n-E_0)4Z^2a_0^2\int_{q_{\min}}^{q_{\max}}\frac{k'}{k}\frac{1}{q^4}\frac{2\pi q}{kk'}|F_n(\mathbf{q})|^2\,dq \\
&=\frac{8\pi N}{k^2a_0^2}\sum_n(E_n-E_0)
\int_{q_{\min}}^{q_{\max}}\left|\left\langle n\left|\sum_{i=1}^{Z}e^{i\mathbf{q}\cdot\mathbf{x}_i}\right|0\right\rangle\right|^2\frac{dq}{q^3}.
\end{aligned} \tag{6.266}
$$

The resulting quantum-mechanical justification of Bohr’s 1913 stopping-power formula is[^9]

$$
\frac{dE}{dx}=\frac{4\pi NZe^4}{m_ev^2}\ln\left(\frac{2m_ev^2}{I}\right), \tag{6.267}
$$

where $I$ is a semiempirical parameter related to the average excitation energy $\langle E_n-E_0\rangle$. If the projectile charge is $\pm ze$, replace $Ze^4$ by $z^2Ze^4$. The $m_e$ in (6.267) is the electron mass, even for projectiles that are not electrons. Thus energy loss depends on projectile charge and velocity but not projectile mass.

Particle tracks in cloud chambers and nuclear emulsions are nearly straight because (6.263) is sharply peaked at small $q$. Most collisions change the momentum direction only slightly, due to the $q^{-4}$ falloff and the dropoff of $F_n(\mathbf{q})$ at large $q$.

### 6.9.1 Nuclear Form Factor

Atomic excitation is important for $q\sim 10^9\ \mathrm{cm}^{-1}$ to $10^{10}\ \mathrm{cm}^{-1}$. At much larger $q$, of order $1/R_{\mathrm{nucleus}}\sim 10^{12}\ \mathrm{cm}^{-1}$, nuclear structure becomes important. The point-nucleus Coulomb potential must be replaced by

$$
-\frac{Ze^2}{r}\to -Ze^2\int \frac{d^3x'\,N(r')}{|\mathbf{x}-\mathbf{x}'|}, \tag{6.268}
$$

where $N(r)$ is the nuclear charge distribution, normalized by

$$
\int d^3x'\,N(r')=1. \tag{6.269}
$$

A point nucleus corresponds to

$$
N(r')=\delta^{(3)}(\mathbf{r}'). \tag{6.270}
$$

The Fourier transform is

$$
\begin{aligned}
Ze^2\int d^3x\int \frac{d^3x'\,e^{i\mathbf{q}\cdot\mathbf{x}}N(r')}{|\mathbf{x}-\mathbf{x}'|}
&=Ze^2\int d^3x'\,e^{i\mathbf{q}\cdot\mathbf{x}'}N(r')\int d^3x\frac{e^{i\mathbf{q}\cdot\mathbf{x}}}{r} \\
&=Ze^2\frac{4\pi}{q^2}F_{\mathrm{nucleus}}(q),
\end{aligned} \tag{6.271}
$$

where

$$
F_{\mathrm{nucleus}}\equiv \int d^3x\,e^{i\mathbf{q}\cdot\mathbf{x}}N(r). \tag{6.272}
$$

The deviation from the Rutherford formula due to finite nuclear size is

$$
\frac{d\sigma}{d\Omega}=\left(\frac{d\sigma}{d\Omega}\right)_{\mathrm{Rutherford}}|F(q)|^2. \tag{6.273}
$$

For small $q$,

$$
\begin{aligned}
F_{\mathrm{nucleus}}(q)
&=\int d^3x\left[1+i\mathbf{q}\cdot\mathbf{x}-\frac{1}{2}q^2r^2(\hat{\mathbf{q}}\cdot\hat{\mathbf{r}})^2+\cdots\right]N(r) \\
&=1-\frac{1}{6}q^2\langle r^2\rangle_{\mathrm{nucleus}}+\cdots.
\end{aligned} \tag{6.274}
$$

The linear term vanishes by spherical symmetry, and the angular average used in the quadratic term is

$$
\frac{1}{2}\int_{-1}^{+1}d(\cos\theta)\cos^2\theta=\frac{1}{3}. \tag{6.275}
$$

The quantity $\langle r^2\rangle_{\mathrm{nucleus}}$ is the mean square radius of the nucleus. Electron scattering can therefore measure nuclear and proton size, with spin and magnetic moment effects also important for the proton.


## Footnotes

[^1]: Integration over the complex plane arises naturally in many subjects, including scattering theory. For a brief summary of the mathematics, see Appendix F of this book. Complex analysis is also covered in many mathematical physics textbooks, such as Arfken et al. (2013) or Byron and Fuller (1992).

[^2]: For a fuller account of the wave packet approach, see Chapter 3 in Goldberger and Watson (1964), and Chapter 6 in Newton (1982).

[^3]: This relationship is in fact due to Eugene Feenberg, *Phys. Rev.*, **40** (1932) 40. See Newton, *Am. J. Phys.*, **44** (1976) 639 for historical background.

[^4]: $(2n+1)!!\equiv (2n+1)(2n-1)(2n-3)\cdots 1$.

[^5]: Solving (6.156) to determine the classical trajectory would be a forbidding task in general.

[^6]: The text leaves behind the “big box” normalization and writes $f(\mathbf{k}',\mathbf{k})$ assuming continuum normalization.

[^7]: The data are available from the Particle Data Group. The figure plots both elastic and total cross sections on the same plot. There are many more total cross-section data points, but as there are no reactions other than $\pi^+p\to\pi^+p$ in this energy range, the cross sections agree.

[^8]: For background on permutation symmetry with identical particles, see Chapter 7 of the textbook.

[^9]: For a relatively elementary discussion, see Gottfried (1966) and Bethe and Jackiw (1968).
