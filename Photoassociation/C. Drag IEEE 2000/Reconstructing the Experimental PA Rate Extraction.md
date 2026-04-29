## Purpose

This note gives a cleaned-up, self-consistent interpretation of how the Pillet paper extracts experimental photoassociation (PA) rates from MOT trap-loss data.

The central point is that the paper uses one symbol, $\beta_{\rm PA}$, in a confusing way. In the MOT loading dynamics, the PA loss coefficient is effectively reduced by the finite overlap between the PA laser beam and the trapped atom cloud. But when the authors quote state-specific rates such as

$$
n_{\rm at}\beta_{\rm PA}(0_u^+, 200~{\rm W/cm^2}) = 3.5~{\rm s^{-1}},
$$

they appear to mean the local, de-overlapped, or “bare” PA atom-loss rate at the PA beam intensity, not the smaller MOT-observed rate. 

All my complaints on the nasty grammar / convention quirks in the paper in this section are summarized in Section 9.

Anyway, a clearer notation is therefore:

$$
\beta_{\rm PA}^{\rm bare}
\quad\text{for the local PA loss coefficient,}
$$

and

$$
\beta_{\rm PA}^{\rm eff}
=
\eta\,\beta_{\rm PA}^{\rm bare}
\quad\text{for the overlap-weighted coefficient in the MOT dynamics.}
$$

Here

$$
\eta = \frac{w_0^2}{w_0^2+2\sigma_R^2}
$$

is the geometric overlap factor between the PA laser beam and the cold atom cloud.

---

## 1. MOT loading equation and notation

The paper starts from the dynamic trap equation

$$
\frac{dN_{\rm at}}{dt}
=
L
-
\gamma N_{\rm at}
-
(\beta+\beta_{\rm PA})\int n_{\rm at}^2({\bf r})\,d^3r.
$$

The intended meanings are:

- $L$: MOT loading rate.
- $\gamma$: one-body loss rate, mainly background-gas collisions.
- $\beta$: two-body cold-collision loss coefficient among trapped atoms.
- $\beta_{\rm PA}$: additional loss due to photoassociation.

For the simplified Gaussian-density treatment used in the paper, the non-PA loss rate per atom is compressed into

$$
\Gamma_0
\equiv
\gamma+\beta n_{\rm at}.
$$

This is the inverse of the ordinary MOT loading time without PA:

$$
\Gamma_0 = \frac{1}{\tau}.
$$

Using the paper's measured loading time,

$$
\tau = 735~{\rm ms}=0.735~{\rm s},
$$

one obtains

$$
\Gamma_0
=
\frac{1}{0.735}
=
1.3605~{\rm s^{-1}}.
$$

This point is important: when the paper says that “the latter quantity corresponds to the inverse of the characteristic loading time of the MOT,” the physically correct “latter quantity” is not $\beta_{\rm PA}$. It is

$$
\gamma+\beta n_{\rm at}.
$$

The wording is grammatically misleading.

---

## 2. Why there is a geometric overlap factor

The PA laser does not illuminate the entire MOT uniformly. Fig. 3(c) in the paper shows a narrow PA laser profile crossing a broader trapped atom cloud.

The paper states that $\beta_{\rm PA}$ is weighted by

$$
\eta
=
\frac{w_0^2}{w_0^2+2\sigma_R^2},
$$

where:

- $w_0$ is the PA laser beam waist;
- $\sigma_R$ is the spatial width parameter of the trapped atom cloud.

A useful derivation is as follows. PA is a two-atom loss process, so the relevant density weighting is $n^2({\bf r})$, not simply $n({\bf r})$. For a Gaussian atom cloud, write

$$
n^2({\bf r}) \propto
\exp\left[-\frac{x^2+y^2+z^2}{\sigma_R^2}\right].
$$

For a Gaussian PA beam propagating through the MOT, the transverse intensity profile is

$$
\frac{I_{\rm PA}(x,y)}{I_0}
=
\exp\left[-\frac{2(x^2+y^2)}{w_0^2}\right].
$$

