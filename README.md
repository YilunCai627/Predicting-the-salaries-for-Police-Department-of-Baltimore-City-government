# Predicting-the-salaries-for-Police-Department-of-Baltimore-City-government
## Background
In this work, we conduct linear regression analysis in Excel with Baltimore City government employee salaries open data to help the Police Department make better decisions about future budget.  

We’re going to see if we can create a model to help us determine an employee’s salary based on the number of years that they’ve worked in a specific department in Baltimore City government.  

## Data Analytics Outline  
### 1. Industry Questions
Whether we can make predictions about the salaries for a specific agency or type of job within city government using available dataset? What kind of additional information can be explored based on existing data? How can we build explainable and applicable models for city government to design a future budget plan?  
### 2. Data Questions
In this study, we work with [Baltimore City government open salary data](https://data.baltimorecity.gov) to perform linear regression analysis. How can we evaluate the effectiveness and robustness of our models? What are the metrics that we care about for interpreting the result of our prediction models? More specifically, how to interpret the results of linear regression statistics in order to get some insights for Baltimore City government current operations?  

The original data were exported from the Baltimore City Open Data portal as [CSV documents]() by fiscal years, and the processed version [Excel document]() in this repository is aggregated by department in Baltimore City government.
### 3. Data Analysis Tools
A linear regression analysis can facilitate us make predictions about variables based on existing data and further precisely describe specific trends and potential relationships between phenomena.  

To evaluate the quality of our regression models, below metrics are developed by statisticians, which enable us to quantify model effectiveness.  
* **Regression Coefficient**  
In linear regression, coefficients are the values that multiply the predictor values. The sign of each coefficient indicates the direction of the relationship between a independent variable and the dependent variable.

* **R-Squared value**  
R-Squared value shows how well our selected independent variable(s) explain the variability in your dependent variable(s). This metric is always between [0, 1], snd higher R-squared value generally indicates a better model.
*  **P-value**  
The p-value for each independent variable tests the null hypothesis that the coefficient is equal to zero (no effect). Simply put, a predictor that has a low p-value is likely to be a meaningful addition to the model.
### 4. Data Answers
Intuitively, length of employment in Police Department of Baltimore City government might be a reliable indicator for employees' annual salary. To verify this idea, simple Linear regression model is conducted, and the chart below makes this relationship convincingly. This model fit our data with an R2 value of 0.761 and a standard error of residual of $5,757. 
![]()  
In addition to the annual salary as determined on their contracts, we are also interested in what the Baltimore Police Department actually pays their employees and how they might want to think through budgeting for salaries in the department. However, if we perform the same analysis with the GROSS column data (the actual payout for the employee’s salary from the department), we see a very different output. This model fit our data with an R2 value of only 0.007 and a untolerable large standard error of residual.
![]()  

It turns out that the years work for Police Department is not a good predictor of Gross salary, and that there might be other independent variables that actually determine how much an employee gets paid in a given fiscal year.  

How can we better determine a model for predicting the employee’s gross salary? More specifically, the overpaid percent of salary (**overpaid_PCT** = (gross - annual_rt / annual_rt)*100%) is introduced as a new independent variable, and together with employment length to help predict the Gross salary.

Next, we model a multiple linear regression equation to explore other factors related to Gross salary. Campared the R squared value of the result with the previous simple linear regression analysis, it is clear that our new model is more robust. Now, the R2 value is 0.893 and the standard error of residual of approximately $11,170.
![]()
### 5. Industry Answers
With simple linear regression model, we notice that the employment length performs relatively well in the prediction of annual salary of police officers in Baltimore City government. However, this predictor doesn’t give us much information about the trend of gross salary. 

To solve this problem, we introduce aother independent variable and perform multiple linear regression analysis and finally derive a robust model for gross salary prediction. In this condition, our least squares line accounts for approximately 90% of the data. 

Therefore, we recognize that there might be other independent variables that actually determine the final salary payment from the City of Baltimore. To better interpret the relationship and help future budget in specific department, it is necessary to exlore and create additional data points such as their department subcategory or certain types of jobs.



## Data Manipulation Instructions
Want to learn more details about data manipulation in Excel to clean complex dataset and conduct linear regression analysis? Click [***here***]() for a simple step-by-step instructions!  

## Data Sources
* [Baltimore City open salary data](https://data.baltimorecity.gov/browse?category=City+Government)
* [Aggregated Baltimore City salary data for fiscal years 2011-2019](https://github.com/jhu-decision-analytics/multiple-linear-regression-excel-example)
* [Integrated data of the Baltimore Police Department employees for Fiscal Year 2018](加链接！！)
* [Description of Baltimore City governmeny salary data](https://data.baltimorecity.gov/browse?category=City+Government)




