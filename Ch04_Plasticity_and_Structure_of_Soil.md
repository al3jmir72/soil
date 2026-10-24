# Chapter 4 — Plasticity and Structure of Soil

> Study notes (my own condensed summary) of Ch. 4 in Das & Sobhan, *Principles of Geotechnical Engineering*, 9th ed., Cengage (2018), pp. 95–123.
> Equation numbers match the textbook. (The PDF you uploaded stops at the start of the chapter summary, so end-of-chapter problems are not covered.)

---

## 1. Big idea — consistency of fine-grained soils

When clay minerals are present, soil can be **remolded** at the right moisture without crumbling, because of the **adsorbed water** around the clay particles. Atterberg (early 1900s) described how fine-grained soil changes behaviour as moisture content rises:

```
 Moisture content  ───────────────────────────────────────────►
   SOLID   |   SEMISOLID   |     PLASTIC     |    LIQUID
         SL               PL                LL
   (Shrinkage limit) (Plastic limit)   (Liquid limit)
                              └──── PI = LL − PL ────┘
```

| Limit | Boundary between… |
|---|---|
| **Shrinkage limit (SL)** | solid ↔ semisolid |
| **Plastic limit (PL)** | semisolid ↔ plastic |
| **Liquid limit (LL)** | plastic ↔ liquid |

Together: the **Atterberg limits**. All are moisture contents in %.

---

## 2. Liquid limit (LL)

### 2.1 Casagrande percussion-cup method (ASTM D-4318)

- Brass cup on a hard-rubber base, dropped by a crank-driven cam from **10 mm** height.
- Soil paste is placed in the cup; a groove is cut with a standard tool (flat or wedge type).
- **Definition:** LL is the moisture content at which the groove closes over **12.5 mm (0.5 in.)** after **25 blows**.
- Hitting exactly 25 blows is hard, so run **≥ 3 tests** at different moisture contents with N between **15 and 35**. Plot $w$ vs. $\log N$ → approximately a straight line = the **flow curve**. Read $w$ at $N = 25$ → LL.

**Flow index** (slope of the flow curve, taken positive):

$$I_F = \frac{w_1 - w_2}{\log\!\left(\dfrac{N_2}{N_1}\right)} \tag{4.1}$$

Equation of the flow line:

$$w = -I_F \log N + C \tag{4.2}$$

**One-point method** (U.S. Army Corps of Engineers; also in ASTM D-4318). Use when you only ran one test with $N$ between about 20 and 30:

$$LL = w_N\left(\frac{N}{25}\right)^{\tan\beta} \tag{4.3}$$

with $\tan\beta = 0.121$ (not exactly true for every soil).

**Table 4.1 — values of $(N/25)^{0.121}$**

| N | 20 | 21 | 22 | 23 | 24 | 25 | 26 | 27 | 28 | 29 | 30 |
|---|---|---|---|---|---|---|---|---|---|---|---|
| factor | 0.973 | 0.979 | 0.985 | 0.990 | 0.995 | 1.000 | 1.005 | 1.009 | 1.014 | 1.018 | 1.022 |

Why the one-point method works: between N = 20 and 30 the moisture content varies only slightly.

### 2.2 Fall-cone method (British Standard BS 1377; popular in Europe and Asia)

- Standard cone, apex angle **30°**, weight **0.78 N (80 gf)**, released from point contact with the soil surface.
- **Definition:** LL is the moisture content at which the cone penetrates **d = 20 mm in 5 s**.
- Run ≥ 4 tests at different moisture contents; plot $w$ vs. $d$ (semi-log) → straight line; read $w$ at $d = 20$ mm.

**Flow index (fall cone):**

$$I_{FC} = \frac{w_2(\%) - w_1(\%)}{\log d_2 - \log d_1} \tag{4.4}$$

**One-point estimates** (single test; $w$ in %, $d$ in mm):

| Author | Formula | Eq. |
|---|---|---|
| Nagaraj & Jayadeva (1981) | $LL = \dfrac{w}{0.77\,\log d}$ | (4.5) |
| Nagaraj & Jayadeva (1981) | $LL = \dfrac{w}{0.65 + 0.0175\,d}$ | (4.6) |
| Feng (2001) | $LL = w\left(\dfrac{20}{d}\right)^{0.33}$ (valid for $15 \le d \le 25$ mm) | (4.7) |

