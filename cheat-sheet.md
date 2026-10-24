# Soil Mechanics Cheat Sheet (Ch. 1–5)

Condensed from my own study notes of Das & Sobhan, *Principles of Geotechnical Engineering*, 9th ed. Last updated 24 Oct 2026.

## Chapter 1: history, names and dates

Learn the four periods and the one-line contribution of each person; Terzaghi's 1925 consolidation book marks the start of modern soil mechanics.

| Period | Years | Theme |
| --- | --- | --- |
| Preclassical | 1700–1776 | Natural slopes, unit weights, semi-empirical earth pressure |
| Classical, Phase I | 1776–1856 | Rigorous earth-pressure theory (mostly French) |
| Classical, Phase II | 1856–1910 | Sand tests, permeability, stress distribution, dilatancy |
| Modern | 1910–1927 | Fundamental behaviour of clays |

| Person | Year | Contribution |
| --- | --- | --- |
| Gautier | 1717 | Natural slopes (angle of repose), unit weights |
| Belidor | 1729 | Earth-pressure theory, early classification |
| Gadroy | 1746 | First lab model wall, slip planes |
| Coulomb | 1776 | Sliding wedge, friction + cohesion |
| Poncelet | 1840 | Graphical earth pressure, symbol φ, bearing capacity |
| Collin | 1846 | Deep slips in clay, cycloid surfaces |
| Darcy | 1856 | Permeability law |
| Rankine | 1857 | Simplified Coulomb earth pressure |
| Boussinesq | 1885 | Stress in an elastic half-space |
| Reynolds | 1887 | Dilatancy in sand |
| Atterberg | 1908–11 | Consistency limits, clay fraction (< 2 µm) |
| Fellenius | 1918, 1926 | Circular-arc slope stability (φ = 0) |
| Terzaghi | 1925 | Consolidation theory, *Erdbaumechanik* |
| Skempton | 1948, 1954 | φ = 0 concept; pore-pressure parameters A and B |
| Bishop and Henkel | 1957 | Triaxial test book |

- **Pisa:** weak clay about 11 m deep compressed unevenly. Lean about 5.5° before 1990; about 70 t of soil removed from the north side cut it to about 5°.
- **Terzaghi (1883–1963):** father of modern soil mechanics. First ISSMFE conference was Harvard 1936; ISSMFE became ISSMGE in 1997.

## Chapter 2: origin of soil and grain size

Soil is weathered rock; exam marks come from the clay-mineral comparison, the size limits, and Cu and Cc.

| Rock type | Origin | Examples |
| --- | --- | --- |
| Igneous | Cooled magma; intrusive = coarse, extrusive = fine | Granite / rhyolite, gabbro / basalt |
| Sedimentary | Sediments compacted and cemented | Sandstone, shale, limestone, conglomerate |
| Metamorphic | Heat and pressure, no melting | Gneiss, slate, schist, marble, quartzite |

- **Weathering:** mechanical breaks rock without changing composition (freeze–thaw, temperature, water). Chemical makes new minerals (clay minerals) with water + CO₂.
- **Residual** soil stays in place; **transported** soil is glacial, alluvial (rivers), lacustrine (lakes), marine, aeolian (wind) or colluvial (gravity).
- **Bowen series:** olivine → augite → hornblende → biotite, and Ca- to Na-feldspar, then orthoclase → muscovite → quartz. Quartz resists weathering most.

| | Kaolinite | Illite | Montmorillonite |
| --- | --- | --- | --- |
| Layers | 1:1, about 7.2 Å | 2:1, about 10 Å | 2:1, 9.6 Å to fully separated |
| Bond between layers | Hydrogen (strong) | Potassium ions | Weak van der Waals, water enters |
| Specific surface | about 15 m²/g | about 80 m²/g | about 800 m²/g |
| Behaviour | Stable, low swelling | Intermediate | Very high swelling and shrinkage |

Clay particles carry a net negative charge and a diffuse double layer of water, which gives plasticity. Quartz sands have Gs about 2.65; clays and silts 2.6–2.9.

| System | Gravel (mm) | Sand (mm) | Silt (mm) | Clay (mm) |
| --- | --- | --- | --- | --- |
| USDA | 76.2–2 | 2–0.05 | 0.05–0.002 | < 0.002 |
| AASHTO | 76.2–2 | 2–0.075 | 0.075–0.002 | < 0.002 |
| USCS | 76.2–4.75 | 4.75–0.075 | Fines < 0.075 (silt + clay) | |

