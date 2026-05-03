# Summary note: reproducing the Table-I value for $0_u^+(6s+6p_{3/2})$, $f+f=4+4$, even $\ell$

This note is meant to parallel the structure of the earlier `body_frame_angular_factor_derivation_remade.md` note, but for the Table-I entry

$$
0_u^+(6s+6p_{3/2}),
\qquad f+f=4+4,
\qquad \text{even }\ell.
$$

The target Table-I value is

$$
A = \frac{35}{1944}.
$$

The result can be reproduced with the same body-frame hyperfine/electronic Clebsch--Gordan machinery used for the $0_g^-$ example, but the final molecular state and the symmetry logic are different.

The important numerical outcome is

$$
B_{q=0}=\frac{7}{24},
\qquad
B_{q=\pm1}=0.
$$

Thus, for this $0_u^+$ case, the perpendicular body-frame channels do not need to be manually discarded. They vanish once the symmetry-adapted $0_u^+$ final state and the boson-allowed entrance sectors are used.

---

## 1. Quick framework

The PA coupling is written as

$$
V_{b,\nu}
=
\frac{\mathcal E_0}{2}
\langle f,\nu|
\boldsymbol\epsilon\cdot\mathbf d
|i,\nu\rangle.
$$

After the radial free-bound overlap and the reduced atomic dipole are factored out,

$$
V_{b,\nu}
=
\frac{\mathcal E_0 d_{\rm at}}{2}
\langle \psi_v|\chi_{E\ell}\rangle
\,a_\nu.
$$

The experimentally quoted angular factor is a line strength:

$$
A(g,e,\boldsymbol\epsilon)
=
\sum_{\rm final}
\overline{|a_\nu|^2}_{\rm initial}.
$$

The amplitude is organized as

$$
a_\nu
=
\sum_{p,q}
(-1)^p\epsilon_p^{\rm lab}
\langle J M\Omega_f|
D^{1*}_{-p,q}
|\ell m_\ell \Omega_i\rangle
\mathcal M_q,
$$

where

$$
\mathcal M_q
=
\left\langle \lambda_f\left|
\frac{d_{1q}^{\rm body}+d_{2q}^{\rm body}}{d_{\rm at}}
\right|\lambda_i\right\rangle.
$$

The calculation therefore naturally splits into three parts:

$$
A
=
\left(\text{rotational/polarization factor}\right)
\left(\text{allowed entrance-state statistical weight}\right)
\left(\text{body-frame internal line strength}\right).
$$

For the present entry, this becomes

$$
A
=
\frac{1}{9}
\times
\frac{45}{81}
\times
\frac{7}{24}
=
\frac{35}{1944}.
$$

Equivalently, if one wants to keep the earlier $0_g^-$ bookkeeping with a separate universal-looking $1/3$ orientation average, one may write

$$
A
=
\frac{1}{3}
\times
\frac{45}{81}
\times
\frac{7}{72}
=
\frac{35}{1944}.
$$

Here

$$
\frac{7}{72}=\frac13\,\frac{7}{24}.
$$

In this note I keep the raw body-frame internal strength as

$$
B_\parallel=B_{q=0}=\frac{7}{24},
$$

and attach the extra factor to the rotational/polarization convention used to reproduce Table I.

---

## 2. Atomic and molecular labels

For cesium on the D2 asymptote,

$$
I=\frac72,
\qquad
j_g=\frac12,
\qquad
j_e=\frac32,
\qquad
f=4.
$$

The entrance channel is two ground-state atoms,

$$
6s_{1/2}+6s_{1/2},
\qquad
f_1=f_2=4.
$$

The excited target channel is

$$
0_u^+(6s+6p_{3/2}).
$$

For an $\Omega=0$ Hund-case-c state made from

$$
j_e=\frac32,
\qquad
j_g=\frac12,
$$

the relevant coupled electronic angular momenta are

$$
J_{12}=1,2.
$$

With the same phase convention used in the earlier $0_g^-$ note,

$$
J_{12}=2,\Omega=0
\quad\leftrightarrow\quad
0^-,
$$

while

$$
J_{12}=1,\Omega=0
\quad\leftrightarrow\quad
0^+.
$$

Therefore, for the present $0_u^+$ entry, the final body-frame electronic state uses

$$
J_{12}=1,
\qquad
\Omega=0.
$$

---

## 3. Bosonic exchange symmetry for the entrance channel

For two identical atoms with equal hyperfine angular momentum $f$, the coupled hyperfine state obeys

$$
P_{12}|f,f;F_tM_F\rangle
=
(-1)^{2f-F_t}|f,f;F_tM_F\rangle.
$$

Here $f=4$, so

$$
(-1)^{2f-F_t}=(-1)^{8-F_t}=(-1)^{F_t}.
$$

