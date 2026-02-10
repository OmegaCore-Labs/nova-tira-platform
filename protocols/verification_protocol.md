# Detailed Verification Protocol

## Section 1: Vector Construction for Verification

**Backbone:** Use a modified, replication-incompetent adenoviral vector (serotype 5, ΔE1/E3). The backbone sequence is available from Addgene (#XXXXX, "pAd5-Empty-Backbone").

**Insert Cloning Site:** The multiple cloning site (MCS) between the CMV promoter and the poly-A signal must be used.

**Critical Note:** The specific, optimized "recognition template" nucleotide sequence is the proprietary component and is **not provided**. For verification purposes, you must insert your *own* test sequence (e.g., a model tumor antigen like OVA) into this MCS to test the vector's functionality. The data in this repo was generated with the proprietary template; your results with a substitute antigen will be proof-of-principle but will not match the efficacy magnitude.

**Production:** Transfect the linearized vector construct into HEK293 cells for viral packaging. Purify via cesium chloride gradient. Titrate via plaque assay.

## Section 2: Flow Cytometry Panels

**Tumor Infiltrating Lymphocyte (TIL) Analysis:**
- Live/Dead Fixable Near-IR
- CD45 BV785
- CD3 FITC
- CD8 APC-Cy7
- CD4 PerCP-Cy5.5
- FoxP3 PE (intracellular)
- PD-1 APC
- Tim-3 BV421

**Gating Strategy:**
Singlets -> Live -> CD45+ -> CD3+ -> Then subset into CD8+, CD4+, and CD4+FoxP3+ (Tregs).

Full antibody clones, dilutions, and fixation/permeabilization buffers listed in the spreadsheet linked in data/.
