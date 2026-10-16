# Diabetes Progression Analysis

## Overview
This project explores the relationship between clinical measurements and diabetes disease progression using statistical analysis and regression models in R.

The goal is to identify variables associated with diabetes progression, investigate relationships between predictors, and evaluate how well linear regression models explain variation in the outcome.

## Dataset
The dataset contains **442 observations and 11 variables**, including clinical measurements and a quantitative measure of diabetes progression.

The analysis focuses on the progression outcome and selected predictors, including:
- **BMI** — Body Mass Index
- **BP** — Blood Pressure
- **S5** — A clinical measurement included in the dataset

## Tools and Technologies
- **R**
- **RStudio**
- **dplyr** — Data manipulation
- **ggplot2** — Data visualization
- **tidyr** — Data tidying

## Methodology
The analysis includes:

1. **Exploratory Data Analysis (EDA):** Examining distributions, descriptive statistics, and unusual observations.
2. **Correlation Analysis:** Investigating associations between numerical variables and diabetes progression.
3. **Data Visualization:** Creating histograms, scatterplots, a correlation heatmap, and diagnostic plots.
4. **Simple Linear Regression:** Modelling progression using BMI as the predictor.
5. **Multiple Linear Regression:** Modelling progression using BMI, blood pressure, and S5.
6. **Model Evaluation:** Comparing model fit, examining residuals, and assessing potential multicollinearity and uncertainty.

## Key Findings
- BMI showed a positive correlation with progression (**r ≈ 0.59**).
- S5 also showed a positive correlation (**r ≈ 0.57**).
- Blood pressure showed a moderate positive correlation (**r ≈ 0.44**).
- The simple linear regression model using BMI had an **R² of 0.344**.
- The multiple regression model using BMI, blood pressure, and S5 had an **R² of 0.480**.
- The higher R-squared indicates a better fit to the observed sample, but further validation is needed to assess predictive performance on new data.

The multiple regression model explained a larger proportion of the observed variation in progression than the simple model. However, model fit alone does not establish that the model is better in every respect.

## Limitations
This is an observational analysis, so the results describe statistical associations rather than causal relationships. The findings may be affected by unmeasured variables, measurement uncertainty, and limitations of linear regression. In addition, the residual diagnostics suggest possible non-linearity, indicating that the model assumptions require further investigation.

Therefore, the results should not be interpreted as evidence that any predictor causes changes in diabetes progression, nor should the model be used as a clinical diagnostic tool without further validation.

## Project Files

- [`Diabetes_Progression_Analysis.R`](./Diabetes_Progression_Analysis.R) — R script containing the complete analysis.
- [`Diabetes_Progression_Report.pdf`](./Diabetes_Progression_Report.pdf) — Final analytical report.
- [`Diabetes_Progression_Decision_Maker_Presentation.pdf`](./Diabetes_Progression_Decision_Maker_Presentation.pdf) — Decision-maker presentation.
- [`diabetes.tab.txt`](./diabetes.tab.txt) — Dataset used for the analysis.

## Figures

- [Correlation heatmap](./Correlation%20heatmap.png)
- [Distribution of BMI](./Distribution%20of%20BMI.png)
- [Distribution of diabetes progression](./Distribution%20of%20diabetes%20progression.png)
- [Progression versus BMI](./Progression%20versus%20BMI.png)
- [Progression versus blood pressure](./Progression%20versus%20blood%20pressure.png)
- [Residuals versus fitted values](./Residuals%20versus%20fitted%20values.png)

This project was completed as part of my learning in data analysis and demonstrates the use of R for exploratory data analysis, statistical modelling, visualization, and interpretation of results.
