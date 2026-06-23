# Development Roadmap
## Topological Photonic Thumb-Server

---

## V1 Prototype — Lab Buildable (Current Target)

**Form factor:** ≈ 60mm × 40mm × 12mm  
**Goal:** Prove the full architecture at reduced scale. Not a product.

### Specifications
- 8-wavelength VCSEL stack (850–1550nm)
- 64×64 passive hexagonal photonic mesh
- Hollow-core waveguide loss: ~0.1 dB/cm
- Loop delay range: 10 ps – 2 ns
- Power (active): 3–5 Watts
- Power (idle): < 200 mW
- Interface: USB-C
- Cooling: passive heatsink base

### V1 Milestones
- [ ] Procure fused silica chassis (custom fire-polished, loop geometry)
- [ ] EPD coating deposition test (Si₃N₄ nanoparticle slurry)
- [ ] VCSEL array alignment and first-light test
- [ ] Holographic exposure calibration (writers = readers alignment verify)
- [ ] Etch-back and waveguide characterization
- [ ] Sol-gel passivation and lid seal
- [ ] Memristor crossbar integration
- [ ] Gateway stack assembly (GRIN + VCSEL + memristor)
- [ ] Full system first-light: data in → compute → data out
- [ ] Power and thermal measurement under load
- [ ] Matrix multiply verification (64×64)

### V1 What Success Looks Like
- End-to-end light path confirmed
- Topological protection demonstrated (backscatter suppression measured)
- Analog matrix multiply result within acceptable error band
- Optical delay loops operating (coherent delay confirmed)
- Power measurements match projections

---

## V2 — Scaled Integration

**Form factor:** ≈ 30mm × 20mm × 6mm (estimated)  
**Goal:** Reduce form factor, increase wavelength count, improve power efficiency.

### Key Changes from V1
- Increase wavelength count beyond 8 (full WDM spectrum)
- Tiled mesh: 128×128 or larger
- Reduce chassis thickness (improved GRIN integration)
- Reduce PMIC footprint
- Evaluate Method B (Light-Grown) manufacturing at this scale
- USB-C → potential PCIe or M.2 interface option for embedded deployments

### V2 Milestones
- [ ] V1 proven before V2 begins
- [ ] Wavelength count expansion (12–16λ)
- [ ] Light-Grown (Method B) pilot fabrication
- [ ] Mesh tiling verification (2×2 tile, 128×128 effective)
- [ ] Reduced power budget: target < 1W active

---

## V3 / Final Form Factor — Target (2026+)

**Form factor:** ≈ 15mm × 10mm × 3.5mm  
**Goal:** Thumb-server. USB-C device. Ships as a product.

### Target Specifications
- Footprint: 15mm × 10mm
- Thickness: ≤ 3.5mm (at gateway stack)
- Bandwidth: > 10 Tb/s aggregate
- Power (active): < 250 mW
- Power (idle): < 5 mW
- Interface: USB-C
- Waveguides: Hollow-core, Topological Photonic Crystal
- Manufacturing: Method B (Light-Grown) preferred at this scale

### What This Enables
- Edge AI inference at USB power budget
- Portable photonic matrix compute (laptop, IoT, embedded)
- SGAIL Harborlight security processing offload
- Defense / embedded / field-deployed compute
- Potential DHS/DARPA program relevance (edge AI, resilient compute)

---

## Funding Path

| Stage | Target | Amount | Notes |
|---|---|---|---|
| V1 Lab Build | Prototype fabrication | ~$50–150K | University fab partnership or commercial nanofab |
| V2 | Scaled prototype | ~$300–500K | DHS SBIR Phase 1 / Phase 2 candidate |
| V3 | Product | ~$2–5M | Series A or DARPA program |

### Near-term funding paths
- **DHS SBIR Phase 1** (~$300K) — primary near-term path for SGAIL
- **NSF SBIR Phase 1** (~$275K) — alternative, photonic compute research angle
- **University research partnership** — access to nanofab (e.g., UH Manoa, Stanford NanoFab)
- **Angel / pre-seed** — hardware AI investor angle (photonic edge compute)

---

## Technology Risk Assessment

| Risk | Severity | Mitigation |
|---|---|---|
| Waveguide alignment at 15mm scale | High | Method B (Light-Grown) eliminates alignment step entirely |
| EPD uniformity inside narrow loops | Medium | Field simulation; Landau-Levich equation implies uniform coating |
| Memristor integration with optical stack | Medium | Silicon interposer layer provides electrical-optical separation |
| Topological protection bandwidth | Medium | Loop geometry designed for 850–1550nm; needs experimental verification |
| VCSEL phase coherence for holographic patterning | High | Critical for Method A and B; needs beam characterization before fab |
| Thermal stability (VCSEL heating during write) | Low–Medium | Invar chassis (Method B) and aluminum baseplate (V1) address this |
