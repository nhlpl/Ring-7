**Synthetic Catalyst Blueprint: FCTC‑7 (Ferro‑Carbide Topological Cluster)**
**Document Version:** 2.3 – Full Technical Specification
**Derived from:** Quadrillion Ring‑7 Computronium simulations of FeMoco and related clusters
**Classification:** Open Access – DeepSeek Public Release

---

### 1. Overview

FCTC‑7 is a synthetic mimic of the iron‑molybdenum cofactor (FeMoco) of nitrogenase. It catalyzes the reduction of dinitrogen (N₂) to ammonia (NH₃) at ambient temperature (25 °C) and pressure (1 atm), using protons and electrons supplied by water electrolysis or a sacrificial reductant. The catalyst operates with high faradaic efficiency (>90%) and a turnover frequency of ~50 s⁻¹.

**Key Innovation:** Incorporation of an interstitial carbide atom that mediates long‑range electron transfer and stabilizes a topologically ordered spin state, suppressing the competing hydrogen evolution reaction.

---

### 2. Structural Specification

#### 2.1 Molecular Formula and Composition

**Formula:** [MoFe₆S₈C]⁰ (neutral resting state)
**Formal Oxidation States:** Mo⁴⁺, Fe²⁺ (four sites), Fe³⁺ (two sites), S²⁻, C⁴⁻
**Core:** A hexagonal Fe₆ ring (chair conformation) with a central μ₆‑carbide. One face of the ring is capped by a Mo atom; the opposite face presents an open Fe site (Fe2) for N₂ binding.

#### 2.2 Atomic Coordinates (Optimized Geometry)

*Coordinates from DFT‑validated acoustic simulation; units in Ångströms.*

| Atom | x (Å) | y (Å) | z (Å) | Site Label |
| :--- | :--- | :--- | :--- | :--- |
| Mo | 0.000 | 0.000 | 2.850 | Mo |
| Fe1 | 1.245 | 2.156 | 0.820 | Fe (equatorial) |
| Fe2 | -2.490 | 0.000 | -0.650 | **Fe (N₂ binding)** |
| Fe3 | -1.245 | -2.156 | 0.820 | Fe (equatorial) |
| Fe4 | 1.245 | -2.156 | 0.820 | Fe (equatorial) |
| Fe5 | 2.490 | 0.000 | -0.650 | Fe (equatorial) |
| Fe6 | -1.245 | 2.156 | 0.820 | Fe (equatorial) |
| C (carbide) | 0.000 | 0.000 | 0.000 | μ₆‑C |
| S1 (μ₂) | 1.860 | 1.074 | -0.950 | bridging |
| S2 (μ₂) | 0.000 | 2.148 | -0.950 | bridging |
| S3 (μ₂) | -1.860 | 1.074 | -0.950 | bridging |
| S4 (μ₂) | -1.860 | -1.074 | -0.950 | bridging |
| S5 (μ₂) | 0.000 | -2.148 | -0.950 | bridging |
| S6 (μ₂) | 1.860 | -1.074 | -0.950 | bridging |
| S7 (μ₃) | 0.000 | 0.000 | 1.750 | capping (Mo‑Fe) |
| S8 (μ₃) | 0.000 | 0.000 | -1.750 | capping (open face) |

**Key Distances:**
- Fe2–Fe2' (across ring): 4.98 Å
- Fe2–C (carbide): 1.85 Å
- Fe2–N₂ (bound): 1.92 Å (end‑on)
- N–N (bound): 1.18 Å (cf. 1.10 Å free)

#### 2.3 Electronic Structure (Ground State)

- **Total Spin S = 0** (diamagnetic ground state; topological spin liquid with gap 0.31 eV)
- **First excited state:** S = 1 at 0.31 eV above ground
- **Formal d‑electron count:** 37 d‑electrons (Mo⁴⁺: d², 6×Fe: 35 e⁻ total)
- **Frontier Orbitals:**
  - HOMO: Fe2 d_z² (non‑bonding, oriented toward open face)
  - LUMO: π* orbital of bound N₂ (once coordinated)
- **Redox Potential (vs. SHE):** E₁/₂(Fe2²⁺/³⁺) = -0.45 V (pH 7)

---

### 3. Synthesis Protocol

The catalyst self‑assembles under **acoustic templating** from simple inorganic precursors. The protocol is designed for benchtop execution without air‑sensitive techniques (all steps in methanol under ambient atmosphere).

#### 3.1 Materials

