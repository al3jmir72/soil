# Chapter 2 — Origin of Soil and Grain Size

> Study notes (my own condensed summary) of Ch. 2 in Das & Sobhan, *Principles of Geotechnical Engineering*, 9th ed., Cengage (2018), pp. 16–63.
> Equation numbers match the textbook.

---

## 1. Chapter roadmap

1. Rock cycle and origin of soil (weathering)
2. Rock-forming minerals and rock structures
3. Particle-size classification
4. Clay minerals and clay–water interaction
5. Specific gravity of solids ($G_s$)
6. Mechanical analysis: **sieve** and **hydrometer** tests
7. Particle-size distribution curve ($D_{10}$, $C_u$, $C_c$)
8. Particle shape

---

## 2. Rock cycle and the origin of soil

Soils are the product of **weathering of rock**. Their properties depend on the minerals in the grains (hence on the parent rock), grain size, shape and chemistry.

### The three rock types

| Rock type | Origin | Examples |
|---|---|---|
| **Igneous** | Solidification of molten **magma** | granite, rhyolite, gabbro, basalt, diorite, andesite, syenite, trachyte, peridotite |
| **Sedimentary** | Weathering products deposited, compacted and **cemented** (or chemically precipitated) | conglomerate, sandstone, shale, limestone, gypsum |
| **Metamorphic** | Changed by **heat and pressure** (without melting) | gneiss, slate, schist, marble, quartzite |

**Rock cycle:** magma → (cooling) igneous → (weathering, erosion, transport) sediments → (compaction, cementation) sedimentary → (heat/pressure) metamorphic → (melting) magma. Any rock type can weather into sediments or metamorphose.

### 2.1 Igneous rocks
- **Intrusive (plutonic):** magma cools slowly beneath the surface → **large crystals (coarse-grained)**, visible to the naked eye.
- **Extrusive:** lava cools quickly at the surface → **fine-grained**.

| Intrusive (coarse) | Extrusive (fine) | Abundant minerals |
|---|---|---|
| Granite | Rhyolite | quartz, Na- and K-feldspar |
| Gabbro | Basalt | plagioclase, pyroxenes, olivine |
| Diorite | Andesite | plagioclase, hornblende |
| Syenite | Trachyte | K-feldspar |
| Peridotite | — | olivine, pyroxenes |

**Bowen's reaction series (1922)** — order in which minerals crystallise as magma cools:
- **Discontinuous (ferromagnesian) series:** olivine → augite → hornblende → biotite (black mica) — minerals differ in chemistry *and* crystal structure.
- **Continuous (plagioclase feldspar) series:** calcium feldspar → sodium feldspar — different composition, similar structure.
- Both then merge: **orthoclase (K-feldspar) → muscovite (white mica) → quartz**.
- High-temperature minerals (top of the series) are **less resistant to weathering**; **quartz is most resistant**.

| Mineral | Composition |
|---|---|
| Olivine | (Mg, Fe)₂SiO₄ |
| Augite | Ca, Na(Mg, Fe, Al)(Al, Si₂O₆) |
| Hornblende | complex ferromagnesian silicate of Ca, Na, Mg, Ti, Al |
| Biotite | K(Mg, Fe)₃AlSi₃O₁₀(OH)₂ |
| Ca-feldspar | Ca(Al₂Si₂O₈) |
| Na-feldspar | Na(AlSi₃O₈) |
| Orthoclase | K(AlSi₃O₈) |
| Muscovite | KAl₃Si₃O₁₀(OH)₂ |
| Quartz | SiO₂ |

### 2.2 Weathering

| | Mechanical (physical) | Chemical |
|---|---|---|
| What happens | Rock broken into smaller pieces **without** change in composition | Minerals **transformed** into new minerals by reaction |
| Agents | Temperature cycles (expansion/contraction), **freeze–thaw** (water expands as ice), glaciers, wind, running water, waves | Water + CO₂ → carbonic acid; dissolved salts; organic acids from decayed matter |
| Typical product | Gravel, sand, silt | **Clay minerals**, silica, soluble salts |

**Example – weathering of orthoclase into kaolinite:**

