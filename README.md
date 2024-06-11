# HR Analytics Dashboard

## Description:
The Dashboard helps to enhance employee retention while reducing attrition rates and pinpoint areas of concern and develop targeted retention strategies. This may include improving work-life balance, career development opportunities, compensation and benefits, or addressing issues related to workplace culture or leadership.

Objective: Help the organization to improve Employee Retention (Reduce Attrition) by creating HR Analytics Dashboard. 


### Steps followed:

1.	Select HR Analytics as Dataset.
1.	Use HR Analytics Dataset.
2.	Go to Transform data, Open Power Query Editor – In HR Analytics Dataset, the following are the changes made - 

•	Data quality – Use column quality to find the distribution of valid, error, and empty values within a column. 
Remove null values are using remove rows in reduce row under Home tab.
Replace values using replace values.

•	Datatypes – Use Detect data type under transform tab.

•	Duplicates – Remove duplicates using remove duplicates. 
  
2.	Create charts: Charts provide insights into Key Performance Indicators (KPIs).
3.	Create Slicers: Departments listed in them. Here, Departments are filtered to view specific data.


4.	Create Calculated Fields related to Key Performance Indicators and name it.

5.	Create a dashboard: Align all charts in the dashboard.


6.	Show the below following details of Key Performance Indicators - 

•	Count of Employee

•	Attrition 

•	Attrition Rate

•	Average Age

•	Average Salary 

•	Average Years

New Calculated Fields using DAX functions:

•	Count of Employee - DISTINCTCOUNT(HR_Analytics[EmpID])

•	Attrition Count - 

Formula used: If (Attrition) = ‘yes’
Then 1
Else 0
End



•	Attrition Rate -

Formula used: SUM(HR_Analytics[AttritionCount])/SUM(HR_Analytics[EmployeeCount])

•	Average Age - AVERAGE(HR_Analytics[Age])

•	Average Salary - AVERAGE(HR_Analytics[MonthlyIncome])

•	Average Years - AVERAGE(HR_Analytics[YearsAtCompany])

 # Dashboard Snapshot (Power BI DESKTOP)
 
![HR Analytics Dashboard](https://github.com/anushar779/Power-BI-Project-work-1/assets/170659132/7aea9582-d0e2-43db-8e33-1402a500bda8)

# Interpretation:

### Key Metrics Overview: 

Visualization:

•	Count of Employees: Number of employees currently in the organization.

•	Attrition: Employees who left the organization within a specific period.

•	Attrition Rate: Percentage of employees who left the organization within a specific period.

•	Average Age: Average age of employees in the organization.

•	Average Salary: Average Salary of employees in the organization.

•	Average Tenure/Average Years: Average length of time employees stay with the organization.

Interpretation:

•	Attrition Rate: A high attrition rate may indicate dissatisfaction or other issues within the organization. Compare against industry benchmarks.

•	Average Tenure: Short average tenure might suggest issues with employee satisfaction or onboarding processes.

•	Average Age: Average age may indicate the general age distribution within an organization.

•	Average Salary: Average Salary may indicate the typical compensation level within an organization.
           
### Employee Turnover Analysis:

Visualization:

•	Attrition by Education: Donut chart showing attrition rates at Education level.

•	Attrition by Salary: Horizontal bar chart showing attrition by Salary.

•	Attrition by Job Role: Horizontal bar chart showing attrition by Job Role.

•	Attrition by Age: Vertical bar chart showing attrition by Age.

•	Attrition by Gender: Tree map showing attrition by Gender.

•	Turnover Trend Over Time/Attrition by Years: Line chart showing attrition trends over years.

Interpretation:

•	Attrition by Education: Higher attrition rates among certain education levels may suggest varying career expectations or opportunities.

•	Attrition by Salary: Higher attrition among lower salary bands may suggest dissatisfaction with pay or limited opportunities for advancement. Conversely, elevated turnover in higher salary brackets could signal issues like burnout or unmet expectations.

•	Attrition by Job Role: High attrition in certain roles may indicate challenges such as job dissatisfaction, limited growth opportunities, or poor fit.

•	Attrition by Age: Higher attrition among younger employees might signal career exploration or dissatisfaction, while elevated turnover among older employees could indicate retirement or workplace challenges.

•	Attrition by Gender: Higher attrition among one gender may indicate potential issues such as unequal opportunities, workplace culture disparities, or work-life balance challenges.

•	Attrition by Years: Higher attrition among newer employees might suggest onboarding or cultural alignment issues, while elevated turnover among longer-tenured employees could signal burnout or lack of career growth opportunities.
  
  ### Descriptive analysis:

Visualization:

•	Job satisfaction at Job level: The table chart displays ratings or scores provided by employees regarding their job satisfaction.

Interpretation:

•	Table chart presents job satisfaction ratings provided by employees, rating ranging from 1 to 4 with 1 representing the highest level of satisfaction and 4 representing the lowest level of satisfaction. Each cell in the table represents the number of employees who rated their satisfaction at a job level. 

•	Ratings may be based on various factors such as work-life balance, compensation, career development opportunities, organizational culture, and job responsibilities.

 ### Recommendations:

For Retention:

•	Implement career development programs.

•	Review and adjust compensation packages to be competitive.

•	Conduct regular stay interviews to understand employee needs and concerns.
 

