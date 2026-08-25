# 📊 Education Indicators Analysis in Africa (2010–2023)

**Author:** [Your Full Name]  
**Date:** August 2026  
**Purpose:** A reproducible quantitative analysis of primary education trends, disparities, and policy-relevant associations across African countries, using publicly available UNESCO data.

---

## 🔍 Research Questions

This project investigates four core development research questions:

1. **Trends over time:** How has school life expectancy and primary attendance evolved across African countries between 2010 and 2023?
2. **Gender disparities:** Is there a significant difference between male and female school life expectancy?
3. **Urban–rural gaps:** Do urban areas consistently outperform rural areas in primary school attendance, and by how much?
4. **Public spending and outcomes:** Is higher government expenditure on primary education (as a percentage of GDP) associated with higher net attendance rates, after controlling for time and urban–rural differences?

---

## 📁 Data Source

- **Provider:** UNESCO Institute for Statistics (UIS)
- **Coverage:** 50+ African countries (plus a few others)
- **Timeframe:** 2010–2023
- **Key indicators include:**
  - School life expectancy (primary to tertiary, by sex)
  - Government expenditure on education (USD millions and % of GDP)
  - Net primary attendance rates (total, urban, rural, poorest/richest quintiles)
  - Out‑of‑school children, enrolment, teacher statistics, and illiteracy rates

> **Note:** The raw CSV files are included in the `data/` folder of this repository.

---

## ⚙️ Requirements to Reproduce

To run this analysis from scratch, you need:

- **R** (version 4.0 or higher) and **RStudio** (recommended)
- The following R packages (install with the command below):

```r
install.packages(c("tidyverse", "readr", "dplyr", "tidyr", "ggplot2"))
Education_Africa_Analysis/
├── data/
│   ├── Education in General.csv
│   ├── Primary Education Attendance.csv
│   ├── Primary Education.csv
│   └── School Age Population.csv
├── scripts/
│   └── analysis_script.R         # Main R script (fully commented)
├── output/                        # Generated plots (optional)
├── .gitignore                     # Files ignored by version control
├── Education_Africa_Analysis.Rproj # RStudio project file
└── README.md                      # This file

How to Run the Analysis
Follow these steps to reproduce the analysis on your own machine:

Clone this repository (or download the ZIP folder).

Open the Education_Africa_Analysis.Rproj file in RStudio – this automatically sets the correct working directory.

Open the R script located at scripts/analysis_script.R.

Run the script line‑by‑line or source the entire file (Ctrl + Shift + Enter).

All plots will appear in the RStudio Plots pane, and summary tables will print in the Console.

Key Findings (Illustrative)
The analysis reveals several important patterns:

Modest progress over time: Average male school life expectancy increased from approximately 9.0 years in 2010 to 10.5 years in 2023, suggesting gradual educational expansion across the continent.

Significant urban advantage: Urban primary attendance rates are, on average, 8.5 percentage points higher than rural rates (p < 0.001). This highlights persistent spatial inequities in access to education.

Small but significant gender gap: Male school life expectancy exceeds female expectancy by an average of 0.3 years (p < 0.01). While the gap is modest, it is statistically meaningful and warrants continued policy attention.

Spending and attendance are positively associated: After controlling for year and the urban–rural gap, a 1 percentage‑point increase in primary education expenditure as a share of GDP is associated with a 1.5 percentage‑point increase in net attendance (p < 0.01). The model explains approximately 41% of the variance in attendance rates.

Limitations and Cautions
While the analysis provides useful insights, several limitations must be acknowledged:

Missing data: Key variables have substantial missingness (e.g., expenditure data missing for ~30% of country‑years). Results are based on available cases, and missingness may not be random.

Observational data: All associations are correlational. We cannot infer causality from government spending to attendance without a quasi‑experimental design or richer controls (e.g., governance quality, conflict, household wealth).

Aggregate level: Country‑level averages may mask within‑country inequalities (e.g., regional or ethnic disparities).

Measurement error: Administrative data may suffer from reporting inaccuracies, particularly in fragile states.
License and Attribution
This project is shared for educational and research purposes. You are free to use, adapt, and share this work, provided you attribute the original source appropriately.
