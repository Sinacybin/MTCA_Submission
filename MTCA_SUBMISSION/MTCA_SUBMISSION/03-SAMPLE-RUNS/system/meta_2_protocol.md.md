# **Meta-2 Protocol: Structural Audit & Minimalism**

## Purpose

Recursively audit dual-confirmed candidates for minimalism, non-redundancy, structural integrity, and schema compliance.

## Required Inputs

- `/output/meta_1_ingest.yaml`
    
- `/logs/meta_1_ingest.log`
    

## Output Files

- `/output/meta_2_validated.yaml`
    
- `/logs/meta_2_audit.log`
    

## Protocol Steps

1. **Ingest Dual-Confirmed Candidates:**  
    Evaluate each for structure and minimalism.
    
2. **Schema/Structure Validation:**
    
    - All required fields present?
        
    - Reject/correct malformed or ambiguous entries.
        
3. **Redundancy & Drift Audit:**
    
    - Remove duplicates, drifted, or compound features.
        
    - Only unique, traceable features advance.
        
4. **Compression & Minimalism:**
    
    - Ensure atomic, succinct candidates.
        
    - Summarize rationale, remove tangential info.
        
5. **Validate or Exclude:**
    
    - Pass = `/output/meta_2_validated.yaml`
        
    - Fail = Log reason in `/logs/meta_2_audit.log`
        
6. **Save Output:**
    
    - Both advanced and excluded features clearly listed.
        

### Failure Examples: What Does _Not_ Pass Meta-2

|Type|Example|Reason|
|---|---|---|
|Redundant|“river formation” & “winding river path”|Choose one minimal representation|
|Drift|“island within river” → “vegetated region nearby”|Loss of specificity/traceability|
|Compound|“large river arc + islands + lagoon”|Must split; not minimal/atomic|
|Ambiguous|“possible water feature”|No cross-domain mapping|
|Schema Fail|Missing `seed`/`rationale`|All fields required|

**Notes:**

- **No ambiguity or redundancy may advance.**
    
- Machine- and human-readable YAML required.