$$\text{H}_2\text{O} + \text{CO}_2 \to \text{H}_2\text{CO}_3 \to \text{H}^+ + (\text{HCO}_3)^-$$
$$2\,\text{K(AlSi}_3\text{O}_8) + 2\text{H}^+ + \text{H}_2\text{O} \to 2\text{K}^+ + 4\text{SiO}_2 + \text{Al}_2\text{Si}_2\text{O}_5(\text{OH})_4$$

(orthoclase → silica + **kaolinite** clay mineral; released K⁺ is carried away in solution or used by plants). Ferromagnesians also give clay minerals plus hematite/limonite (iron oxides).

The clay minerals — mainly **kaolinite, illite, montmorillonite** — come from chemical weathering of feldspars, ferromagnesians and micas, and give soil its **plasticity**.

### 2.3 Transportation of weathering products

- **Residual soils:** formed and left in place. Typical profile: **fine-grained at the surface, grain size increasing with depth**; angular rock fragments deeper down.
- **Transported soils** (by ice, water, wind, gravity):

| Type | Agent / environment |
|---|---|
| **Glacial** | glaciers |
| **Alluvial** | running water, deposited along streams |
| **Lacustrine** | deposited in quiet lakes |
| **Marine** | deposited in the sea |
| **Aeolian** | wind |
| **Colluvial** | gravity (e.g., landslides) |

### 2.4 Sedimentary rocks

**Detrital (clastic texture)** — compacted and cemented by iron oxide, calcite, dolomite, quartz:

| Particle size | Rock |
|---|---|
| Gravel (≥ 2–4 mm) | **Conglomerate** (if particles are angular → **breccia**) |
| Sand (1/16 – 2 mm) | **Sandstone** (nearly all quartz → **orthoquartzite**) |
| Silt and clay (< 1/16 mm) | **Mudstone** (blocky) and **shale** (splits into platy slabs) |

**Chemical sedimentary rocks:**

| Composition | Rock |
|---|---|
| Calcite (CaCO₃) | Limestone (chalk = biochemical calcite from tiny organisms) |
| Halite (NaCl) | Rock salt |
| Dolomite | Dolomite |
| Gypsum (CaSO₄·2H₂O) | Gypsum |

Gypsum, anhydrite and rock salt are **evaporites** (precipitate from evaporating sea water).

### 2.5 Metamorphic rocks

Heat and pressure change composition and texture (often a **foliated** texture) without melting.

| Rock | Parent / notes |
|---|---|
| **Gneiss** | high-grade regional metamorphism of granite, gabbro, diorite |
| **Slate** | low-grade metamorphism of shale/mudstone (clay → chlorite + mica) |
| **Phyllite** | slate subjected to more heat (> 250–300 °C) |
| **Schist** | well-foliated with visible platy/micaceous flakes |
| **Marble** | recrystallised calcite/dolomite (larger grains) |
| **Quartzite** | quartz-rich sandstone cemented by silica — one of the hardest rocks |

With extreme heat and pressure, metamorphic rocks melt → magma → cycle repeats.

(Sec. 2.3 also points to colour inserts of common minerals/rocks and old structures on rock, e.g., the Parthenon (marble on limestone over phyllite) and the Corinth Canal (completed 1893; 6,346 m long; slopes in marls at 3V:1H–5V:1H).)

---

## 3. Soil-particle size

**Table 2.3 – Size limits (mm) of the main systems**

| System | Gravel | Sand | Silt | Clay |
|---|---|---|---|---|
| MIT (historical) | > 2 | 2 – 0.06 | 0.06 – 0.002 | < 0.002 |
| USDA | 76.2 – 2 | 2 – 0.05 | 0.05 – 0.002 | < 0.002 |
| AASHTO | 76.2 – 2 | 2 – 0.075 | 0.075 – 0.002 | < 0.002 |
| **Unified (USCS; ASTM)** | 76.2 – 4.75 | 4.75 – 0.075 | **Fines (silt + clay): < 0.075** | |

- Sieve No. 4 = 4.75 mm; No. 10 = 2 mm; No. 200 = 0.075 mm.
- **Gravel:** rock fragments; **sand:** mostly quartz and feldspar; **silt:** very fine quartz plus flaky mica fragments; **clay:** flake-shaped microscopic/submicroscopic particles of mica, clay minerals, etc.
- *Clay-size* ≠ *clay mineral*: some very fine quartz/feldspar grains fall in the clay size range. Hence "**clay-sized particles**" (< 2 µm, or < 5 µm in some systems). True clay develops **plasticity** when mixed with limited water (Grim, 1953). Clay particles are mostly colloidal (< 1 µm).

