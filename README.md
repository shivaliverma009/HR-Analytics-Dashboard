# HR-Analytics-Dashboard
Interactive Tableau dashboard analyzing HR attrition and workforce insights.

HR Analytics Dashboard - Tableau

📊 This HR Analytics Dashboard provides a detailed view of workforce insights such as employee distribution, attrition trends, education impact, job satisfaction, and demographics.
The goal of this project is to help the HR team understand attrition causes and employee engagement patterns to take data-driven decisions.


---

🚀 Objectives

Analyze employee attrition by various factors (gender, department, age, education).

Track key workforce KPIs like attrition rate, employee count, and active employees.

Identify patterns in job satisfaction ratings and their relation to attrition.

Provide an overview of demographic insights for better HR planning.



---

🔑 Key Metrics (KPIs)

Employee Count: 1470

Attrition Count: 237

Attrition Rate: 16.12%

Active Employees: 1233

Average Age: 37 years

---

🧮 Calculated Fields Used

1. Attrition Count

IF [Attrition] = "Yes" THEN 1 ELSE 0 END

✔ Used to calculate the number of employees who left.

2. Active Employees

COUNT([Employee ID]) - SUM([Attrition Count])

✔ Shows current employees after removing attrition.

3. Attrition Rate

(SUM([Attrition Count]) / COUNT([Employee ID])) * 100

✔ Measures the percentage of employees who left.

4. Age Grouping

IF [Age] >= 18 AND [Age] <= 25 THEN "18-25"
ELSEIF [Age] >= 26 AND [Age] <= 35 THEN "26-35"
ELSEIF [Age] >= 36 AND [Age] <= 45 THEN "36-45"
ELSEIF [Age] >= 46 AND [Age] <= 55 THEN "46-55"
ELSE "56-60"
END

✔ Used to segment employees into age groups.

5. Gender-wise Attrition

IF [Attrition] = "Yes" THEN [Gender] END

✔ Helps visualize male vs female attrition counts.


---

📊 Visualizations in Dashboard

KPI Cards → Employee Count, Attrition Count, Attrition Rate, Active Employees, Avg Age

Pie Chart → Department-wise Attrition

Bar Chart → Education-wise Attrition

Donut Charts → Attrition by Gender & Age Groups

Bar Chart → Employees by Age Group

Heatmap → Job Satisfaction Rating across Job Roles



---

🛠 Tools Used

Tableau → Dashboard development & visualization

Excel → Data preparation & cleaning



---

🔍 Insights


This file explains the key insights from the HR Analytics Dashboard built in Tableau.
Key Insights:

1. Overall Attrition Rate: Shows the percentage of employees leaving the company. Helps HR evaluate overall retention performance.

2. Attrition by Department: Highlights departments with the highest attrition rates. For example, Sales may have higher turnover than R&D, indicating the need for department-specific retention strategies.

3. Attrition by Age Group & Gender: Provides demographic insights into workforce turnover. Helps identify if specific age groups or genders need more engagement initiatives.

4. Job Satisfaction Levels: Analyzes satisfaction ratings across departments and roles. Lower satisfaction scores may indicate issues in work culture, workload, or growth opportunities.

5. Attrition by Education Field: Examines the relationship between education background and attrition. Useful for HR to align training programs or skill development plans.

6. Attrition by Salary Slab: Compares attrition rates across salary ranges to check if compensation plays a role in employee exits.


Purpose:

>Improve employee retention strategies

>Enhance workforce planning

>Make data-driven decisions for better employee experience




📷 Dashboard Preview

<img width="1542" height="880" alt="Screenshot 2025-09-25 091821" src="https://github.com/user-attachments/assets/c584d12f-66d3-4c52-9943-caa1bf93b269" />






