# Chapter 3 — Weight–Volume Relationships

> Study notes (my own condensed summary) of Ch. 3 in Das & Sobhan, *Principles of Geotechnical Engineering*, 9th ed., Cengage (2018), pp. 64–94.
> Equation numbers match the textbook so you can cross-reference. Eq. numbers in `(3.x)`.

---

## 1. Big idea

Soil is a **three-phase system**: solids + water + air. Almost every geotechnical calculation (earthwork, compaction, stresses, settlement) starts by describing how much of each phase is present, by **volume** and by **weight**.

| State | Voids contain |
|---|---|
| Dry soil | air only |
| Saturated soil | water only (no air) |
| Moist (partially saturated) soil | air **and** water |

---

## 2. The phase diagram

Separate the soil element into its three phases (air on top, water in the middle, solids at the bottom):

**Volumes**

$$V = V_s + V_v = V_s + V_w + V_a \tag{3.1}$$

- $V_s$ = volume of solids
- $V_v$ = volume of voids
- $V_w$ = volume of water
- $V_a$ = volume of air

**Weights** (weight of air is neglected)

$$W = W_s + W_w \tag{3.2}$$

> **Tip:** always draw the phase diagram first. Put volumes on one side, weights (or masses) on the other, then fill in what you know.

---

## 3. Definitions

### Volume relationships (dimensionless)

| Quantity | Symbol | Definition | Equation |
|---|---|---|---|
| Void ratio | $e$ | $V_v / V_s$ | (3.3) |
| Porosity | $n$ | $V_v / V$ | (3.4) |
| Degree of saturation | $S$ | $V_w / V_v$ (often in %) | (3.5) |

- $n$ is always $<1$ (or <100%); $e$ can exceed 1 (e.g., soft organic clays).
- $S = 0\%$ → dry, $S = 100\%$ → saturated.

**Converting between $e$ and $n$:**

$$e = \frac{n}{1-n} \tag{3.6} \qquad\qquad n = \frac{e}{1+e} \tag{3.7}$$

### Weight relationships

| Quantity | Symbol | Definition | Equation |
|---|---|---|---|
| Moisture (water) content | $w$ | $W_w / W_s$ | (3.8) |
| (Moist / total) unit weight | $\gamma$ | $W / V$ | (3.9) |
| Dry unit weight | $\gamma_d$ | $W_s / V$ | (3.11) |

$$\gamma = \frac{W_s + W_w}{V} = \frac{W_s\,(1+w)}{V} \tag{3.10}$$

$$\gamma_d = \frac{\gamma}{1+w} \tag{3.12}$$

### Densities (SI, mass-based)

$$\rho = \frac{M}{V} \tag{3.13} \qquad\qquad \rho_d = \frac{M_s}{V} \tag{3.14}$$

Unit weight from density:

$$\gamma\ (\text{kN/m}^3) = \frac{g\,\rho\ (\text{kg/m}^3)}{1000}, \qquad g = 9.81\ \text{m/s}^2$$

### Water constants to remember

- $\gamma_w = 9.81\ \text{kN/m}^3 = 62.4\ \text{lb/ft}^3$
- $\rho_w = 1000\ \text{kg/m}^3$

---

## 4. Typical values (natural state) — Table 3.1

| Soil type | Void ratio $e$ | Natural $w$ when saturated (%) | $\gamma_d$ (lb/ft³) | $\gamma_d$ (kN/m³) |
|---|---|---|---|---|
| Loose uniform sand | 0.8 | 30 | 92 | 14.5 |
| Dense uniform sand | 0.45 | 16 | 115 | 18 |
| Loose angular silty sand | 0.65 | 25 | 102 | 16 |
| Dense angular silty sand | 0.4 | 15 | 121 | 19 |
| Stiff clay | 0.6 | 21 | 108 | 17 |
| Soft clay | 0.9–1.4 | 30–50 | 73–93 | 11.5–14.5 |
| Loess | 0.9 | 25 | 86 | 13.5 |
| Soft organic clay | 2.5–3.2 | 90–120 | 38–51 | 6–8 |
| Glacial till | 0.3 | 10 | 134 | 21 |

---

## 5. Key relationships using $e$ and $G_s$

**Trick:** take $V_s = 1$. Then $V_v = e$, $V = 1+e$, $W_s = G_s\gamma_w$, $W_w = wG_s\gamma_w$.

Specific gravity of solids:

$$G_s = \frac{W_s}{V_s\,\gamma_w} \tag{3.15}$$

Unit weights:

$$\gamma = \frac{(1+w)\,G_s\,\gamma_w}{1+e} \tag{3.16}$$

$$\gamma_d = \frac{G_s\,\gamma_w}{1+e} \tag{3.17}$$

