# Chapter 5 — Classification of Soil

> Study notes (my own condensed summary) of Ch. 5 in Das & Sobhan, *Principles of Geotechnical Engineering*, 9th ed., Cengage (2018), pp. 129–155.
> Table/equation numbers match the textbook. The big flow-charts (Figs. 5.4–5.6) are summarised as rules rather than redrawn — open the book for the exact charts.

---

## 1. Why classify?

Classification gives engineers a **common language** for soils without long descriptions. No system fits every purpose, but most are built on two simple index properties: **particle-size distribution** and **plasticity** (LL, PI).

Two families:

| Family | Basis | Systems in this chapter |
|---|---|---|
| **Textural** | % sand, silt, clay only | USDA |
| **Engineering behaviour** | grain size **and** plasticity | AASHTO, Unified (USCS) |

- Textural systems ignore plasticity → inadequate for most engineering work.
- **AASHTO** is used mostly by state/county **highway** departments; **USCS** is preferred by **geotechnical** engineers.

---

## 2. USDA textural classification

**Size limits (USDA):**

| Fraction | Diameter |
|---|---|
| Sand | 2.0 – 0.05 mm |
| Silt | 0.05 – 0.002 mm |
| Clay | < 0.002 mm |

**How to use the triangular chart (Fig. 5.1):** enter the % sand, % silt, % clay (they sum to 100) and read the zone (e.g., clay loam, sandy loam, silty clay, loamy sand …).

**Gravel correction.** The chart only covers material **passing the No. 10 sieve (2 mm)**. If gravel is present, re-normalise the other fractions:

$$\text{Modified \% (sand, silt or clay)} = \frac{\text{\% of that fraction}}{100 - \%\text{gravel}}\times 100$$

Then classify on the chart, and add "gravelly" to the name when there's a lot of gravel.

**Ex. 5.1 (setups/results)**

| Soil | Gravel | Sand | Silt | Clay | Modified sand / silt / clay | Name |
|---|---|---|---|---|---|---|
| A | 12 | 25 | 32 | 31 | 28.4 / 36.4 / 35.2 | **Gravelly clay loam** |
| B | 18 | 31 | 30 | 21 | 37.8 / 36.6 / 25.6 | **Gravelly loam** |
| C | 0 | 15 | 30 | 55 | 15 / 30 / 55 | **Clay** |
| D | 12 | 22 | 26 | 40 | 25 / 29.5 / 45.5 | **Gravelly clay** |

(Worked example in the text: 30 % sand / 40 % silt / 30 % clay → **clay loam**.)

---

## 3. AASHTO classification (ASTM D-3282; AASHTO M145)

Origin: 1929 Public Roads Administration system; present form from the Highway Research Board (1945).

### 3.1 Criteria

**Grain size**
| Fraction | Size |
|---|---|
| Gravel | passes 75 mm (3 in.) sieve, retained on **No. 10** (2 mm) |
| Sand | passes No. 10, retained on **No. 200** (0.075 mm) |
| Silt + clay | passes **No. 200** |

(Cobbles/boulders > 75 mm are excluded from the sample being classified, but their percentage is recorded.)

**Plasticity (of the fraction passing No. 40)**
- **Silty** if PI ≤ 10; **clayey** if PI ≥ 11.

**Two big divisions:**
- **Granular** materials: ≤ 35 % passing No. 200 → groups **A-1, A-2, A-3**
- **Silt–clay** materials: > 35 % passing No. 200 → groups **A-4, A-5, A-6, A-7**

### 3.2 Table 5.1 — Classification of highway subgrade materials

**Granular materials (≤ 35 % passing No. 200)**

| Group | A-1-a | A-1-b | A-3 | A-2-4 | A-2-5 | A-2-6 | A-2-7 |
|---|---|---|---|---|---|---|---|
| % passing No. 10 | ≤ 50 | — | — | — | — | — | — |
| % passing No. 40 | ≤ 30 | ≤ 50 | ≥ 51 | — | — | — | — |
| % passing No. 200 | ≤ 15 | ≤ 25 | ≤ 10 | ≤ 35 | ≤ 35 | ≤ 35 | ≤ 35 |
| LL (of fraction passing No. 40) | — | — | — | ≤ 40 | ≥ 41 | ≤ 40 | ≥ 41 |
| PI | ≤ 6 | ≤ 6 | NP | ≤ 10 | ≤ 10 | ≥ 11 | ≥ 11 |
| Typical materials | stone fragments, gravel, sand | ← same | fine sand | silty or clayey gravel and sand | ← | ← | ← |
| Subgrade rating | Excellent to good | | | | | | |

