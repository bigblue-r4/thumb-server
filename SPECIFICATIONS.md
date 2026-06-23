# Technical Specifications
## Topological Photonic Thumb-Server

---

## Target Device (Final Form Factor)

| Parameter | Value |
|---|---|
| Footprint | ≈ 15mm × 10mm |
| Thickness (max) | ≈ 3.5mm (at gateway stack) |
| Waveguide type | Hollow-core, Topological Photonic Crystal |
| Bandwidth (aggregate) | > 10 Tb/s (prototype target) |
| Power (active, VCSEL firing) | < 250 mW |
| Power (idle/passive) | < 5 mW |
| Interface | USB-C (data + power) |
| Supply voltage | 1.8 V – 3.6 V (VBAT) |

---

## V1 Prototype

| Parameter | Value |
|---|---|
| Footprint | ≈ 60mm × 40mm |
| Thickness (max, including stack) | ≈ 12mm |
| Wavelengths (λ) | 8 channels (850–1550nm) |
| Mesh size | 64×64 |
| Waveguide loss | ≈ 0.1 dB/cm |
| Loop delay range | 10 ps – 2 ns |
| Power (active) | ≈ 3–5 Watts |
| Power (idle/passive) | < 200 mW |
| Interface | USB-C (data + power) |
| Cooling | Passive (heatsink base) |

### V1 Goals
- Prove full light path end-to-end
- Demonstrate topological protection
- Demonstrate analog matrix multiply
- Demonstrate optical delay loops
- Measure power and thermal behavior

### What V1 Can Do
- End-to-end: data in → light compute → data out
- Topological protection around loops
- Analog matrix multiply up to 64×64
- Optical delay line memory
- On-chip weight storage (memristor)
- Power efficiency measurement
- Thermal behavior under load

---

## Gateway Stack (Sector 1) — Monolithic Interface

### 1.1 GRIN Lens Edges
- Graded-Index lens walls gather divergent light and collimate into parallel beams
- Curved graded-index lens focuses incoming light into emitter array
- Minimal insertion loss

### 1.2 VCSEL Emitter Array
- V1: 8-wavelength VCSEL stack (850nm–1550nm)
- Target: thousands of vertically stacked VCSELs
- Electrically driven to generate WDM data channels
- Wavelength Division Multiplexing generates full spectrum of data channels

### 1.3 Memristor Array / State Array
- Non-volatile memristor crossbar
- Stores AI model weights and initial states (starting physics)
- Located behind emitter stack
- Defines state before photonic processing begins

### Gateway Stack Cross-Section (layer order, surface to electrical)
1. GRIN Lens Surface
2. Anti-Reflection Coating
3. Optical Coupling Layer
4. VCSEL Layer (λ1)
5. VCSEL Layer (λ2)
6. … (additional VCSEL layers)
7. VCSEL Layer (λ8)
8. MEMRISTOR Crossbar
9. Silicon Interposer
10. Electrical Interface

---

## Distribution Loops (Sector 2) — Full-Spectrum Distribution

### 2.1 Hollow-Core Waveguides (Vacuum Channels)
- Evacuated (low-index) hollow-core tunnels
- Guide full spectrum with ultra-low loss
- Eliminate thermal crosstalk

### 2.2 Topological Insulator Geometry
- Topological Photonic Crystal loop geometry
- Prevents backscattering around sharp bends
- Preserves coherence around bends
- Provides coherent delay memory simultaneously

---

## Topological Multiplier Mesh (Sector 3) — Geometric Center

### 3.1 Passive Photonic Logic Array / Passive Hexagonal Mesh
- Uniform crystal mesh of beam-splitters and phase-shifters
- Hexagonal geometry (silicon photonic platform)
- Light interference (constructive and destructive) performs matrix multiplications
- No active gates — physics computes
- Trillions of matrix multiplications simultaneously at near-zero power

### 3.2 Analog Interference
- Light interference performs matrix multiplications in analog optical domain

### 3.3 Scalable Tiling
- Mesh can be tiled to larger sizes in future versions
- V1 prototype: 64×64 mesh

---

## Peripheral Control (Sector 4)

### A — System Orchestrator
- Advanced RISC-V / NPU controller
- Handles slow tasks: communication (USB / Wi-Fi / etc.), command interpretation
- Converts final photonic output (via photodetectors) back to electrical data
- V1: RISC-V based, interfaces via USB-C

### B — Integrated Power Management (PMIC)
- Connects to power source (VBAT)
- Precise, low-noise regulation to drive VCSEL stack only when launching new data
- Rest of system is passive and consumes minimal power
- V1: Includes DC-DC conversion, monitoring, and protection

---

## EPD Layer Parameters (Calculated, Method A)

| Parameter | Value |
|---|---|
| EPD Coating Thickness | 100–500 nm |
| Passivation Layer Thickness | 10–30 µm |
| Process Time (EPD) | 10 min |
| Process Time (Sedimentation/Decant/Cure) | 4 hours |
| Cure Temp | 200°C max (compatible with Si components) |
| Alignment Tolerance | ≤ 1 µm |
| Fluid Viscosity/Tension | controlled |

---

## V1 Prototype Packaging

- Aluminum baseplate for thermal stability
- Transparent lid for optical access
- Stack height ≈ 12mm
- USB-C interface for power and data

### Important Notes
- Research prototype — not a product
- Alignment tolerances in microns
- Requires temperature control in lab
- Calibration required before each run
- Future versions: increase wavelength count, mesh size, integration density

---

## Competitive Positioning vs. QANT Photonic NPU

| | QANT Native Photonic NPU | V1 Topological Thumb-Server |
|---|---|---|
| Primary material | Thin-Film Lithium Niobate (TFLN) | Hollow-Core Silica & Memristors |
| Signal protection | Precision Waveguides | Topological Geometry |
| Backscatter | Sensitive to defects/backscatter | Immune (math-protected path) |
| Memory | Electronic RAM (external) | Coherent Delay Loops (optical, no OEO) |
| Memory latency | External RAM transfer | 10 ps – 2 ns, no conversion |
| Form factor | PCIe Server Card (~270mm) | Monolithic Thumb-Server (15mm) |
| Compute | Native Nonlinear Networks (MZI) | Passive Hexagonal Mesh |
| Weights | — | Non-volatile memristors |
