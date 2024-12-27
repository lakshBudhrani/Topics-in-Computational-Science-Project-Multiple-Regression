# Topics-in-Computational-Science-Project-Multiple-Regression

## Project Description

This project aims to predict the percentage of body fat (%BodyFat) using multiple regression models with various predictors. The dataset used for this analysis is `Bodyfat.xlsx`, provided by the professor. The analysis involves creating at least three different multiple regression models, each including at least three predictors. The predictors are categorized into three distinct body regions:

- **Upper Body**: Neck, Chest, Abdomen
- **Lower Body**: Hip, Thigh, Knee
- **Hands**: Biceps, Forearms, Wrist

By segmenting the body in this manner, we can compare the influence of different body regions on %BodyFat. This approach allows us to identify which body parts are most predictive of body fat percentage and to develop targeted regression models for each region.

## Steps Involved

1. **Data Exploration**: Initial exploration of the dataset to understand the distribution and relationships between variables.
2. **Model Development**: Creation of three multiple regression models using the `lm` function in R, each focusing on different body regions.
3. **Model Interpretation**: Interpretation of the regression coefficients and overall model performance.
4. **Assumption Checking**: Verification of multiple regression assumptions, including:
   - Checking the straight enough condition for each independent variable.
   - Residual analysis (residual plots against each independent variable and predicted values).
   - Histogram of residuals.
   - Normal probability plot of residuals.
5. **Conclusion**: Summarizing the findings and discussing the issues/limitations of the models.

## R Functions Used

- `geom_point()`
- `geom_smooth()`
- `geom_histogram()`
- `geom_density()`
- `geom_qq()`
- `geom_qq_line()`
- `lm()`
- `summary()`
- `anova()`
- `residuals()`
- `sd()`

## Issues/Limitations

- **Sample Size**: The dataset consists of only 250 observations, which may limit generalizability and increase the risk of overfitting.
- **Gender Bias**: The dataset includes only men, making the model potentially inapplicable to women.
- **Exclusion of Age**: Age was not considered, though it significantly affects body fat percentage.
- **Feature Selection**: The chosen features may overlook other important body parts influencing body fat percentage.
- **Multicollinearity**: High correlation among predictors can lead to instability in regression coefficients.

## Conclusion

The analysis provides insights into which body regions are most predictive of body fat percentage. The models developed can help in understanding the relationship between body measurements and body fat, which can be useful for health and fitness assessments.