**Table 4.2 — fall cones used around the world** (penetration duration is 5 s in all cases)

| Country | Cone | Penetration at LL (mm) |
|---|---|---|
| Russia | 30°, 76 g | 10 |
| Britain, France | 30°, 80 g | 20 |
| India | 31°, 148 g | 20.4 |
| Sweden, Canada (Quebec) | 60°, 60 g | 10 |

**Other facts**
- Undrained shear strength of soil **at the liquid limit** ≈ **1.7–2.3 kN/m²** (many studies agree).
- Correlation between the two standards (Feng, 2001):

$$LL_{(BS)} = 2.6 + 0.94\,LL_{(ASTM)} \tag{4.8}$$

### Examples (setups and results)

- **Ex. 4.1** — percussion data: (N, w) = (15, 42.0 %), (20, 40.8 %), (28, 39.3 %). Plot on semi-log paper → **LL = 39.5 %** at N = 25. $I_F = (42 - 39.3)/\log(28/15) = $ **9.96**.
- **Ex. 4.2** — one test only: N = 20, w = 40.8 %. $LL = 40.8\,(20/25)^{0.121} = $ **39.7 %**.
- **Ex. 4.3** — fall cone data: (d, w) = (15, 29.5), (26, 35.5), (34, 38.5), (43, 41.5). Plot → $w$ at $d = 20$ → **LL ≈ 32.5 %**.
- **Ex. 4.4** — one test from Ex. 4.3 (w = 29.5 % at d = 15 mm): Eq. 4.5 → 32.58; Eq. 4.6 → 32.33; Eq. 4.7 → 32.43 (all close to 32.5).

---

## 3. Plastic limit (PL)

- **Definition:** moisture content (%) at which the soil **crumbles when rolled into 3.2 mm (⅛ in.) threads**. It's the **lower** bound of the plastic stage.
- Test: repeatedly roll an ellipsoidal soil mass by hand on a ground-glass plate (ASTM D-4318).
- Fall-cone alternative: same cone geometry but heavier (**2.35 N, 240 gf**); PL = moisture content at **d = 20 mm**.

**Table 4.3 — typical LL, PL and activity of clay minerals**

| Mineral | LL | PL | Activity $A$ |
|---|---|---|---|
| Kaolinite | 35–100 | 20–40 | 0.3–0.5 |
| Illite | 60–120 | 35–60 | 0.5–1.2 |
| Montmorillonite | 100–900 | 50–100 | 1.5–7.0 |
| Halloysite (hydrated) | 50–70 | 40–60 | 0.1–0.2 |
| Halloysite (dehydrated) | 40–55 | 30–45 | 0.4–0.6 |
| Attapulgite | 150–250 | 100–125 | 0.4–1.3 |
| Allophane | 200–250 | 120–150 | 0.4–1.3 |

---

## 4. Plasticity index (PI)

$$PI = LL - PL \tag{4.9}$$

**Burmister (1949) qualitative scale**

| PI | Description |
|---|---|
| 0 | Nonplastic |
| 1–5 | Slightly plastic |
| 5–10 | Low plasticity |
| 10–20 | Medium plasticity |
| 20–40 | High plasticity |
| > 40 | Very high plasticity |

PI is central to fine-grained soil classification (Casagrande chart → USCS, Chapter 5).

**Correlations with flow index** (Sridharan et al., 1999):

$$PI(\%) = 4.12\,I_F(\%) \tag{4.10}$$
$$PI(\%) = 0.74\,I_{FC}(\%) \tag{4.11}$$

---

## 5. Shrinkage limit (SL)

**Definition:** the moisture content (%) below which further drying causes **no further volume change**. Above SL, the soil shrinks as it loses water; below SL, volume is constant.

### Test procedure (porcelain dish ≈ 44 mm dia. × 12.7 mm high)
1. Coat the dish with petroleum jelly, fill completely with wet soil, strike off excess.
2. Record the wet mass $M_1$ and initial volume $V_i$ (= dish volume).
3. Oven-dry the pat → dry mass $M_2$ and final volume $V_f$.

### Formulas

