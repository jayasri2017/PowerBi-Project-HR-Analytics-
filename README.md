# PowerBi-Project-HR-Analytics-
Power Bi Project on HR Analytics
Dashboard Link: https://app.powerbi.com/groups/a0b05096-0323-4632-9271-baa870223b84/reports/be6f0e7b-f012-4988-8259-5d19d3998874/ReportSection7e10738d509697f56bd0?experience=power-bi
_________________________________________________________________________________________________________________________________________________________________
Dashboard Snapshots

https://github.com/jayasri2017/PowerBi-Project-HR-Analytics-/blob/b769199f16a0871c898ea9e744f846db7946ed52/DashBoard-Screenshot.png
___________________________________________________________________________________________________________________________________________________________________
Problem Statement
The HR Analytics Dashboard is designed to provide HR professionals with actionable insights into workforce trends and metrics. It helps monitor employee attrition, analyze job roles, and identify demographic patterns that influence retention. By leveraging this tool, HR teams can make data-driven decisions to improve employee satisfaction and organizational efficiency.
___________________________________________________________________________________________________________________________________________________________________
Key issues addressed by this dashboard include:

*Understanding employee attrition across various demographics.

*Identifying high-risk groups with elevated attrition rates.

*Visualizing trends in age, education, and income distribution.

*Providing department and job-level insights for strategic planning.
__________________________________________________________________________________________________________________________________________________________________
Project Objectives

1.Analyze and visualize employee attrition across different demographics.

2.Track age distribution, job roles, and average monthly income trends.

3.Provide HR managers with KPIs such as total employees, attrition rate, and average age.

4.Enable dynamic filtering for granular insights based on gender, department, job level, and more.
___________________________________________________________________________________________________________________________________________________________________
Technology Stack

*Power BI: For interactive dashboard creation.

*DAX (Data Analysis Expressions): For measures and dynamic calculations.
___________________________________________________________________________________________________________________________________________________________________
Dataset Overview

Data Source: Structured dataset with 35 columns and 1,470 rows, containing employee attributes like age, gender, job role, department, education field, monthly income, and attrition status.
___________________________________________________________________________________________________________________________________________________________________
Key Metrics:

*Total Employees: 1,470

*Active Employees: 1,233

*Attrition Count: 237 (16.12%)

*Average Age: 36.92 years
___________________________________________________________________________________________________________________________________________________________________

Data Preprocessing:

Cleaned missing values and categorized key columns (job role, education field, age group).Calculated attrition percentage as a KPI.
___________________________________________________________________________________________________________________________________________________________________
DAX Formulas Used

1. Attrition Percentage:
Attrition Percentage = DIVIDE(COUNTROWS(FILTER(HR_Data, HR_Data[Attrition Status] = "Yes")),COUNTROWS(HR_Data)) * 100

2. Average Monthly Income:
Average Monthly Income = AVERAGE(HR_Data[Monthly Income])

3. Total Employees:
Total Employees = COUNTROWS(HR_Data)

4. Attrition Count:
Attrition Count = CALCULATE(COUNT(HR_Data[Employee ID]),  HR_Data[Attrition Status] = "Yes")

5. Count of Employees by Job Role:
Employees by Job Role = COUNT(HR_Data[Job Role])

6. Average Age:
Average Age = AVERAGE(HR_Data[Age])
___________________________________________________________________________________________________________________________________________________________________
Dashboard Design
Visualizations:
1.Attrition Rate by Age: Funnel chart highlighting the highest attrition rate in the 18–20 age group (57.14%).

2.Employee Count by Age: Bar chart showing distribution across age brackets.

3.Attrition by Education Field: Pie chart representing attrition across education fields (e.g., Life Sciences at 41.22%).

4.Average Monthly Income by Job Role: Bar chart with Managers earning the highest.

5.Job Role Breakdown: Table of employee count by job roles and job levels.
___________________________________________________________________________________________________________________________________________________________________
Filters:

*Gender

*Department

*Job Level

*Work-Life Balance
___________________________________________________________________________________________________________________________________________________________________
Insights
Key Findings:
Attrition Trends:Younger employees (18–20) have the highest attrition rates, suggesting a need for retention strategies.
Attrition is highest among employees with Life Sciences education.
Demographic Insights:Most employees fall in the 30–35 age bracket.
Over 81% of employees are returning customers.
Income Analysis:Managers earn the highest average income.
HR and Sales Executives have lower earnings.
Employee Distribution:Business class travelers account for 69.06% of travel.
___________________________________________________________________________________________________________________________________________________________________
Challenges & Solutions

Challenges:

1.Ensuring accurate KPI calculations (e.g., dynamic attrition rates).

2.Handling performance issues with filters across multiple visualizations.

Solutions:

1.Used DAX measures for efficient and dynamic filtering.

2.Applied consistent data transformations for clarity.
___________________________________________________________________________________________________________________________________________________________________
Results & Impact

Business Impact:

*Empowered HR managers with real-time insights.

*Identified high-risk groups for attrition, enabling targeted strategies.

*Highlighted salary discrepancies for potential adjustments.

Key Outcomes:

*Improved employee retention strategies.

*Reduced manual effort for HR analytics.

*Enhanced decision-making with visual data insights.
___________________________________________________________________________________________________________________________________________________________________
Future Enhancements

1.Integrate predictive models for attrition forecasting.

2.Expand coverage to include recruitment and training metrics.

3.Add time-series analysis for tracking changes in demographics over time.