**Silt–clay materials (> 35 % passing No. 200)**

| Group | A-4 | A-5 | A-6 | A-7-5 / A-7-6 |
|---|---|---|---|---|
| % passing No. 200 | ≥ 36 | ≥ 36 | ≥ 36 | ≥ 36 |
| LL | ≤ 40 | ≥ 41 | ≤ 40 | ≥ 41 |
| PI | ≤ 10 | ≤ 10 | ≥ 11 | ≥ 11 |
| Typical materials | silty soils | silty soils | clayey soils | clayey soils |
| Subgrade rating | Fair to poor | | | |

- **A-7-5:** $PI \le LL - 30$
- **A-7-6:** $PI > LL - 30$

**Procedure:** apply the test data to the table **from left to right**; the **first group** the soil fits is the answer (process of elimination).

### 3.3 Group index (GI)

Added in parentheses after the group name, e.g., **A-6(5)**. Evaluates subgrade quality — **performance is inversely related to GI** (higher GI = worse).

$$GI = (F_{200} - 35)\big[0.2 + 0.005\,(LL - 40)\big] + 0.01\,(F_{200} - 15)(PI - 10) \tag{5.1}$$

- $F_{200}$ = % passing No. 200 sieve
- LL, PI = of the fraction passing No. 40
- 1st term = partial GI from LL; 2nd term = partial GI from PI

**Rules**
1. Negative result → GI = 0.
2. Round to the nearest whole number (3.4 → 3; 3.5 → 4). No upper limit.
3. GI = 0 for groups **A-1-a, A-1-b, A-2-4, A-2-5, A-3**.
4. For **A-2-6** and **A-2-7**, use only the PI term:

$$GI = 0.01\,(F_{200} - 15)(PI - 10) \tag{5.2}$$

### 3.4 AASHTO examples

**Ex. 5.2** — Passing: No. 10 = 42 %, No. 40 = 35 %, No. 200 = 20 %; LL = 25, PL = 20 → PI = 5.
≤ 35 % passes No. 200 → granular. Going left to right, fits **A-1-b** → GI = 0 → **A-1-b(0)**.

**Ex. 5.3** — 95 % passes No. 200; LL = 60; PI = 40.
Silt-clay; LL ≥ 41, PI ≥ 11, and PI = 40 > LL − 30 = 30 → **A-7-6**.
$GI = (95-35)[0.2+0.005(20)] + 0.01(95-15)(40-10) = 18 + 24 = 42$ → **A-7-6(42)**.

**Ex. 5.5** — (soil from Ex. 5.4: 58 % passes No. 200, LL = 30, PI = 10) → silt-clay, LL ≤ 40 and PI ≤ 10 → **A-4**.
$GI = (58-35)[0.2 + 0.005(30-40)] + 0.01(58-15)(0) = 23(0.15) = 3.45$.
The book writes this as ≈ 4 and labels the soil **A-4(4)**. *(Heads-up: by the rounding rule above, 3.45 would round to 3, so A-4(3). Worth checking with your instructor which convention your course uses.)*

---

## 4. Unified Soil Classification System (USCS) — ASTM D-2487

Proposed by **A. Casagrande (1942)** for WWII airfield work; revised with the U.S. Bureau of Reclamation (1952). Widely used in geotechnical practice.

### 4.1 Two broad categories

| Category | Definition | Prefixes |
|---|---|---|
| **Coarse-grained** | **> 50 % retained** on No. 200 (< 50 % passes) | **G** = gravel/gravelly, **S** = sand/sandy |
| **Fine-grained** | **≥ 50 % passes** No. 200 | **M** = inorganic silt, **C** = inorganic clay, **O** = organic silt/clay |
| Highly organic | peat, muck | **Pt** |