Sieves: No. 4 = 4.75 mm, No. 10 = 2 mm, No. 40 = 0.425 mm, No. 200 = 0.075 mm. Sieve test is for particles above 0.075 mm; hydrometer is for particles below it.

```latex
F = \frac{\Sigma M - \text{cumulative retained}}{\Sigma M} \times 100
```

```latex
D\ (\text{mm}) = K \sqrt{\frac{L\ (\text{cm})}{t\ (\text{min})}}, \qquad L = 16.29 - 0.164\,R \ \text{cm}
```

```latex
C_u = \frac{D_{60}}{D_{10}}, \qquad C_c = \frac{D_{30}^{2}}{D_{60}\, D_{10}}
```

- **Well graded:** Cu > 4 for gravel, Cu > 6 for sand, **and** 1 ≤ Cc ≤ 3.
- **Stokes' law:** bigger particles settle faster (v proportional to D²); a hotter suspension has lower viscosity, so K is smaller.
- **Example 2.1** (450 g): Cu = 0.41 / 0.09 = 4.56 and Cc = 0.185² / (0.41 × 0.09) = 0.93, so not well graded.

## Chapter 3: weight–volume relationships

Draw the three-phase diagram first, then S·e = w·Gs links almost everything.

| Quantity | Definition | Notes |
| --- | --- | --- |
| Void ratio e | Vv / Vs | Can exceed 1 |
| Porosity n | Vv / V | Always below 1 |
| Saturation S | Vw / Vv | 0% dry, 100% saturated |
| Water content w | Ww / Ws | Divide by solids, not total |
| Unit weight γ | W / V | γ = 9.81 × ρ / 1000 in kN/m³ |
| Dry unit weight γd | Ws / V | γd = γ / (1 + w) |

Constants: γw = 9.81 kN/m³ = 62.4 lb/ft³, ρw = 1000 kg/m³.

```latex
S\,e = w\,G_s \qquad e = \frac{n}{1-n} \qquad n = \frac{e}{1+e}
```

```latex
\gamma_d = \frac{G_s\gamma_w}{1+e} \qquad \gamma = \frac{(1+w)\,G_s\gamma_w}{1+e} \qquad \gamma_{sat} = \frac{(G_s+e)\,\gamma_w}{1+e}
```

```latex
D_r = \frac{e_{max} - e}{e_{max} - e_{min}}
```

- **Saturated soil:** S = 1, so e = w·Gs. Also γsat = γd + n·γw.
- **Porosity forms:** γd = Gsγw(1 − n) and wsat = n / [(1 − n)Gs].
- **Relative density** (sands and gravels only): 0–15% very loose, 15–50 loose, 50–70 medium, 70–85 dense, 85–100 very dense.
- **Fines effect:** up to about 30% non-plastic fines, emax and emin fall (fines fill voids); above about 40% they rise.

| Example | Key result |
| --- | --- |
| 3.2: V = 1.2 m³, M = 2350 kg, w = 8.6%, Gs = 2.71 | e = 0.503, n = 0.335, S = 46.3%, Vw = 0.186 m³ |
| 3.7: emax 0.75, emin 0.40, e = 0.67 | Dr = 22.9% |
| 3.8: clean sand, D50 = 0.5 mm | emax 0.875, emin 0.525, Dr = 61.4% |

**Recipe:** (1) sketch the phase diagram; (2) choose a basis, Vs = 1 if you know e, V = 1 if you know n; (3) fill in from Gs, w, γw; (4) use S·e = w·Gs; (5) keep units consistent. For borrow-pit problems the dry weight of solids stays the same.

## Chapter 4: plasticity and soil structure

As water content rises a fine-grained soil goes solid → semisolid → plastic → liquid, and the three boundaries are SL, PL and LL (all in %).

| Limit | Boundary | Test definition |
| --- | --- | --- |
| Shrinkage limit SL | Solid / semisolid | Below it, drying causes no more volume change |
| Plastic limit PL | Semisolid / plastic | Soil crumbles at 3.2 mm threads |
| Liquid limit LL | Plastic / liquid | Groove closes 12.5 mm at 25 blows (cup, 10 mm drop), or 20 mm penetration in 5 s (30°, 80 g cone) |

