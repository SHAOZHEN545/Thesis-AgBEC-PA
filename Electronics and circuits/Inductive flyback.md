This note develops, from first principles, what happens when a switch interrupts the current in an inductive load. The physical setting is a magnetic coil driven from a DC supply through an IGBT, which is exactly the topology used to switch the Feshbach and MOT coils. The questions answered here are: how large is the voltage that appears when the switch opens, which terminal of the switch it appears on, and why the naive Lenz-law argument is so easy to get backwards. Protection networks (freewheeling diodes, varistors, RC and RCD snubbers) are deliberately left out; they are the subject of a companion note, and they cannot be designed sensibly until the unprotected problem is understood.

Consider such a circuit:

![[Simple_IGBT_Inductor.svg|530]]

A DC supply drives a current down the top rail, through the inductor $L$, into the collector $C$ of the IGBT $Q1$, out of its emitter $E$, and back along the bottom rail to the supply. Applying a high voltage on the gate drive turns the IGBT on, and current flows around the loop. Dropping the gate voltage to zero turns it off. Everything in this note is about that second event.

Throughout, take the supply negative terminal as the ground reference, and let

- $V_s$ = supply rail voltage (the compliance voltage of the coil supply),
- $I_0$ = steady-state coil current before turn-off,
- $A$ = the node at the *top* of the inductor (the positive rail),
- $B$ = the node at the *bottom* of the inductor, which is also the collector node; its potential is $v_C$,
- $v_{CE} = v_C - 0 = v_C$, the collector--emitter voltage that the IGBT must withstand.

The conventional current flows $A \to B$ through the inductor.

---

## 1. Where the minus sign really lives

Almost all of the confusion in this subject comes from the fact that two different, both-correct, expressions are in circulation:

$$
\mathcal{E} = -L\frac{dI}{dt}
\qquad\text{versus}\qquad
v_L = +L\frac{dI}{dt}.
$$

These are not contradictory; they refer to different quantities. Keeping them apart is the whole game.

**The first is Faraday's law.** The flux linked by the coil is $\Phi = LI$, with the sign of $\Phi$ fixed by the right-hand rule applied to the positive current direction. Faraday's law states

$$
\mathcal{E} \;=\; \oint \vec{E}\cdot d\vec{l} \;=\; -\frac{d\Phi}{dt} \;=\; -L\frac{dI}{dt},
$$

where the line integral is taken *around the coil in the direction of positive current*. So $\mathcal{E}$ is the **electromotive force**: the net "push" per unit charge that the coil supplies to the circuit, measured along the current direction. It is a source-like quantity, on the same footing as a battery's EMF.

**The second is the circuit-theory terminal voltage.** In the passive sign convention we define the voltage *drop* across the element from the terminal the current enters to the terminal it leaves,

$$
v_L \;\equiv\; v_A - v_B .
$$

A drop measured *along* the current is minus the push measured along the current, exactly as for a battery traversed from $-$ to $+$. Hence

$$
v_L = -\mathcal{E} = +L\frac{dI}{dt}.
$$

**Only $v_L$ goes into Kirchhoff's voltage law.** If you write KVL and also insert $-L\,dI/dt$, you have double-counted the sign, and you will conclude that the collector goes *negative* — the classic wrong answer. The rule to internalise:

> $\mathcal{E} = -L\,dI/dt$ is the sentence Lenz's law is speaking. $v_L = +L\,dI/dt$ is the sentence KVL is speaking. Never mix the two in one equation.

For completeness, with a small series resistance $R$ representing the coil winding and leads, the full terminal relation of the physical coil is

$$
v_A - v_B \;=\; L\frac{dI}{dt} + IR .
$$

---

## 2. The ON state

With the gate driven high, the IGBT is in saturation and behaves as a small voltage drop $V_{CE,\text{sat}}$, typically $1.5$--$3$ V. In steady state $dI/dt = 0$, so the inductor is just a piece of wire with resistance $R$:

$$
v_A - v_B = I_0 R,
\qquad
v_C = V_{CE,\text{sat}},
\qquad
I_0 = \frac{V_s - V_{CE,\text{sat}}}{R}
$$

(or, more realistically for a coil supply, $I_0$ is set by the current regulator and $V_s$ adjusts itself to whatever compliance is needed).

Two facts about this state matter for what follows.

**The inductor is a load.** $v_A - v_B = I_0 R > 0$: its top terminal is the $+$ terminal, current enters at $+$, and it absorbs power $I_0^2 R$, dissipated in the winding.

**The inductor is holding stored energy,**

$$
W = \tfrac{1}{2} L I_0^2 ,
$$

which is *not* dissipated and has nowhere to go as long as the current keeps circulating. This number is the single most important quantity in the whole problem. For a representative coil bank,