**Suffix letters**
- **W** well graded, **P** poorly graded
- **L** low plasticity (LL < 50), **H** high plasticity (LL ≥ 50)
- (Second letter in coarse soils: **M** = silty fines, **C** = clayey fines)

### 4.2 Information needed

1. % gravel (passes 76.2 mm, retained on **No. 4** — 4.75 mm)
2. % sand (passes No. 4, retained on **No. 200** — 0.075 mm)
3. % fines (silt + clay, passes No. 200)
4. $C_u$ and $C_c$

$$C_u = \frac{D_{60}}{D_{10}}, \qquad C_c = \frac{(D_{30})^2}{D_{60}\,D_{10}}$$

5. LL and PI of the fraction passing **No. 40**

### 4.3 Table 5.2 — assigning group symbols

**Coarse-grained soils**

| Soil | Fines | Condition | Symbol |
|---|---|---|---|
| **Gravels** (> 50 % of coarse fraction retained on No. 4) | < 5 % (clean) | $C_u \ge 4$ **and** $1 \le C_c \le 3$ | **GW** |
| | | $C_u < 4$ and/or $C_c < 1$ or $> 3$ | **GP** |
| | > 12 % | PI < 4 or plots below A-line | **GM** |
| | > 12 % | PI > 7 and on/above A-line | **GC** |
| **Sands** (≥ 50 % of coarse fraction passes No. 4) | < 5 % (clean) | $C_u \ge 6$ **and** $1 \le C_c \le 3$ | **SW** |
| | | $C_u < 6$ and/or $C_c < 1$ or $> 3$ | **SP** |
| | > 12 % | PI < 4 or below A-line | **SM** |
| | > 12 % | PI > 7 and on/above A-line | **SC** |

**Dual symbols**
- **5–12 % fines** → dual symbols: GW-GM, GW-GC, GP-GM, GP-GC; SW-SM, SW-SC, SP-SM, SP-SC (first = gradation, second = type of fines).
- If fines have **4 ≤ PI ≤ 7** and plot in the **hatched zone** of the plasticity chart → **GC-GM** or **SC-SM**.

**Fine-grained soils** (use the plasticity chart, Fig. 5.3)

| LL | Type | Condition | Symbol |
|---|---|---|---|
| **< 50** | Inorganic | PI > 7 and on/above A-line | **CL** |
| | Inorganic | PI < 4 or below A-line | **ML** |
| | Inorganic | 4 ≤ PI ≤ 7 and in hatched zone | **CL-ML** (dual) |
| | Organic | $\dfrac{LL_{\text{oven-dried}}}{LL_{\text{not dried}}} < 0.75$ | **OL** |
| **≥ 50** | Inorganic | PI on/above A-line | **CH** |
| | Inorganic | PI below A-line | **MH** |
| | Organic | $\dfrac{LL_{\text{oven-dried}}}{LL_{\text{not dried}}} < 0.75$ | **OH** |
| — | Highly organic: mostly organic matter, dark colour, organic odour | | **Pt** |

### 4.4 Plasticity chart (Fig. 5.3)
- **A-line:** $PI = 0.73\,(LL - 20)$ — above = clays, below = silts/organics.
- **U-line:** $PI = 0.9\,(LL - 8)$ — practical upper limit.
- **LL = 50** splits low (L) from high (H) plasticity.
- Hatched zone: $4 \le PI \le 7$ just above the A-line → CL-ML.

### 4.5 Group names (ASTM D-2487, Figs. 5.4–5.6) — rules of thumb

Definitions to use:
- Fine fraction = % passing No. 200
- Coarse fraction = % retained on No. 200
- Gravel fraction = % retained on No. 4
- Sand fraction = (% retained on No. 200) − (% retained on No. 4)

**Coarse-grained soils (gravels and sands):**
- Name = *well/poorly graded* + **gravel/sand** (or *silty/clayey/silty clayey* when fines > 12 %; "*… with silt / clay*" for dual symbols).
- Add **"with sand"** (for gravels) or **"with gravel"** (for sands) when the *other* coarse component is **≥ 15 %**.

**Fine-grained soils (inorganic):**
| Symbol | Base name |
|---|---|
| CL | lean clay |
| CH | fat clay |
| ML | silt |
| MH | elastic silt |
| CL-ML | silty clay |

