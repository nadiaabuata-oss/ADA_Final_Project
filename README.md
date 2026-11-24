# ADA Final Project

## Project Title

**Association Between Urinary 3-Phenoxybenzoic Acid and Serum Anti-Müllerian Hormone Among U.S. Women Aged 20–44: NHANES 2017–2018**

## Overview

This project examines the association between urinary 3-phenoxybenzoic acid (3-PBA), a biomarker of pyrethroid insecticide exposure, and serum anti-Müllerian hormone (AMH), a marker of ovarian reserve.

The secondary objective is to assess whether age modifies this association.

The analysis was completed for the Advanced Data Analysis course, Fall 2026.

## Data Source

Data were obtained from the publicly available National Health and Nutrition Examination Survey (NHANES) 2017–2018 cycle, conducted by the National Center for Health Statistics.

Data source: https://www.cdc.gov/nchs/nhanes/

The R Markdown analysis downloads the required NHANES datasets directly from CDC URLs. The original datasets are not duplicated in this repository.

## Study Population

The eligible sample includes 253 nonpregnant women aged 20–44 with available urinary 3-PBA and serum AMH measurements.

The primary regression analysis includes 223 complete cases after excluding participants with missing income-to-poverty ratio data.

## Statistical Analysis

The analysis includes:

- Survey-weighted descriptive statistics.
- Survey-weighted linear regression using natural-log-transformed urinary 3-PBA as the exposure and serum AMH (ng/mL) as the outcome.
- Primary adjustment for age, income-to-poverty ratio, and urinary creatinine.
- An age interaction test.
- Regression diagnostics and influence screening.
- Sensitivity analyses adjusting for race/ethnicity and excluding potentially influential observations.

The analysis accounts for NHANES subsample weights, strata, and primary sampling units.

## Repository Contents

- `Analysis_cleaned.Rmd` — annotated R Markdown containing data preparation, analysis, statistical models, diagnostics, and figures.
- `ADA-final-project.Rproj` — RStudio project configuration.

## Reproducibility

1. Download or clone this repository.
2. Install the required R packages if necessary: haven, survey, ggplot2, and tidyr
3. Open `Analysis_cleaned.Rmd`.
4. Run the analysis

## Main Findings

The primary adjusted model did not identify a statistically significant association between urinary 3-PBA and serum AMH (β = −0.046; 95% CI: −0.376 to 0.283; p = 0.763).

There was no statistical evidence of age effect modification (interaction p = 0.915).

These results should be interpreted cautiously given the cross-sectional design, limited regression sample, and model diagnostic findings.

## Author

Nadia Abu Ata

Advanced Data Analysis - Fall 2026

### AI Use Disclosure

I used ChatGPT to help me learn linear regression and NHANES survey-weighted analysis in R, troubleshoot code, and resolve errors. 
The research topic, statistical decisions, interpretation of results, and PowerPoint presentation are my own work.
