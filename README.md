# BMResilience_ScRNAseq

**Analysis code and notebooks for:**  
> *Functional resilience of the bone marrow after leukemia induced changes in the BM micro-environment*  
> Lang S. *et al.*, 2025

This repository is a **code companion** to the manuscript. It contains Jupyter notebooks (Python)
and R scripts used to preprocess data, run analyses, and generate figures. It is **not** a Python
package and is intended for transparency and reproducibility.

---

## Repository Layout

```
BMResilience_ScRNAseq/
├── python_scripts/
│   ├── WhatCanWeUseFromHere.ipynb
│   ├── Experiment1_from_raw_h5ad.ipynb
│   ├── Experiment2_from_raw_h5ad.ipynb
│   └── Experiment3_from_raw_h5ad.ipynb
├── R_scripts/
│   ├── Figure3A.R
│   ├── Figure3B.R
│   ├── Figure4_summary_plots.R
│   └── Supplementary_analysis.R
└── README.md
```

> **Note**: `python_scripts/WhatCanWeUseFromHere.ipynb` **only creates the `raw_h5ad` file** used by the other notebooks.

---

## Figure-to-Script Table

This table documents **which script(s) generate each figure panel** in the manuscript.  
Paths are relative to the repository root.

| Figure / Panel | Primary Script(s) |
|---|---|---|
| **Figure 3 + 4 ** | [`python_scripts/Experiment2_from_raw_h5ad.ipynb`](python_scripts/Experiment1_from_raw_h5ad.ipynb) | 
| **Figure 5 + 6 ** | [`python_scripts/Experiment3_from_raw_h5ad.ipynb`](python_scripts/Experiment2_from_raw_h5ad.ipynb) | 
| **Figure 7 + 8 ** | [`R_scripts/Experiment1_from_raw_h5ad.ipynb`](python_scripts/Experiment1_from_raw_h5ad.ipynb) | 
| **Figure 3B** | [`R_scripts/Figure3B.R`](R_scripts/Figure3B.R) | 
| **Figure 3 (data prep)** | [`python_scripts/Experiment3_from_raw_h5ad.ipynb`](python_scripts/Experiment3_from_raw_h5ad.ipynb) | 
| **Figure 4** (summary panels) | [`R_scripts/Figure4_summary_plots.R`](R_scripts/Figure4_summary_plots.R) | 

> If you only need the **exact script for Figure 3A**, use:  
> **[`R_scripts/Figure3A.R`](R_scripts/Figure3A.R)**

---

## Data Inputs / Outputs

- **Inputs**: The notebooks expect an `.h5ad` produced by
  [`python_scripts/WhatCanWeUseFromHere.ipynb`](python_scripts/WhatCanWeUseFromHere.ipynb).  
  Any additional input file paths are declared at the top of each notebook/script.

- **Outputs**: Figures are written to a `figures/` directory (created automatically by scripts) and
  intermediate CSV/TSV tables to `results/`. Exact paths are defined in the corresponding script.

---


## Citation

If you use this repository, please cite the manuscript and this repository:

> Lang S. *et al.* (2025). *Functional resilience of the bone marrow after leukemia induced changes in the BM micro-environment.*  
> Repository: https://github.com/stela2502/BMResilience_ScRNAseq

---

## License

This repository is released under the **BSD 3-Clause License** unless otherwise stated within individual files.