---

## 4. Clay minerals

Complex **aluminium silicates** built from two units:
1. **Silica tetrahedron** — one Si surrounded by 4 O; tetrahedra link into a **silica sheet** (3 base oxygens shared).
2. **Alumina octahedron** — one Al surrounded by 6 OH; octahedra link into an **octahedral (gibbsite) sheet**. If Mg replaces Al → **brucite** sheet.

In the silica sheet, the apex oxygens carry an unbalanced charge; when stacked on a gibbsite sheet they replace hydroxyls and balance the charges.

### The three main clay minerals

| | **Kaolinite** | **Illite** | **Montmorillonite** |
|---|---|---|---|
| Layer structure | 1:1 (one silica + one gibbsite sheet) | 2:1 (gibbsite between two silica sheets) | 2:1 (same as illite) |
| Layer thickness / spacing | ≈ 7.2 Å | ≈ 10 Å | variable, from 9.6 Å to complete separation |
| Bonding between layers | **Hydrogen bonds** (strong) | **Potassium ions** (fairly strong) | Weak van der Waals; **water enters** between layers |
| Isomorphous substitution | little | Al for Si in tetrahedral sheet (balanced by K⁺) | Mg, Fe for Al in octahedral sheet |
| Particle size (lateral × thickness) | 1000–20,000 Å × 100–1000 Å | 1000–5000 Å × 50–500 Å | 1000–5000 Å × 10–50 Å |
| **Specific surface** | ≈ **15 m²/g** | ≈ **80 m²/g** | ≈ **800 m²/g** |
| Behaviour | stable, low swelling | intermediate; "clay mica" | very high swelling/shrinkage |

(1 Å = 10⁻¹⁰ m. **Specific surface** = surface area per unit mass.)

Other clay minerals: chlorite, halloysite, vermiculite, attapulgite.

**Isomorphous substitution** = one element replaces another in the crystal without changing crystal form → net charge imbalance.

### Surface charge and water

- Clay particles carry a **net negative surface charge** (from isomorphous substitution and broken bonds at edges); small positive sites exist at **edges**.
- More specific surface → larger negative charge.
- Reciprocal of average surface charge density (Å² per electronic charge): kaolinite 25 · clay mica and chlorite 50 · montmorillonite 100 · vermiculite 75. (Larger number = lower charge density.)
- In dry clay the negative charge is balanced by **exchangeable cations** (Ca²⁺, Mg²⁺, Na⁺, K⁺). With water, these cations and some anions form a **diffuse double layer** — cation concentration decreases with distance from the surface.
- **Water is dipolar** (H–O–H bond angle ≈ 105°) and is attracted to: (1) the negative clay surface, (2) the cations of the double layer, (3) by **hydrogen bonding** with surface oxygens, and (4) partially hydrated cations.
- **Double-layer water** = all water held by these forces; the innermost, strongly held layer is **adsorbed water** (more viscous than free water). This oriented water is what gives clays their **plasticity**.
- When clay content is ≳ 50 %, sand and silt grains "float" in a clay matrix and the clay minerals control soil behaviour.

---

## 5. Specific gravity of soil solids ($G_s$)

$$G_s = \frac{\text{unit weight of solids}}{\text{unit weight of water}}$$

Determined accurately in the lab. Typical: light-coloured quartz sands ≈ **2.65**; clayey and silty soils **2.6–2.9**.

**Table 2.4**

| Mineral | $G_s$ | Mineral | $G_s$ |
|---|---|---|---|
| Quartz | 2.65 | Biotite | 2.8–3.2 |
| Kaolinite | 2.6 | Muscovite | 2.76–3.1 |
| Illite | 2.8 | Hornblende | 3.0–3.47 |
| Montmorillonite | 2.65–2.80 | Limonite | 3.6–4.0 |
| Halloysite | 2.0–2.55 | Olivine | 3.27–3.7 |
| K-feldspar | 2.57 | Chlorite | 2.6–2.9 |
| Na/Ca feldspar | 2.62–2.76 | | |