For bosonic $^{133}$Cs and even partial waves $\ell$, the total two-atom state must be symmetric under atom exchange. Therefore the entrance hyperfine part must be symmetric, and we keep the even-$F_t$ sectors:

$$
F_t=0,2,4,6,8.
$$

Their total degeneracy is

$$
\sum_{F_t=0,2,4,6,8}(2F_t+1)
=1+5+9+13+17
=45.
$$

The full $f=4+f=4$ product space has

$$
(2f+1)^2=9^2=81
$$

states, so the bosonic entrance-state statistical weight is

$$
W_{\rm boson}=\frac{45}{81}=\frac59.
$$

This part is exactly analogous to the $0_g^-$, $f+f=4+4$, even-$\ell$ example.

---

## 4. Molecular symmetry: building the $0_u^+$ final state

Define the ordered excited-ground basis states

$$
|eg;J_{12}\Omega\rangle
=
\sum_{\omega_e,\omega_g}
\langle j_e\omega_e;j_g\omega_g|J_{12}\Omega\rangle
|6p_{3/2},\omega_e\rangle_1
|6s_{1/2},\omega_g\rangle_2,
$$

and

$$
|ge;J_{12}\Omega\rangle
=
\sum_{\omega_g,\omega_e}
\langle j_g\omega_g;j_e\omega_e|J_{12}\Omega\rangle
|6s_{1/2},\omega_g\rangle_1
|6p_{3/2},\omega_e\rangle_2.
$$

For the present case,

$$
J_{12}=1,
\qquad
\Omega=0.
$$

The Clebsch--Gordan order-exchange identity is

$$
\langle j_g\omega_g;j_e\omega_e|J_{12}\Omega\rangle
=
(-1)^{j_g+j_e-J_{12}}
\langle j_e\omega_e;j_g\omega_g|J_{12}\Omega\rangle.
$$

Since

$$
j_g+j_e-J_{12}
=
\frac12+\frac32-1
=1,
$$

we have the sign

$$
(-1)^{j_g+j_e-J_{12}}=-1.
$$

This sign is important. It means that the same apparent plus sign between the two absorption pathways can represent the ungerade molecular combination in the CG convention used here.

Thus in the Mathematica implementation below, the $0_u^+$ final state is represented by

$$
|\Phi_{0_u^+}\rangle
=
\frac{1}{\sqrt2}
\left(
|eg;J_{12}=1,\Omega=0\rangle
+
|ge;J_{12}=1,\Omega=0\rangle
\right),
$$

with the understanding that the second ket is expanded using the reversed CG order

$$
\langle j_g\omega_g;j_e\omega_e|J_{12}\Omega\rangle.
$$

Changing the phase convention for the $ge$ ket would flip this apparent plus/minus sign, but the physical line strength is unchanged.

---

## 5. Entrance hyperfine expansion

The entrance state is expanded as

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

The one-atom body-frame dipole matrix element is

$$
\frac{
\langle 6p_{3/2},\omega_e|
 d_q^{\rm body}
|6s_{1/2},\omega_g\rangle
}{d_{\rm at}}
=
\langle 1q;\tfrac12\omega_g|\tfrac32\omega_e\rangle.
$$

This one-atom CG coefficient enforces

$$
\omega_e=\omega_g+q.
$$

By itself, this one-atom rule does not know about $g/u$ symmetry or bosonic exchange symmetry. Those enter through the coherent sum of the two absorption pathways and through the allowed $F_t$ sectors.

---

## 6. Internal amplitude for the $0_u^+$ case

For fixed $F_t,M_F,q,m_{I1},m_{I2}$, define

$$
\mathcal M_q(F_t,M_F;m_{I1},m_{I2})
=
\left\langle
\Phi_{0_u^+};m_{I1},m_{I2}
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
\langle \tfrac32\omega_e;\tfrac12\omega_g|1,0\rangle
\delta_{\omega_g,\omega_2}
\langle 1q;\tfrac12\omega_1|\tfrac32\omega_e\rangle
\\
&\qquad+
\sum_{\omega_g,\omega_e}
\langle \tfrac12\omega_g;\tfrac32\omega_e|1,0\rangle
\delta_{\omega_g,\omega_1}
\langle 1q;\tfrac12\omega_2|\tfrac32\omega_e\rangle
\Bigg].
\end{aligned}
$$

The first term is the amplitude where atom 1 absorbs the photon. The second term is the amplitude where atom 2 absorbs the photon. The plus sign is the convention that gives the $0_u^+$ molecular combination when the second term is expanded in the reversed CG order.

The body-frame internal line strength for a chosen set of body-frame dipole components is

$$
B(q\text{-set})
=
\frac{1}{45}
\sum_{F_t=0,2,4,6,8}
\sum_{M_F=-F_t}^{F_t}
\sum_{q\in q\text{-set}}
\sum_{m_{I1},m_{I2}}
\left|
\mathcal M_q(F_t,M_F;m_{I1},m_{I2})
\right|^2.
$$

