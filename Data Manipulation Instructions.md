# Data Manipulation Instructions
## Data Cleaning
### 1. Organize departments by name only by using the **Text to Columns** functionality
Data > Text to Columns > Select “Delimited” > Select “Other” and typing > Select “Do not import column (Skip).”  

After the above steps, the department subcategory numbers in *DESCR column* can be removed and new column with only the department name is created.  

### 2. Calculate the employment time by using the TODAY Excel formula.
* Edit in the Excel formula bar to calculate the length of time for employers.
* Divide the result value by 365 (unit: year) and adjust the cell format to keep only two digits after the decimal point. Save as a new column.  

### 3. Calculate the overpaid_PCT
In multiple linear regression analysis, we calculate and introduce a new independent variable *overpaid_PCT*.
* Formula: overpaid_PCT = (gross - annual_rt / annual_rt)*100%

### 4. Filter data with AutoFilter in Excel
* Filter the data to include only the variables related to our research interest (certain department/job titles/fiscal year). Delete irrelevant columns to integrate a more readable dataset.
* Copy the filtered data into a new excel spreadsheet in our workbook, and rename it for subsequent analysis.  


## Linear Regression Analysis
### 1. Load the Excel Data Analysis ToolPak
Click **File > Options > Add-Ins > Analysis ToolPak** and then you can apply the powerful analysis tool and get your regression result instantly!  
### 2. Conduct Linear regression and interpret the result
* Pay attention to the linear regression statistics and determine what they mean for specific data. 
* Use several metrics (R squared value, p-value, F significance, etc.) to evaluate and adjust your model for better fitting of existing data.



 