The effective PA rate in the MOT dynamics is the density-squared-weighted average of the local PA rate over the PA laser intensity profile:

$$
\eta
=
\frac{
\int n^2({\bf r})\, I_{\rm PA}(x,y)/I_0\,d^3r
}{
\int n^2({\bf r})\,d^3r
}.
$$

The $z$-integral cancels because the beam is taken to propagate through the cloud and its transverse intensity profile depends only on $x,y$. Thus this is effectively a two-dimensional transverse overlap, not a full three-dimensional volume fraction.

The remaining Gaussian integrals give

$$
\eta
=
\frac{
\int \exp\left[-(x^2+y^2)\left(\sigma_R^{-2}+2w_0^{-2}\right)\right]dxdy
}{
\int \exp\left[-(x^2+y^2)/\sigma_R^2\right]dxdy
}
=
\frac{1}{1+2\sigma_R^2/w_0^2}
=
\frac{w_0^2}{w_0^2+2\sigma_R^2}.
$$

Therefore the MOT dynamics see

$$
\lambda_{\rm PA}^{\rm eff}
=
\eta\,n_{\rm at}\beta_{\rm PA}^{\rm bare},
$$

not directly $n_{\rm at}\beta_{\rm PA}^{\rm bare}$.

---

## 3. Dynamic extraction from Fig. 5(b)

Without PA, the MOT loads with characteristic time

$$
\tau = \frac{1}{\Gamma_0}.
$$

With PA applied, the additional observed loss rate is

$$
\lambda_{\rm PA}^{\rm eff}
=
\eta\, n_{\rm at}\beta_{\rm PA}^{\rm bare}.
$$

The loading time becomes

$$
\tau'
=
\left(\Gamma_0+\lambda_{\rm PA}^{\rm eff}\right)^{-1}
=
\left(\tau^{-1}+\eta n_{\rm at}\beta_{\rm PA}^{\rm bare}\right)^{-1}.
$$

The paper reports approximately

$$
\tau'=585~{\rm ms}=0.585~{\rm s}.
$$

Therefore the observed PA-induced MOT-loss rate is