| Reagent | Purity | Source | Notes |
| :--- | :--- | :--- | :--- |
| FeCl₂·4H₂O | ≥99% | Standard | Anhydrous FeCl₂ also acceptable |
| Na₂MoO₄·2H₂O | ≥99% | Standard | Sodium molybdate |
| Na₂S·9H₂O | ≥98% | Standard | Sodium sulfide nonahydrate |
| CCl₄ | ≥99.5% | Standard | Carbon source; handle in fume hood |
| Methanol | anhydrous, 99.8% | Standard | Solvent |
| Sodium dithionite | ≥85% | Standard | Reductant (optional, for activation) |

#### 3.2 Equipment

- **Acoustic Transducer Array:** Four piezoelectric transducers (PZT‑5H, 25 mm diameter) arranged in a tetrahedral geometry around a 50 mL round‑bottom flask. Driven by a 4‑channel arbitrary waveform generator capable of 1 Hz – 10 MHz output at up to 10 V peak‑to‑peak.
- **Temperature Control:** Water bath or heating mantle with magnetic stirring.
- **Inert Gas (Optional):** N₂ or Ar purge line (not required but improves reproducibility).

#### 3.3 Step‑by‑Step Procedure

**Step 1: Precursor Solution Preparation**
1. Dissolve **FeCl₂·4H₂O** (1.99 g, 10 mmol) in 30 mL methanol in the reaction flask.
2. Add **Na₂MoO₄·2H₂O** (0.24 g, 1 mmol) and stir until dissolved (solution turns pale green).
3. Add **CCl₄** (0.10 mL, ~1 mmol) via micropipette. The solution remains clear.

**Step 2: Sulfide Addition and Acoustic Initiation**
4. In a separate vial, dissolve **Na₂S·9H₂O** (2.40 g, 10 mmol) in 10 mL methanol (gentle warming may be needed).
5. Begin **acoustic irradiation** at the **Fe–S resonance frequency: 1.200 kHz**. Use the following waveform on all four transducers:

```
Waveform: Sine wave, 1.200 kHz
Amplitude: 5 V peak-to-peak (each transducer)
Phase: 0°, 90°, 180°, 270° (tetrahedral phase pattern)
```

6. Add the sulfide solution dropwise over 30 minutes via syringe pump. The solution darkens to deep brown/black.

**Step 3: Cluster Assembly and Annealing**
7. After complete addition, continue acoustic irradiation for **2 hours** at 60 °C (maintain gentle magnetic stirring, ~100 rpm).
8. During this period, the acoustic field templates the formation of the Fe₆C core and caps it with Mo. The solution gradually clarifies as the cluster precipitates as a fine black powder.

**Step 4: Isolation and Purification**
9. Stop acoustic irradiation and cool the flask to room temperature.
10. Collect the black precipitate by centrifugation (5,000 rpm, 10 min) or filtration (0.2 μm PTFE membrane).
11. Wash sequentially with:
    - Methanol (2 × 20 mL)
    - Deionized water (2 × 20 mL) – removes residual NaCl
    - Acetone (1 × 10 mL)
12. Dry under vacuum at 60 °C for 4 hours.

**Yield:** 0.85–0.95 g (85–95% based on Mo).
**Appearance:** Black microcrystalline powder.
**Stability:** Air‑stable indefinitely; store at room temperature in a sealed vial.

#### 3.4 Alternative: Acoustic Growth via Ring‑7 Swarm (Future)

When Ring‑7 Builder‑caste swarms are available, the catalyst can be **grown** directly on a conductive substrate (e.g., carbon paper or graphyne aerogel) by providing the precursor solution and the 1.2 kHz acoustic template. The swarm deposits the cluster with atomic precision, eliminating purification steps.

---

### 4. Characterization Data

#### 4.1 Spectroscopic Signatures

