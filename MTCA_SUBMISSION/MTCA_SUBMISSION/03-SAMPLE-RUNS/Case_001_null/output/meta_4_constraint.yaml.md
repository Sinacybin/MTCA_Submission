## Meta-4: Domain Constraints & Rule Enforcement

**Quick Explanation:**  
This file applies all domain-specific constraints and exclusion rules to schema-validated features from Meta-3.  
Each feature is evaluated for ecological, geomorphic, and historical plausibility.  
Only features passing all domain and measurement constraints advance; all others are excluded with explicit rationale.

---

## Candidates YAML

```yaml
meta_4_constraint:
  mythic_chunks: []
  terrain_chunks: []
  exclusions:
    - chunk: "anaconda movement = river formation"
      reason: "No features advanced; excluded upstream (Meta-3)."
    - chunk: "anaconda rest = lagoon formation"
      reason: "No features advanced; excluded upstream (Meta-3)."
    - chunk: "anaconda coil = island creation"
      reason: "No features advanced; excluded upstream (Meta-3)."
    - chunk: "anaconda becomes guardian of water"
      reason: "No features advanced; excluded upstream (Meta-3)."
  summary: "Null result—no candidates reached domain constraint audit; all excluded in previous layer."
  input_source: "meta_3_schema.yaml"
```

### Traceability & Audit Chain

- **Upstream source:** [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/output/meta_3_schema.yaml]] — Schema enforcement and spatial normalization
    
- **This file:** [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/output/meta_4_constraint.yaml]] — Domain constraint and rule filtering
    
- **Downstream audit:** [[meta_5_alignment.yaml]] — Philosophical and alignment filter
    
- **Audit log:** [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/logs/meta_4_constraint.log]] — Domain-specific constraints, exclusions, and rationale
    

---

> **To reproduce, validate, or audit this constraint layer:**
> 
> 1. Review schema-normalized outputs in [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/output/meta_3_schema.yaml]].
>     
> 2. Check all domain constraint/filtering decisions in [[MTCA_SUBMISSION/03-SAMPLE-RUNS/Case_001_null/logs/meta_4_constraint.log]].
>     
> 3. Follow all features or exclusions through to [[meta_5_alignment.yaml]].

---

