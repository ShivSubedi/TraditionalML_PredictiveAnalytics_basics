This directory 'Check_RandomVariableEffect' builds upon the 'Simple Linear Regression Model' example of 'GPA' and 'SAT' score and adds new variable called 'Rand 1,2,3' in the dataframe. 
'Rand 1,2,3' assigns random valuse from 1-3 to each student.
We will build a multiple linear regression with the:
- dependent variables 'SAT' and 'Rand 1,2,3'
- independent variable 'GPA'

Goal: Test how the model behaves to addition of a totally unrelated random parameter like 'Rand 1,2,3' in the model. What will be the test results and will the model be able to identify and reject inclusion of this random variable?

Following are the steps performed in the analysis:

=======Table of contents========
Bulding a Multiple Regression Model (Population Model)
- Step 1: Import relevant libraries
- Step 2: Load the Data
- Step 3: Descriptive Statistics
- Step 4: Build the Multiple Regression model
  - 4(a) Define the dependent and independent variables
  - 4(b) Perform Regression Analysis
- Step 5: Comparison with the 'Simple Regression Model'
  - 5(a) Comparing R-squared and Adj. R-squared
  - 5(b) Can adding impractical variable be pointed by the model itself?
  - 5(c) Comparing the F-statisti
