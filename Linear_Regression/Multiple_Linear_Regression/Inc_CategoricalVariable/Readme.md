
#Bulding a Multiple Regression Model (Population Model) with categorical variable
We build a multiple regression model upon the 'simple regression model'. 
The data contains 'SAT' and 'GPA' parameters (like in the simple linear regression model), and now to explore the multiple regression model case, a new parameter (independent variable) is also included called as the 'Attendance'.

Attendace, however, is a categorical variable (either present/absent i.e Yes/No) and we explore how to include such variable in our model. Attendance is marked as 'Yes' if a student attended more that 75% of the lecture and if not it is marked as 'No'.

Analysis steps:
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
