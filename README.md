# Reducing Fuel Misuse & Improving Profitability per Trip

**Data Analytics II — Capstone Case Study 1**  
AB InBev Sagamu Transport Operations — Q1 2026

[![View on RPubs](https://img.shields.io/badge/RPubs-View%20Report-blue?style=for-the-badge&logo=r)]((https://rpubs.com/anthoniaokocha/1434920))
[![R Version](https://img.shields.io/badge/R-4.x-276DC3?style=flat-square&logo=r)](https://www.r-project.org/)
[![Quarto](https://img.shields.io/badge/Quarto-1.4-75AADB?style=flat-square&logo=quarto)](https://quarto.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](LICENSE)

---

## 📌 Overview

This repository contains the complete analysis for a logistics cost-optimisation study examining **1,073 truck-trip records** from DP World's Sagamu Transport Operations hub, serving AB InBev deliveries across Nigeria in Q1 2026.

### Business Problem

Fuel waste remains a major operational cost driver.

Analysis revealed that:

- **36.7%** of all trips generated misused fuel costs
- Total waste amounted to:

## ₦30.5 Million in a Single Quarter

### Key Finding

Dead kilometres emerged as the strongest operational predictor of financial waste:

- **Spearman Correlation:** ρ = 0.65
- **Statistical Significance:** p < 0.001
- Every additional **100 dead kilometres** was associated with approximately:

## ₦77,727 in Misused Fuel Value

### Strategic Recommendation

Implementation of a:

## Long-Haul Fuel Accountability Protocol

Projected savings:

## ₦21+ Million per Quarter

---

## 🔗 Access the Published Report

The complete rendered report is available on RPubs:

👉 **[Reducing Fuel Misuse and Improving Profitability per Trip — Full Report](https://rpubs.com/anthoniaokocha/1432977)**

The RPubs version includes:

- Interactive tables
- Collapsible code chunks
- Statistical outputs
- Styled visualisations
- Full analytical commentary

---

## 📁 Repository Structure

```text
├── TripReviewReport_ABNBEV_JAN_FEB_MAR.xlsx   # Raw operational dataset
├── analysis.qmd                               # Quarto analysis document
├── custom.css                                 # Custom HTML styling
├── README.md                                  # Project documentation
└── LICENSE                                    # MIT License
```

---

## 🎯 Business Context

This analysis was conducted within real commercial transport operations at **DP World**.

Key responsibilities connected to this work include:

- Commercial cost modelling
- Contract profitability optimisation
- Tender pricing support (RFIs, RFPs, RFQs)
- Transport performance analysis
- Commercial risk identification

The operational metrics analysed directly influence:

- Fleet profitability
- Fuel efficiency
- Asset utilisation
- Route performance
- Controller accountability

---

## 🔬 Analytical Techniques Applied

| Technique | Business Application |
|---|---|
| **Exploratory Data Analysis (EDA)** | Establish operational performance baselines |
| **Data Visualisation** | Executive reporting and quarterly reviews |
| **Welch ANOVA** | Validate controller performance differences |
| **Spearman Correlation** | Detect operational waste relationships |
| **Multiple Linear Regression** | Quantify primary fuel cost drivers |

---

## 📊 Key Findings

| Insight | Result |
|---|---|
| Total Q1 Waste | ₦30,472,200 |
| Waste Trips | 394 trips |
| Waste Rate | 36.7% |
| Long-Haul Waste Contribution | 77.7% |
| Mean Dead KM per Trip | 47.7 km |
| Total Dead KM | 51,165 km |
| Highest Average Waste Route | Kano |
| Kano Avg Waste | ₦236,313 |
| Kaduna Avg Waste | ₦121,329 |

### Additional Findings

- Top 10% of waste trips contributed **33.8% of total losses**
- Long-haul routes (>700 km) showed the highest operational inefficiency
- Controller-level differences in fuel efficiency were statistically significant

---

## 📈 Visualisations Included

| Figure | Description |
|---|---|
| Figure 1 | Fuel misuse distributions |
| Figure 2 | Operational variable distributions |
| Figure 3 | Monthly waste trend analysis |
| Figure 4 | Waste by fleet controller |
| Figure 5 | Route-type waste comparison |
| Figure 6 | Destination-level waste analysis |
| Figure 7 | Weekly efficiency trends |
| Figure 8 | Controller boxplot distributions |
| Figure 9 | Waste-trip proportions |
| Figure 10 | Correlation matrix |
| Figure 11 | Predictor vs waste scatterplots |

---

## 🛠️ Requirements

### Required R Packages

```r
library(tidyverse)
library(readxl)
library(lubridate)
library(ggplot2)
library(scales)
library(corrplot)
library(GGally)
library(knitr)
library(kableExtra)
library(broom)
library(car)
library(moments)
library(effectsize)
library(patchwork)
library(ggridges)
library(viridis)
```

---

## ▶️ Render the Quarto Report

```bash
# Install Quarto
https://quarto.org/docs/get-started/

# Render HTML output
quarto render analysis.qmd --to html
```

Or render directly inside **RStudio** using the **Render** button.

---

## 📝 Recommended Operational Actions

### Long-Haul Fuel Accountability Protocol

1. GPS-verified dead-kilometre reconciliation
2. Dead-KM threshold enforcement
3. Daily fuel log monitoring
4. Controller performance scorecards
5. Long-haul trip escalation controls

### Financial Impact

Reducing long-haul dead kilometres from:

- **71 km average**

to:

- **20 km average**

could recover:

## ₦85+ Million Annually

---

## ⚠️ Study Limitations

| Limitation | Proposed Improvement |
|---|---|
| Single-client dataset | Multi-client expansion |
| Q1-only analysis | Multi-quarter analysis |
| Associational analysis | Controlled intervention studies |
| Static fuel pricing | Dynamic fuel index integration |
| Missing cargo-weight data | Load-factor modelling |

---

## 🔧 Future Work

Planned extensions include:

- ARIMA / Prophet forecasting
- Predictive risk classification models
- Real-time operational dashboards
- Difference-in-differences causal analysis
- Live fleet monitoring integration

---

## 📚 References

Adi, B. (2026).  
*AI-powered business analytics: A practical textbook for data-driven decision making.*

R Core Team. (2024).  
*R: A language and environment for statistical computing.*

Wickham, H. et al. (2019).  
*Welcome to the tidyverse.* Journal of Open Source Software.

Okocha, A. (2026).  
*AB InBev Q1 2026 trip review report — Sagamu Transport Operations.*

---

## 📧 Contact

**Anthonia Okocha**  
Business Development Specialist — DP World

Course: **Data Analytics II — Lagos Business School**  
Instructor: **Prof Bongo Adi**

For collaboration or questions, please open an issue on this repository.

---

## 📄 License

This project is licensed under the **MIT License**.

---

## 🙏 Acknowledgments

- **Prof Bongo Adi** — Lagos Business School
- **DP World MDS** — Operational data access
- **AB InBev Nigeria** — Commercial partnership support

---

> This analysis was conducted using real operational transport data as part of the Data Analytics II programme at Lagos Business School.
# Reducing Fuel Misuse & Improving.txt
Displaying # Reducing Fuel Misuse & Improving.txt.