---

## 7. Why $B_\perp=0$ here

For the present $0_u^+$ state, the direct CG calculation gives

$$
B_\perp
\equiv
B(q=\pm1)
=0,
$$

and

$$
B_\parallel
\equiv
B(q=0)
=\frac{7}{24}.
$$

This is different from the earlier $0_g^-$ case. In the $0_g^-$ case, the raw CG sum did not remove $q=0$; one had to impose a molecular reflection filter by hand before forming the desired line strength. Here, after the $0_u^+$ final state and even-$F_t$ bosonic entrance sectors are built into the amplitude, the $q=\pm1$ contributions cancel algebraically.

A quick way to see the cancellation is the following.

For $q=+1$, the one-atom rule

$$
\omega_e=\omega_g+q
$$

allows only

$$
\omega_g=-\frac12,
\qquad
\omega_e=+\frac12
$$

inside the $\Omega=0$ final state. Therefore the contributing entrance electronic projection is essentially

$$
(\omega_1,\omega_2)=\left(-\frac12,-\frac12\right).
$$

There are two ways to reach the same molecular final state: atom 1 absorbs, or atom 2 absorbs. For the even-$F_t$ boson-allowed entrance sectors, the entrance coefficient is symmetric under atom exchange. But the $J_{12}=1$ reversed-order CG coefficient carries the sign

$$
(-1)^{j_g+j_e-J_{12}}=-1.
$$

Thus the two coherent pathways cancel.

The same argument applies to $q=-1$, where the relevant entrance electronic projection is

$$
(\omega_1,\omega_2)=\left(+\frac12,+\frac12\right).
$$

For $q=0$, the allowed electronic projections are mixed,

$$
(\omega_1,\omega_2)=\left(+\frac12,-\frac12\right)
\quad\text{or}\quad
\left(-\frac12,+\frac12\right),
$$

and the coherent pathway sum no longer cancels. This is why the parallel component survives.

So the statement is not quite that the one-atom CG coefficient alone imposes the good molecular symmetry. Rather:

> Once the molecular final state is constructed as the symmetry-adapted $0_u^+$ state, and once the boson-allowed even-$F_t$ entrance sectors are used, the CG algebra automatically implements the cancellation of the perpendicular channels.

---

## 8. Numerical result and partial checks

The unaveraged $q=0$ contributions from each allowed $F_t$ sector are

$$
\begin{array}{c|c|c}
F_t & \sum_{M_F,m_{I1},m_{I2}}|\mathcal M_{q=0}|^2
& \sum_{M_F,m_{I1},m_{I2},q=\pm1}|\mathcal M_q|^2
\\ \hline
0 & \frac34 & 0 \\
2 & \frac{55}{16} & 0 \\
4 & \frac{39}{8} & 0 \\
6 & \frac{65}{16} & 0 \\
8 & 0 & 0
\end{array}
$$

The total unaveraged parallel strength is

$$
\frac34+\frac{55}{16}+\frac{39}{8}+\frac{65}{16}+0
=
\frac{105}{8}.
$$

Averaging over the 45 boson-allowed entrance hyperfine states gives

$$
B_\parallel
=
\frac{1}{45}\frac{105}{8}
=
\frac{7}{24}.
$$

The perpendicular result is

$$
B_\perp=0.
$$

The final Table-I angular factor is therefore

$$
A
=
R_\parallel\,W_{\rm boson}\,B_\parallel
=
\frac19\times\frac{45}{81}\times\frac{7}{24}
=
\frac{35}{1944}.
$$

---

## 9. Mathematica verification

```mathematica
ClearAll["Global`*"];

(* Cs and D2-line constants *)
Ics = 7/2;
jg = 1/2;
je = 3/2;
f = 4;

(* 0_u^+(6s+6p_3/2): use the J12=1, Omega=0 Hund-c component *)
J12 = 1;
Omega = 0;

(*
   With the CG ordering used below,
   (-1)^(je+jg-J12) = -1 for J12=1.
   Therefore the plus coherent combination of the two terms below
   represents the desired 0_u^+ molecular combination in this convention.
*)
exchangeSign = +1;

(* even ell, f=4+4, bosonic Cs: keep even Ft sectors *)
allowedF = {0, 2, 4, 6, 8};
allowedDeg = Total[2 allowedF + 1];  (* 45 *)
statWeight = FullSimplify[allowedDeg/(2 f + 1)^2];  (* 45/81 = 5/9 *)

mList[j_] := Range[-j, j, 1];

validM[j_, m_] := MemberQ[mList[j], m];

