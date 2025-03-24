This directory will contain:
1. the data which will be tested to be fitted with linear regression model
2. analysis script building the linear regression model

Analytis steps of Simple Linear Regression Example
- Step 1: Import the relevant libraries
- Step2: Load the Data
- Step 3: Descriptive Statistics
- Step 4: Create Regression model
  - 4(A) Define the dependent and independent variables
  - 4(B) Perform Exploratory Data Analysis (EDA)
  - 4(C) Perform Regression analysis
- Step 5: Check if the assumptions of Linear Regression Model hold
  - 5(A) Linearity
  - 5(B) Independence (of observations)
  - 5(C) No-autocorelation (of residuals)
  - 5(D) Homoscedasticity (Constant Variance)
  - 5(E) Normality
- Step 6: Summarization of the violations in linearity assumptions and their impact
- Step 7: How to address the above violations in linearity assumption


What to look-out in the summary?

- A) Model Fit Strength (R-squared & Adjusted R-squared):

  - R-squared:
    - measures goodness of fit of the model (i.e. how well the model fits the data).
    - is the ratio of variability explained by regression to the total variability of the dataset.
    - Represents the proportion of variance in the dependent variable (y) explained by the independent variables (x), i.e., how much of the total variability of the data is explained by regression model.
    - Has value [0, 1]. A higher value (closer to 1) indicates a better fit.
    - Consider the context; a "good" R-squared varies across disciplines.
    - Example: If 0.406, indicates ~ 40% variance in GPA is explained by SAT score. It is a moderate fit. While statistically significant, a considerable portion of GPA variance is left unexplained, suggesting other influential factors.

  - Adjusted R-squared:
    - Like R-squared, measured how well the regression model fits the data.
    - Accounts for the number of predictors, penalizing the inclusion of unnecessary variables.
    - Use when comparing models with different numbers of predictors.
    - It is always lower than the R squared.
    - Example: If 0.399
      
- B) Overall Model Significance (F-statistic & Prob(F-statistic)):

  - F-statistic:
    - Tests if the independent variables, as a group, have a significant effect on the dependent variable.
    - A high F-statistic suggests a significant relationship.

  - Prob(F-statistic):
    - The p-value associated with the F-statistic.
    - A low p-value (typically < 0.05) indicates the overall model is statistically significant.

- C) Individual Variable Significance (Coefficients & P>|t|):
  - Coefficients (coef):
    - Estimated values of the regression coefficients (e.g. 'm' and 'c').
    - Indicate the change in the dependent variable for a one-unit change in the independent variable.
    - Sign and magnitude are crucial.
      
  - t-statistic:
    - = coeff/standard error
    - small t-statistic will resuls in a high p-value (P>|t|).

  - P>|t| (p-value):
    - Tests the significance of individual coefficients.
    - A low p-value (typically < 0.05) indicates the coefficient is statistically significant.
    - Confidence intervals also help to verify significance.
   
D) Assumption Violations (Residual Diagnostics: Omnibus, Durbin-Watson, Jarque-Bera, Skew, Kurtosis):

  - Omnibus & Jarque-Bera (JB):
    - Test the normality of residuals.
    - Significant p-values indicate non-normal residuals.
    - JB test quantifies how far the distribution is from a normal distribution based on the skewness and kurtosis.
      
  - Durbin-Watson:
    - Tests for autocorrelation (independence) of residuals.
    - Values far from 2 indicate potential autocorrelation.
      
  - Skew & Kurtosis:
    - Describe the shape of the residual distribution.
    - Deviations from 0 (skew) and 3 (kurtosis) suggest non-normality.
    - Residual analysis is important for model validity.
      
E) Multicollinearity (Condition Number):

  - Condition Number:
    - Refers to a situation in multiple linear regression where two or more independent variables are highly correlated.
    - High values suggest multicollinearity, which can destabilize coefficient estimates.
    - This is very important when there are multiple independent variables.
