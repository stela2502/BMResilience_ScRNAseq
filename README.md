# BMResilience_ScRNAseq

**Analysis code and notebooks for:**  
> *Functional resilience of the bone marrow after leukemia induced changes in the BM micro-environment*  

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
└── README.md
```

> **Note**: `python_scripts/WhatCanWeUseFromHere.ipynb` **only creates the `raw_h5ad` file** used by the other notebooks.

### Related Repository

Several notebooks in this project depend on  
[`ScanpyAutoAnalyzer`](https://github.com/stela2502/ScanpyAutoAnalyzer),  
a companion Python library providing shared analysis and visualization functions.

To make sure it’s available, install it first:

```bash
pip install git+https://github.com/stela2502/ScanpyAutoAnalyzer.git
```

---

## Figure-to-Script Table

This table documents **which script(s) generate each figure panel** in the manuscript.  
Paths are relative to the repository root.

| Figure / Panel | Script |
|----------------|--------|
| Figure 3 + 4 | [`python_scripts/Experiment2_from_raw_h5ad.ipynb`](python_scripts/Experiment1_from_raw_h5ad.ipynb) | 
| Figure 5 + 6 | [`python_scripts/Experiment3_from_raw_h5ad.ipynb`](python_scripts/Experiment2_from_raw_h5ad.ipynb) |
| Figure 7 + 8 | [`python_scripts/Experiment1_from_raw_h5ad.ipynb`](python_scripts/Experiment1_from_raw_h5ad.ipynb) |
| Figure 8 + 9 missing | [`R_scripts/Figure_8_9.R`](R_scripts/Figure_8_9.R) |

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

