# scRNA-seq Analysis of Murine Haematopoiesis: Clustering and Trajectory Analysis

**Dataset:** Dahlin et al., *Blood* (2018) — GSM2877127–GSM2877134  
**Tool:** Scanpy (Python) | **Environment:** Jupyter Notebook

---

## Overview

This notebook presents an end-to-end single-cell RNA-seq analysis of murine bone marrow haematopoiesis using publicly available data from Dahlin et al. (2018). The analysis spans quality control, batch integration, unsupervised clustering, cell type annotation, and pseudotime trajectory inference, with systematic justification of parameter choices at each step.

---

## Methods

- **Preprocessing & QC:** Filtering, normalisation, log-transformation, and highly variable gene selection
- **Batch correction:** Harmony integration using sample as covariate; UMAP embeddings compared before and after correction to validate
- **Dimensionality reduction:** PCA with systematic comparison of 10, 20, and 30 PCs; 30 PCs selected to preserve rare population signals
- **Clustering:** Leiden algorithm with multiple resolutions compared; final annotation across 16 biologically meaningful clusters
- **Cell type annotation:** Literature-supported marker genes including LT-HSC (*Procr*, *Fgd5*, *Hoxb5*), HSC/MPP, lymphoid progenitors (*Dntt*, *Flt3*), basophil/mast cell progenitors (*Cpa3*, *Ms4a2*), megakaryocyte progenitors, erythroid, myeloid/neutrophil, and cycling populations
- **Trajectory inference:** Diffusion Pseudotime (DPT) with LT-HSC as root; trajectories reconstructed across myeloid, erythroid, and lymphoid lineages

---

## Key Results

- 16 haematopoietic clusters identified, including rare populations resolved only at higher clustering resolutions
- Harmony correction successfully removed batch effects while preserving biological variation across 8 samples
- DPT trajectories recapitulate known haematopoietic differentiation hierarchy from LT-HSC through committed lineages

---

## Repository Contents

| File | Description |
|------|-------------|
| `HaematopoiesisTrajectoryAnalysis_ParulK.pdf` | Full analysis notebook rendered as PDF, including all code, outputs, and figures |

---

## Reference

Dahlin JS et al. A single-cell hematopoietic landscape resolves 8 lineage trajectories and defects in Kit mutant mice. *Blood*. 2018;131(21):e1–e11.

---

*GitHub: [github.com/parulkuls26](https://github.com/parulkuls26)*# placeholder