cg[j1_, m1_, j2_, m2_, J_, M_] :=
  If[
    validM[j1, m1] && validM[j2, m2] && validM[J, M] && m1 + m2 == M,
    ClebschGordan[{j1, m1}, {j2, m2}, {J, M}],
    0
  ];

amp[F_, MF_, q_, mI1_, mI2_] :=
  FullSimplify[
    Sum[
      Module[
        {mf1, mf2, ci, me1, me2, term1, term2},

        mf1 = mI1 + mj1;
        mf2 = mI2 + mj2;

        ci =
          cg[f, mf1, f, mf2, F, MF] *
          cg[Ics, mI1, jg, mj1, f, mf1] *
          cg[Ics, mI2, jg, mj2, f, mf2];

        (* atom 1 absorbs: g1 -> e1 *)
        me1 = mj1 + q;
        term1 =
          cg[1, q, jg, mj1, je, me1] *
          cg[je, me1, jg, mj2, J12, Omega] / Sqrt[2];

        (* atom 2 absorbs: g2 -> e2 *)
        me2 = mj2 + q;
        term2 =
          cg[1, q, jg, mj2, je, me2] *
          cg[jg, mj1, je, me2, J12, Omega] / Sqrt[2];

        ci * (term1 + exchangeSign term2)
      ],
      {mj1, mList[jg]},
      {mj2, mList[jg]}
    ]
  ];

bodyRaw[qset_] :=
  FullSimplify[
    (1/allowedDeg) *
      Sum[
        amp[F, MF, q, mI1, mI2]^2,
        {F, allowedF},
        {MF, mList[F]},
        {q, qset},
        {mI1, mList[Ics]},
        {mI2, mList[Ics]}
      ]
  ];

Bq0 = bodyRaw[{0}];
Bperp = bodyRaw[{-1, 1}];
Ball = bodyRaw[{-1, 0, 1}];

rotPol0uParallel = 1/9;
A = FullSimplify[rotPol0uParallel * statWeight * Bq0];

{Bperp, Bq0, Ball, statWeight, A}

(* Expected output:
   {0, 7/24, 7/24, 5/9, 35/1944}
*)
```

Partial $F_t$ checks:

```mathematica
Table[
  {
    F,
    FullSimplify[
      Sum[
        amp[F, MF, 0, mI1, mI2]^2,
        {MF, mList[F]},
        {mI1, mList[Ics]},
        {mI2, mList[Ics]}
      ]
    ],
    FullSimplify[
      Sum[
        amp[F, MF, q, mI1, mI2]^2,
        {MF, mList[F]},
        {q, {-1, 1}},
        {mI1, mList[Ics]},
        {mI2, mList[Ics]}
      ]
    ]
  },
  {F, allowedF}
]

(* Expected output:
   {
     {0, 3/4, 0},
     {2, 55/16, 0},
     {4, 39/8, 0},
     {6, 65/16, 0},
     {8, 0, 0}
   }
*)
```

---

## 10. Relation to the previous $0_g^-$ concern

In the earlier $0_g^-$ calculation, the raw CG machinery gave a nonzero $q=0$ contribution. Therefore, reproducing the Table-I value required excluding $q=0$ on molecular-symmetry grounds.

That is not the same situation as the present $0_u^+$ case. Here the perpendicular channels vanish after the symmetry-adapted $0_u^+$ final state and the bosonic even-$F_t$ entrance sectors are built into the calculation. So this entry is less ambiguous: there is no hidden nonzero perpendicular strength that must be manually discarded.

For the $0_g^-$ case, the most plausible interpretation is:

1. The colliding ground atoms are not just an arbitrary asymptotic $f+f=4+4$ product space once one assigns a body-frame molecular symmetry.
2. At the relevant molecular range, the ground entrance channel is effectively associated with the usual cesium ground molecular potentials

   $$
   X^1\Sigma_g^+,
   \qquad
   a^3\Sigma_u^+.
   $$

3. Both are $\Sigma^+$ states, hence reflection-even.
4. A transition from a reflection-even $0^+$ or $\Sigma^+$ entrance component to a $0^-$ final state uses the perpendicular, reflection-odd body-frame dipole component.
5. Therefore the parallel $q=0$ piece should not be included in that particular $0^+\to0_g^-$ line strength.

This gives a reasonable physical explanation for why the authors' $0_g^-$ value corresponds to dropping $q=0$.

However, it is also fair to say that this assumption is not derivable from the bare asymptotic statement

$$
\ell=0,
\qquad
f+f=4+4
$$

alone. To justify the $q=0$ exclusion, one needs an additional molecular entrance-channel assumption, namely that the scattering state being used in the PA coupling is the reflection-even $\Sigma^+$ molecular component connected to the $X^1\Sigma_g^+$ or $a^3\Sigma_u^+$ ground potentials.

That is why the $0_g^-$ case still feels less automatic than the present $0_u^+$ case.
