# **Meta-1 Protocol: Dual-Domain Mapping (Statistical Inevitability/Rule Z Enforcement)**

## Purpose

Map each mythic seed to candidate features in satellite imagery, then independently confirm/reject with LIDAR/DEM. Only dual-confirmed features advance.

## Required Inputs

- `/output/meta_0_seed.yaml` (seeds)
    
- Satellite imagery (geo-referenced)
    
- LIDAR/DEM data (geo-referenced)
    

## Output Files

- `/output/meta_1_ingest.yaml`
    
- `/logs/meta_1_ingest.log`
    

## Protocol Steps

1. **Ingest Seeds:**  
    Read all seeds from `/output/meta_0_seed.yaml`.
    
2. **Satellite Mapping:**  
    For each seed, map features in satellite imagery (e.g., river arcs, lagoons).
    
    - Record coordinates, dimensions, and rationale.
        
    - Save/reference annotated images.
        
3. **LIDAR/DEM Confirmation (Rule Z):**  
    For each satellite-mapped feature:
    
    - Independently analyze with LIDAR/DEM.
        
    - Confirm geomorphic presence/absence.
        
    - **Explicitly reject** any not confirmed by LIDAR/DEM.
        
4. **Document All Decisions:**
    
    - Record satellite and LIDAR/DEM results (included/rejected + rationale + file refs).
        
5. **Save Output:**  
    Write dual-domain results to `/output/meta_1_ingest.yaml`:
    
    yaml
    
    CopyEdit
    
    `meta_1_ingest:   candidates:     - seed: "anaconda movement = river formation"       satellite_feature: "sinuous river channel, ~2,900m arc"       lidar_feature: "DEM confirms riverbed"       included: true       rationale: "Direct spatial match to motif; confirmed by LIDAR/DEM."       images:         - "photos/Satellite_Anaconda_Movement.png"         - "photos/LIDAR_River_Confirm.png"   summary: "Only dual-confirmed candidates advanced; rejection is default."   input_sources:     - "meta_0_seed.yaml"`
    
6. **Log All Decisions:**  
    `/logs/meta_1_ingest.log`: every mapping attempt (success/rejection) + reasoning + file refs.
    
7. **Audit Completeness:**  
    Confirm presence of all referenced files.
    

**Notes:**

- **Rule Z is strict:** only features confirmed by both domains.
    
- All inclusions/exclusions must be explicit and referenced.
