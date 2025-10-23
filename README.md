# Predicting-Austin-House-Prices: Statistical Modeling of Real Estate Values in Austin, TX
Experimental modeling study to identify the key factors influencing housing prices in Austin, Texas. Examined relationships among housing characteristics such as living area, number of bathrooms, school ratings, and home age to create a predictive model using multiple linear regression.

## Approach
Collaborated with a team of UCLA students as part of our regression modeling course.
Utilized a dataset of single-family homes in Austin, TX, scraped from Zillow (January 2021).
Focused on determining which property features most strongly predict house prices.
Cleaned and filtered the dataset to remove inconsistencies and outliers, then applied a sequence of models to improve fit and adherence to statistical assumptions:

1. **Model 1:** Untransformed multiple linear regression.
2. **Model 2:** Box-Cox and inverse response transformations to address non-linearity and heteroscedasticity.
3. **Model 3 (Final):** Forward selection using AIC and BIC criteria, adding *house age* as a new predictor.

## Analysis:
Performed in R using multiple regression and transformation techniques.

* Diagnostics: Examined residuals vs. fitted, Q-Q, and scale-location plots for linearity, normality, and constant variance.
* Feature selection: Based on AIC, BIC, and adjusted R².
* Multicollinearity check: Verified with VIF values (<5).
* Interpretation: Derived relationships between living area, number of bathrooms, school ratings, and house age with predicted prices.

## Findings:
* The final model explained ~46.8% of the variation in housing prices.
* Living area (sqft) and number of bathrooms had the strongest positive effects on price.
* Average school rating also positively correlated with home value, though less strongly.
* House age showed a small but positive association — possibly reflecting the higher value of established or historic homes.
* The model achieved the best balance of interpretability and predictive performance after applying power transformations (Box-Cox and inverse response).

These results align with real-world housing economics, where larger homes and better school districts command higher prices. Future work could extend this model by incorporating neighborhood-level or economic indicators to improve predictive accuracy.
