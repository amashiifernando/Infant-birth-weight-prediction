# Pregnancy Data Analysis: Infant Birth Weight Prediction

## Project Overview
[cite_start]This project investigates the factors influencing infant birth weight using historical data from the San Francisco East Bay area (1960–1967)[cite: 11]. [cite_start]The primary goal was to identify key predictors—such as gestation, parity, age, height, weight, and smoking status—and develop a predictive model for birth weight[cite: 12].

## Objectives
* [cite_start]Find out influential factors on birth weight[cite: 19].
* [cite_start]Examine the most important factors to keep birth weight in the healthy range (between 88 and 141 ounces)[cite: 20].
* [cite_start]Model the data to achieve the highest possible $R^{2}$ (coefficient of determination) without overfitting[cite: 21].

## Dataset
* [cite_start]**Observations:** 1236[cite: 15].
* [cite_start]**Target Variable:** Birth weight (`bwt`) in ounces[cite: 62].
* [cite_start]**Predictor Variables:** * `gestation`: Length of gestation, in days[cite: 63].
    * [cite_start]`parity`: Binary indicator for first pregnancy[cite: 64].
    * [cite_start]`age`: Mother's age in years[cite: 65].
    * [cite_start]`height`: Mother's height in inches[cite: 66].
    * [cite_start]`weight`: Mother's weight in pounds[cite: 67].
    * [cite_start]`smoke`: Binary indicator for whether the mother smokes[cite: 68].

## Methodology
1. [cite_start]**Descriptive Data Analysis:** Performed EDA using histograms, boxplots, and scatterplots to visualize relationships[cite: 14, 70].
2. [cite_start]**Regression Analysis:** Utilized forward selection to build a multiple linear regression model[cite: 141].
3. [cite_start]**Model Validation:** Checked for multicollinearity using Variance Inflation Factor (VIF) and performed residual analysis (Q-Q plots, residuals vs. fitted values)[cite: 54, 224, 228].

## Key Findings
* [cite_start]The final model incorporates `gestation`, `smoke`, `height`, `parity`, and `weight` as significant predictors[cite: 185].
* [cite_start]The model achieved an adjusted $R^{2}$ of 0.2547, explaining approximately 25.79% of the variation[cite: 183, 186].
* [cite_start]Residual analysis confirmed the model meets linearity, constant variance, and normality assumptions[cite: 54, 226].

## Repository Contents
* `report/`: Contains the full project documentation (PDF).
* `code/`: Contains the R scripts used for data processing and model fitting.

## Credits
* **Authors:** D.G. Sandani Gunasekara, H.S.S. Perera, W.A.D. Fernando, J.B.A.A.Y. Dharmasena, O.S. [cite_start]Jayathunga[cite: 5, 6, 7, 8, 9].
* [cite_start]**Data Source:** [Kaggle - Babies Birth Weight Dataset](https://www.kaggle.com/datasets/debjeetdas/babies-birth-weight)[cite: 22].