$$SL = w_i(\%) - \Delta w(\%) \tag{4.12}$$

$$w_i(\%) = \frac{M_1 - M_2}{M_2}\times 100 \tag{4.13}$$

$$\Delta w(\%) = \frac{(V_i - V_f)\,\rho_w}{M_2}\times 100 \tag{4.14}$$

Combined:

$$SL = \left(\frac{M_1 - M_2}{M_2}\right)(100) - \left(\frac{V_i - V_f}{M_2}\right)(\rho_w)(100) \tag{4.15}$$

**Finding the volumes (ASTM D-4943)**
- $V_i = \dfrac{\text{mass of water filling the dish}}{\rho_w}$ (4.16)
- Dip the dry pat in molten wax, then weigh in air ($M_3$) and submerged ($M_4$):
  - Mass of water displaced: $M_5 = M_3 - M_4$ (4.17)
  - Volume of pat + wax: $V_{fw} = M_5/\rho_w$ (4.18)
  - Mass of wax: $M_6 = M_3 - M_2$ (4.19)
  - Volume of wax: $V_{wx} = \dfrac{M_6}{G_{wx}\,\rho_w}$ (4.20)
  - **Dry pat volume:** $V_f = V_{fw} - V_{wx}$ (4.21)

**Shrinkage ratio** (volume change as % of dry volume ÷ corresponding moisture change):

$$SR = \frac{M_2}{V_f\,\rho_w} \tag{4.22}$$

(i.e., the density of the dry soil relative to water.)

**Specific gravity of solids from the shrinkage test:**

$$G_s = \frac{1}{\dfrac{1}{SR} - \dfrac{SL}{100}} \tag{4.23}$$

**Maximum expected shrinkage at moisture content $w$ (> SL):**

$$VS(\%) = SR\,\big[w(\%) - SL\big] \quad \text{(volumetric shrinkage)} \tag{4.24}$$

$$LS(\%) = 100\left[1 - \left(\frac{100}{VS(\%) + 100}\right)^{1/3}\right] \quad \text{(linear shrinkage)} \tag{4.25}$$

**Typical SL of clay minerals (Mitchell, 1976)**

| Mineral | SL (%) |
|---|---|
| Montmorillonite | 8.5–15 |
| Illite | 15–17 |
| Kaolinite | 25–29 |

### Examples (same data for 4.5–4.7)

Data: saturated volume 24.6 cm³, dry volume 15.9 cm³, saturated mass 44.0 g, dry mass 30.1 g.

| Example | Asked | Result |
|---|---|---|
| 4.5 | Shrinkage limit | $SL = \frac{44.0-30.1}{30.1}(100) - \frac{24.6-15.9}{30.1}(1)(100) = 46.18 - 28.9 = \mathbf{17.28\%}$ |
| 4.6 | SR and $G_s$ | $SR = 30.1/15.9 = \mathbf{1.89}$; $G_s = 1/(1/1.89 - 0.1728) \approx \mathbf{2.81}$ |
| 4.7 | At $w = 28\%$: VS and LS | $VS = 1.89(28 - 17.28) = \mathbf{20.26\%}$; $LS \approx \mathbf{5.96\%}$ |

---

## 6. Liquidity index (LI) and consistency index (CI)

Describe where the **natural (in situ) moisture content $w$** sits between PL and LL.

$$LI = \frac{w - PL}{LL - PL} \tag{4.26}$$

$$CI = \frac{LL - w}{LL - PL} \tag{4.27}$$

Note $LI + CI = 1$.

| Condition | LI | CI | Meaning |
|---|---|---|---|
| $w = PL$ | 0 | 1 | at the plastic limit |
| $w = LL$ | 1 | 0 | at the liquid limit |
| $w > LL$ | > 1 | < 0 | natural moisture above LL → **sensitive clay**; when remolded it can flow like a viscous liquid |
| $w < PL$ | < 0 | > 1 | typical of **heavily overconsolidated** deposits |

**Table 4.4 — CI vs. unconfined compression strength (approx.)**

| CI | kN/m² | lb/ft² |
|---|---|---|
| < 0.5 | < 25 | < 500 |
| 0.5–0.75 | 25–80 | 500–1700 |
| 0.75–1.0 | 80–150 | 1700–3100 |
| 1.0–1.5 | 150–400 | 3100–8400 |
| > 1.5 | > 400 | > 8400 |

