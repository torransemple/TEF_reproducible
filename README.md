# README.md

# Redefining Fuel Poverty: The Temporal Equity Framework (TEF)

This repository contains the replication package for the manuscript **"Redefining Fuel Poverty: Introducing the Temporal Equity Framework (TEF)"**, currently under review at *Energy Policy*.

The package includes the synthetic dataset, R Markdown analysis script, and environment specifications required to reproduce the sensitivity analysis and visualisations presented in the paper.

## Repository Contents

| File | Description |
| :--- | :--- |
| `SNH_TEF.csv` | **Synthetic Nottingham Homes (SNH) Dataset.** A unit-level dataset containing 105,570 synthetic household records with income, modelled energy expenditure and energy efficiency variables. |
| `TEF_analysis.Rmd` | **R Markdown Notebook.** The complete analytical pipeline, including data cleaning, fuel poverty quantification (LIHC, LILEE, and TEF), and scenario-based sensitivity analysis. |
| `tef_session_info.txt` | **System Metadata.** Detailed versioning of the R environment, operating system, and all package dependencies used during the original analysis. |



## Requirements

### Software
* **R (v4.5.1 or later)**
* **RStudio** (recommended for running the `.Rmd` notebook)

### R Packages
The analysis relies on the `tidyverse` suite and several supporting libraries. The script will attempt to install any missing packages automatically, but the primary dependencies are:
* `tidyverse` (v2.0.0)
* `cowplot` (v1.1.3)
* `janitor` (v2.2.0)
* `sessioninfo` (v1.2.3)

## Instructions for Reproduction

1. **Download:** Download all files into a single local directory.
2. **Environment:** Ensure the `SNH_TEF.csv` file and `TEF_analysis.Rmd` are in the same folder. The script uses relative paths to load the data.
3. **Execution:** Open `TEF_analysis.Rmd` in RStudio and select **"Run All"** or Knit the document to HTML/PDF.
4. **Validation:** The script will generate the fuel poverty rates in baseline, scenario 1 and scenario 2 conditions, as well as all visualisations in the results section.



## Data Notes

The `SNH_TEF.csv` dataset is a synthetic representation of the Nottingham housing stock. It was generated using a microsimulation approach to protect household privacy while maintaining the statistical properties of the original administrative data. 

* **Income variables:** Derived using a spatial microsimulation model.
* **Energy variables:** Derived from Energy Performance Certificate (EPC) data and local authority administrative records.

## Anonymity Notice

This repository has been anonymised for the double-blind peer-review process. All author names, institutional affiliations, and absolute local file paths have been removed from the code and metadata.

## Contact

For queries regarding the code or data during the review process, please contact the Editor of *Energy Policy*, who can facilitate communication with the authors.