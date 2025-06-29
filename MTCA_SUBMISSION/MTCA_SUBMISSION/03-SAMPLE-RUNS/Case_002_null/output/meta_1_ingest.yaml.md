## Meta-1: Dual-Domain Mapping (Satellite + LIDAR/DEM)

**Quick Explanation:**  
This file records the mapping of each mythic seed to candidate real-world features.  
Each is checked with both satellite imagery and LIDAR/DEM; only dual-confirmed features are advanced.  
All rejections are explicit and traceable (per protocol).  
All four motif seeds from Meta-0 were checked using the same two reference images (`Case_2_Satellite.png`, `Case_2_LIDAR.png`), ensuring transparent audit coverage.

---

## Candidates YAML

``` yaml
meta_1_ingest:
  candidates:
    - seed: "anaconda movement = river formation"
      satellite_feature: "sinuous river channel, ~2,900m arc visible in Case_2_Satellite.png"
      lidar_feature: "DEM confirms only standard riverbed; no anomalous or myth-correspondent feature in Case_2_LIDAR.png"
      included: false
      rationale: "Rejected: only standard river morphology detected in both domains; no unique or anomalous feature."
      images: ["photos/Case_2_Satellite.png", "photos/Case_2_LIDAR.png"]
    - seed: "anaconda rest = lagoon formation"
      satellite_feature: "discrete pond/lagoon visible SW of meander in Case_2_Satellite.png"
      lidar_feature: "DEM shows only shallow, indistinct depression; not hydrologically or geomorphically unique."
      included: false
      rationale: "Rejected: no geomorphically distinct or myth-correspondent lagoon/depression confirmed by DEM."
      images: ["photos/Case_2_Satellite.png", "photos/Case_2_LIDAR.png"]
    - seed: "anaconda coil = island creation"
      satellite_feature: "no true island present; meander is fully enclosed by forest."
      lidar_feature: "DEM shows continuous terrain; no isolated elevation for island."
      included: false
      rationale: "No island feature detected; motif excluded for lack of spatial match and DEM support."
      images: ["photos/Case_2_Satellite.png", "photos/Case_2_LIDAR.png"]
    - seed: "anaconda becomes guardian of water"
      satellite_feature: "river depth not measurable; no distinct anomaly."
      lidar_feature: "DEM does not indicate unique basin or extreme depth in region."
      included: false
      rationale: "No geomorphically unique feature or deep basin; motif excluded."
      images: ["photos/Case_2_Satellite.png", "photos/Case_2_LIDAR.png"]
  summary: "All motif seeds checked in new region (Case 2); no dual-confirmed anomalies detected by LIDAR/DEM. No features advanced; strict Rule Z enforced."
  input_sources:
    - "meta_0_seed.yaml"
    - "photos/Case_2_Satellite.png"
    - "photos/Case_2_LIDAR.png"
```

### Traceability & Audit Chain

- **Upstream source:** [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_002_null/output/meta_0_seed.yaml]] — Motif seed extraction
    
- **This file:** [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_002_null/output/meta_1_ingest.yaml]] — Dual-domain mapping (satellite + LIDAR/DEM)
    
- **Downstream audit:** [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_002_null/output/meta_2_validated.yaml]] — Structural audit of dual-confirmed candidates
    
- **Audit log:** [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/logs/meta_1_ingest.log]] — Mapping decisions, dual-confirmation checks, and explicit exclusions
    

---

> **To reproduce, validate, or audit this mapping:**
> 
> 1. Review motif seeds and rationales in [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_002_null/output/meta_0_seed.yaml]].
>     
> 2. Cross-check mapping logic, candidate inclusions, and exclusions in [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/logs/meta_1_ingest.log]].
>     
> 3. Follow candidates and rejections through to [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_002_null/output/meta_2_validated.yaml]].
>     

---
