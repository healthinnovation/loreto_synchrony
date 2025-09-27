# Spatiotemporal co-distribution and time lagged cross correlation of malaria and dengue in Loreto, Peru

**Authors:** Paloma M. Cárcamo, Gabriel Carrasco-Escobar, Samantha R. Kaplan, Jesús M. Quispe, Gordon C. McCord, Tarik Benmarhnia  

This repository contains R code and figures for analyzing spatiotemporal synchrony between malaria and dengue in the Loreto region. The key analyses include cross-correlation, spatial synchronization, sensitivity checks, and mapping.  

---

## Repository structure

```bash
loreto_synchrony/
├── data/                        # Raw and processed data files
├── 01-synchrony_plots.Rmd       # Main analysis workflow
├── 02-sensitivity_analyses.Rmd  # Resampling for sensitivity analysis
├── loreto_synchrony.Rproj       # RStudio project file
├── README.md
├── LICENSE
└── .gitignore
```

- The `.Rmd` files are the core scripts:  
  - [01-synchrony_plots.Rmd](https://github.com/healthinnovation/loreto_synchrony/blob/main/01-synchrony_plots.Rmd): loads data, computes cross-correlations, fits models, produces time series and maps.  
  - [02-sensitivity_analyses.Rmd](https://github.com/healthinnovation/loreto_synchrony/blob/main/02-sensitivity_analyses.Rmd): runs robustness checks (resampling).  
---

## Reproducing results and figures

1. Clone or download this repository:

 ```bash
git clone https://github.com/healthinnovation/loreto_synchrony.git
cd loreto_synchrony
```
2. Open the project file ([loreto_synchrony.Rproj](https://github.com/healthinnovation/loreto_synchrony/blob/main/loreto_synchrony.Rproj)) in RStudio.

3. Ensure raw data files with malaria and dengue incidence are located in `data/` folder.

4. Run all chunks in [01-synchrony_plots.Rmd](https://github.com/healthinnovation/loreto_synchrony/blob/main/01-synchrony_plots.Rmd) to produce the main figures, cross-correlation tables, and maps.

5. Run sensitivity analyses by running all chunks in [02-sensitivity_analyses.Rmd](https://github.com/healthinnovation/loreto_synchrony/blob/main/02-sensitivity_analyses.Rmd).

5. Inspect results generated in the `.Rmd` documents.
