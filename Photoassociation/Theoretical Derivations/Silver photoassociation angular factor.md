# Angular factor for Ag$_2$ photoassociation into $0_g^-(S_{1/2}+P_{3/2})$

This note derives the angular factor for photoassociation of two identical silver atoms, both prepared in the lower ground-state hyperfine manifold $F=1$, into the molecular state correlated with the $S_{1/2}+P_{3/2}$ asymptote and having Hund's-case-(c) symmetry $0_g^-$.

The result is for a homonuclear sample of either isotope, $^{107}\mathrm{Ag}_2$ or $^{109}\mathrm{Ag}_2$, not for mixed-isotope $^{107}\mathrm{Ag}$-$^{109}\mathrm{Ag}$ collisions. The calculation assumes an unpolarized statistical mixture of the initial $m_F$ states and the same line-strength convention used in the Cs-style angular-factor table discussed in the uploaded note.

The final results are

$$
A_{\mathrm{even}\,\ell}=\frac{7}{162}\approx 0.0432
$$

and

$$
A_{\mathrm{odd}\,\ell}=\frac{1}{81}\approx 0.0123.
$$

For ultracold identical bosons, the dominant entrance channel is usually $s$-wave, so the practically relevant result is normally the even-$\ell$ value

$$
A_{s\text{-wave}}=\frac{7}{162}.
$$

---

## 1. Factorization of the angular factor

Following the same convention as the Cs derivation, the line-strength angular factor is written as

$$
A=\frac{1}{3}\,W_{\ell}\,B_{\ell}.
$$

Here:

- $1/3$ is the rotational and polarization factor for linearly polarized light in an isotropic sample.
- $W_{\ell}$ is the exchange-symmetry statistical weight: the fraction of the initial two-atom hyperfine states that have the correct exchange symmetry for a given partial-wave parity.
- $B_{\ell}$ is the body-fixed electronic and hyperfine line strength, averaged over the allowed total hyperfine quantum numbers $F_t$.

Silver has nuclear spin

$$
I=\frac{1}{2}.
$$

The ground electronic angular momentum is

$$
j_g=s=\frac{1}{2}.
$$

The two ground hyperfine manifolds are therefore $F=0$ and $F=1$. We assume both atoms are in the lower $F=1$ manifold. The fact that $F=1$ is lower than $F=0$ for Ag changes which manifold is experimentally populated, but it does not change the Clebsch--Gordan algebra once we specify $F=1$.

---

## 2. Exchange-symmetry factor

For two identical atoms, each with hyperfine angular momentum $F=1$, the two-atom hyperfine states can be coupled to total hyperfine angular momentum

$$
F_t=0,1,2.
$$

The total number of initial two-atom Zeeman product states is

$$
(2F+1)^2=3^2=9.
$$

For two identical spin-$F$ objects, the exchange parity of the coupled hyperfine state $|(F F)F_t M_t\rangle$ is

$$
P_{\mathrm{hf}}=(-1)^{2F-F_t}.
$$

For $F=1$, this becomes

$$
P_{\mathrm{hf}}=(-1)^{2-F_t}=(-1)^{F_t}.
$$

For a gerade $0_g^-$ excited molecular state, using the same convention as the Cs derivation, the electronic exchange part is symmetric. The spatial partial wave contributes

$$
P_{\mathrm{spatial}}=(-1)^\ell.
$$

Since $^{107}\mathrm{Ag}$ and $^{109}\mathrm{Ag}$ atoms are bosons, the total two-atom wavefunction must be symmetric under exchange. Therefore the allowed entrance channels satisfy

$$
(-1)^{F_t}(-1)^\ell=+1.
$$

Equivalently,

$$
F_t+\ell\ \text{is even}.
$$

### Even-$\ell$ channels

For even $\ell$, the allowed values are

$$
F_t=0,2.
$$

The number of allowed hyperfine substates is

$$
(2\cdot 0+1)+(2\cdot 2+1)=1+5=6.
$$

Thus

$$
W_{\mathrm{even}}=\frac{6}{9}=\frac{2}{3}.
$$

### Odd-$\ell$ channels

For odd $\ell$, the allowed value is

$$
F_t=1.
$$

The number of allowed hyperfine substates is

$$
2\cdot 1+1=3.
$$

Thus

$$
W_{\mathrm{odd}}=\frac{3}{9}=\frac{1}{3}.
$$

---

## 3. One-atom hyperfine basis for Ag with $I=1/2$ and $F=1$

Let $|\uparrow_I\rangle$ and $|\downarrow_I\rangle$ denote nuclear-spin projections $m_I=+1/2$ and $m_I=-1/2$. Let $|\uparrow_s\rangle$ and $|\downarrow_s\rangle$ denote electronic-spin projections $m_s=+1/2$ and $m_s=-1/2$.