---

## 7. Activity

Plasticity comes from the adsorbed water around clay particles, so the **type and amount** of clay minerals control LL, PL and PI. Skempton (1953) found PI grows **linearly** with the **clay-size fraction** (% finer than 2 µm by weight), with a different slope for each clay. That slope is the **activity**:

$$A = \frac{PI}{\%\ \text{of clay-size fraction (by weight)}} \tag{4.28}$$

- Use: an index of **swelling potential** of clay soils. (Typical values in Table 4.3.)
- Skempton's examples: Shellhaven clay $A = 1.33$; London clay 0.95; Weald clay 0.63; Horten clay 0.42.
- Seed, Woodward & Lundgren (1964a) — tests on artificial sand–clay mixtures: the PI-vs-clay-fraction relation is linear, but **not always through the origin**, so:

$$A = \frac{PI}{\%\ \text{of clay-size fraction} - C'} \tag{4.29}$$

with $C'$ a constant for the soil ($C' = 9$ for their test data). Examples from their mixtures: commercial bentonite $A \approx 5.4$; commercial kaolinite $A \approx 0.36$ (mixtures lie in between).
- Seed et al. (1964b): the relationship is better shown as **two straight lines**; for clay fractions **> 40 %** the line, projected back, passes through the origin.

---

## 8. Plasticity chart (Casagrande)

Plot **PI (y-axis) against LL (x-axis)**. Two key lines:

| Line | Equation |
|---|---|
| **A-line** | $PI = 0.73\,(LL - 20)$ |
| **U-line** (upper limit for any known soil) | $PI = 0.9\,(LL - 8)$ (4.30) |

Interpreting the chart:
- **Above the A-line** → inorganic **clays**.
- **Below the A-line** → inorganic **silts**.
- **Organic silts** plot in the same zone as inorganic silts of *medium* compressibility (below the A-line, LL ≈ 30–50).
- **Organic clays** plot in the same zone as inorganic silts of *high* compressibility (below the A-line, LL > 50).
- This chart is the basis for classifying fine-grained soils in the **Unified Soil Classification System** (Ch. 5).

### Estimating the shrinkage limit from the chart (Casagrande; Holtz & Kovacs, 1981)
1. Plot the soil's (LL, PI) as point **A**.
2. Extend the A-line and U-line downward until they meet at point **B** at **LL = −43.5, PI = −46.4**.
3. Draw a straight line from **B** through **A** and continue to the LL axis (PI = 0) → point **C**. The **LL-value at C ≈ shrinkage limit**.

---

## 9. Soil structure

*Soil structure = geometric arrangement of particles.* It depends on particle shape, size, mineralogy and the nature/composition of the pore water. Two groups: **cohesionless** and **cohesive**.

### 9.1 Cohesionless soils

**(a) Single-grained structure** — each particle is in stable contact with its neighbours; can be **loose or dense**, giving a wide range of void ratios.

Idealisation: packing of **equal spheres**

| Packing | Void ratio $e$ | Notes |
|---|---|---|
| Simple cubical (very loose) | **0.91** | $e = \dfrac{d^3 - \pi d^3/6}{\pi d^3/6} = \dfrac{6}{\pi} - 1$ |
| Simple stagger | **0.65** | each sphere touches 6 neighbours in its layer; layers stacked directly on top of one another |
| Double stagger | **0.43** | like simple stagger but each sphere slides into contact with 2 spheres in the next layer |
| Pyramidal (very dense) | **0.35** | |

McGeary (1961): steel spheres poured into a container reached an average **minimum $e \approx 0.6$** (≈ 20 % in double-stagger, ≈ 80 % in single-stagger arrangement).

Real soils vs. the sphere model: smaller grains fill voids between larger ones (⇒ lower $e$), but irregular grain shapes raise $e$ — the two effects roughly cancel, so real soils have a similar range of void ratios as equal spheres.

**(b) Honeycombed structure** — fine sand and silt form small arches/chains of particles. **Large void ratio**; carries ordinary static load but **collapses** under heavy or shock loading → large settlement.

### 9.2 Cohesive soils

