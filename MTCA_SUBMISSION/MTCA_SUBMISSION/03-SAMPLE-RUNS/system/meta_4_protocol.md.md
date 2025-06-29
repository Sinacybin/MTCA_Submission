# **Meta-4 Protocol: Domain Constraints & Rule Enforcement**

## Purpose

To apply domain-specific constraints, scientific rigor, and context-dependent exclusion rules to all schema-validated features from Meta-3, ensuring only ecologically, geomorphically, and historically plausible candidates advance.

## Required Inputs

- `/output/meta_3_schema.yaml` (schema-validated features)
    
- `/logs/meta_3_schema.log`
    

## Output Files

- `/output/meta_4_constrained.yaml` (all features surviving domain constraints)
    
- `/logs/meta_4_constrained.log` (constraint decisions and rationale)
    

## Stepwise Protocol

1. **Ingest Schema-Validated Features**
    
    - Read all candidates from `/output/meta_3_schema.yaml`.
        
2. **Apply Domain Constraints**
    
    - Evaluate each feature against:
        
        - **Ecological plausibility** (e.g., water features must fit known hydrology)
            
        - **Geomorphic rules** (e.g., no “islands” in upland zones)
            
        - **Historical/archaeological context** (e.g., must not conflict with established findings)
            
    - Reject any feature failing one or more constraints; log specific reason.
        
3. **Enforce Measurement Tolerances**
    
    - Cross-check all feature coordinates, dimensions, and spatial relationships.
        
    - Reject features outside plausible measurement error or with spatial drift.
        
4. **Document All Decisions**
    
    - Log inclusions and exclusions with rationale and file references in `/logs/meta_4_constrained.log`.
        
5. **Save Output**
    
    - Output all constraint-surviving features to `/output/meta_4_constrained.yaml`:
        
        yaml
        
        CopyEdit
        
        `meta_4_constrained:   mythic_chunks:     - chunk: "anaconda movement = river formation"       rationale: "Survived all scientific and domain constraints."   terrain_chunks:     - chunk: "sinuous river channel, 2,900 m arc"       rationale: "Hydrologically plausible; validated by DEM."   exclusions:     - chunk: "lagoon feature"       reason: "Rejected: not plausible per hydrological constraints."   summary: "All features have passed domain constraint audit."   input_source: "meta_3_schema.yaml"`
        
6. **Audit Completeness**
    
    - Confirm all output, log, and source files are present and referenced.

### Failure Examples: What Does _Not_ Pass Meta-4

|Type|Example Entry|Reason for Exclusion|
|---|---|---|
|Ecological Violation|`chunk`: “lagoon on hilltop”|Contradicts hydrological/geomorphic rules|
|Historical Clash|`chunk`: “artifact site in active river channel”|Conflicts with known archaeological evidence|
|Measurement Drift|`terrain_chunk`: “island, ~50m off expected coordinates”|Exceeds spatial tolerance for case|
|Domain Vague|`chunk`: “possible mound, not clear”|Ambiguous—fails domain constraint filter|
|Outdated Source|Feature only appears in outdated or unreliable maps|Fails modern data requirement|

**Only features passing all domain-specific and constraint filters advance.**