$$
L = 500\ \mu\text{H},\qquad I_0 = 100\ \text{A}
\;\;\Longrightarrow\;\;
W = \tfrac12 (5\times10^{-4})(10^4) = 2.5\ \text{J}.
$$

Turning the switch off does not delete this energy. It only forces the circuit to find somewhere to put it, in a very short time. Everything below is a consequence of that one sentence.

---

## 3. Lenz's law, done carefully

Lenz's law says that the induced EMF opposes *the change in flux that produced it*. The universal trap is to hear "opposes" and picture the coil opposing the *current*. It does not. It opposes the *change*. That distinction is the entire answer.

![[Flyback_Polarity.svg|660]]

### 3.1 The chain of reasoning

**(i) Flux tracks current.** $\Phi = LI$. Cutting the current means collapsing the flux.

**(ii) The change is a decrease.** At turn-off, $I$ falls from $I_0$ toward zero, so

$$
\frac{dI}{dt} < 0,\qquad \frac{d\Phi}{dt} < 0 .
$$

**(iii) Lenz: the coil fights the decrease.** Opposing a *decrease* of flux means acting to *sustain* the flux, which means acting to **keep the current flowing in the same direction it was already flowing**. The induced EMF therefore points *along* the original current, not against it. Formally, $\mathcal{E} = -L\,dI/dt > 0$ when $dI/dt<0$: the EMF is positive in the sense of the positive current direction.

**(iv) Sustaining a current means becoming a source.** An element that *pushes* current out of one of its terminals into the rest of the circuit is behaving as a source, and the terminal it pushes out of is by definition its $+$ terminal. Current leaves the inductor at node $B$. Therefore **$B$ becomes the positive terminal**.

**(v) $B$ is the collector.** Hence the collector node is driven positive.

So the coil does not reverse its current; it reverses its *role*. It stops being a load and becomes a source, while the current direction is untouched. And an element that keeps its current direction while flipping from load to source must flip its voltage polarity. That is the whole content of the polarity reversal, and it is worth keeping in the memorable form:

> **The current direction is continuous. The voltage polarity is what jumps.**

### 3.2 The same result from KVL

Nothing above needed the magnitude. Getting it is one line. Around the loop, with the coil relation from §1,

$$
V_s = \left(L\frac{dI}{dt} + IR\right) + v_C
\qquad\Longrightarrow\qquad
v_C = V_s - IR - L\frac{dI}{dt}.
$$

During turn-off $dI/dt<0$, so $-L\,dI/dt = +L|dI/dt|$ and

$$
\boxed{\;v_{CE} = v_C = V_s - IR + L\left|\frac{dI}{dt}\right|\;}
$$

The induced term **adds to** the supply rail. The coil behaves as a battery of EMF $L|dI/dt|$ placed in series with $V_s$ and pointing the *same* way, so the two push the collector node up together. This is why the answer is $V_s + L|dI/dt|$ and never $L|dI/dt| - V_s$.

### 3.3 The cross-check that never lies: follow the current

If the Lenz argument ever feels slippery, use this instead. It is equivalent, and much harder to get backwards.

Inductor current is a *continuous state variable*: $I(0^-) = I(0^+) = I_0$, because a discontinuity in $I$ would require infinite $dI/dt$ and hence infinite voltage. So one nanosecond after the gate goes low, $100$ A is still flowing down into node $B$ — and the IGBT has stopped accepting it.

The current must go somewhere. The only thing left at node $B$ is the parasitic capacitance $C_p$ to ground: the IGBT's output capacitance $C_{oes}$, the coil's self-capacitance, and the wiring. So the coil charges it:

$$
\frac{dv_C}{dt} = \frac{I_0}{C_p} \;>\; 0 .
$$

Positive, immediately, with no sign conventions involved: **the collector rises**. With $I_0 = 100$ A and $C_p \sim 1$ nF,

$$
\frac{dv_C}{dt} = \frac{100\ \text{A}}{1\ \text{nF}} = 10^{11}\ \text{V/s} = 100\ \text{V/ns},
$$

so a $1200$ V rating is reached about $12$ ns after the gate goes low. The two arguments agree, as they must.

---

## 4. The switch-limited estimate

Now the magnitude. Suppose the IGBT turns off in a finite fall time $t_f$ and, for the moment, that the current falls linearly to zero over that interval:

$$
\left|\frac{dI}{dt}\right| \simeq \frac{I_0}{t_f}
\qquad\Longrightarrow\qquad
v_{CE}^{\text{peak}} \simeq V_s + \frac{L I_0}{t_f}.
$$