Then look at the % retained on No. 200 ("plus No. 200"):
- **< 15 %** → just the base name (e.g., *lean clay*)
- **15–29 %** → add **"with sand"** or **"with gravel"** (whichever is greater; sand if equal)
- **≥ 30 %** → prefix **"sandy"** or **"gravelly"** (whichever is greater), and add "with gravel"/"with sand" if the other one is ≥ 15 %

**Organic soils (OL, OH):** the same pattern, with names *organic silt* or *organic clay* (organic clay when PI ≥ 4 and on/above the A-line; organic silt otherwise).

### 4.6 USCS examples

| Ex. | Given | Reasoning | Result |
|---|---|---|---|
| **5.4** | 58 % passes No. 200; LL = 30, PI = 10 | Fine-grained; LL < 50; plots above A-line → CL. Plus-200 = 42 % (≥ 30 %), sand 42 % > gravel 0 %, gravel < 15 % | **CL — sandy lean clay** |
| **5.6** | 70 % passes No. 4; 30 % passes No. 200; LL = 33, PL = 12 | Coarse (30 % < 50 %). Gravel = 30 %; of the coarse fraction 70 %, sand > 50 % → sandy. Fines > 12 %; PI = 21 > 7, above A-line → SC. Gravel ≥ 15 % | **SC — clayey sand with gravel** |
| **5.7 (soil A)** | 8 % fines, 0 % gravel; $D_{10}$ = 0.085, $D_{30}$ = 0.12, $D_{60}$ = 0.135 mm; LL = 30, PL = 22 | $C_u = 1.59 < 6$ → poorly graded ($C_c = 1.25$); 5–12 % fines; PI = 8 > 7, above A-line | **SP-SC — poorly graded sand with clay** |
| **5.7 (soil B)** | 61 % passes No. 200; LL = 26, PL = 20 | Fine-grained; PI = 6 in hatched zone → CL-ML. Plus-200 = 39 % (≥ 30 %), sand 39 > gravel 0 | **CL-ML — sandy silty clay** |
| **5.8** | 100 % passes No. 4; 77 % passes No. 200; LL = 63, PI = 25 | LL ≥ 50, below A-line → MH. Plus-200 = 23 % (15–29 %), sand > gravel | **MH — elastic silt with sand** |
| **5.9** | Sieve data: 94 % passes No. 4, 3 % passes No. 200; nonplastic; $D_{60}$ = 1.41, $D_{30}$ = 0.96, $D_{10}$ = 0.41 mm | Sand (94 % passes No. 4), clean. $C_u = 3.44 < 6$ → poorly graded ($C_c = 1.59$). Gravel = 6 % < 15 % | **SP — poorly graded sand** |
| **5.10** | Fuller–Thompson ideal gradation, $D_{max}$ = 40 mm: $p = \sqrt{D/D_{max}}\times 100$ | $D_{60}$ = 14.4, $D_{30}$ = 3.6, $D_{10}$ = 0.4 mm → $C_u = 36$, $C_c = 2.25$; gravel | **GW** |

---

## 5. AASHTO vs. Unified — comparison

| Feature | AASHTO | USCS |
|---|---|---|
| Fine-grained threshold | **> 35 %** passes No. 200 | **≥ 50 %** passes No. 200 |
| Gravel / sand boundary | **No. 10** (2 mm) | **No. 4** (4.75 mm) |
| Organic soils | no place for them | OL, OH, Pt |
| Descriptiveness | letter groups A-1…A-7 (A-2 lumps many soil types) | symbols like GW, SM, CH are more descriptive; gravel and sand clearly separated |
| Extra index | group index (subgrade quality) | group name |

- A coarse soil with about 35 % fines behaves like a fine-grained soil (fines fill the voids and hold coarse grains apart) → the AASHTO threshold is arguably more appropriate.
- No. 10 is the more widely accepted upper limit for sand (used in concrete and highway base-course practice).
- Peats: high moisture content, low $G_s$, low unit weight.

### Rough equivalence (Liu, 1967) — "most probable" matches

**AASHTO → USCS**