For $I=1/2$ and $s=1/2$, the $F=1$ hyperfine states are the triplet combinations

$$
|1,+1\rangle=|\uparrow_I\uparrow_s\rangle,
$$

$$
|1,0\rangle=\frac{1}{\sqrt{2}}\left(|\uparrow_I\downarrow_s\rangle+|\downarrow_I\uparrow_s\rangle\right),
$$

$$
|1,-1\rangle=|\downarrow_I\downarrow_s\rangle.
$$

These are the only single-atom hyperfine states that enter the calculation.

---

## 4. Body-fixed electronic transition amplitude

The excited asymptote is $S_{1/2}+P_{3/2}$. In the body-fixed frame, the one-atom dipole matrix element is proportional to the atomic Clebsch--Gordan coefficient

$$
\frac{\langle P_{3/2},m_p|d_q|S_{1/2},m_s\rangle}{D}=\left\langle 1q;\frac{1}{2}m_s\middle|\frac{3}{2}m_p\right\rangle,
$$

where $D$ is the reduced atomic dipole matrix element and

$$
m_p=m_s+q.
$$

For the $0_g^-$, $j_{12}=2$, $\Omega=0$ component, the ordered electronic pair state with atom 1 excited and atom 2 in the ground $S$ state is

$$
|e_{PS}\rangle=\frac{1}{\sqrt{2}}\left(|P_{-1/2}S_{+1/2}\rangle+|P_{+1/2}S_{-1/2}\rangle\right).
$$

The symmetrized gerade molecular state is taken as

$$
|\Phi_{0_g^-}\rangle=\frac{1}{\sqrt{2}}\left(|e_{PS}\rangle+|e_{SP}\rangle\right),
$$

where $|e_{SP}\rangle$ is the exchanged state with atom 2 excited and atom 1 in the ground $S$ state.

The body-fixed perpendicular components $q=\pm 1$ are the ones entering this $0_g^-$ line-strength convention. The relevant atomic Clebsch--Gordan coefficients are

$$
\left\langle 1,+1;\frac{1}{2},-\frac{1}{2}\middle|\frac{3}{2},+\frac{1}{2}\right\rangle=\frac{1}{\sqrt{3}},
$$

and

$$
\left\langle 1,-1;\frac{1}{2},+\frac{1}{2}\middle|\frac{3}{2},-\frac{1}{2}\right\rangle=\frac{1}{\sqrt{3}}.
$$

Because the molecular state contains a factor $1/\sqrt{2}$ from the $j_{12}=2$, $\Omega=0$ projection and a factor $1/\sqrt{2}$ from the gerade symmetrization, each of the two excitation paths carries a molecular projection factor $1/2$.

For an electronic spin component $|\downarrow_s\downarrow_s\rangle$, the $q=+1$ light can excite atom 1 or atom 2. Each path contributes

$$
\frac{1}{2}\cdot\frac{1}{\sqrt{3}}.
$$

Adding the two indistinguishable paths gives

$$
\mathcal{M}_{q=+1}\left(|\downarrow_s\downarrow_s\rangle\right)=\frac{1}{\sqrt{3}}.
$$

Similarly,

$$
\mathcal{M}_{q=-1}\left(|\uparrow_s\uparrow_s\rangle\right)=\frac{1}{\sqrt{3}}.
$$

The anti-parallel electronic spin components $|\uparrow_s\downarrow_s\rangle$ and $|\downarrow_s\uparrow_s\rangle$ do not project onto this $q=\pm1$, $j_{12}=2$, $\Omega=0$ target component. Thus, for the purpose of this body-fixed factor,

$$
|\downarrow_s\downarrow_s\rangle\xrightarrow{q=+1}\frac{1}{\sqrt{3}},
$$

$$
|\uparrow_s\uparrow_s\rangle\xrightarrow{q=-1}\frac{1}{\sqrt{3}},
$$

and all anti-parallel electronic-spin components give zero.

---

## 5. Definition of the channel-resolved body-fixed strength $b_{F_t}$

For a fixed total hyperfine angular momentum $F_t$, define

$$
b_{F_t}=\frac{1}{2F_t+1}\sum_{M_t=-F_t}^{F_t}\sum_{q=\pm1}\sum_{m_{I1},m_{I2}}\left|\mathcal{M}_{F_tM_t}^{(q)}(m_{I1},m_{I2})\right|^2.
$$

Here $\mathcal{M}_{F_tM_t}^{(q)}(m_{I1},m_{I2})$ is the transition amplitude from the initial two-atom hyperfine state $|(FF)F_tM_t\rangle$ into the $0_g^-$ electronic state, leaving the two nuclear spin projections $m_{I1}$ and $m_{I2}$ unchanged.

The only ingredients in this sum are:

1. the two-atom Clebsch--Gordan expansion of $|(1,1)F_tM_t\rangle$ in the product basis $|1,m_1\rangle|1,m_2\rangle$,
2. the one-atom hyperfine expansions from Section 3,
3. the electronic transition rule from Section 4.

---

## 6. Worked examples of the amplitude calculation

### Example 1: $F_t=0$, $M_t=0$, $q=+1$

The two-spin-1 coupled state is

$$
|F_t=0,M_t=0\rangle=\frac{1}{\sqrt{3}}\left(|1,+1\rangle|1,-1\rangle-|1,0\rangle|1,0\rangle+|1,-1\rangle|1,+1\rangle\right).
$$

Only the $|1,0\rangle|1,0\rangle$ term contains a $|\downarrow_s\downarrow_s\rangle$ component. Using

$$
|1,0\rangle=\frac{1}{\sqrt{2}}\left(|\uparrow_I\downarrow_s\rangle+|\downarrow_I\uparrow_s\rangle\right),
$$

the coefficient of $|\uparrow_I\downarrow_s;\uparrow_I\downarrow_s\rangle$ inside $|F_t=0,M_t=0\rangle$ is

$$
-\frac{1}{\sqrt{3}}\cdot\frac{1}{\sqrt{2}}\cdot\frac{1}{\sqrt{2}}=-\frac{1}{2\sqrt{3}}.
$$

The electronic transition amplitude for $|\downarrow_s\downarrow_s\rangle$ with $q=+1$ is $1/\sqrt{3}$, so the total amplitude is

$$
-\frac{1}{2\sqrt{3}}\cdot\frac{1}{\sqrt{3}}=-\frac{1}{6}.
$$

Therefore the contribution to the line strength is

$$
\left|-\frac{1}{6}\right|^2=\frac{1}{36}.
$$

The $q=-1$ contribution is the analogous $|\downarrow_I\uparrow_s;\downarrow_I\uparrow_s\rangle$ contribution and is also $1/36$.

Thus

$$
b_0=\frac{1}{1}\left(\frac{1}{36}+\frac{1}{36}\right)=\frac{1}{18}.
$$

### Example 2: $F_t=1$, $M_t=-1$, $q=+1$

The coupled state is

$$
|F_t=1,M_t=-1\rangle=\frac{1}{\sqrt{2}}\left(|1,-1\rangle|1,0\rangle-|1,0\rangle|1,-1\rangle\right).
$$

The first term has a $|\downarrow_s\downarrow_s\rangle$ component with nuclear spins $|\downarrow_I;\uparrow_I\rangle$ and coefficient

$$
\frac{1}{\sqrt{2}}\cdot\frac{1}{\sqrt{2}}=\frac{1}{2}.
$$

The second term has a $|\downarrow_s\downarrow_s\rangle$ component with nuclear spins $|\uparrow_I;\downarrow_I\rangle$ and coefficient

$$
-\frac{1}{\sqrt{2}}\cdot\frac{1}{\sqrt{2}}=-\frac{1}{2}.
$$

Multiplying each by the electronic transition amplitude $1/\sqrt{3}$ gives the two nuclear-resolved amplitudes

$$
\frac{1}{2\sqrt{3}}
$$

and

$$
-\frac{1}{2\sqrt{3}}.
$$

The contribution for this $M_t$ and $q$ is therefore

$$
\left|\frac{1}{2\sqrt{3}}\right|^2+\left|-\frac{1}{2\sqrt{3}}\right|^2=\frac{1}{12}+\frac{1}{12}=\frac{1}{6}.
$$

The corresponding $F_t=1$, $M_t=+1$, $q=-1$ contribution is also $1/6$, while $M_t=0$ gives zero. Therefore

$$
b_1=\frac{1}{3}\left(\frac{1}{6}+\frac{1}{6}\right)=\frac{1}{9}.
$$

---

## 7. Complete table for $b_{F_t}$

The following table lists

$$
\mathcal{S}_{F_tM_t}^{(q)}=\sum_{m_{I1},m_{I2}}\left|\mathcal{M}_{F_tM_t}^{(q)}(m_{I1},m_{I2})\right|^2.
$$

| $F_t$ | $M_t$ | $\mathcal{S}^{(-1)}$ | $\mathcal{S}^{(+1)}$ |
|---:|---:|---:|---:|
| $0$ | $0$ | $1/36$ | $1/36$ |
| $1$ | $-1$ | $0$ | $1/6$ |
| $1$ | $0$ | $0$ | $0$ |
| $1$ | $+1$ | $1/6$ | $0$ |
| $2$ | $-2$ | $0$ | $1/3$ |
| $2$ | $-1$ | $0$ | $1/6$ |
| $2$ | $0$ | $1/18$ | $1/18$ |
| $2$ | $+1$ | $1/6$ | $0$ |
| $2$ | $+2$ | $1/3$ | $0$ |

Averaging over $M_t$ gives