---

## 6. Mechanical analysis (particle-size distribution)

| Method | Particle sizes | Principle |
|---|---|---|
| **Sieve analysis** | > 0.075 mm | shaking through stack of sieves |
| **Hydrometer analysis** | < 0.075 mm | sedimentation (Stokes' law) |

### 6.1 Sieves

- Sizes 100 mm → 6.3 mm are designated by opening; below that use sieve **numbers** (No. 4 → No. 400).
- **Commonly used US sieves:**

| No. | 4 | 10 | 20 | 30 | 40 | 60 | 100 | 140 | 200 |
|---|---|---|---|---|---|---|---|---|---|
| Opening (mm) | 4.75 | 2.00 | 0.850 | 0.600 | 0.425 | 0.250 | 0.150 | 0.106 | 0.075 |

- Successive sieve openings follow approximately:

$$\text{Opening}_i = \frac{\text{Opening}_{i-1}}{(2)^{0.25}} \tag{2.1}$$

(e.g., No. 5 = 4.75/1.1892 ≈ 4.00 mm; No. 50 ≈ 0.300 mm). The British and Australian standards use their own aperture series (Tables 2.7–2.8).

- Sieves are typically 203 mm (8 in.) in diameter. The smallest sieve for this test is **No. 200**.
- **Procedure:** oven-dry soil, break lumps; shake through stack (largest on top, pan at bottom). For cohesive soils, **wash** through the sieves as a slurry, then oven-dry what is retained.

**Calculation steps**
1. Mass retained on each sieve: $M_1, M_2, \dots, M_n$ and pan $M_p$.
2. Total mass $\Sigma M = M_1 + M_2 + \dots + M_n + M_p$.
3. Cumulative mass retained above the $i$th sieve: $M_1 + \dots + M_i$.
4. Mass passing $i$th sieve: $\Sigma M - (M_1 + \dots + M_i)$.
5. **Percent finer:**

$$F = \frac{\Sigma M - (M_1 + M_2 + \dots + M_i)}{\Sigma M}\times 100$$

6. Plot **percent finer (arithmetic axis) vs. particle size (log axis)** → **particle-size distribution curve**.

### 6.2 Hydrometer analysis

Based on sedimentation. Particles are assumed to be spheres obeying **Stokes' law**:

$$v = \frac{\rho_s - \rho_w}{18\,\eta}\,D^2 \tag{2.2}$$

($v$ = settling velocity, $\rho_s$ = particle density, $\rho_w$ = water density, $\eta$ = water viscosity, $D$ = particle diameter.)

Solving for $D$ with $v = L/t$ (settling distance / time) and $\rho_s = G_s\rho_w$:

$$D = \sqrt{\frac{18\eta v}{\rho_s - \rho_w}} \tag{2.3}$$
$$D = \sqrt{\frac{18\,\eta}{(G_s - 1)\rho_w}}\sqrt{\frac{L}{t}} \tag{2.5}$$

Practical form (with $\rho_w \approx 1$ g/cm³, $L$ in cm, $t$ in min, $D$ in mm, $\eta$ in g·s/cm²):

$$D\ (\text{mm}) = K\sqrt{\frac{L\ (\text{cm})}{t\ (\text{min})}} \tag{2.6}$$

$$K = \sqrt{\frac{30\,\eta}{G_s - 1}} \tag{2.7}$$

$K$ depends on $G_s$ and on temperature (through $\eta$). **Table 2.9** tabulates it, e.g.:

| $G_s$ | $K$ at 20 °C | $K$ at 25 °C |
|---|---|---|
| 2.60 | 0.01386 | 0.01306 |
| 2.65 | 0.01365 | 0.01286 |
| 2.70 | 0.01344 | 0.01267 |

(Higher temperature → lower viscosity → smaller $K$.)

**Test set-up**
- 50 g (sometimes 100 g) oven-dried soil; dispersing agent **sodium hexametaphosphate**; made up to **1000 mL** with distilled water in a sedimentation cylinder (457 mm high, 63.5 mm diameter).
- **ASTM 152H hydrometer** placed in the suspension; at time $t$ it reads the density in the vicinity of its bulb at depth $L$. At that moment, particles still in suspension at depth $L$ are *smaller than $D$* from Eq. (2.6) — larger ones have already settled below.
- The hydrometer is calibrated for $G_s = 2.65$ (correct if different). Effective down to ≈ **0.5 µm**.

**Effective depth $L$ for the 152H hydrometer**

$$L = L_1 + \frac12\left(L_2 - \frac{V_B}{A}\right) \tag{2.8}$$

with $L_2 = 14$ cm (bulb length), $V_B = 67$ cm³ (bulb volume), $A = 27.8$ cm² (cylinder cross-section). $L_1 = 10.5 - 0.164R$ cm (10.5 cm at $R=0$, 2.3 cm at $R=50$), so

$$L = 16.29 - 0.164\,R\ \text{(cm)} \tag{2.9}$$

($R$ = hydrometer reading corrected for meniscus.) Table 2.10 lists $L$ for each $R$: e.g., $R = 0 \to 16.3$ cm, $R = 20 \to 13.0$, $R = 40 \to 9.7$, $R = 60 \to 6.5$.

**Combining sieve + hydrometer curves:** a small discontinuity appears in the overlap because a sieve measures an *intermediate dimension* of the (irregular) grain, whereas the hydrometer gives the *diameter of an equivalent settling sphere*.

---

## 7. Particle-size distribution curve

**Key diameters (read from the curve; $D_x$ = size at which $x$ % is finer):**

| Parameter | Definition | Use |
|---|---|---|
| **Effective size $D_{10}$** | diameter at 10 % finer | good indicator of hydraulic conductivity/drainage of granular soil |
| **Uniformity coefficient $C_u$** | $C_u = \dfrac{D_{60}}{D_{10}}$ (2.10) | spread of grain sizes |
| **Coefficient of gradation (curvature) $C_c$** | $C_c = \dfrac{D_{30}^2}{D_{60}\,D_{10}}$ (2.11) | shape of the curve |

**Gravel/sand/fines percentages (USCS) from the curve.** Example: percent finer = 100 at 76.2 mm, 100 at 4.75 mm, 62 at 0.075 mm → gravel 0 %, sand 38 %, silt + clay 62 %.

**Types of gradation (Fig. 2.29)**

| Curve | Type | Description |
|---|---|---|
| I | **Poorly (uniformly) graded** | most grains the same size (steep curve) |
| II | **Well graded** | wide range of sizes (gentle curve) |
| III | **Gap graded** | two or more uniform fractions with missing sizes (flat portion) |

**Well-graded criteria:** $C_u > 4$ for gravels, $C_u > 6$ for sands, **and** $1 \le C_c \le 3$.

---

## 8. Worked examples

**Example 2.1 — Sieve analysis** (450 g sample).

| Sieve | Opening (mm) | Mass retained (g) | Cumulative retained (g) | % finer |
|---|---|---|---|---|
| 4 | 4.75 | 0 | 0 | 100 |
| 10 | 2.00 | 21.6 | 21.6 | 95.2 |
| 20 | 0.850 | 49.5 | 71.1 | 84.2 |
| 40 | 0.425 | 102.6 | 173.7 | 61.4 |
| 60 | 0.250 | 89.1 | 262.8 | 41.6 |
| 100 | 0.150 | 95.6 | 358.4 | 20.4 |
| 200 | 0.075 | 60.4 | 418.8 | 6.9 |
| Pan | — | 31.2 | 450 | 0 |

From the curve: $D_{60} = 0.41$, $D_{30} = 0.185$, $D_{10} = 0.09$ mm →
$C_u = 0.41/0.09 = 4.56$, $C_c = (0.185)^2/(0.41\times0.09) = 0.93$.

**Example 2.2 — Mixing two soils** (6000 kg of A + 4000 kg of B → 60 % A, 40 % B).
For each sieve: mass retained in mixture (%) = 0.6 × (A's % retained) + 0.4 × (B's % retained); then cumulate and subtract from 100.

| Sieve | 4 | 10 | 20 | 40 | 60 | 100 | 200 |
|---|---|---|---|---|---|---|---|
| % passing (mixture) | 92.08 | 73.76 | 58.0 | 41.98 | 23.90 | 13.42 | 5.86 |

Book reads $D_{60} \approx 1$ mm, $D_{30} = 0.3$ mm, $D_{10} = 0.13$ mm and gives $C_c = 0.69$ and $C_u = 10$.
*Heads-up:* the book's $C_u$ line uses $D_{10} = 0.1$ (→ 10), while $C_c$ uses 0.13. With 0.13, $C_u$ would be ≈ 7.7. If you log-interpolate the table I get roughly $D_{60} \approx 0.95$, $D_{10} \approx 0.11$, $C_u \approx 8.6$, $C_c \approx 0.86$. The conclusion is the same either way: $C_c < 1$, so the mixture is **not well graded** by the USCS criteria.

**Example 2.3 — Combined sieve + hydrometer (AASHTO sizes).**
From the plot: passing 2 mm = 92 %; passing 0.075 mm = 31 %; passing 0.002 mm = 10 % →
Gravel = 100 − 92 = **8 %**; Sand = 92 − 31 = **61 %**; Silt = 31 − 10 = **21 %**; Clay = **10 %**.

---

## 9. Particle shape

Three categories:

| Shape | Typical particles | Notes |
|---|---|---|
| **Bulky** | gravel, sand, silt (product of mechanical weathering) | described as angular, subangular, subrounded, rounded; grains near their source are very angular, long-transported grains become rounded |
| **Flaky** | clay minerals, micas | very low sphericity (≈ 0.01 or less) |
| **Needle-shaped** | some coral deposits, attapulgite clays | uncommon |

Shape of granular particles affects maximum/minimum void ratio, shear strength parameters, compressibility, etc.

**Angularity:**

$$A = \frac{\text{average radius of corners and edges}}{\text{radius of the maximum inscribed sphere}} \tag{2.12}$$

**Sphericity of bulky particles:**

$$S = \frac{D_e}{L_p}, \qquad D_e = \sqrt[3]{\frac{6V}{\pi}} \tag{2.13}$$

where $D_e$ = equivalent-sphere diameter, $V$ = particle volume, $L_p$ = particle length.

---

## 10. Chapter summary

1. Rocks: **igneous, sedimentary, metamorphic**.
2. Soil forms by **mechanical and chemical weathering** of rock.
3. By size: gravel, sand, silt, clay. USCS limits: gravel 76.2–4.75 mm; sand 4.75–0.075 mm; fines < 0.075 mm.
4. Clays: flake-shaped microscopic particles; clay minerals are complex **aluminium silicates** with a **net negative charge**; a **diffuse double layer** of water gives **plasticity**.
5. Mechanical analysis = **sieve** (> 0.075 mm) + **hydrometer** (< 0.075 mm).
6. Sieve analysis: percent finer = $100 - \dfrac{\text{cumulative mass retained}}{\text{total mass}}\times 100$. Hydrometer analysis: particle diameter $D = K\sqrt{L/t}$ at each reading time.

---

## 11. Formula cheat-sheet

| Quantity | Formula |
|---|---|
| Sieve openings | $\text{Opening}_i = \text{Opening}_{i-1}/2^{0.25}$ |
| Percent finer | $F = \dfrac{\Sigma M - \text{cum. retained}}{\Sigma M}\times 100$ |
| Stokes' law | $v = \dfrac{(\rho_s - \rho_w)D^2}{18\eta}$ |
| Hydrometer diameter | $D\,(\text{mm}) = K\sqrt{L/t}$, $K = \sqrt{30\eta/(G_s-1)}$ |
| Effective depth (152H) | $L = 16.29 - 0.164R$ cm |
| Uniformity coefficient | $C_u = D_{60}/D_{10}$ |
| Coefficient of gradation | $C_c = D_{30}^2/(D_{60}D_{10})$ |
| Angularity | $A = r_{avg\ corners}/r_{inscribed}$ |
| Sphericity | $S = D_e/L_p$, $D_e = (6V/\pi)^{1/3}$ |

---

*End-of-chapter problems (2.1–2.15, plus critical-thinking problems 2.C.1–2.C.2) practise: computing $C_u$/$C_c$ and judging gradation; sieve-analysis tables and grain-size curves; combined sieve + hydrometer curves with soil fractions per MIT, USDA and AASHTO; hydrometer diameter calculations from $G_s$, temperature, $L$ and $t$; and blending soils to get a target gradation.*