```latex
PI = LL - PL \qquad LI = \frac{w - PL}{LL - PL} \qquad CI = \frac{LL - w}{LL - PL} \qquad LI + CI = 1
```

```latex
A = \frac{PI}{\%\ \text{clay-size fraction (finer than 2 }\mu\text{m)}}
```

```latex
SL = \frac{M_1 - M_2}{M_2}(100) - \frac{(V_i - V_f)\,\rho_w}{M_2}(100) \qquad SR = \frac{M_2}{V_f\,\rho_w} \qquad G_s = \frac{1}{\frac{1}{SR} - \frac{SL}{100}}
```

```latex
VS = SR\,(w - SL) \qquad LS = 100\left[1 - \left(\frac{100}{VS + 100}\right)^{1/3}\right]
```

| PI | Plasticity (Burmister) | LI | Meaning |
| --- | --- | --- | --- |
| 0 | Nonplastic | < 0 | Stiff, often overconsolidated |
| 1–5 | Slight | 0 | At PL |
| 5–10 | Low | 1 | At LL |
| 10–20 | Medium | > 1 | Sensitive clay, flows when remoulded |
| 20–40 | High | | |
| > 40 | Very high | | |

| Mineral | Activity A | Swelling |
| --- | --- | --- |
| Kaolinite | 0.3–0.5 | Low |
| Illite | 0.5–1.2 | Medium |
| Montmorillonite | 1.5–7.0 | Very high |

- **One-point LL (cup):** LL = wN (N / 25)^0.121, valid for N about 20–30.
- **Plasticity chart:** PI on y, LL on x. A-line: PI = 0.73 (LL − 20). U-line: PI = 0.9 (LL − 8). Above the A-line is clay, below is silt or organic soil.
- **Example 4.5:** SL = 46.18 − 28.9 = 17.28%. **Example 4.6:** SR = 30.1 / 15.9 = 1.89 and Gs = 2.81. **Example 4.7:** VS = 1.89 (28 − 17.28) = 20.26% and LS = 5.96%.

| Structure | Key facts |
| --- | --- |
| Single-grained (sand, gravel) | Loose or dense; equal spheres: simple cubic e = 0.91, simple stagger 0.65, double stagger 0.43, pyramidal 0.35 |
| Honeycombed (fine sand, silt) | Large e; carries static load but collapses under shock |
| Dispersed clay | Particles settle roughly parallel |
| Flocculent clay | Edge-to-face contact, open, high e; marine clays are highly flocculent |
| Clay hierarchy | Domains → clusters (light microscope) → peds (naked eye) |

## Chapter 5: soil classification

AASHTO splits at 35% passing No. 200 and No. 10; USCS splits at 50% passing No. 200 and No. 4. Mixing these up is the most common lost mark.

| | AASHTO | USCS |
| --- | --- | --- |
| Coarse / fine split | 35% passes No. 200 (granular if ≤ 35%) | 50% passes No. 200 (coarse if < 50%) |
| Gravel / sand split | No. 10 (2 mm) | No. 4 (4.75 mm) |
| Plasticity tested on | Fraction passing No. 40 | Fraction passing No. 40 |
| Organic soils | No place for them | OL, OH, Pt |

**USDA:** only material passing 2 mm is plotted on the triangle, so with gravel present re-scale first.

```latex
\text{Modified \%} = \frac{\%\ \text{of sand, silt or clay}}{100 - \%\ \text{gravel}} \times 100
```

**AASHTO:** go through the table left to right and take the first group that fits.

| Group set | Test | Groups |
| --- | --- | --- |
| Granular, F200 ≤ 35% | A-1-a, A-1-b, A-3, then A-2-4 to A-2-7 | GI = 0 for A-1, A-2-4, A-2-5, A-3 |
| Silt–clay, F200 > 35% | A-4 (LL ≤ 40, PI ≤ 10), A-5 (LL ≥ 41, PI ≤ 10), A-6 (LL ≤ 40, PI ≥ 11), A-7 (LL ≥ 41, PI ≥ 11) | A-7-5 if PI ≤ LL − 30, A-7-6 if PI > LL − 30 |

```latex
GI = (F_{200} - 35)\left[0.2 + 0.005\,(LL - 40)\right] + 0.01\,(F_{200} - 15)(PI - 10)
```

