# Employee Attrition: Short Analysis of IBM HR Data using Tableau
In the dynamic landscape of business, comprehending and mitigating employee attrition is crucial for organizational success. Employee turnover not only disrupts workforce stability but also profoundly impacts productivity and overall performance. This report delves into the realm of human resources data analytics, conducting a short analysis of employee attrition by dissecting HR data and employee performance to uncover valuable insights into the factors influencing attrition.
# Data source:
The data used for this analysis is an augmented version created by real IBM data scientists, though not precisely reflective of actual data. The dataset can be accessed here.
Link to dataset: https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset
# Business questions:
1. How many people leave the company?
2. Which factors contribute to the decision to leave the company?
## Data accuracy:
Before addressing the questions, an assessment of data accuracy is imperative. The dataset comprises 1470 unique values with no missing entries across all columns, and no alterations were made to the original database.
## Answering questions:
Link to the dashboard: https://public.tableau.com/app/profile/nhung.ly/viz/Employeeatrrition/Dashboard1
### Question number 1: Overall Attrition Statistics
A total of 237 individuals left the company, categorized by gender, education field, and marital status.
- By gender:
Female: 87
Male: 150
- By education field:
Human Resources: 7
Life sciences: 89
Marketing: 35
Medical: 63
Technical degree: 32
Other: 11
- By marital status:
Divorced: 33
Married: 84
Single: 120
### Question number 2:
To precisely identify the elements influencing attrition decisions, we must **rely on the attrition rate across various attributes, considering the substantial disparities in the number of individuals within each distinct element**.
- _Overtime_:
Employees **working overtime exhibit a 31% attrition rate compared to 10% for those without overtime requirements.**
--> The substantial difference in attrition rates highlights the potential strain imposed by overtime on employee retention, emphasizing the need for a balanced workload.
- _Business travel_:
No Travel: 8%
Rare Travel: 14.96%
Frequent Travel: 24.91%
--> The **escalating attrition rate with increased travel frequency** underscores the importance of assessing the impact of business trips on employee satisfaction and retention.
- _Departments_:
The rate of people leaving between departments is relatively equal: 19.05% for human resources, 13.84% for research and development, and 20.63% for the sales department.
- _Position_:
**A notable thing here is that sales representatives have a very high churn rate, nearly 40%**.
- _Job level_:
The inverse relationship between job level and attrition indicates potential dissatisfaction among lower-level employees, necessitating a review of career growth opportunities and recognition.
- _Job satisfaction, environment satisfaction, job involvement, and work-life balance_
Among these four factors, the emphasis should be placed on job involvement, as individuals assigning the **lowest scores exhibit a significant churn rate of up to 33.73%. In contrast, those with the highest scores experience a churn rate of less than 10%**. This underscores the critical importance of prioritizing job involvement when formulating effective talent retention policies for companies.
### Suggestions:
To improve the attrition rate of the company, the HR team should prioritize improving job involvement. Additionally, investigating and addressing the reasons behind the high attrition among sales representatives is crucial. Efforts to reduce overtime/business travel demands or provide higher compensation for overtime work/business travel could enhance overall job satisfaction and retention.
![image](https://github.com/nhungly2805/employee-attrition/assets/128270865/8c97ac60-1fbd-47e8-9904-c3207d5ab300)