$$e = \frac{G_s\,\gamma_w}{\gamma_d} - 1 \tag{3.18}$$

$$\gamma_{sat} = \frac{(G_s+e)\,\gamma_w}{1+e} \tag{3.20}$$

**The "golden" relationship** (works for any soil):

$$\boxed{\,S\,e = w\,G_s\,} \tag{3.19}$$

For a **saturated** soil ($S=1$):

$$e = w\,G_s \tag{3.21}$$

**Density versions** (replace $\gamma_w \to \rho_w$):

$$\rho = \frac{(1+w)G_s\rho_w}{1+e} \tag{3.22}$$
$$\rho_d = \frac{G_s\rho_w}{1+e} \tag{3.23}$$
$$\rho_{sat} = \frac{(G_s+e)\rho_w}{1+e} \tag{3.24}$$

---

## 6. Key relationships using porosity $n$

**Trick:** take total $V = 1$. Then $V_v = n$, $V_s = 1-n$.

$$\gamma_d = G_s\gamma_w\,(1-n) \tag{3.27}$$

$$\gamma = G_s\gamma_w\,(1-n)(1+w) \tag{3.28}$$

$$\gamma_{sat} = \big[(1-n)G_s + n\big]\gamma_w \tag{3.29}$$

$$w_{sat} = \frac{n}{(1-n)\,G_s} \tag{3.30}$$

(Also, $W_s = G_s\gamma_w(1-n)$ and $W_w = wW_s$ — Eqs. 3.25–3.26.)

### Handy derived identity (Example 3.1)

For a saturated soil:

$$\gamma_{sat} = \left(\frac{1+w_{sat}}{1+w_{sat}G_s}\right) G_s\,\gamma_w$$

*How it's derived:* start from $\gamma_{sat} = (1+w_{sat})W_s/V$, use $W_s = G_sV_s\gamma_w$, then $V/V_s = 1+e$, and $e = w_{sat}G_s$.

---

## 7. Relative density (granular soils only)

Describes how dense/loose a sand or gravel is *in situ* compared with its loosest and densest possible states.

$$D_r = \frac{e_{max} - e}{e_{max} - e_{min}} \tag{3.31}$$

- $D_r$ ranges 0% (loosest) → 100% (densest).
- In-place soils rarely have $D_r < 20$–$30\%$; compacting above $\sim 85\%$ is difficult.

**In terms of porosity** (with $e = n/(1-n)$, Eqs. 3.32–3.34):

$$D_r = \frac{(1-n_{min})(n_{max}-n)}{(n_{max}-n_{min})(1-n)} \tag{3.35}$$

**In terms of dry unit weight:**

$$D_r = \left[\frac{\gamma_d - \gamma_{d(min)}}{\gamma_{d(max)} - \gamma_{d(min)}}\right]\left[\frac{\gamma_{d(max)}}{\gamma_d}\right] \tag{3.36}$$

and the same with $\rho_d$ in place of $\gamma_d$ (3.37).

Where $\gamma_{d(min)}$ ↔ $e_{max}$ (loosest) and $\gamma_{d(max)}$ ↔ $e_{min}$ (densest).

### Qualitative description (Table 3.2)

| $D_r$ (%) | Description |
|---|---|
| 0–15 | Very loose |
| 15–50 | Loose |
| 50–70 | Medium |
| 70–85 | Dense |
| 85–100 | Very dense |

### Lab determination (ASTM D-4253, D-4254)

- Mold volume ≈ 2830 cm³ (0.1 ft³).
- **Minimum** dry unit weight: pour sand loosely through a funnel (12.7 mm spout, fall height ≈ 25.4 mm):

$$\gamma_{d(min)} = \frac{W_{s(mold)}}{V_m} \tag{3.38}$$

- **Maximum** dry unit weight: vibrate sand in the mold for 8 min under a surcharge of 14 kN/m² (2 psi), table at 3600 cycles/min, amplitude 0.635 mm.
- The value of $\gamma_{d(max)}$ depends on acceleration, surcharge and vibration geometry, so more intense methods can give a larger value than the ASTM standard.

---

## 8. What controls $e_{max}$ and $e_{min}$

They depend on:
1. Grain size
2. Grain shape (angularity)
3. Shape of the grain-size distribution curve (uniformity coefficient $C_u = D_{60}/D_{10}$)
4. Fines content $F_c$ (fraction finer than 0.075 mm)

**Youd (1973) — angularity $A$ of sand particles**

