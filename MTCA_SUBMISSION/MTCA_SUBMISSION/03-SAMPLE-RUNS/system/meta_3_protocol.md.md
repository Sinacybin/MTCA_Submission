# **Meta-3 Protocol: Schema Enforcement & Spatial Normalization (Template)**

_This is the logical next step for your pipeline; I provide it below so you can keep the rapid pace._

## Purpose

To enforce a normalized, domain-agnostic schema on all validated features, ensuring cross-case consistency, spatial reference integrity, and readiness for automated or manual downstream audit.

## Required Inputs

- `/output/meta_2_validated.yaml` (minimal, non-redundant features)
    
- `/logs/meta_2_audit.log`
    

## Output Files

- `/output/meta_3_schema.yaml`
    
- `/logs/meta_3_schema.log`
    

## Protocol Steps

1. **Ingest Validated Features**  
    Read all advanced features from `/output/meta_2_validated.yaml`.
    
2. **Schema Normalization**
    
    - Ensure each candidate includes:
        
        - `seed`
            
        - `satellite_feature` (with explicit geo-coordinates)
            
        - `lidar_feature` (with explicit geo-coordinates)
            
        - `included` (boolean)
            
        - `rationale` (single-sentence, audit-focused)
            
        - `images` (paths/IDs)
            
        - `spatial_reference` (geoJSON or standardized format for precise mapping)
            
        - `lineage` (direct pointer to original mythic seed)
            
3. **Enforce Naming/Field Standards**
    
    - All entries conform to field names/types.
        
    - No free-form text or ambiguous categories.
        
4. **Log and Correct Inconsistencies**
    
    - Any missing, malformed, or ambiguous entries are either corrected or excluded (with reason).
        
5. **Save Output**
    
    - All schema-compliant features to `/output/meta_3_schema.yaml`
        
    - Log all changes/exclusions in `/logs/meta_3_schema.log`
        

**Example Output**

yaml

CopyEdit

`meta_3_schema:   candidates:     - seed: "anaconda movement = river formation"       satellite_feature: "sinuous river channel, ~2,900m arc"       lidar_feature: "DEM confirms riverbed"       included: true       rationale: "Dual-confirmed, schema-validated."       images:         - "photos/Satellite_Anaconda_Movement.png"         - "photos/LIDAR_River_Confirm.png"       spatial_reference:         type: "Feature"         geometry: {...}  # (GeoJSON or standard spatial format)       lineage: "meta_0_seed.yaml:anaconda movement = river formation"   summary: "All features schema-validated and spatially referenced; non-conforming features excluded."   input_source: "meta_2_validated.yaml"`

---

### Failure Examples: What Does _Not_ Pass Meta-3

|Type|Example Entry|Reason for Exclusion|
|---|---|---|
|Missing Field|No `spatial_reference` or `lineage` field|All fields required for downstream traceability|
|Free-Form|`satellite_feature`: “River feature, see above”|All features must be explicit and machine-parseable|
|Ambiguous|`spatial_reference`: “North of the lagoon”|Must be in geoJSON or standardized spatial format|
|Naming Drift|`lidar_feature`: “Area looks interesting”|No vague descriptors; scientific description only|
|Inconsistent|Field types inconsistent between entries|All fields must match protocol specification|

**No entry advances unless it is schema-validated, spatially referenced, and lineage-traceable.**