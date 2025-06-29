**MTCA Case 2: meta_1_ingest.log**

- Source seeds: `output/meta_0_seed.yaml`
    
- Satellite imagery: `photos/Case_2_Satellite.png`
    
- LIDAR/DEM imagery: `photos/Case_2_LIDAR.png`
    
- Analyst: Simon Martin
    
- Date: 2025-06-28
    

---

**Protocol Steps:**  
• Each motif seed from `meta_0_seed.yaml` was mapped to candidate features using the provided satellite and LIDAR/DEM images for the new region.  
• All seeds were evaluated in the _same spatial context_, referencing the Case 2 image pair for full auditability and transparency.  
• **Dual confirmation** (clear correspondence in both modalities) was required for inclusion; all others were explicitly rejected with rationale.

---

**Detailed Results:**

1. **"anaconda movement = river formation"**
    
    - Satellite: Sinuous river channel (~2,900m arc) visible in `Case_2_Satellite.png`.
        
    - LIDAR/DEM: Only standard riverbed and meander path present; no anomalous or myth-correspondent feature in `Case_2_LIDAR.png`.
        
    - **Status:** REJECTED (no unique or anomalous feature; standard morphology only).
        
2. **"anaconda rest = lagoon formation"**
    
    - Satellite: Discrete pond/lagoon visible SW of meander in `Case_2_Satellite.png`.
        
    - LIDAR/DEM: Shallow, indistinct depression at same location; not hydrologically or geomorphically unique in `Case_2_LIDAR.png`.
        
    - **Status:** REJECTED (no dual-domain confirmation; depression is not myth-correspondent).
        
3. **"anaconda coil = island creation"**
    
    - Satellite: No true island present; meander fully enclosed by forest in `Case_2_Satellite.png`.
        
    - LIDAR/DEM: Continuous terrain; no isolated elevation for island in `Case_2_LIDAR.png`.
        
    - **Status:** REJECTED (no island feature detected; not supported by DEM).
        
4. **"anaconda becomes guardian of water"**
    
    - Satellite: River depth not measurable; no distinct anomaly visible in `Case_2_Satellite.png`.
        
    - LIDAR/DEM: No unique basin or extreme depth in `Case_2_LIDAR.png`.
        
    - **Status:** REJECTED (no geomorphically unique feature or deep basin detected).
        

---

**Traceability & Audit Chain**

- **Upstream source:** [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_002_null/logs/meta_0_seed.log]] — Motif extraction log
    
- **This log:** [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_002_null/logs/meta_1_ingest.log]] — Dual-domain (satellite + LIDAR/DEM) mapping and exclusion process
    
- **Downstream audit:** [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_002_null/logs/meta_2_validated.log]] — Structural/minimalism audit of mapped features
    

> **To audit this step:**
> 
> 1. Review motif extraction process in [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_002_null/logs/meta_0_seed.log]].
>     
> 2. Examine all mapping logic and rejection rationale in [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_002_null/logs/meta_1_ingest.log]].
>     
> 3. Follow feature advancement/exclusion decisions in [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_002_null/logs/meta_2_validated.log]].

---
