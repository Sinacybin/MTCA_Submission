## Meta-1: Dual-Domain Mapping (Satellite + LIDAR/DEM)

**Quick Explanation:**  
This file records the mapping of each mythic seed to candidate real-world features.  
Each is checked with both satellite imagery and LIDAR/DEM; only dual-confirmed features are advanced.  
All rejections are explicit and traceable (per protocol).  
All four motif seeds from Meta-0 were checked using the same two reference images (`Case_001_Satellite.png`, `Case_001_LIDAR.png`), ensuring transparent audit coverage.

---

## Candidates YAML

``` yaml
meta_1_ingest:   candidates:     - seed: "anaconda movement = river formation"       satellite_feature: "sinuous river channel (standard, non-anomalous; visible in Case_001_Satellite.png)"       lidar_feature: "continuous riverbed visible in Case_001_LIDAR.png"       included: false       rationale: "Rejected: only standard river morphology detected; not a unique or anomalous feature."       images: ["Case_001_Satellite.png", "Case_001_LIDAR.png"]      - seed: "anaconda rest = lagoon formation"       satellite_feature: "no clear lagoon visible in Case_001_Satellite.png"       lidar_feature: "DEM shows no depression or enclosed water in region"       included: false       rationale: "Rejected: both satellite and DEM fail to indicate a lagoon in this area."       images: ["Case_001_Satellite.png", "Case_001_LIDAR.png"]      - seed: "anaconda coil = island creation"       satellite_feature: "island-like region present, but not distinct in satellite"       lidar_feature: "DEM does not support clear island topography"       included: false       rationale: "Rejected: island feature not geomorphically distinct per both images."       images: ["Case_001_Satellite.png", "Case_001_LIDAR.png"]      - seed: "anaconda becomes guardian of water"       satellite_feature: "deep channel visible but not anomalous in satellite"       lidar_feature: "no unusual depth or basin detected in DEM"       included: false       rationale: "Rejected: no evidence of unique guardian/depth feature at site."       images: ["Case_001_Satellite.png", "Case_001_LIDAR.png"]    summary: "All motif seeds checked against available satellite and DEM data. No dual-confirmed anomalies detected; no features advanced."   input_sources: [     "meta_0_seed.yaml",     "Case_001_Satellite.png",     "Case_001_LIDAR.png"   ]
```

### Traceability & Audit Chain

- **Upstream source:** [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/output/meta_0_seed.yaml]] — Motif seed extraction
    
- **This file:** [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/output/meta_1_ingest.yaml]] — Dual-domain mapping (satellite + LIDAR/DEM)
    
- **Downstream audit:** [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/output/meta_2_validated.yaml]] — Structural audit of dual-confirmed candidates
    
- **Audit log:** [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/logs/meta_1_ingest.log]] — Mapping decisions, dual-confirmation checks, and explicit exclusions
    

---

> **To reproduce, validate, or audit this mapping:**
> 
> 1. Review motif seeds and rationales in [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/output/meta_0_seed.yaml]].
>     
> 2. Cross-check mapping logic, candidate inclusions, and exclusions in [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/logs/meta_1_ingest.log]].
>     
> 3. Follow candidates and rejections through to [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/output/meta_2_validated.yaml]].
>     

---