| Description | Range of $A$ | Mean $A$ |
|---|---|---|
| Very angular | 0.12–0.17 | 0.14 |
| Angular | 0.17–0.25 | 0.21 |
| Subangular | 0.25–0.35 | 0.30 |
| Subrounded | 0.35–0.49 | 0.41 |
| Rounded | 0.49–0.70 | 0.59 |
| Well-rounded | 0.70–1.0 | 0.84 |

(The book's text lists the "Rounded" range as 0.49–0.79 and "Well-rounded" starting at 0.7 — a small overlap in the original.)

**Trends:**
- For a given $C_u$: $e_{max}$ and $e_{min}$ **increase** as angularity **decreases** (rounder → larger range of void ratio).
- For a given $A$: $e_{max}$ and $e_{min}$ **decrease** as $C_u$ **increases** (well-graded soils pack more tightly).

**Effect of non-plastic fines (Lade et al., 1998)** — sand + fines mixtures:
- **0 → ~30 % fines (by volume):** $e_{max}$, $e_{min}$ **decrease** — fines *fill the voids* between sand grains.
- **~30 → 40 %:** transition zone.
- **> ~40 % fines:** $e_{max}$, $e_{min}$ **increase** — fines *replace* solids; the sand grains get pushed apart.

---

## 9. Empirical correlations (Cubrinovski & Ishihara, 2002)

Linear relations between $e_{max}$ and $e_{min}$ by soil type ($F_c$ = fines fraction $<0.075$ mm, $P_c$ = clay-size fraction $<0.005$ mm):

| Soil | Relationship | Eq. |
|---|---|---|
| Clean sand ($F_c = 0$–5 %) | $e_{max} = 0.072 + 1.53\,e_{min}$ | (3.39) |
| Sand with fines ($5 < F_c \le 15\%$) | $e_{max} = 0.25 + 1.37\,e_{min}$ | (3.40) |
| Sand with fines & clay ($15 < F_c \le 30\%$; $P_c = 5$–20 %) | $e_{max} = 0.44 + 1.21\,e_{min}$ | (3.41) |
| Silty soils ($30 < F_c \le 70\%$; $P_c = 5$–20 %) | $e_{max} = 0.44 + 1.32\,e_{min}$ | (3.42) |

Range of void ratio vs. median grain size (sandy and gravelly soils):

$$e_{max} - e_{min} = 0.23 + \frac{0.06}{D_{50}\,(\text{mm})} \tag{3.43}$$

Use (3.43) together with one of (3.39)–(3.42) to solve for both $e_{max}$ and $e_{min}$ when only $D_{50}$ is known.

---

## 10. Worked examples — setups and results

**Ex. 3.1 — Derive $\gamma_{sat}$ in terms of $w_{sat}$ and $G_s$.**
Result shown in §6 above.

**Ex. 3.2 — Moist soil sample** ($V = 1.2\ \text{m}^3$, $M = 2350$ kg, $w = 8.6\%$, $G_s = 2.71$).
Two methods are shown: formulas, or build the phase diagram with numbers.

| Quantity | Result |
|---|---|
| Moist density $\rho = M/V$ | 1958.3 kg/m³ |
| Dry density $\rho_d = \rho/(1+w)$ | 1803.3 kg/m³ |
| Void ratio $e = G_s\rho_w/\rho_d - 1$ | 0.503 |
| Porosity $n = e/(1+e)$ | 0.335 |
| Degree of saturation $S = wG_s/e$ | 46.3 % |
| Volume of water | 0.186 m³ |

*Phase-diagram route:* $M_s = M/(1+w) = 2163.9$ kg → $V_s = M_s/(G_s\rho_w) = 0.798$ m³ → $V_v = 1.2 - 0.798 = 0.402$ m³ → $M_w = 186.1$ kg → $V_w = 0.186$ m³.

**Ex. 3.3 — Water needed to saturate 10 m³** ($n = 0.4$, $G_s = 2.68$, $w = 12\%$).
Use $\rho = G_s\rho_w(1-n)(1+w)$ and $\rho_{sat} = [(1-n)G_s + n]\rho_w$.
$\rho = 1800.96$, $\rho_{sat} = 2008$ kg/m³ → difference 207.04 kg/m³ → **2070.4 kg** of water for 10 m³.

**Ex. 3.4 — Saturated soil, $\gamma_d = 103$ lb/ft³, $w = 23\%$.**
- $\gamma_{sat} = \gamma_d(1+w) \approx 126.7$ lb/ft³
- Combine $\gamma_d = G_s\gamma_w/(1+e)$ with $e = wG_s$ → $G_s = 2.66$
- $e = wG_s = 0.61$

**Ex. 3.5 — Sand with $n = 0.387$, $\rho_d = 1600$ kg/m³.**
$e = n/(1-n) = 0.63$ → from $\rho_d = G_s\rho_w/(1+e)$, $G_s = 2.61$.

**Ex. 3.6 — Borrow-pit volume for an embankment** (cross-section 25 ft top, 15 ft high, 1V:2H side slopes, 1000 ft long; borrow soil $e = 0.68$, $G_s = 2.68$, $w = 10\%$).
Idea: *the dry weight of solids must be the same in the borrow pit and in the finished embankment.*
- Embankment volume = 825,000 ft³
- Borrow-pit $\gamma_d = G_s\gamma_w/(1+e) = 99.54$ lb/ft³
- Borrow volume $= 825{,}000 \times \dfrac{\gamma_{d,\ embankment}}{\gamma_{d,\ borrow}} = 825{,}000\times\dfrac{110}{99.54} \approx 911{,}700\ \text{ft}^3$
- (The book uses 110 lb/ft³ as the embankment *dry* unit weight in this ratio, even though the problem statement just says "$\gamma$".)

**Ex. 3.7 — Relative density in the field** ($e_{max} = 0.75$, $e_{min} = 0.4$, $G_s = 2.68$, $\gamma = 112$ lb/ft³, $w = 12\%$).
$e = G_s\gamma_w(1+w)/\gamma - 1 = 0.67$ → $D_r = (0.75-0.67)/(0.75-0.40) = 22.9\%$ (very loose/loose).

**Ex. 3.8 — Using correlations** (clean sand, $D_{50} = 0.5$ mm, $\gamma_d = 15.72$ kN/m³, $G_s = 2.66$).
1. Eliminate $e_{min}$ using (3.39) inside (3.43): $e_{max} - \dfrac{e_{max}-0.072}{1.53} = 0.23 + \dfrac{0.06}{0.5}$ → $e_{max} = 0.875$
2. $e_{min} = (0.875 - 0.072)/1.53 = 0.525$
3. $e_{field} = G_s\gamma_w/\gamma_d - 1 = 0.66$
4. $D_r = (0.875-0.66)/(0.875-0.525) = 61.4\%$ (medium).

---

## 11. Formula cheat-sheet

| Want | Use |
|---|---|
| $e \leftrightarrow n$ | $e = \dfrac{n}{1-n}$, $n = \dfrac{e}{1+e}$ |
| $S, e, w, G_s$ | $Se = wG_s$ |
| Dry unit weight | $\gamma_d = \dfrac{G_s\gamma_w}{1+e} = \dfrac{\gamma}{1+w} = G_s\gamma_w(1-n)$ |
| Moist unit weight | $\gamma = \dfrac{(1+w)G_s\gamma_w}{1+e} = \gamma_d(1+w)$ |
| Saturated unit weight | $\gamma_{sat} = \dfrac{(G_s+e)\gamma_w}{1+e} = \gamma_d + n\gamma_w$ *(see note)* |
| Void ratio from $\gamma_d$ | $e = \dfrac{G_s\gamma_w}{\gamma_d} - 1$ |
| Sat. water content | $w_{sat} = \dfrac{e}{G_s} = \dfrac{n}{(1-n)G_s}$ |
| Relative density | $D_r = \dfrac{e_{max}-e}{e_{max}-e_{min}}$ |

*Note:* $\gamma_{sat} = \gamma_d + n\gamma_w$ follows directly from the phase diagram (dry solids + water filling all voids); it is one of the identities the chapter's Problem 3.1 asks you to prove.

### Problem-solving recipe

1. Sketch the three-phase diagram.
2. Pick a convenient basis: $V_s = 1$ (when you know $e$) or $V = 1$ (when you know $n$) or use the actual volume given.
3. Fill in everything you can from the given data using $G_s$, $w$, $\gamma_w$.
4. Use $Se = wG_s$ to link degree of saturation to the others.
5. Keep units consistent ($\gamma_w$ = 9.81 kN/m³ or 62.4 lb/ft³; $\rho_w$ = 1000 kg/m³).

---

## 12. Chapter summary (one paragraph)

Soil is described by volume ratios ($e$, $n$, $S$) and weight ratios ($w$, $\gamma$, $\gamma_d$, $\gamma_{sat}$), all interconnected through $G_s$. Relative density quantifies how dense a granular soil is between its loosest and densest states, and $e_{max}$, $e_{min}$ depend on grain size, angularity, gradation and fines content; simple empirical correlations let you estimate them from $D_{50}$ and fines content.

---

*End-of-chapter problems (3.1–3.29, plus critical-thinking problems 3.C.1–3.C.3) cover: proving the identities in §11, finding unknowns from partial data using the phase diagram, water to add for target saturation, embankment/backfill borrow volumes, and relative-density calculations — all solvable with the formulas above.*