The product $L I_0$ is fixed by the coil and the operating point — it is the total flux linkage, $\Phi_0 = LI_0 = 0.05$ Wb for the numbers above — so the overshoot is $\Phi_0/t_f$ and scales as one over the switching time. This is brutal:

| $t_f$ | $L I_0 / t_f$ | verdict for a 1200 V IGBT |
|---|---|---|
| $1$ ms | $50$ V | harmless |
| $100\ \mu$s | $500$ V | marginal |
| $10\ \mu$s | $5$ kV | destroyed |
| $1\ \mu$s | $50$ kV | destroyed |
| $200$ ns | $250$ kV | destroyed |

The point of the table is the *sensitivity*: a factor of ten in turn-off speed is a factor of ten in the voltage the switch has to absorb. It is worth measuring $t_f$ on the actual hardware rather than assuming it, since the difference between "marginal" and "vaporised" lives in exactly that factor. Datasheet fall times for power IGBTs are typically $0.1$--$1\ \mu$s, which puts an unprotected coil switch deep in the destroyed rows.

---

## 5. Why that estimate is circular, and what really sets the ceiling

The formula $v_{CE} = V_s + L I_0/t_f$ contains a hidden falsehood: it assumes the switch is free to dictate $dI/dt$. It is not. The inductor is the element imposing the current, and it will impose it through whatever path exists. If the switch tries to reduce the current faster than the rest of the circuit allows, the voltage simply rises until *something* accepts the current. Taken literally, $t_f \to 0$ gives $v_{CE}\to\infty$, which is unphysical: a finite $\tfrac12 LI_0^2$ cannot produce infinite voltage.

The resolution is §3.3. There is always a parasitic capacitance $C_p$ across the switch, and it is that capacitance, not the gate drive, that sets the ceiling once the switch is fast.

### 5.1 The LC ringdown

Idealise the switch as an instantaneous open circuit and neglect $R$ (justified below). The loop is now $V_s$ — $L$ — $C_p$, with $v \equiv v_{CE}$ across the capacitance and $I = C_p\,dv/dt$:

$$
V_s = L\frac{dI}{dt} + v
\qquad\Longrightarrow\qquad
LC_p \ddot{v} + v = V_s .
$$

With initial conditions $v(0)=V_{CE,\text{sat}}\approx 0$ and $\dot v(0) = I_0/C_p$, and defining

$$
\omega_0 = \frac{1}{\sqrt{LC_p}},
\qquad
Z_0 = \sqrt{\frac{L}{C_p}}\;\;\text{(characteristic impedance)},
$$

the solution is

$$
v(t) = V_s\bigl(1-\cos\omega_0 t\bigr) \;+\; I_0 Z_0 \sin\omega_0 t .
$$

The oscillating part has amplitude $\sqrt{V_s^2 + (I_0Z_0)^2}$ about the offset $V_s$, so

$$
\boxed{\;v_{CE}^{\text{peak}} = V_s + \sqrt{V_s^{\,2} + Z_0^{\,2} I_0^{\,2}}\;}
$$

Two limits check this. With $I_0=0$ it reduces to $v^{\text{peak}} = 2V_s$, the familiar factor-of-two overshoot of a step applied to an undamped LC. With $I_0 Z_0 \gg V_s$, which is the practical case,

$$
v_{CE}^{\text{peak}} \simeq V_s + I_0 Z_0 = V_s + I_0\sqrt{\frac{L}{C_p}} .
$$

The same result follows from energy conservation without solving anything. At the peak $\dot v = 0$, so $I=0$, and all the magnetic energy plus the work done by the supply sits in the capacitance:

$$
\tfrac12 C_p v_{pk}^2 = \tfrac12 L I_0^2 + V_s C_p v_{pk}
\;\Longrightarrow\;
v_{pk}^2 - 2V_s v_{pk} - \frac{L}{C_p}I_0^2 = 0,
$$

whose positive root is the boxed formula. The transfer $\tfrac12 LI_0^2 \to \tfrac12 C_p v^2$ is the cleanest way to see what a flyback event *is*: the coil dumping its stored energy into the only reservoir available, with the voltage being whatever it takes to hold that energy in a very small capacitance.

### 5.2 Numbers, and the crossover

With $L = 500\ \mu$H, $I_0 = 100$ A, $V_s = 50$ V and $C_p = 1$ nF:

$$
Z_0 = \sqrt{\frac{5\times10^{-4}}{10^{-9}}} = 707\ \Omega,
\qquad
I_0 Z_0 = 70.7\ \text{kV},
\qquad
v_{CE}^{\text{peak}} \approx 70.8\ \text{kV}.
$$

The timescale is

