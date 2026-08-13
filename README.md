# Ames Housing Market Intelligence

A statistical analysis of the Ames, Iowa housing market, translating 2,930 home sales into actionable investment strategies for real estate stakeholders.

**Live Site:** [pratikkmane.github.io/ames-housing-project](https://pratikkmane.github.io/ames-housing-project/)

---

## Overview

This project analyzes home sales in Ames, Iowa (2006–2010) to identify the key drivers of home value and the optimal timing for buying, selling, and investing. The dataset spans a full market cycle — the pre-2008 housing bubble, the financial crisis, and early recovery — making the findings relevant to both stable and volatile markets.

**Audience:** Ames Real Estate Investment Group (sellers, buyers, investors, and developers)

**Objective:** Identify key drivers of home values and translate statistical findings into stakeholder-specific investment recommendations.

---

## Key Findings

| Finding | Detail |
|---|---|
| **Quality is King** | Overall quality rating is the strongest price predictor (+$32,000 per quality point, r = 0.80) |
| **Timing Matters** | $20,000 seasonal swing between summer peak and winter trough listings |
| **Crisis Impact** | 22% price decline from 2007 peak to 2009 trough, with recovery beginning in late 2009 |
| **Age Penalty** | Homes depreciate ~$650/year; renovation does not fully offset age-related discounts |

---

## Methodology

1. **Exploratory Data Analysis** – Distributions, correlations, outliers, and missing data assessment
2. **Hypothesis Testing** – t-tests and ANOVA on central air, construction recency, and house style (all p < 0.001)
3. **Multiple Regression** – Predictive model using Overall Quality, Living Area, Garage Area, and Age at Sale (R² = 0.76, RMSE = $39K)
4. **Time Series Analysis** – Seasonal decomposition and trend analysis to identify market timing patterns

---

## Repository Structure

```
ames-housing-project/
├── index.qmd              # Home page — executive summary, video, and slides
├── background.qmd         # Audience, dataset, and variable definitions
├── eda.qmd                # Exploratory data analysis
├── price-drivers.qmd      # Correlation analysis, hypothesis tests, ANOVA
├── pricing-model.qmd      # Multiple regression model and diagnostics
├── timing.qmd             # Time series analysis and seasonal patterns
├── recommendations.qmd    # Stakeholder-specific recommendations
├── slides.qmd             # Presentation slides
├── Ames_Housing_Presentation.pptx
├── Ames_Housing_Presentation.pdf
├── _quarto.yml             # Site configuration
└── data/
    └── ames.csv            # Ames Housing dataset
```

---

## Tech Stack

- **R** (tidyverse, broom, car, scales, knitr)
- **Quarto** for website generation and publishing
- **GitHub Pages** for hosting

---

## Running Locally

```bash
git clone https://github.com/pratikkmane/ames-housing-project.git
cd ames-housing-project
quarto render
```

Open `docs/index.html` in your browser to view the site.

---

## Dataset

The Ames Housing dataset contains 2,930 home sales in Ames, Iowa (2006–2010) with 82 variables covering size, quality, age, features, and location. Originally compiled by Dean De Cock as a modern alternative to the Boston Housing dataset.

---

## Author

**Pratik Mane**
[GitHub](https://github.com/pratikkmane) · [Live Project](https://pratikkmane.github.io/ames-housing-project/)
