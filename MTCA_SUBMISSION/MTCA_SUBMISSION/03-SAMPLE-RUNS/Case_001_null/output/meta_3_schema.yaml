## Meta-3: Schema Enforcement & Spatial Normalization

**Quick Explanation:**  
This file enforces a normalized schema on all validated candidates from Meta-2.  
Each feature includes standardized field names, explicit geo-coordinates, and lineage for traceability.  
Only schema-compliant, spatially referenced features advance; all inconsistencies are excluded.

---

### Candidates YAML

```yaml
meta_3_schema:
  candidates: []
  exclusions:
    - seed: "anaconda movement = river formation"
      reason: "Rejected in Meta-1/2: not schema-eligible; standard river only."
    - seed: "anaconda rest = lagoon formation"
      reason: "Rejected in Meta-1/2: not schema-eligible; no lagoon detected."
    - seed: "anaconda coil = island creation"
      reason: "Rejected in Meta-1/2: not schema-eligible; no island detected."
    - seed: "anaconda becomes guardian of water"
      reason: "Rejected in Meta-1/2: not schema-eligible; no unique depth/basin detected."
  summary: "No candidates advanced to schema validation; all motif seeds were previously excluded."
  input_source: "meta_2_validated.yaml"
```

---

### Traceability & Audit Chain

- **Upstream source:** [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/output/meta_2_validated.yaml]] — Structural audit output
    
- **This file:** [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/output/meta_3_schema.yaml]] — Schema enforcement and spatial normalization
    
- **Downstream audit:** [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/output/meta_4_constraint.yaml]] — Domain constraint and rule filtering
    
- **Audit log:** [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/logs/meta_3_schema.log]] — Schema enforcement, normalization steps, and all rationale
    

---

> **To reproduce, validate, or audit this schema layer:**
> 
> 1. Review prior structural audit results in [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/output/meta_2_validated.yaml]].
>     
> 2. Check schema logic, normalization, and all audit steps in [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/logs/meta_3_schema.log]].
>     
> 3. Track remaining (or excluded) features through to [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/output/meta_4_constraint.yaml]].

---

