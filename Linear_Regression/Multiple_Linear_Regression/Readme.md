We build a multiple regression model upon the 'simple regression model'. The data contains 'SAT' and 'GPA' parameters (like in the simple linear regression model), and now to explore the multiple regression model case, a new parameter (independent variable) is also included called as the 'Attendance'.

Attendace, however, is a categorical variable (either present/absent i.e Yes/No) and we explore how to include such variable in our model. Attendance is marked as 'Yes' if a student attended more that 75% of the lecture and if not it is marked as 'No'.

The approach is inspired by concepts presented in the 'Complete Data Science Bootcamp 2025' course on Udemy, and it expands on these fundamental principles with a detailed explanation of the modeling process, results, and linearity assumption testing.

Here are the steps followed in the analysis:

- Step 1: Import the needed libraries
- Step 2: Load the Data
- Step 3: Map the data
- Step 4: Perform Descriptive Statistics
- Step 5: Build the Multiple Regression model
  - 5(a) Define the dependent and independent variables
  - 5(b) Perform Regression Analysis
  - 5(c) Formulate the regression lines for two cases of dummy variable
  - 5(d) Plot the two regression line(s) on the scatter plot
  - 5(e) Easy visualization with color coded data points
  - 5(f) Add the original regression line in the above plot
- Step 6: Making predictions using the regression model
  - 6(a) create a data-frame and use it for prediction
  - 6(b) Make predictions for new data from the fitted regression
  - 6(c) Arrange predicted value along with the data used for prediction
  - 6(d) Impact of dummy variable in prediction
