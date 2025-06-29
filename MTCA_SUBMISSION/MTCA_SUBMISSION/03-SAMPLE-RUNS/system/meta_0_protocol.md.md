# **Meta-0 Protocol: Mythic Seeding (Final Audit-Ready Version)**

## Purpose

Extract and normalize atomic, mappable “seeds” (motifs/features) from raw mythic narrative, establishing the foundation for all downstream analysis.

## Required Inputs

- `/data/[case_name].md` – single indigenous myth or legend, region/case-specific.
    

## Output Files

- `/output/meta_0_seed.yaml` (all extracted seeds + rationale)
    
- `/logs/meta_0_seed.log` (decisions & exclusions)
    

## Protocol Steps

1. **Ingest Narrative:**  
    Read `/data/[case_name].md`.
    
2. **Identify Motifs:**  
    Extract explicit spatial, geomorphic, or environmental motifs. Omit non-mappable or purely metaphorical content.
    
3. **Extract Seeds:**  
    For each motif, write an atomic chunk (e.g., `anaconda movement = river formation`). Must be spatially specific.
    
4. **Annotate Rationale:**  
    Brief rationale for every seed (why included? why mappable?).
    
5. **Log Decisions:**  
    Record all inclusions & major exclusions in `/logs/meta_0_seed.log`. If none excluded: note “No ambiguous motifs detected.”
    
6. **Save Output:**  
    Write all seeds/rationales in `/output/meta_0_seed.yaml` as:
    
    yaml
    
    CopyEdit
    
    `meta_0_seed:   extracted_seeds:     - chunk: "anaconda movement = river formation"       rationale: "Direct spatial transformation motif."   extraction_log: "All seeds are direct, spatial motifs; no ambiguous content included."   input_source: "/data/[case_name].md"`
    
7. **Audit Completeness:**  
    Output must include:
    
    - `/data/[case_name].md`
        
    - `/output/meta_0_seed.yaml`
        
    - `/logs/meta_0_seed.log`
        

**Notes:**

- **Ambiguity always resolves to exclusion** (only mappable seeds).
    
- **Seed rationale is mandatory.**
    
- Downstream protocols depend on atomic clarity here.
    

---