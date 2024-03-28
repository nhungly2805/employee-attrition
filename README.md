# Employee Attrition: Short Analysis of IBM HR Data using Power BI
In the fast-changing world of business, it is essential to understand and address employee attrition to achieve organizational success. Employee turnover not only disrupts workforce stability but also significantly affects productivity and overall performance. This report explores the field of human resources data analytics by conducting a brief analysis of employee attrition. It dissects HR data and employee performance to reveal valuable insights into the factors that contribute to attrition.

# Data source:
The data used for this analysis is an augmented version created by real IBM data scientists, though not precisely reflective of actual data. The dataset can be accessed here.

Link to dataset: https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset

# Business questions:
1. What is the overall picture of the company's human resources situation?
2. Which factors contribute to the attrition rate?
3. In the future, in what ways can the company help retain employees?

## Data accuracy:
Before addressing the questions, an assessment of data accuracy is imperative. The dataset comprises 1470 unique values with no missing entries across all columns, and no alterations were made to the original database.

## Answering questions:
### Question number 1: What is the overall picture of the company's human resources situation?

Overall, IBM has 1470 employees, among whom 237 have left the company, and 1233 are still working. 

**Regarding the active workforce:**

- _Department_:

Research and Development has 828 employees

Sales has 354 employees

Human Resources has 51 employees

- _Job Role_:

Sales executives make up the largest employee group with 269 members, while the smallest group consists of 40 employees in Human Resources roles.

- _Department and Job Role_:

For managerial positions, there are 51 Research and Development managers, 31 Sales managers, and 11 Human Resources managers.

![image](https://github.com/nhungly2805/employee-attrition/assets/128270865/38928c5a-c1cb-4a84-bda1-a1c8f35a13c8)

**Overall demographic analysis of the company's workforce:**

The youngest employee is 18, and the oldest is 60. To delve deeper into this factor, I categorize employees into 5 age groups as follows: <20, 20-29, 30-39, 40-49, and>50. The group with the highest number of employees is aged 30-39, with 622 employees. The lowest is the <20 age group with 17 employees. The ratio of men and women between groups is relatively equal.

In terms of gender, although the total number of female employees is lower than male employees, the average income of female employees is higher, **indicating no gender discrimination in the workplace.**

Analyzing marital status, the proportion of married individuals is 45.78%, single individuals are 31.97%, and divorced individuals are 22.24%.

The attrition rate is currently at 16.12%. On average, employees tend to stay with the organization for around 7 years. Based on these metrics, it appears that IBM has a good level of employee attachment.

![image](https://github.com/nhungly2805/employee-attrition/assets/128270865/112287c9-ffbf-43b9-aae0-3b53dae016a0)


### Question number 2: Which factors contribute to the attrition rate?

To precisely identify the elements influencing attrition decisions, we must **rely on the attrition rate across various attributes, considering the substantial disparities in the number of individuals within each distinct element**.

One of the most important metrics is **the new hire attrition rate**. This metric tracks the number of new employees who leave the company within the first year of employment, to calculate the new hire retention rate, divide the number of employees who leave within their first year with the organization (or whatever period seems relevant) by the total number of employees who left during the same period. This metric, **at 31.65%, is relatively high.**

- _Age Group_:

The attrition rate within the <20 age group is the highest. This group has a small number of employees, only 17. Therefore, instead of focusing deeply on this group, attention should be directed towards **the 20-29 age group, which has the second-highest attrition rate**.

- _Departments_:

The rate of people leaving between departments is relatively equal: 19.05% for human resources, 13.84% for research and development, and 20.63% for the sales department.

- _Job Role_:
- 
**A notable thing here is that sales representatives have a very high churn rate, nearly 40%**.
  
- _Job satisfaction, environment satisfaction, job involvement, and work-life balance_

Among these four factors, the emphasis should be placed on job involvement, as individuals assigning the **lowest scores exhibit a significant churn rate of up to 33.73%. In contrast, those with the highest scores experience a churn rate of less than 10%**. This underscores the critical importance of prioritizing job involvement when formulating effective talent retention policies for companies.

### Question number 3: In the future, in what ways can the company help retain employees?

Lastly, a deeper investigation into the reasons for attrition will focus on three important groups: the 20-29 age group, sales representatives, and new hires.

To identify factors contributing to high attrition rates in these groups, a decomposition tree chart will be used, considering factors such as Job Satisfaction, Job Involvement, Environment Satisfaction, work-life balance, work overtime, and business travel. I use the "high-value" option to determine the most impactful factors.

- **_Sales group_**:

An interesting finding is that employees with high work-life balance have the highest attrition rates. Thus, **work-life balance is not the factor leading to attrition in the Sales group**. 

Instead, factors such as Business Travel, Environment Satisfaction, Job Involvement, and Job Satisfaction are likely more influential. Therefore, a different starting point is chosen for analysis, resulting in a picture below.

After analyzing the situation, **two areas that need improvement have been identified: job involvement and business travel**. However, it's important to note that Sales is a job that requires frequent travel to meet clients. Instead of reducing travel, the company could **consider enhancing travel budgets or commissions to improve employee satisfaction**.

![image](https://github.com/nhungly2805/employee-attrition/assets/128270865/a1dae65f-9796-4049-8446-7f8ec5f38cbd)
![image](https://github.com/nhungly2805/employee-attrition/assets/128270865/cf832f29-472b-4d40-9625-b550d03a5afc)

- **_Employees with less than 1 year of tenure_**:

In relation to the business travel factor, the explanations provided are almost the same for each answer. I will go through each answer and display the three images below. 

It is not clear which of the six factors has the most impact. However, low satisfaction with the environment seems to be the most significant factor as it is the only similarity between 3 visuals.

![image](https://github.com/nhungly2805/employee-attrition/assets/128270865/c4f3e7db-9244-4059-b041-ae1789e8e0dc)

![image](https://github.com/nhungly2805/employee-attrition/assets/128270865/44b5ec42-4119-4cae-b20f-a9463645c2dd)

![image](https://github.com/nhungly2805/employee-attrition/assets/128270865/3353f86d-0446-4a41-a808-78f266b8d518)

However, when I use "Environment satisfaction" as the starting point (Image below), the effect is still unclear. It's hard to know which factors are most important in this group so **further analysis should be made**.

![image](https://github.com/nhungly2805/employee-attrition/assets/128270865/5f5a7502-c7c9-48f0-9024-c400f3670e8c)


- **_20-29 Age group_**:

Based on the chart, the three most **crucial factors to consider are work-life balance, job involvement, and working overtime**. As the group is still young, they may not be aware of ways to balance work and life. Therefore, the HR team could provide a short lesson to teach them how to manage their work-life balance. Additionally, reducing overtime or offering higher compensation for overtime work could significantly improve job satisfaction and retention.

![image](https://github.com/nhungly2805/employee-attrition/assets/128270865/4046eadf-a998-4be7-94ad-57cb151a37f4)

### Conclusions:
In order to reduce the overall attrition rate of the company, we should prioritize improving job involvement. For employees in the Sales representative roles, the company could consider enhancing travel budgets or commissions. For employees who have worked in the company for a year or less, further analysis should be conducted to investigate and address the reasons behind the high attrition. For employees aged between 20-29 years, the HR team could provide a short lesson to teach them how to manage their work-life balance effectively. Additionally, reducing overtime or offering higher compensation for overtime work could significantly improve job satisfaction and retention.