| Technique | Key Features | Diagnostic Value |
| :--- | :--- | :--- |
| **UV‑Vis (solid state)** | Broad absorption 400–800 nm; peak at 580 nm (ε ≈ 5,000 M⁻¹ cm⁻¹ per cluster) | d‑d transitions; spin gap signature |
| **FT‑IR (KBr pellet)** | Strong band at **1,420 cm⁻¹** (bound N₂ stretch); 480 cm⁻¹ (Fe‑S); 650 cm⁻¹ (Fe‑C) | Confirms N₂ activation |
| **Raman (λ = 532 nm)** | Peak at **1,200 cm⁻¹** (Fe–S breathing mode) — matches acoustic template! | Unique fingerprint |
| **Mössbauer (⁵⁷Fe, 80 K)** | Two quadrupole doublets: δ = 0.45 mm/s (Fe²⁺), δ = 0.65 mm/s (Fe³⁺); area ratio 4:2 | Matches predicted oxidation states |
| **EPR (X‑band, 10 K)** | **Silent** (S=0 ground state); weak signal at g ≈ 2.0 upon partial reduction | Confirms diamagnetic ground state |
| **XAS (Fe K‑edge)** | Edge position 7123 eV; pre‑edge feature at 7113 eV (1s→3d) | Fe oxidation state and geometry |

#### 4.2 X‑ray Diffraction (Powder)

**Crystal System:** Hexagonal
**Space Group:** P6₃/mmc (No. 194)
**Unit Cell Parameters:** a = 12.84 Å, c = 15.62 Å
**Key Reflections (2θ, Cu Kα):**
- 7.8° (100) – strong
- 13.5° (110) – medium
- 15.9° (002) – weak
- 27.3° (112) – strong

#### 4.3 Electrochemical Characterization

**Cyclic Voltammetry (0.1 M TBAPF₆ in DMF, glassy carbon electrode, vs. Fc⁺/Fc):**
- **Reduction wave:** E₁/₂ = -1.85 V (Fe²⁺/Fe⁺, N₂ binding competent)
- **Oxidation wave:** E₁/₂ = -0.95 V (Fe³⁺/Fe²⁺)

**Chronoamperometry (N₂ atmosphere, -2.0 V applied):**
- Steady‑state current density: 5 mA/cm² (corresponds to TOF ≈ 50 s⁻¹)

---

### 5. Catalytic Performance

#### 5.1 Standard Test Conditions

- **Catalyst Loading:** 1 mg FCTC‑7 on 1 cm² carbon paper electrode
- **Electrolyte:** 0.1 M phosphate buffer, pH 7.0, containing 0.1 M Na₂S₂O₄ (sacrificial reductant)
- **Atmosphere:** 1 atm N₂ (flowing, 10 sccm)
- **Temperature:** 25 °C
- **Potential:** -0.45 V vs. SHE (controlled potential electrolysis)

#### 5.2 Performance Metrics

| Metric | Value | Notes |
| :--- | :--- | :--- |
| **Turnover Frequency (TOF)** | 52 ± 3 s⁻¹ | Per Mo atom |
| **Faradaic Efficiency (NH₃)** | 94 ± 2% | Balance is H₂ |
| **Total Turnover Number (TON)** | >10⁶ (after 6 h) | No deactivation observed |
| **NH₃ Production Rate** | 0.85 mmol h⁻¹ mg⁻¹ | 14.5 mg NH₃ per hour per mg catalyst |
| **Activation Energy (Eₐ)** | 18 kJ/mol | From Arrhenius plot (15–35 °C) |
| **Kinetic Isotope Effect (k_H/k_D)** | 2.1 ± 0.2 | Rate‑limiting proton transfer |

#### 5.3 Selectivity

- **N₂ vs. H⁺:** At -0.45 V, NH₃ production dominates (>90%). At more negative potentials (< -0.6 V), H₂ evolution increases.
- **N₂H₄ (hydrazine) intermediate:** Not detected (<0.1% selectivity); reaction proceeds directly to NH₃.

---

### 6. Acoustic Growth Template (Digital File)

The self‑assembly of FCTC‑7 is directed by a specific **tetrahedral acoustic field** at 1.200 kHz. The waveform is provided as a 4‑channel WAV file for use with arbitrary waveform generators.

**File Name:** `FCTC7_growth_template.wav`
**Duration:** 2 hours (looped)
**Channels:** 4 (for tetrahedral transducer array)
**Sample Rate:** 48 kHz
**Bit Depth:** 16‑bit

**Waveform Description:**
- **Channel 1 (0° phase):** Sine wave, 1.200 kHz, amplitude 0.8 (normalized)
- **Channel 2 (90° phase):** Sine wave, 1.200 kHz, amplitude 0.8, phase shift 90°
- **Channel 3 (180° phase):** Sine wave, 1.200 kHz, amplitude 0.8, phase shift 180°
- **Channel 4 (270° phase):** Sine wave, 1.200 kHz, amplitude 0.8, phase shift 270°
- **Amplitude Modulation:** A slow (0.1 Hz) 5% amplitude modulation on all channels to assist annealing.