$$
\sqrt{LC_p} = 707\ \text{ns},
\qquad
t_{\text{peak}} = \frac{\pi}{2}\sqrt{LC_p} \approx 1.1\ \mu\text{s}.
$$

Damping is negligible on this first peak: the coil resistance $R\sim$ tens of m$\Omega$ is four orders of magnitude below $Z_0$, so the quality factor $Q = Z_0/R$ is enormous and the first excursion is essentially the undamped one. Neglecting $R$ in §5.1 was safe.

This gives the criterion that reconciles §4 and §5:

- **Slow turn-off, $t_f \gg \sqrt{LC_p}$.** The switch genuinely controls $dI/dt$, and $v_{CE}^{\text{peak}} \approx V_s + LI_0/t_f$. Making the switch slower does help.
- **Fast turn-off, $t_f \lesssim \sqrt{LC_p}$.** The switch has already stopped mattering. The current commutates into $C_p$, and the answer saturates at the $t_f$-independent hard ceiling $V_s + I_0\sqrt{L/C_p}$.

For the numbers here the crossover is around $t_f \sim 1\ \mu$s, which is precisely where real IGBT fall times sit. Note also that both branches give tens of kilovolts. There is no version of this problem in which an unprotected switch survives.

---

## 6. Why the IGBT is the component that dies

None of the above voltages actually appears on an oscilloscope, because the IGBT fails long before the LC peak is reached. Three ratings are in play.

**Blocking voltage $V_{CES}$.** An IGBT in the off state can only hold off a fixed collector--emitter voltage — typically $600$, $1200$ or $1700$ V — set by the doping and thickness of the drift region. Above it the device avalanches. In §3.3 the collector was climbing at $100$ V/ns, so a $1200$ V part reaches breakdown roughly $12$ ns after the gate goes low, long before the $1.1\ \mu$s LC peak.

**What happens next is the actual failure mechanism.** Once the device avalanches it clamps the node near $V_{(BR)CES}$ and conducts the coil current *itself*. The coil now discharges through the die, dumping

$$
W = \tfrac12 L I_0^2 = 2.5\ \text{J}
$$

into a silicon chip of order $1\ \text{cm}^2$, over a time $\sim L I_0 / V_{(BR)} \approx 40\ \mu$s. That is an instantaneous power of $V_{(BR)}I_0 \approx 120$ kW. Unlike many power MOSFETs, IGBTs are generally *not* avalanche-energy rated at all, and the avalanche current filaments rather than spreading, so the energy lands in a small fraction of the die. The result is a localised melt and a permanent collector--emitter short.

**RBSOA.** Even below $V_{CES}$, an IGBT has a reverse-bias safe operating area: a boundary in the $(v_{CE}, i_C)$ plane that must not be crossed *while current is still flowing*. Turn-off traverses exactly this region, with high current and rising voltage simultaneously. A hard flyback drives the operating point straight out of the RBSOA, and can trigger dynamic latch-up of the parasitic thyristor even if the peak voltage never reaches the blocking limit.

So the failure has nothing to do with the coil and nothing to do with the supply. The switch is simply the component asked to absorb $\tfrac12 LI_0^2$ in microseconds, and it cannot.

---

## 7. Summary

1. $\mathcal{E} = -L\,dI/dt$ is the induced EMF, the quantity Lenz's law describes. $v_L = +L\,dI/dt$ is the terminal voltage drop, the quantity KVL uses. Mixing them is the origin of most sign errors here.
2. Inductor current is continuous; voltage is what jumps. At turn-off the current keeps its direction, and the coil flips from load to source, which forces its terminal polarity to reverse.
3. The bottom terminal of the coil — the collector node — therefore becomes positive, and its EMF *adds* to the supply: $v_{CE} = V_s - IR + L|dI/dt|$.
4. For a slow switch the peak is $V_s + LI_0/t_f$. For a fast switch it saturates at the parasitic-capacitance ceiling $V_s + I_0\sqrt{L/C_p}$, reached in $\tfrac{\pi}{2}\sqrt{LC_p}$. Both are tens of kilovolts for a realistic coil.
5. In practice the IGBT avalanches within nanoseconds and then absorbs the coil's entire $\tfrac12 LI_0^2$ in its own die, which destroys it.

The framing that carries over to the protection note is point 5. The stored energy $\tfrac12 L I_0^2$ is a fixed, non-negotiable quantity the instant the gate goes low. **You cannot forbid it from existing; you can only choose where it is dissipated.** Every protection scheme — freewheeling diode, RC or RCD snubber, transient-voltage-suppressor or varistor clamp, or a deliberate series dump resistor — is a different answer to the question "where does the 2.5 J go, and how long may it take to get there?" Those answers, and the trade-off between clamp voltage and coil turn-off time that they all share, are developed next.
