# Graduate Admission Prediction Model

This repository contains the files and resources for a final project aimed at predicting graduate admission likelihood using applicant data. The project applies various data analysis and regression techniques to identify key factors influencing admissions and build a reliable prediction model.

## Files in this Repository

- **adm_data.csv**: The dataset used for the analysis, sourced from Kaggle, containing 9 columns and 400 entries related to graduate admissions.
- **MurphyFinalProject.pdf**: The final report summarizing the project's methodology, results, and conclusions.
- **MurphyFinalProject.Rmd**: The R Markdown file with the code and analysis used to develop the project.

## Dataset Description

The dataset includes the following variables:
- **GRE Score**: Out of 340
- **TOEFL Score**: Out of 120
- **University Rating**: Rating of the university (1–5)
- **SOP**: Strength of Statement of Purpose (1–5)
- **LOR**: Strength of Letter of Recommendation (1–5)
- **CGPA**: Undergraduate GPA (10-point scale)
- **Research**: Binary indicator for research experience (0 or 1)
- **Chance of Admit**: Probability of admission (0–1)

## Project Objectives

1. Identify the key factors influencing the likelihood of graduate admission.
2. Build and evaluate a regression model to predict admission chances based on applicant data.
3. Test the significance of interaction terms and resolve multicollinearity issues in the model.

## Key Findings

- The most important predictors for admission are **CGPA**, **GRE Score**, **LOR**, and **Research**.
- A Box-Cox transformation was applied to resolve heteroscedasticity, resulting in a well-fitted model with an adjusted R-squared of 0.8186.
- Interaction terms were tested but did not improve the model's performance.
- Diagnostic tests confirmed that the final model satisfies regression assumptions.

## How to Use

1. **Dataset**: Load the `adm_data.csv` file for analysis.
2. **Code**: Open the `MurphyFinalProject.Rmd` file to view the R code and analysis.
3. **Report**: Refer to `MurphyFinalProject.pdf` for a detailed explanation of the project's findings and conclusions.

## Future Improvements

- Incorporating additional predictors.
- Using larger and more diverse datasets to capture more variability and improve model performance.

## Tools and Libraries

The following R libraries were used in this analysis:
- `readr`
- `ggplot2`
- `GGally`
- `caTools`
- `Metrics`
- `car`
- `lmtest`
- `MASS`
- `tidyverse`

## Author

Aidan Murphy  
**Course**: DATA 501  
**Institution**: Binghamton University  
**Submission Date**: December 20, 2024
**Source**: Mohan S. Acharya, Asfia Armaan, Aneeta S. Antony, "A Comparison of Regression Models for Prediction of Graduate Admissions," *IEEE International Conference on Computational Intelligence in Data Science*, 2019. DOI: [10.1109/ICCIDS.2019.8862113](https://doi.org/10.1109/ICCIDS.2019.8862113)