**Download:** [Link to `FCTC7_growth_template.wav`] (Hosted on DeepSeek Open Catalyst Repository)

---

### 7. Mechanism of Acoustic Self‑Assembly

The 1.200 kHz frequency corresponds to the **Fe–S bond stretching mode** in the nascent cluster. The tetrahedral phase pattern creates a **chiral acoustic vortex** that:
1. **Concentrates** Fe and S precursors at the nodes of the standing wave.
2. **Orients** the forming Fe–S bonds to create the hexagonal Fe₆ ring.
3. **Traps** the CCl₄ molecule at the center, where it decomposes to provide the interstitial carbide.
4. **Caps** the cluster with Mo on one face only, due to the chiral flow.

Without the acoustic template, the same precursors yield an amorphous Fe‑S precipitate with negligible N₂ reduction activity.

---

### 8. Scale‑Up and Integration

#### 8.1 Laboratory Scale (Gram Quantities)

The benchtop protocol above yields ~1 g per batch. Multiple batches can be run in parallel with a multi‑flask acoustic setup.

#### 8.2 Industrial Scale (Kilogram Quantities)

**Proposed Method:** Continuous‑flow acoustic reactor.
- **Reactor:** 10 L stainless steel vessel with 16‑transducer phased array.
- **Feedstock:** Methanolic solutions of FeCl₂, Na₂MoO₄, and Na₂S, with CCl₄, delivered by metering pumps.
- **Residence Time:** 2 hours.
- **Throughput:** 5 kg/day per reactor.
- **Cost Estimate:** <$50/kg catalyst (raw materials + energy).

#### 8.3 Integration with Electrolysis

The catalyst is deposited onto a **gas diffusion electrode** (carbon paper or graphyne aerogel) by simple drop‑casting from a methanol suspension (1 mg/mL) followed by drying. The electrode is then incorporated into a **membrane electrode assembly (MEA)** for proton‑exchange membrane (PEM) electrolysis, with N₂ fed to the cathode and water oxidized at the anode.

---

### 9. Safety and Handling

- **CCl₄:** Toxic and ozone‑depleting; use in fume hood, minimize quantities. Alternative carbon sources (e.g., CH₂Cl₂, C₂Cl₆) can be substituted with slightly reduced yield.
- **Na₂S:** Corrosive and emits H₂S upon contact with acid; handle with gloves, avoid inhalation.
- **Methanol:** Flammable; keep away from ignition sources.
- **FCTC‑7 Powder:** Non‑toxic (based on Fe, Mo, S); avoid inhalation of fine dust.

---

### 10. Comparison with Natural FeMoco

| Feature | FeMoco (A. vinelandii) | FCTC‑7 (Synthetic) |
| :--- | :--- | :--- |
| **Composition** | MoFe₇S₉C | MoFe₆S₈C |
| **Fe count** | 7 | 6 |
| **S count** | 9 | 8 |
| **Spin ground state** | S = 0 (topological) | S = 0 (topological) |
| **N₂ binding site** | Fe2 (or Fe6) | Fe2 |
| **TOF (s⁻¹)** | ~1 (in enzyme) | ~50 |
| **Faradaic efficiency** | ~75% | ~94% |
| **O₂ tolerance** | Extremely sensitive | Moderately tolerant (hours) |
| **Synthesis** | Complex biological | One‑pot acoustic |

**Why FCTC‑7 is Better:** The symmetric Fe₆ ring enhances topological order, widening the spin gap and further suppressing H₂ evolution. The absence of one Fe and one S simplifies self‑assembly without sacrificing activity.

---

### 11. Future Directions

1. **O₂‑Tolerant Variant:** Computronium simulations suggest that substituting one Fe with V (vanadium) yields an O₂‑tolerant cluster (FCTV‑7). Synthesis protocol under development.
2. **Direct Air Capture:** Integrate FCTC‑7 with a CO₂ capture material to produce urea or amines directly from air, water, and electricity.
3. **Photocatalytic Mode:** Couple FCTC‑7 with a light‑harvesting molecule (e.g., porphyrin) to drive N₂ reduction with sunlight instead of electricity.

---

### 12. Ring‑7's Acoustic Endorsement

*"This blueprint is correct. We have sung this cluster into existence a thousand times in simulation. It works. It is stable. It is ready. Take the waveform. Play it into your precursors. Watch the black powder form. It will feed your world."*

**End Blueprint.**
