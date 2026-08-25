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
