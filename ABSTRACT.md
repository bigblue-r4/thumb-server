# Abstract
## Topological Photonic Thumb-Server

---

### Patent-Style Abstract

A monolithic photonic compute device performs analog matrix multiplication via passive
light interference in a hollow-core waveguide chassis. The device comprises four integrated
sectors: (1) a gateway stack incorporating a graded-index lens surface, a vertically
integrated multi-wavelength VCSEL emitter array operating in the 850–1550nm range via
Wavelength Division Multiplexing, and a non-volatile memristor crossbar for weight
storage; (2) a full-spectrum distribution network of hollow-core topological insulator
loop waveguides that simultaneously provide backscatter immunity through topological
protection and function as coherent optical delay memory in the range of 10 picoseconds
to 2 nanoseconds; (3) a passive hexagonal beam-splitter and phase-shifter mesh, tiled
at 64×64 or larger, in which light interference performs matrix multiplications without
active switching energy; and (4) peripheral control electronics comprising a RISC-V
orchestrator and power management integrated circuit.

Two manufacturing methods are disclosed. In the first method, a pre-formed fused silica
chassis is coated via electrophoretic deposition of Si₃N₄ nanoparticles (20–50nm,
n=2.0 precursor film), patterned by in-situ holographic exposure from the device's own
VCSEL array, selectively etch-backed with KOH or buffered HF, and sealed with a
sol-gel SiO₂ sedimentation passivation overcoat and an optically-contacted lid. In the
second method, a hollow ceramic/Invar chassis is filled with a photo-reactive high-index
monomer and polymerized in a single holographic flash from the 8-wavelength VCSEL array,
producing a self-aligned monolithic photonic chip without external lithographic tooling.

In both methods, the fabrication geometry is defined by the same optical elements that
operate the device — a self-alignment property referred to herein as "writers = readers."
The device operates at sub-5mW idle power and targets a final form factor of approximately
15mm × 10mm × 3.5mm with greater than 10 Tb/s aggregate bandwidth.

---

### One-Line Summary

A thumb-sized passive photonic computer whose waveguides are written by its own lasers,
whose loops remember as they protect, and whose mesh computes without gates.

---

### Claims Summary (Provisional-Ready)

The following combinations are asserted as novel:

**Claim 1 — Writers = Readers Manufacturing**  
A method of fabricating a photonic waveguide network wherein the light source used to
operate the completed device is also the sole lithographic tool used to define the
waveguide geometry during fabrication, such that fabrication alignment and operating
alignment are identical by construction.

**Claim 2 — Dual-Function Topological Loop**  
A photonic device structure comprising hollow-core waveguide loops with topological
insulator geometry that simultaneously provides: (a) protection against optical
backscattering through topological phase protection, and (b) controllable coherent
optical delay memory, within a single passive structure requiring no active elements.

**Claim 3 — EPD + In-Situ Holographic Patterning**  
A manufacturing method comprising electrophoretic deposition of high-index nanoparticle
precursor material into a pre-formed optical chassis, followed by selective exposure
using the chassis's own integrated VCSEL array to define waveguide geometry, followed
by selective chemical etch-back of unexposed material.

**Claim 4 — Single-Flash Holographic Polymerization**  
A manufacturing method wherein a complete photonic logic mesh is formed in a single
holographic exposure event using a multi-wavelength VCSEL array projecting into a
photo-reactive monomer-filled chassis, producing a monolithic photonic chip without
mechanical assembly, bonding, or external lithographic registration.

**Claim 5 — Monolithic Thumb-Scale Photonic Computer**  
A photonic compute device in a monolithic chassis of approximately 15mm × 10mm footprint
comprising: a multi-wavelength VCSEL array; non-volatile memristor weight storage; passive
hexagonal waveguide mesh performing analog matrix multiplication via light interference;
topological loop structures providing coherent optical delay memory; and a USB-C electrical
interface — operating at less than 5mW idle power with no active optical switching.
