## Overview

**Case Study:** MTCA Application – Amazonian Anaconda Myth (Case 2)

This folder documents the full audit pipeline for Case 2 of the Mythic Terrain Compression Auditor (MTCA).  
The case applies MTCA’s seven-layer, protocol-driven audit system to a canonical Amazonian creation myth, testing for statistically inevitable archaeological hypotheses using dual-domain geospatial data (satellite and LIDAR/DEM).

---

## Input Narrative

**Mythic Input:**  
_Amazonian Anaconda creation myth_

> “In the beginning, a colossal anaconda descended from the sky and slithered across the land, carving the winding rivers and forming deep lagoons where it rested. Where it coiled, islands appeared. The anaconda vanished into the waters, becoming the guardian of all depths. The Amazon landscape bears the memory of the anaconda’s movement.”

**Reference:**  
Traditional Amazonian creation myth (Yagua, Ticuna, et al.; see Santos-Granero 2009, Roosevelt 2013).

---

## Region / Data

- **Target Region:** Segment of the Amazon basin (see file references below)
    
- **Satellite Imagery:** `photos/Case_2_Satellite.png`
    
- **LIDAR/DEM:** `photos/Case_2_LIDAR.png`
    

---

## Motif Seeds Extracted

- _anaconda movement = river formation_
    
- _anaconda rest = lagoon formation_
    
- _anaconda coil = island creation_
    
- _anaconda becomes guardian of water_
    

(See: `meta_0_seed.yaml`)

---

## Audit Outcome

All motif seeds were rigorously tested against both satellite and LIDAR/DEM data per MTCA protocol.  
**Result:**

> **Strict null result.**  
> All motifs were denied at Meta-1; no dual-confirmed (narrative + empirical) features detected.  
> No features advanced to downstream audit layers.  
> This outcome demonstrates maximal resistance to false positives and full audit transparency (Rule Z).

---

## File Manifest

- `input-myth.md` – Canonical mythic narrative
    
- `photos/Case_2_Satellite.png` – Satellite imagery used for mapping
    
- `photos/Case_2_LIDAR.png` – LIDAR/DEM file used for independent ground-truthing
    
- `meta_0_seed.yaml` – Extracted motif seeds
    
- `meta_1_ingest.yaml` – Dual-domain mapping results (all seeds rejected)
    
- `meta_1_ingest.log` – Line-by-line mapping and rejection log
    
- `meta_2_validated.yaml` – Structural audit output (null result)
    
- `meta_2_audit.log` – Structural audit log
    
- `meta_3_schema.yaml` – Schema and spatial normalization (null result)
    
- `meta_3_schema.log` – Schema audit log
    
- `meta_4_constrained.yaml` – Domain constraint audit (null result)
    
- `meta_4_constrained.log` – Domain audit log
    
- `meta_5_alignment.yaml` – Philosophical/alignment audit (null result)
    
- `meta_5_alignment.log` – Alignment audit log
    
- `meta_6_final.yaml` – Final compression/justification (null result)
    
- `meta_6_final.log` – Final audit log
    

---

## Data & Imagery

- **Satellite Image:** `photos/Case_2_Satellite.png` (public satellite region, Amazon Basin)
- **LIDAR/DEM:** `photos/Case_2_LIDAR.png` (public DEM, processed with QGIS for pseudo-color and contours)
- **Note:** Images generated from open-access sources (OpenTopography/OpenTopoMap); no proprietary data used. No unique scene/tile ID available—region and methods are documented in the root README.

 **Reviewer Note:**  
> All processing steps (export, pseudo-coloring, contour overlay) are fully described in the root README under "Data Sources & Provenance." Raw DEM tiles and step-by-step QGIS instructions are available on request.

---

## Protocol Notes

- **Rule Z strictly enforced:** No motif is accepted unless dual-confirmed by both mythic pattern and empirical ground-truth.
    
- **Audit discipline:** All inclusions and exclusions are explicit and traceable at every layer.
    
- **Null result is expected and desired** for regions with no statistically inevitable motif-feature correspondence; this demonstrates the MTCA system’s maximal resistance to false positives.
    

---

**Contact:**  
Simon Martin | simon.d.martin01@gmail.com

---

**For more on MTCA system structure, see the root project README.**

---