- **GI rules:** negative gives 0; round to the nearest whole number; for A-2-6 and A-2-7 use only the PI term, 0.01 (F200 − 15)(PI − 10). Higher GI means worse subgrade.
- **Example 5.3:** F200 = 95, LL = 60, PI = 40 gives A-7-6 and GI = 18 + 24 = 42, so **A-7-6(42)**.
- **Example 5.5:** F200 = 58, LL = 30, PI = 10 gives A-4 and GI = 3.45. The rounding rule says 3, so A-4(3); the book prints 4. State which convention you used.

**USCS symbols**

| Soil | Fines | Condition | Symbol |
| --- | --- | --- | --- |
| Gravel (more than half of coarse on No. 4) | < 5% | Cu ≥ 4 and 1 ≤ Cc ≤ 3 | GW; otherwise GP |
| Sand | < 5% | Cu ≥ 6 and 1 ≤ Cc ≤ 3 | SW; otherwise SP |
| Gravel or sand | > 12% | PI < 4 or below A-line | GM / SM |
| Gravel or sand | > 12% | PI > 7 and on or above A-line | GC / SC |
| Gravel or sand | 5–12% | Dual symbol, gradation first | e.g. SP-SC, GW-GM |
| Fine, LL < 50 | | PI > 7 and on or above A-line | CL |
| Fine, LL < 50 | | PI < 4 or below A-line | ML |
| Fine, LL < 50 | | 4 ≤ PI ≤ 7 in the hatched zone | CL-ML |
| Fine, LL ≥ 50 | | On or above A-line / below A-line | CH / MH |
| Organic | | Oven-dried LL / undried LL < 0.75 | OL (LL < 50) or OH (LL ≥ 50) |

- **A-line:** PI = 0.73 (LL − 20). **U-line:** PI = 0.9 (LL − 8).
- **Base names:** CL lean clay, CH fat clay, ML silt, MH elastic silt, CL-ML silty clay.
- **Fine-grained naming (percent retained on No. 200):** below 15% base name only; 15–29% add "with sand" or "with gravel"; 30% or more add the prefix "sandy" or "gravelly", whichever is greater.
- **Coarse-grained naming:** add "with sand" or "with gravel" when the other coarse part is 15% or more.
- **Example 5.4 (same soil as 5.5):** 58% fines, LL = 30, PI = 10 gives CL, sandy lean clay. A-line at LL 30 is 7.3, and PI 10 is above it.
- **Quick check:** LL = 65, PI = 20; A-line is 0.73 × 45 = 32.85, PI is below it, so MH.

**Recipe:** USCS: F200 under 50% is coarse, otherwise fine; coarse soils check fines (5%, 12%) then Cu and Cc or the A-line; fine soils use LL against 50 and the chart. AASHTO: percent passing 10, 40, 200, then LL and PI, then GI.

## Exam traps and last-night checklist

Most lost marks come from six slips: wrong denominator, one gradation coefficient, mixed units, skipped gravel correction, swapped thresholds, wrong sample fraction.

| Trap | Do this instead |
| --- | --- |
| Water content w | Divide by the weight of solids: w = Ww / Ws |
| Gradation | Check Cu **and** Cc (1 to 3); gravel needs Cu ≥ 4, sand Cu ≥ 6 |
| Units | γ (kN/m³) = 9.81 × ρ (kg/m³) / 1000 |
| USDA with gravel | Re-scale by 100 − % gravel before plotting |
| Thresholds | AASHTO 35% and No. 10; USCS 50% and No. 4 |
| Atterberg tests | LL and PI use the fraction passing No. 40 |
| GI rounding | Round to the nearest whole number and say so (3.45 gives 3) |

- [ ] Write every formula from memory on blank paper, then compare with this sheet
- [ ] Redo Examples 2.1, 3.2, 4.5 and 5.3 without looking
- [ ] Draw the phase diagram and label V and W on each side
- [ ] Sketch the plasticity chart: A-line, U-line, LL = 50, hatched CL-ML zone
- [ ] Say the four periods of Chapter 1 and three names for each from memory
- [ ] Pack calculator, pencil, a spare calculator battery and ID
- [ ] Sleep: stop studying at least an hour before bed

For every calculation: write the formula, substitute with units, box the answer. The first two steps carry the partial marks.
