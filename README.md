# Pregnancy Data Analysis: Infant Birth Weight Prediction

## Project Overview
This project investigates the factors influencing infant birth weight using historical data from the San Francisco East Bay area (1960–1967). The primary goal was to identify key predictors—such as gestation, parity, age, height, weight, and smoking status—and develop a predictive model for birth weight.

## Objectives
* Find out influential factors on birth weight.
* Examine the most important factors to keep birth weight in the healthy range (between 88 and 141 ounces).
* Model the data to achieve the highest possible $R^{2}$ (coefficient of determination) without overfitting.

## Dataset
* **Observations:** 1236.
* **Target Variable:** Birth weight (`bwt`) in ounces.
* **Predictor Variables:** * `gestation`: Length of gestation, in days.
    * `parity`: Binary indicator for first pregnancy.
    * `age`: Mother's age in years.
    * `height`: Mother's height in inches.
    * `weight`: Mother's weight in pounds.
    * `smoke`: Binary indicator for whether the mother smokes.

## Methodology
1. **Descriptive Data Analysis:** Performed EDA using histograms, boxplots, and scatterplots to visualize relationships.
2. **Regression Analysis:** Utilized forward selection to build a multiple linear regression model.
3. **Model Validation:** Checked for multicollinearity using Variance Inflation Factor (VIF) and performed residual analysis (Q-Q plots, residuals vs. fitted values).

## Key Findings
* The final model incorporates `gestation`, `smoke`, `height`, `parity`, and `weight` as significant predictors.
* The model achieved an adjusted $R^{2}$ of 0.2547, explaining approximately 25.79% of the variation.
* Residual analysis confirmed the model meets linearity, constant variance, and normality assumptions.

## Repository Contents
* `report/`: Contains the full project documentation. 
  [View the PDF Report](Infant_bwt_prediction_project/report/Infant_bwt_prediction_report.pdf)
* `code/`: Contains the R scripts used for data processing and model fitting. 
  [View the R Script](Infant_bwt_prediction_project/code/group3.R)

## Credits
* **Authors:** D.G. Sandani Gunasekara, H.S.S. Perera, W.A.D. Fernando, J.B.A.A.Y. Dharmasena, O.S. Jayathunga.
* **Data Source:** [Kaggle - Babies Birth Weight Dataset](https://www.kaggle.com/datasets/debjeetdas/babies-birth-weight).