$$
b_0=\frac{1}{18},
$$

$$
b_1=\frac{1}{9},
$$

and

$$
b_2=\frac{1}{5}\left(\frac{1}{3}+\frac{1}{6}+\frac{1}{18}+\frac{1}{18}+\frac{1}{6}+\frac{1}{3}\right)=\frac{2}{9}.
$$

---

## 8. Body-fixed factors for even and odd partial waves

The body-fixed factor $B_{\ell}$ is the degeneracy-weighted average of $b_{F_t}$ over the $F_t$ values allowed by exchange symmetry.

### Even-$\ell$

For even $\ell$, the allowed values are $F_t=0,2$. Therefore

$$
B_{\mathrm{even}}=\frac{(2\cdot0+1)b_0+(2\cdot2+1)b_2}{(2\cdot0+1)+(2\cdot2+1)}.
$$

Substituting $b_0=1/18$ and $b_2=2/9$ gives

$$
B_{\mathrm{even}}=\frac{1\cdot\frac{1}{18}+5\cdot\frac{2}{9}}{1+5}.
$$

Thus

$$
B_{\mathrm{even}}=\frac{\frac{1}{18}+\frac{10}{9}}{6}=\frac{\frac{21}{18}}{6}=\frac{7}{36}.
$$

### Odd-$\ell$

For odd $\ell$, the only allowed value is $F_t=1$. Therefore

$$
B_{\mathrm{odd}}=b_1=\frac{1}{9}.
$$

These are the body-fixed factors that were quoted earlier:

$$
B_{\mathrm{Ag,even}}=\frac{7}{36},
$$

and

$$
B_{\mathrm{Ag,odd}}=\frac{1}{9}.
$$

---

## 9. Final angular factors

Now combine the rotational/polarization factor, the exchange-symmetry factor, and the body-fixed factor.

### Even-$\ell$ result

For even $\ell$,

$$
A_{\mathrm{even}}=\frac{1}{3}\,W_{\mathrm{even}}\,B_{\mathrm{even}}.
$$

Using

$$
W_{\mathrm{even}}=\frac{2}{3}
$$

and

$$
B_{\mathrm{even}}=\frac{7}{36},
$$

we get

$$
A_{\mathrm{even}}=\frac{1}{3}\cdot\frac{2}{3}\cdot\frac{7}{36}=\frac{14}{324}=\frac{7}{162}.
$$

Numerically,

$$
A_{\mathrm{even}}\approx 0.0432.
$$

### Odd-$\ell$ result

For odd $\ell$,

$$
A_{\mathrm{odd}}=\frac{1}{3}\,W_{\mathrm{odd}}\,B_{\mathrm{odd}}.
$$

Using

$$
W_{\mathrm{odd}}=\frac{1}{3}
$$

and

$$
B_{\mathrm{odd}}=\frac{1}{9},
$$

we get

$$
A_{\mathrm{odd}}=\frac{1}{3}\cdot\frac{1}{3}\cdot\frac{1}{9}=\frac{1}{81}.
$$

Numerically,

$$
A_{\mathrm{odd}}\approx 0.0123.
$$

---

## 10. Interpretation

For ultracold photoassociation, the lowest collision channel is usually $s$-wave, so $\ell=0$ and the even-$\ell$ value is the relevant one:

$$
A_{\mathrm{Ag}}(F=1+F=1\rightarrow 0_g^-,\ell=0)=\frac{7}{162}\approx 0.0432.
$$

This is slightly larger than the corresponding Cs example discussed in the uploaded note, where the $F=4+F=4$, even-$\ell$ value for $0_g^-(S_{1/2}+P_{3/2})$ is

$$
A_{\mathrm{Cs}}=\frac{125}{3888}\approx 0.0322.
$$

The larger Ag value is mostly due to the much smaller hyperfine Hilbert space. For Ag with $F=1$, there are only $9$ initial two-atom Zeeman product states, while for Cs with $F=4$ there are $81$. The angular momentum projection and exchange-symmetry penalties are still significant, but they are somewhat less severe in this specific Ag case.

---

## 11. Caveats

This result assumes:

1. A homonuclear sample, either pure $^{107}\mathrm{Ag}$ or pure $^{109}\mathrm{Ag}$.
2. Both atoms initially in $F=1$.
3. An unpolarized statistical mixture over initial $m_F$ states.
4. Linear polarization and the same isotropic rotational/polarization convention that gives the prefactor $1/3$.
5. The $0_g^-(S_{1/2}+P_{3/2})$ line-strength convention where the body-fixed $q=\pm1$ components are used.

If the atoms are prepared in a specific Zeeman state, such as $|F=1,m_F=+1\rangle$, or if the PA light is circularly polarized, then the averaged factor $A=7/162$ should be replaced by the corresponding channel-resolved Clebsch--Gordan factor.