$$
\lambda_{\rm PA}^{\rm eff}
=
\frac{1}{\tau'}-\frac{1}{\tau}
=
\frac{1}{0.585}-\frac{1}{0.735}
=0.3489~{\rm s^{-1}}.
$$

This is the rate directly visible in the atom-number transient of Fig. 5(b). It is not $3~{\rm s^{-1}}$.

If the authors quote the de-overlapped local rate

$$
n_{\rm at}\beta_{\rm PA}^{\rm bare}
\approx
3.0~{\rm s^{-1}},
$$

then the implied overlap factor is

$$
\eta
=
\frac{0.3489}{3.0}
=
0.116.
$$

If instead one uses the steady-state quoted value

$$
n_{\rm at}\beta_{\rm PA}^{\rm bare}
\approx
3.5~{\rm s^{-1}},
$$

then

$$
\eta
=
\frac{0.3489}{3.5}
=0.0997.
$$

Thus the data imply

$$
\eta\sim 0.10\text{--}0.12.
$$

This is plausible from Fig. 3(c). Solving the overlap equation for the beam/cloud width ratio gives

$$
\frac{w_0}{\sigma_R}
=
\sqrt{\frac{2\eta}{1-\eta}}.
$$

For $\eta=0.10$,

$$
\frac{w_0}{\sigma_R}=0.471.
$$

For $\eta=0.116$,

$$
\frac{w_0}{\sigma_R}=0.512.
$$

So the required PA beam radius is about one-half of the relevant atom-cloud width parameter. In a one-dimensional schematic plot, this can easily look like a narrow PA beam whose apparent width is roughly one-third of the broader trap profile. This generally agrees with what we see in Fig. 3(c).

---

## 4. Consistency check: expected trap loss from the dynamic rate

The steady-state atom-number ratio with PA is

$$
\frac{N_{\rm PA}}{N_0}
\approx
\frac{\Gamma_0}{\Gamma_0+\lambda_{\rm PA}^{\rm eff}}.
$$

Using

$$
\Gamma_0=1.3605~{\rm s^{-1}},
\qquad
\lambda_{\rm PA}^{\rm eff}=0.3489~{\rm s^{-1}},
$$

one finds

$$
\frac{N_{\rm PA}}{N_0}
=
\frac{1.3605}{1.3605+0.3489}
=0.7959.
$$

Therefore the expected trap loss is

$$
1-\frac{N_{\rm PA}}{N_0}
=0.2041,
$$

or about

$$
20\%.
$$

This is consistent with the scale of Fig. 5(b). By contrast, if one incorrectly inserted the local value $3~{\rm s^{-1}}$ directly into the MOT dynamics without the overlap factor, one would get

$$
\frac{N_{\rm PA}}{N_0}
=
\frac{1.3605}{1.3605+3.0}
=0.312,
$$

corresponding to about $69\%$ trap loss, which is incompatible with Fig. 5(b).

Therefore the correct reading is:

$$
\boxed{
\text{Fig. 5(b) measures } \lambda_{\rm PA}^{\rm eff}\approx0.35~{\rm s^{-1}}.
}
$$

But after correcting for geometry,

$$
\boxed{
 n_{\rm at}\beta_{\rm PA}^{\rm bare}
 \approx
 3.0\text{--}3.5~{\rm s^{-1}}.
}
$$

---

## 5. Steady-state extraction from trap-loss fraction

Fig. 5(a) gives the trap-loss fraction versus PA laser power. This can be used to extract a PA rate at each PA laser power, subject to saturation and systematic uncertainties.

The paper's steady-state relation is

$$
\frac{N_{\rm PA}}{N_{\rm at}}
\approx
\frac{\gamma+\beta n_{\rm at}}
{\gamma+(\beta+\beta_{\rm PA})n_{\rm at}}.
$$

In cleaned-up notation, this should be written as

$$
\frac{N_{\rm PA}}{N_0}
\approx
\frac{\Gamma_0}
{\Gamma_0+\lambda_{\rm PA}^{\rm eff}}
=
\frac{\Gamma_0}
{\Gamma_0+\eta n_{\rm at}\beta_{\rm PA}^{\rm bare}}.
$$

Let

$$
r\equiv\frac{N_{\rm PA}}{N_0}
$$

be the remaining atom-number fraction, and let

$$
f\equiv 1-r
$$

be the trap-loss fraction read from Fig. 5(a).

Then

$$
r
=
\frac{\Gamma_0}{\Gamma_0+\lambda_{\rm PA}^{\rm eff}}.
$$

Solving for the observed PA loss rate gives

$$
\lambda_{\rm PA}^{\rm eff}
=
\Gamma_0\left(\frac{1}{r}-1\right).
$$

Equivalently, in terms of the trap-loss fraction $f$,

$$
\lambda_{\rm PA}^{\rm eff}
=
\Gamma_0\frac{f}{1-f}.
$$

The bare, local PA atom-loss rate is then

$$
\boxed{
 n_{\rm at}\beta_{\rm PA}^{\rm bare}
 =
 \frac{1}{\eta}\,
 \Gamma_0\left(\frac{1}{r}-1\right)
}
$$

or

$$
\boxed{
 n_{\rm at}\beta_{\rm PA}^{\rm bare}
 =
 \frac{1}{\eta}\,
 \Gamma_0\frac{f}{1-f}.
}
$$

Since

$$
\Gamma_0 = \frac{1}{\tau}=1.3605~{\rm s^{-1}},
$$

the practical extraction formula is

$$
\boxed{
 n_{\rm at}\beta_{\rm PA}^{\rm bare}
 =
 \frac{1.3605}{\eta}\frac{f}{1-f}
 \quad {\rm s^{-1}}.
}
$$

For $\eta\approx0.10\text{--}0.12$, this becomes approximately

$$
n_{\rm at}\beta_{\rm PA}^{\rm bare}
 \approx
 (11.3\text{--}13.6)\frac{f}{1-f}
 \quad {\rm s^{-1}}.
$$

Example: if the trap-loss fraction is $f=0.20$, then

$$
\lambda_{\rm PA}^{\rm eff}
=
1.3605\frac{0.20}{0.80}
=0.3401~{\rm s^{-1}}.
$$

For $\eta=0.10$,

$$
n_{\rm at}\beta_{\rm PA}^{\rm bare}
=3.40~{\rm s^{-1}}.
$$

For $\eta=0.116$,

$$
n_{\rm at}\beta_{\rm PA}^{\rm bare}
=2.93~{\rm s^{-1}}.
$$

This agrees with the paper's quoted ${0}_u^+$ values near ${3}.0\text{--}3.5~{\rm s^{-1}}$.

---

## 6. How to use Fig. 5(a) to study saturation

For each point in Fig. 5(a):

1. Read the PA laser power $P$.
2. Read the trap-loss percentage ${100f}$.
3. Convert to remaining atom fraction:

$$
r=1-f.
$$

4. Compute the effective MOT-observed PA loss rate:

$$
\lambda_{\rm PA}^{\rm eff}(P)
=
\Gamma_0\frac{f(P)}{1-f(P)}.
$$

5. Correct for geometry:

$$
n_{\rm at}\beta_{\rm PA}^{\rm bare}(P)
=
\frac{\lambda_{\rm PA}^{\rm eff}(P)}{\eta}.
$$

6. Plot either

$$
\lambda_{\rm PA}^{\rm eff}(P)
$$

   or

$$
n_{\rm at}\beta_{\rm PA}^{\rm bare}(P)
$$

   versus PA laser power.

The first quantity is what the MOT directly observes. The second quantity is what should be compared with local PA theory at the stated PA laser intensity.

For low powers, if PA is in the perturbative regime, one expects the bare PA rate to be roughly proportional to PA intensity or power:

$$
n_{\rm at}\beta_{\rm PA}^{\rm bare}(P)\propto P.
$$

At higher powers, Fig. 5(a) indicates saturation, especially for the ${0}_g^-$ state. Therefore high-power points should not be used as simple linear-theory benchmarks.

---

## 7. Benchmark numerical table

Using

$$
\tau=0.735~{\rm s},
\qquad
\tau'=0.585~{\rm s},
$$

gives

$$
\Gamma_0=1.3605~{\rm s^{-1}},
\qquad
\lambda_{\rm PA}^{\rm eff}=0.3489~{\rm s^{-1}}.
$$

| Quantity | Value |
|---|---:|
| MOT loading time without PA, $\tau$ | ${0.735}~{\rm s}$ |
| MOT loading time with PA, $\tau'$ | ${0.585}~{\rm s}$ |
| Background + cold-collision rate, $\Gamma_0=1/\tau$ | ${1}.3605~{\rm s^{-1}}$ |
| Observed PA loss rate, ${1/\tau'-1/\tau}$ | $0.3489~{\rm s^{-1}}$ |
| Observed PA time, $1/\lambda_{\rm PA}^{\rm eff}$ | $2.87~{\rm s}$ |
| Implied $\eta$ if local rate is $3.0~{\rm s^{-1}}$ | $0.116$ |
| Implied $\eta$ if local rate is $3.5~{\rm s^{-1}}$ | $0.0997$ |
| Predicted remaining atom fraction | $0.7959$ |
| Predicted trap-loss fraction | $20.4\%$ |

---

## 8. Benchmark rates for the two states

The paper reports approximately:

| State and condition | Reported local/bare atom-loss rate | Notes |
|---|---:|---|
| $0_u^+$, $200~{\rm W/cm^2}$, steady-state extraction | $3.5\pm0.5~{\rm s^{-1}}$ | Extracted from steady-state trap loss after geometry correction. |
| $0_u^+$, $200~{\rm W/cm^2}$, dynamic extraction | $3.0\pm1.0~{\rm s^{-1}}$ | Consistent with Fig. 5(b) only if this is de-overlapped using $\eta\sim0.1$. |
| $0_g^-$, $55~{\rm W/cm^2}$, steady-state extraction | $2.45\pm0.6~{\rm s^{-1}}$ | Safer low-power comparison point than saturated high-power data. |

Assuming the same approximate geometry factor $\eta\sim0.10\text{--}0.12$, the corresponding directly observed MOT loss rates would be roughly:

| State and condition | Bare rate | Expected observed rate $\eta n_{\rm at}\beta_{\rm PA}^{\rm bare}$ |
|---|---:|---:|
| $0_u^+$, dynamic, $200~{\rm W/cm^2}$ | $3.0~{\rm s^{-1}}$ | $0.30\text{--}0.35~{\rm s^{-1}}$ |
| $0_u^+$, steady-state, $200~{\rm W/cm^2}$ | $3.5~{\rm s^{-1}}$ | $0.35\text{--}0.42~{\rm s^{-1}}$ |
| $0_g^-$, $55~{\rm W/cm^2}$ | $2.45~{\rm s^{-1}}$ | $0.25\text{--}0.29~{\rm s^{-1}}$ |

---

## 9. The paper's confusing conventions and likely typos

The paper is not clean about notation. The following are the main traps.

### 9.1 “The latter quantity” is grammatically misleading

The paper says that knowing $\gamma+\beta n_{\rm at}$, the authors determine $\beta_{\rm PA}$, and then says “the latter quantity” corresponds to the inverse characteristic loading time of the MOT.

Grammatically, “the latter quantity” sounds like $\beta_{\rm PA}$. Physically, that cannot be right. The inverse loading time without PA is

$$
\gamma+\beta n_{\rm at}=\tau^{-1}.
$$

So this sentence should be read as referring to $\gamma+\beta n_{\rm at}$, not $\beta_{\rm PA}$.

### 9.2 The symbol $\beta_{\rm PA}$ is used ambiguously

The paper first says $\beta_{\rm PA}$ is weighted by the geometric factor. That suggests it is an effective MOT-dynamics coefficient.

But later the paper writes state-specific quantities such as

$$
n_{\rm at}\beta_{\rm PA}(0_u^+,200~{\rm W/cm^2})
$$

and compares them with PA theory. In that context, the quantity must be the local/bare, de-overlapped rate at the stated PA laser intensity.

A clean notation would distinguish

$$
\beta_{\rm PA}^{\rm eff}=\eta\beta_{\rm PA}^{\rm bare}.
$$

The paper does not do this explicitly. When they use a single one symbol, $\beta_{\rm PA}$, that means the weighted one; when they use the parenthesized, state-and-intensity-dependent quantity, literally like $\beta_{\rm PA}(0_u^+, 200~{\rm W/cm^2})$, this means the local, de-overlapped rate. 

This is definitely an absurd and confusing convention.

### 9.3 The dynamic equation hides the geometry factor

The paper writes

$$
\tau'=(\tau^{-1}+\tau_{\rm PA}^{-1})^{-1}.
$$

The unambiguous version should be

$$
\tau'
=
\left(
\tau^{-1}+\eta n_{\rm at}\beta_{\rm PA}^{\rm bare}
\right)^{-1}.
$$

Thus

$$
\tau_{\rm PA}^{-1}
=
\eta n_{\rm at}\beta_{\rm PA}^{\rm bare},
$$

not simply $n_{\rm at}\beta_{\rm PA}^{\rm bare}$, unless $\beta_{\rm PA}$ has already been defined as the effective, overlap-weighted coefficient.

### 9.4 The tempting but probably wrong “3 seconds, not 3 inverse seconds” interpretation

From the measured times alone,

$$
\tau_{\rm PA,obs}^{-1}
=
0.3489~{\rm s^{-1}},
$$

so

$$
\tau_{\rm PA,obs}=2.87~{\rm s}.
$$

This is numerically close to ${3}~{\rm s}$. Therefore one might suspect that the authors accidentally wrote ${3}~{\rm s^{-1}}$ when they meant $(3~{\rm s})^{-1}$.

However, this is probably not the intended final interpretation, because later the paper compares experimental rates around ${2.4}$ and ${3.5}~{\rm s^{-1}}$ with theoretical PA rates and says that both lie in the ${1}\text{--}5~{\rm s^{-1}}$ range. That comparison only makes sense if the quoted ${3.0}\text{--}3.5~{\rm s^{-1}}$ values are local, de-overlapped rates.

Thus the better interpretation is:

$$
\tau_{\rm PA,obs}^{-1}\approx0.35~{\rm s^{-1}}
$$

is what the MOT dynamics directly see, while

$$
n_{\rm at}\beta_{\rm PA}^{\rm bare}
\approx3.0\text{--}3.5~{\rm s^{-1}}
$$

is obtained after correcting for $\eta\sim0.1$.

---

## 10. Factor of two: atom-loss rate versus molecule-formation rate

A final convention must be tracked separately from the geometric factor.

A PA event involves two atoms. Depending on the definition, a “PA rate” may mean either:

1. the rate at which atom pairs are photoassociated into excited molecules; or
2. the rate at which atoms are lost from the trap.

If every PA event removes two atoms, then

$$
R_{\rm atom\ loss}=2R_{\rm molecule\ formation}.
$$

The extracted quantity

$$
n_{\rm at}\beta_{\rm PA}^{\rm bare}
$$

is best treated as a local bare atom-loss rate per atom unless the paper or the theory section explicitly redefines it as a molecule-formation rate.

This factor of two is separate from the overlap factor:

$$
\text{geometry:}\quad
\lambda_{\rm obs}=\eta\,R_{\rm atom\ loss}^{\rm bare},
$$

while

$$
\text{molecule/atom convention:}\quad
R_{\rm atom\ loss}^{\rm bare}=2R_{\rm molecule\ formation}^{\rm bare}.
$$

These should not be mixed.

---

## 11. Final clean story

The internally consistent reconstruction is:

1. The normal MOT loading time gives

$$
\Gamma_0=\gamma+\beta n_{\rm at}=1/\tau=1.3605~{\rm s^{-1}}.
$$

2. Fig. 5(b) gives the overlap-weighted PA contribution to the MOT dynamics:

$$
\lambda_{\rm PA}^{\rm eff}=1/\tau'-1/\tau=0.3489~{\rm s^{-1}}.
$$

3. The paper's quoted state-specific PA rates are local/bare rates:

$$
n_{\rm at}\beta_{\rm PA}^{\rm bare}
\approx
3.0\text{--}3.5~{\rm s^{-1}}
\quad
\text{for }0_u^+\text{ at }200~{\rm W/cm^2}.
$$

4. Therefore the implied geometry factor is

$$
\eta
=
\frac{\lambda_{\rm PA}^{\rm eff}}
{n_{\rm at}\beta_{\rm PA}^{\rm bare}}
\approx
0.10\text{--}0.12.
$$

5. This geometry factor is plausible because the PA beam is much narrower than the trapped atom cloud, and the relevant Gaussian overlap is transverse and pair-density-weighted:

$$
\eta=\frac{w_0^2}{w_0^2+2\sigma_R^2}.
$$

6. The predicted steady-state trap-loss fraction is then about $20\%$, consistent with Fig. 5:

$$
1-\frac{N_{\rm PA}}{N_0}
=
1-
\frac{1.3605}{1.3605+0.3489}
=20.4\%.
$$

7. Fig. 5(a) can be used to extract a bare rate at each PA power via

$$
n_{\rm at}\beta_{\rm PA}^{\rm bare}(P)
=
\frac{1}{\eta}\frac{1}{\tau}\frac{f(P)}{1-f(P)},
$$

   where $f(P)$ is the trap-loss fraction read from the plot.

The most important operational rule is therefore:

$$
\boxed{
\text{Compare MOT atom-number dynamics to }
\eta n_{\rm at}\beta_{\rm PA}^{\rm bare}.
}
$$

But

$$
\boxed{
\text{Compare local PA theory to }
 n_{\rm at}\beta_{\rm PA}^{\rm bare},
\text{ with the molecule/atom factor of two handled separately.}
}
$$



