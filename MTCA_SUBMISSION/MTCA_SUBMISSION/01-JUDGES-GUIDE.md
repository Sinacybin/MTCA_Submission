## udges' Guide: Reviewing MTCA in 5 Steps

1. **Open the Sample Myth**
    
    - **File:** `input-myth.md`
        
    - **Purpose:** This file contains the original narrative “seed” for all downstream analysis.
        
    - _You should see:_ A short mythic text or excerpt with motifs to be mapped.
        
2. **Trace a Motif Across Layers**
    
    - **Files:**
        
        - `meta_0_seed.yaml`
            
        - `meta_1_compression.yaml`
            
        - `meta_2_audit.yaml`
            
        - ...
            
        - `meta_6_final.yaml`
            
    - **Purpose:** Select a motif (e.g., “anaconda = river formation”). Track how it is transformed, filtered, and validated at each meta-layer.
        
    - _You should see:_ The motif included, excluded, or annotated at each stage—reflecting structural, narrative, and empirical checks.
        
3. **Review the Audit Logs**
    
    - **Folder:** `logs/`
        
    - **Purpose:** Confirm that every inclusion, exclusion, and rationale is fully documented at every meta-layer.
        
    - _You should see:_ For each motif, explicit notes on decisions. If nothing is excluded, this will be stated for audit completeness.
        
4. **Validate the Final Output**
    
    - **File:** `meta_6_final.yaml`
        
    - **Purpose:** Only features that survive all filters—including both narrative correspondence and scientific (LIDAR/DEM) confirmation—appear here.
        
    - _You should see:_ Only motifs with dual-domain, auditable confirmation. If the file is empty, this is a valid (null) result under Rule Z.
        
5. **Reference the Full Protocol as Needed**
    
    - **File:** `04-WORKFLOW.md`
        
    - **Purpose:** Consult for technical details, system rationale, or stepwise methodology at any point.
        
    - _You should see:_ A comprehensive description of every processing and audit step.
        

---

> **Note:**  
> **MTCA’s “Rule Z”** enforces that no hypothesis is accepted unless it is independently validated by both mythic pattern and scientific ground-truth. Every inclusion, exclusion, and rationale is logged for complete transparency and traceability.
