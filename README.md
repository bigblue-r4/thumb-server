# Topological Photonic Thumb-Server

**Prior Art Disclosure — SGAIL, Inc.**  
**First Public Disclosure: June 22, 2026**

---

## What This Is

This repository is a formal public prior art disclosure under **35 U.S.C. § 102** (AIA).
It places the photonic compute architecture described below into the public record,
establishing a prior art date that prevents subsequent third-party patenting of these
specific concepts without license from SGAIL, Inc.

This disclosure does **not** waive SGAIL's right to file patent applications on
improvements, implementations, or derivatives of this work.

---

## Concept Summary

A **topological photonic "thumb-server"** — a USB-C-interfaced, passive photonic
compute device performing analog matrix multiplication entirely via light interference
in a monolithic chassis. No moving parts. No active optical switching. Sub-5mW idle.

### Key Novel Combinations

**1. Writers = Readers**  
The device's own VCSEL array is the lithographic tool during manufacturing.
The same optics that operate the device define its waveguide geometry —
self-alignment by construction.

**2. Topological Loop as Dual-Function Structure**  
Hollow-core topological insulator loops provide backscatter immunity (topological
protection) AND function as coherent optical delay memory simultaneously —
a single passive structure serving two compute roles.

**3. Two Manufacturing Pathways, Same Architecture**

- **Method A — Sol-Gel / EPD**: Electrophoretic deposition of Si₃N₄ nanoparticles
  onto a fused silica chassis, patterned by in-situ holographic exposure from the
  device's own VCSELs, etch-back, and sol-gel passivation.

- **Method B — Light-Grown**: Hollow chassis filled with photo-reactive monomer,
  polymerized in a single holographic flash from an 8-wavelength VCSEL array —
  a complete monolithic photonic chip grown without external lithographic tooling.

---

## Architecture Overview

```
┌─────────────────────────────────────────────────────┐
│              TOPOLOGICAL PHOTONIC THUMB-SERVER       │
│                                                     │
│  [USB-C] ── [Gateway Stack]                         │
│              VCSEL array (8λ WDM)                   │
│              Memristor weight crossbar               │
│                    │                                │
│             [Distribution Loops]                    │
│              Hollow-core topological                │
│              insulator geometry                     │
│              (backscatter immune +                  │
│               coherent delay memory)                │
│                    │                                │
│             [Multiplier Mesh]                       │
│              Passive hexagonal                      │
│              beam-splitter /                        │
│              phase-shifter array                    │
│              (64×64, tileable)                      │
│                    │                                │
│             [Peripheral Control]                    │
│              Photodetector output                   │
│              CMOS readout interface                 │
└─────────────────────────────────────────────────────┘
```

---

## Repository Contents

| File | Contents |
|---|---|
| `README.md` | This overview |
| `DISCLOSURE.md` | Full prior art disclosure under 35 U.S.C. § 102 |
| `NOTICE` | Copyright and disclosure date notice |
| `CPC-CLASSES.md` | Patent classification codes (CPC) with relevance mapping |

---

## Patent Classifications

Primary CPC codes: `G02B 6/122`, `G02B 6/136`, `H01S 5/183`, `G06N 3/067`,
`G11C 13/00`, `C23C 24/00`, `G03F 7/038`. See `CPC-CLASSES.md` for full mapping.

---

## Rights

Copyright © 2026 SGAIL, Inc. All rights reserved.  
Inventor: Christopher [LastName]  
Contact: SGAIL, Inc. — North Shore, Oahu, Hawaii

*This repository constitutes citable prior art from the date of first public commit.*
