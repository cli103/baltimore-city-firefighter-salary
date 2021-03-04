# Regression Analyses for Baltimore City Fire Fighter Salaries
## Background

I used Microsoft Excel to conduct data analysis on the annual salary of fire fighters in Baltimore City. I used open data from the Baltimore City government on employee salaries from 2011 – 2020 to generate a regression model to predict the future annual salary of fire fighters. 

## Business Question
Can we predict the annual salary for a fire fighter based on data from previous years?

## Data Sources – Open Data
[Baltimore City Government Employee Salaries](https://data.baltimorecity.gov/datasets/baltimore-employee-salaries).
The relevant file can be found [here](https://github.com/cli103/baltimore-city-firefighter-salary/blob/main/Baltimore_City_Employee_Salaries.csv)

## Data Analysis
Find step-by-step instructions [here](https://github.com/cli103/baltimore-city-firefighter-salary/blob/main/excel-instructions)

I generated a simple linear regression model pictured below. 

![alt text](https://github.com/cli103/baltimore-city-firefighter-salary/blob/main/Simple%20Regression%20Annual%20Salary.png)

As labeled, the best fit line is y = 0.5718x + 18668 and the r squared value is 0.3127. This means that a one dollar difference in the previous year’s salary is associated with a 0.5718 dollar difference in the current year’s salary. As the r squared value is quite low, the model only represents around 31% of the variation in a fire fighter’s average annual salary is explained by their salary from the previous year. The standard error of the residual is 6679.82. The p-value is 0.12 which is greater than 0.05, meaning that the average annual salary of the previous year is not a significant predictor of the annual salary in the current year. As a result, the regression model does not seem to provide an accurate prediction of the annual salary of Baltimore City firefighters.

I also generated a simple linear regression model comparing the average gross salary of Baltimore City fire fighters to the previous year pictured below. 

![alt text](https://github.com/cli103/baltimore-city-firefighter-salary/blob/main/Simple%20Regression%20Gross%20Salary.png)

The model represents around 42% of the variation in a fire fighter’s average gross salary is explained by their gross salary from the previous year. It seems to be a more accurate regression model for the prediction of the annual gross salary.

I conducted a multiple regression analysis using the previous year’s average annual salary, the gross salary and the previous year’s gross salary to predict the annual salary of Baltimore City fire fighters. The p-values of the previous year’s average annual salary and gross salary were both greater than 0.05, and therefore were not significant predictors of annual salary. The p-value of average gross pay was significantly less than 0.05 and therefore is a significant predictor of gross pay. The r squared value was 0.96, meaning that the model accounts for 96% of the variation in a firefighter’s annual salary. However, the F test result was 35.58, which is greater than 0.05, meaning that there is a 36% probability that none of the identified parameters are significant for predicting annual salary. View the full analysis [here](https://github.com/cli103/baltimore-city-firefighter-salary/blob/main/Baltimore%20City%20Fire%20Fighter%20Salary%20Analysis.xlsx)

This data may be important for the Baltimore City Fire department to consider when setting the annual salary for fire fighters. A sudden decrease in average salary such as from 2015 – 2016 may affect the retention of fire fighters as well as the longevity of the career path. In 2016, the amount of fire fighters in the Baltimore City Fire Department decreased from 45 to 5. If the department is affected by sudden layoffs and the annual salary does not grow year over year, people may be discouraged from becoming a fire fighter. Other data that may improve this model include number of fire fighters, years worked and differences between part time and full time salaries. This may provide more information regarding why the average annual salary has declined significantly since 2015. 