**Forces between clay particles in water:**
- **Repulsion** from overlapping diffuse double layers (clay surfaces are negatively charged).
- **Attraction** from van der Waals forces (independent of water chemistry).
- Both grow as spacing shrinks, at different rates; at very small spacing, attraction wins.
- Positively charged **edges** can attract negatively charged **faces** (edge-to-face contact).

**Sediment structures**

| Structure | How it forms | Features |
|---|---|---|
| **Dispersed** | Individual particles settle slowly out of a suspension (repulsion dominates at larger spacings; particles may undergo Brownian motion) | Particles ≈ **parallel** to one another |
| **Flocculent (non-salt)** | Particles meet and aggregate **edge-to-face** (electrostatic attraction) into flocs which then settle | Open, high void ratio |
| **Flocculent (salt)** | Salt ions **depress the double layer**, reducing repulsion → flocs form and settle | Particle orientation approaches parallelism (van der Waals); lightweight, high void ratio |

- **Marine clays** are highly flocculent; **freshwater** clay deposits are usually between dispersed and flocculent.
- Pure clay-mineral deposits are rare; a soil with **≥ 50 %** particles ≤ 0.002 mm is generally called clay.

**Microstructure hierarchy (from electron-microscope studies):**

| Level | Description | Visible with |
|---|---|---|
| **Domains** | aggregated/flocculated submicroscopic units of clay particles | electron microscope |
| **Clusters** | groups of domains | light microscope |
| **Peds** | groups of clusters | naked eye |
| Joints and fissures, groups of peds | macrostructural features | naked eye |

Macrostructure matters most for engineering behaviour; microstructure matters for fundamental understanding.

---

## 10. Chapter summary (as far as the supplied PDF goes)

- Consistency of fine-grained soils is described by **LL, PL, SL** (Atterberg limits): the moisture contents at the liquid→plastic, plastic→semisolid and semisolid→solid transitions.
- Derived indices: **PI**, **LI**, **CI**, **activity**, **flow index**, **shrinkage ratio**.
- Plasticity chart (A-line, U-line) separates clays from silts and underlies the USCS.
- Structure: single-grained / honeycombed (coarse), dispersed / flocculent (clay), organised into domains → clusters → peds.

---

## 11. Formula cheat-sheet

| Quantity | Formula |
|---|---|
| Flow index (percussion) | $I_F = \dfrac{w_1 - w_2}{\log(N_2/N_1)}$ |
| One-point LL (percussion) | $LL = w_N (N/25)^{0.121}$ |
| One-point LL (fall cone) | $LL = w(20/d)^{0.33}$, or $w/(0.77\log d)$, or $w/(0.65+0.0175d)$ |
| Plasticity index | $PI = LL - PL$ |
| Shrinkage limit | $SL = \dfrac{M_1 - M_2}{M_2}(100) - \dfrac{(V_i - V_f)\rho_w}{M_2}(100)$ |
| Shrinkage ratio | $SR = \dfrac{M_2}{V_f\rho_w}$ |
| $G_s$ from SL & SR | $G_s = \dfrac{1}{1/SR - SL/100}$ |
| Volumetric shrinkage | $VS = SR\,(w - SL)$ |
| Linear shrinkage | $LS = 100\left[1 - \left(\dfrac{100}{VS+100}\right)^{1/3}\right]$ |
| Liquidity index | $LI = \dfrac{w - PL}{LL - PL}$ |
| Consistency index | $CI = \dfrac{LL - w}{LL - PL}$ |
| Activity | $A = \dfrac{PI}{\%\text{clay} - C'}$ ($C' = 0$ in the simple form) |
| A-line | $PI = 0.73(LL - 20)$ |
| U-line | $PI = 0.9(LL - 8)$ |

**Exam reminders**
- LL: 25 blows, 12.5 mm closure (cup) · 20 mm penetration (30°/80 g cone).
- PL: 3.2 mm thread crumbles.
- PI > 40 → very high plasticity; PI = 0 → nonplastic.
- LI > 1 ⇒ sensitive, can flow when remolded; LI < 0 ⇒ stiff/overconsolidated.
- High activity (montmorillonite, $A$ up to ~7) ⇒ high swelling potential; kaolinite is low ($A$ ≈ 0.3–0.5).
