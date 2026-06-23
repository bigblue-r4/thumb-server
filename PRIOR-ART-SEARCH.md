# Prior Art Search Record
## Topological Photonic Thumb-Server

This document records the inventor's prior art search in good faith.
Search conducted by: Christopher Howard, SGAIL, Inc.
Search date range: Prior to June 22, 2026.

---

## Databases Searched

- [ ] USPTO Patent Full-Text Database (patents.google.com)
- [ ] Espacenet (European Patent Office)
- [ ] Google Scholar
- [ ] arXiv (physics.optics, cs.ET, cond-mat.mes-hall)
- [ ] IEEE Xplore
- [ ] Web of Science

*[Check boxes as searches are performed and record dates]*

---

## Search Terms Used

### Primary searches
- "topological photonic crystal waveguide compute"
- "VCSEL holographic waveguide fabrication"
- "electrophoretic deposition photonic waveguide"
- "passive photonic matrix multiply"
- "memristor VCSEL integrated"
- "hollow core waveguide topological insulator"
- "photopolymerization waveguide self-aligned"
- "monolithic photonic chip thumb"

### Secondary searches
- "photonic neural network passive mesh"
- "coherent optical delay memory"
- "analog optical matrix multiply passive"
- "topological insulator loop waveguide backscatter"
- "in-situ VCSEL lithography self-aligned"

---

## Known Prior Art — Not Invalidating

The following prior art was identified and analyzed. None of the items below,
individually or in combination, teaches the novel combinations asserted in this disclosure.

### Photonic Neural Networks / Optical Matrix Multiply

| Reference | What It Teaches | Why It Doesn't Invalidate |
|---|---|---|
| Shen et al. (2017), "Deep learning with coherent nanophotonic circuits," *Nature Photonics* | MZI mesh for optical neural network inference | Uses active Mach-Zehnder interferometers with thermo-optic phase shifters; requires active switching energy; no topological protection; no self-aligned fabrication |
| Hamerly et al. (2019), "Large-Scale Optical Neural Networks Based on Photoelectric Multiplication" | Coherent optical matrix multiply | Electronic weight loading; no memristor in-situ storage; no topological loops |
| Lightmatter Mars / Envise chips | PCIe photonic inference accelerator | Silicon photonics, external DRAM weights, no self-aligned fab, no topological loops, PCIe form factor |
| QANT Native Photonic NPU | Thin-film lithium niobate (TFLN) photonic NPU | Sensitive to backscatter/defects; external electronic RAM; PCIe server card (~270mm); no topological geometry; no in-situ holographic fabrication |

### Topological Photonics

| Reference | What It Teaches | Why It Doesn't Invalidate |
|---|---|---|
| Ozawa et al. (2019), "Topological photonics," *Reviews of Modern Physics* | Survey of topological protection in photonic systems | Establishes that topological protection in photonics is known; does not teach use as coherent delay memory in a compute context; does not teach the dual-function loop structure asserted here |
| Hafezi et al. (2013), "Imaging topological edge states in silicon photonics" | Topological edge states in silicon photonics | 2D planar chip geometry; no hollow-core waveguide loops; no compute application; no self-aligned fabrication |

### Electrophoretic Deposition / Waveguide Fabrication

| Reference | What It Teaches | Why It Doesn't Invalidate |
|---|---|---|
| Besra & Liu (2007), "A study on fundamentals and applications of electrophoretic deposition," *Progress in Materials Science* | EPD technique for ceramic and nanoparticle coatings | EPD is known; does not teach EPD inside a pre-formed optical chassis, nor subsequent in-situ holographic patterning by the device's own light source |
| General holographic lithography literature | Interference exposure for waveguide patterning | External laser source, external alignment; does not teach using the device's own VCSEL array as the sole lithographic tool |

### Holographic Polymerization

| Reference | What It Teaches | Why It Doesn't Invalidate |
|---|---|---|
| Bunning et al. (2000), "Holographic Polymer-Dispersed Liquid Crystals," *Annual Review of Materials Science* | PDLC formation by holographic exposure | Creates LC-polymer composite, not optical waveguides; external laser source; no self-alignment identity |
| Guo et al. (various), holographic waveguide fabrication | Holographic patterning of polymer waveguides | External laser source and alignment; does not teach single-flash polymerization using the device's own integrated VCSEL array |

---

## Novel Combinations Asserted — No Prior Art Found

Based on the searches above, the following combinations are asserted as novel:

1. **EPD + in-situ holographic patterning using the device's own VCSEL array**  
   EPD of photonic waveguide precursors is known. In-situ holographic exposure is known.
   Using the operational VCSEL array of the device being fabricated as the sole
   lithographic tool, such that writers = readers, is not found in any prior art.

2. **Hollow-core topological insulator loops as dual-function structure (backscatter
   shield + coherent delay memory)**  
   Topological protection in photonics is known. Optical delay lines are known.
   A single passive loop geometry that simultaneously provides topological backscatter
   immunity AND functions as coherent optical delay memory in a compute device is not
   found in prior art.

3. **Single-flash holographic polymerization of complete photonic mesh using integrated
   VCSEL array**  
   Holographic polymerization of polymer waveguides is known. Multi-wavelength VCSEL
   arrays are known. Completing a full photonic logic mesh in a single holographic flash
   using the device's own integrated light source, with zero external tooling or
   alignment, is not found in prior art.

4. **Monolithic thumb-scale photonic computer with non-volatile memristor weights and
   topological loop memory at <5mW idle**  
   The specific combination of scale, architecture, power, and non-volatile weight storage
   in a monolithic passive compute device is not found in prior art.

---

## Counsel Notes

This search was conducted by the inventor and is not a professional patent search.
A formal freedom-to-operate (FTO) search and patentability analysis by registered
patent counsel is recommended before filing any patent application.

Key competitors to include in professional search: Lightmatter, QANT, Luminous Computing,
Recogni, Rain Neuromorphics, Intel Silicon Photonics, Rockley Photonics.