| AASHTO | Most probable USCS |
|---|---|
| A-1-a | GW, GP |
| A-1-b | SW, SP, GM, SM |
| A-3 | SP |
| A-2-4, A-2-5 | GM, SM |
| A-2-6 | GC, SC |
| A-2-7 | GM, GC, SM, SC |
| A-4 | ML, OL |
| A-5 | OH, MH, ML, OL |
| A-6 | CL |
| A-7-5 | OH, MH |
| A-7-6 | CH, CL |

**USCS → AASHTO**

| USCS | Most probable AASHTO |
|---|---|
| GW, GP | A-1-a |
| GM | A-1-b, A-2-4, A-2-5, A-2-7 |
| GC | A-2-6, A-2-7 |
| SW | A-1-b |
| SP | A-3, A-1-b |
| SM | A-1-b, A-2-4, A-2-5, A-2-7 |
| SC | A-2-6, A-2-7 |
| ML, OL | A-4, A-5 |
| CL | A-6, A-7-6 |
| MH, OH | A-7-5, A-5 |
| CH | A-7-6 |
| Pt | — (not classified) |

*(Each table in the book also lists "possible" and "possible but improbable" matches; these are the main ones.)*

---

## 6. Step-by-step recipes

### AASHTO
1. Get % passing No. 10, 40, 200; LL and PI of the minus-No. 40 fraction.
2. If $F_{200} \le 35$ % → check A-1-a, A-1-b, A-3, A-2-4 … A-2-7 **in order**.
   If $F_{200} > 35$ % → check A-4, A-5, A-6, A-7-5/A-7-6.
3. For A-7, compare PI with LL − 30.
4. Compute GI (Eq. 5.1, or 5.2 for A-2-6/A-2-7; 0 for A-1, A-2-4, A-2-5, A-3). Report e.g. "A-6(8)".

### USCS
1. $F_{200}$ < 50 % → coarse; ≥ 50 % → fine.
2. **Coarse:** gravel vs. sand (compare coarse fraction retained on / passing No. 4) → check % fines (< 5, 5–12, > 12) → $C_u$, $C_c$ (clean) or A-line/PI (dirty) → symbol → group name using the 15 % rule.
3. **Fine:** LL < 50 or ≥ 50 → plot (LL, PI) on plasticity chart → symbol (check oven-dried LL ratio for organics) → group name using 15 % / 30 % plus-No. 200 rules.

---

## 7. Chapter summary

1. **Textural (USDA)** — name soils by sand/silt/clay percentages (after gravel correction).
2. **AASHTO** — based on sieve analysis (No. 10, 40, 200), LL, PI; groups A-1…A-7; **group index** quantifies subgrade quality.
3. **USCS** — based on sieve analysis (No. 4, 200), LL, PI, $C_u$, $C_c$; two-letter symbols plus ASTM group names derived from % retained on No. 200, % gravel and % sand.

---

## 8. Quick-reference cheat-sheet

| Item | Value |
|---|---|
| USCS coarse/fine split | 50 % passing No. 200 |
| AASHTO granular/silt-clay split | 35 % passing No. 200 |
| USCS gravel/sand split | No. 4 (4.75 mm) |
| AASHTO gravel/sand split | No. 10 (2 mm) |
| GW / SW criteria | $C_u \ge 4$ / $\ge 6$; $1 \le C_c \le 3$ |
| Clean / dual / dirty | < 5 % / 5–12 % / > 12 % fines |
| A-line | $PI = 0.73(LL - 20)$ |
| U-line | $PI = 0.9(LL - 8)$ |
| L vs. H | LL < 50 vs. ≥ 50 |
| AASHTO silty vs. clayey | PI ≤ 10 vs. ≥ 11 |
| A-7-5 vs. A-7-6 | $PI \le LL-30$ vs. $PI > LL-30$ |
| Group index | $(F_{200}-35)[0.2+0.005(LL-40)] + 0.01(F_{200}-15)(PI-10)$ |

---

*End-of-chapter problems (5.1–5.10, plus a boring-log problem 5.C.1) practise: USDA classification of sand/silt/clay mixtures (with and without gravel), AASHTO classification with group index from sieve and Atterberg data, USCS symbols and group names from sieve data/grain-size curves, and comparing both systems for the soil layers in a boring log.*
