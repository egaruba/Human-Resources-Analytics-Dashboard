# Unlocking HR Performance: A Data-Driven Exploration of Employee Metrics

![](human_resources_department.png)
---

## Table of Contents

- [Project Overview](#project-overview)
- [Background](#background)
- [Problem Statement](#problem-statement)
- [Entity Relationship Diagram](#entity-relationship-diagram)
- [Tools Used](#tools-used)
- [Skills Applied](#skills-applied)
- [Data Preparation](#data-preparation)
- [Data Cleaning](#data-cleaning)
- [Issues Found](#issues-found)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Functional Validation](#functional-validation)
- [Data Validation and Analysis](#data-validation-and-analysis)
- [Insights and Findings](#insights-and-findings)
- [Conclusion](#conclusion)

## Project Overview

This employee data analysis project aims to provide insights into the lack of clear trackable performance metrics for the Human Resources Department. By analysing various aspects of the employee data, I hope to identify trends, make data-driven recommendations and gain a deeper understanding of the Human Resources Department’s key performance metrics.

> *Disclaimer: All datasets and reports do not represent any company, institution or country. This is just a dummy dataset to demonstrate my capabilities in Tableau and SQL.*

### Project Objectives

- Assess the performance of different employees within the Human Resources Department, identifying areas of high attrition and opportunities for job satisfaction. 

- Explore staff patterns, segmentations, and preferences through SQL queries, aiming to improve job satisfaction.

- Analyse employee data to identify trends in staff performance, education based variations and gender preferences to make informed data driven decisions.

- Generate actionable insights from the analysis, empowering decision-makers to make informed and strategic choices that improve the department’s employee satisfaction.

## Background 

The Human Resources Department is responsible for monitoring and managing various aspects of employee data to ensure the organisation maintains a healthy workforce. However, there is a lack of clear performance indicators to track and analyse key Human Resource metrics. Therefore, there is a need to design and implement a set of KPIs to address the following issues: employee count at the company, attrition count of employees at the company, attrition rate of employees at the company, active employees at the company and average age of employees at the company.
 
### Dataset Overview

The raw dataset contains one .xlsx file named “HR Data.xlsx” and one CSV file titled “hrdata.csv”. Both of these files were used for this project. You can find the raw datasets [here](https://github.com/egaruba/Human-Resources-Analytics-Dashboard/tree/main/dataset).

## Dataset Description

- hrdata: The primary dataset used for this analysis is the "hrdata.csv" file, containing detailed information about each employee at the company.
The raw dataset contains 1,470 records of employee data. The file has 1,470 rows and 15 columns. Each record represents a unique employee at the company. The records include various attributes such as gender, employee id number, marital status, age band, age, department, education, job role, education field, business travel, employee count, attrition, attrition label, job satisfaction and active employee. 

- HR Data: The alternative dataset provided for this analysis is the “HR Data.xlsx" file. It contains additional and more detailed information about each employee at the company.
The raw dataset contains 1,470 records of employee data. The file has 1,470 rows and 41 columns. Each record represents the same employee data as provided by the "hrdata.csv" file. 
The additional information not previously provided includes attributes such as over 18, training times last year, -2, 0, daily rate, distance from home, environment satisfaction, hourly rate, job involvement, job level, monthly income, monthly rate, number of companies worked, percent salary hike, performance rating, relationship satisfaction, standard hours, stock option level, total working years, work life balance, years at the company, years in current role, years since last promotion and years with current manager.

[Go to TOC](#table-of-contents)

## Problem Statement

The Human Resources Department is responsible for monitoring and managing various aspects of employee data to ensure the organisation maintains a healthy workforce. However, there is a lack of clear performance indicators to track and analyse key departmental metrics. 

### KPI Requirements

There is a need to analyse and implement a set of KPIs to address the following issues:

- Employee Count at the Company: The Human Resources Department lacks visibility into the total number of employees, making it challenging to assess workforce size and plan for future growth or downsizing effectively.

- Attrition Count of Employees at the Company: The organisation lacks a standardised method to track employee attrition, resulting in incomplete and unreliable data on the number of employees who have left the organisation. 

- Attrition Rate of Employees at the Company: Without a clear measure of attrition rate, the organization cannot assess the overall turnover level or compare it with industry benchmarks, hindering the ability to gauge employee satisfaction and engagement.

- Active Employees at the Company: The organisation lacks a mechanism to differentiate between active and inactive employees, leading to difficulties in accurately assessing the current workforces’s productivity and capacity.

- Average Age of Employees at the Company: The Human Resources Department lacks visibility into the average age of employees, making it difficult to evaluate workforce demographics, succession planning, and the organisation’s ability to attract and retain younger talent.

### Chart Requirements

There is a need to design and visualise charts and graphs to address the following issues:

- Attrition by Gender at the Company: The Human Resources faces challenges in understanding the attrition patterns based on gender, making it difficult to identify any gender-related disparities and implement targeted retention strategies.

- Attrition by Department at the Company: The Human Resources Department lacks visualisations to showcase attrition rates across different departments. This hinders their ability to identify departments with higher attrition rates and address any underlying issues or concerns effectively. 

- Number of Employees by Age Group at the Company: The Human Resources Department requires visual representations to analyse the distribution of employees across various age groups. This helps in assessing workforce demographics, identifying any age-related gaps or imbalances, and implementing targeting Human Resource policies or programs.

- Job Satisfaction Ratings at the Company: The Human Resources Department lacks visualisations to represent job satisfaction ratings, hindering their ability to measure employee engagement and overall job satisfaction.

- Attrition by Education at the Company: The Human Resources Department requires visual representations to analyse attrition rates based on education fields. This helps identify specific educational backgrounds that may be associated with higher attrition, enabling the organisation to tailor retention strategies accordingly.

- Attrition Rate by Gender for Age Groups at the Company:  The Human Resources lacks visualisations that display attrition rates based on gender and different age groups. This makes it challenging to identify any age and gender-related attrition trends, preventing the organisation from implementing targeted retention strategies for specific employee segments.

[Go to TOC](#table-of-contents)

## Tools Used

1. Excel - Data Cleaning
2. MySQL - Data Analysis
3. Tableau - Creating Visualisations and Reports

## Skills Applied

1. Data Validation using SQL
2. Database Creation
3. SQL Functions
4. Functional Validation
5. Aggregations

[Go to TOC](#table-of-contents)

### Data Cleaning Process

The data cleaning process involves the following steps:

1. Data Preparation: This explains how I sourced the Human Resources department dataset for analysis, the structure and the key attributes of our dataset.

2. Data Cleaning: This involves steps taken to clean and preprocess the dataset to ensure its quality and reliability. The techniques used for handling missing values, standardising formats, and cleaning inconsistent data. The dataset was thoroughly examined to understand the structure, columns and their meanings. The data did not have a data dictionary attached.

3. Exploratory Data Analysis with SQL: Running SQL queries allows for the unveiling of employee trends, variations via education, employee behaviours and departmental insights. Exploratory Data Analysis is significant in understanding the dataset’s characteristics. The utilisation of more complex SQL techniques allows for deeper analysis, where the advanced SQL functions, window functions, will be used to derive insights beyond standard queries.

4. Insights and Recommendations: Summarise the key insights derived from the analysis. Discuss actionable recommendations based on SQL driven insights for enhancing employee satisfaction, optimising staff performance and improving employee experiences.

5. Dashboard Visualisation and Report: A dashboard visualisation that explains each segments and displays Key Performance Indicators to the client.

## Data Preparation

In the data preparation phase, I performed the following tasks:

1. Created a database, setup tables, and imported data.[PIC]

| Column                  | Description                             | Data Type      |
| :---------------------- | :-------------------------------------- | :------------- |
| EmployeeID              | Unique identifier for each employee     | VARCHAR(50)    |
| Gender                  | Gender of the employee                  | VARCHAR(50)    |
| MaritalStatus           | Marital status of the employee          | VARCHAR(50)    |
| AgeRange                | Age range of the employee               | VARCHAR(50)    |
| Age                     | Age of the employee                     | INT            |
| Department              | Department where the employee works     | VARCHAR(50)    |
| Education               | Highest education level attained        | VARCHAR(50)    |
| EducationField          | Field of education specialization       | VARCHAR(50)    |
| JobRole                 | Role of the employee within the company | VARCHAR(50)    |
| BusinessTravel          | Frequency of business travel            | VARCHAR(50)    |
| DistanceFromHome        | Distance from home to workplace         | INT            |
| OverTime                | Whether employee works overtime	    | VARCHAR(50)    |
| EmploymentStatus        | Current employment status               | VARCHAR(50)    |
| JobInvolvement          | Level of job involvement                | INT            |
| PerformanceRating       | Performance rating of the employee      | INT            |

2. Navigate to MySQL to create a database. Simply click and name it as “hr_data”. PIC]
3. To create tables, open the hr_data database, then right-click on tables and select “Table Data Import Wizard”. PIC]
4. Select the file you would like to import.PIC]
5. At the “Select Destination,” choose to create a new table for the data. I named my table “hrdata”. Then click next to proceed. PIC] 
6. Proceed to define columns by specifying names and corresponding data types, and next once it’s done. PIC]
7. Continue to click next until the data completes its importation. PIC]
8. I observed that the import of the hrdata table failed. PIC]
9. I encountered issues importing my dataset. To rectify this, I reformatted the document into a new .csv file using Excel and reimported the new file into my database.
10. Following these modifications, successful importation of the dataset was achieved. [PIC]

[Go to TOC](#table-of-contents)

## Data Cleaning

The objective of this data cleaning is to improve the data quality by ensuring the data is accurate, complete, valid, and consistent before the data analysis phase. 

### Data Observation

I used MySQL to complete the cleaning task. Fortunately for me the data was relatively clean and only required minimal cleaning.
You can find the clean “hrdata.csv” file [here](https://github.com/egaruba/Human-Resources-Analytics-Dashboard/blob/main/dataset/clean/hrdata.csv).

1. Check the first 5 rows to make sure it imported well.
```SELECT * FROM orders LIMIT 5;```
Let's see if the database is working correctly. [PIC]

2. Checking for missing values. 
```SELECT * FROM orders WHERE rowid IS NULL OR orderid IS NULL OR orderdate IS NULL OR shipdate IS NULL;```
It revealed blank this shows that we have no missing values. [PIC]

3. Checking for duplicate Row.
```SELECT * FROM orders WHERE (rowid orderid, orderdate, shipdate, shipmode, customerid, customername, sIN ( SELECT rowid, orderid, orderdate, shipdate, shipmode, customerid, customerna FROM orders GROUP BY rowid, orderid, orderdate, shipdate, shipmode, customerid, customer HAVING COUNT(*) > 1)ORDER BY rowid, orderid;```
The query returns an empty table, showing there are no duplicate rows. [PIC]

### Data Transformation

As stated previously, my data was clean and did not require further cleaning. All the raw data in the “hrdata.csv” file was relevant. It did not contain messy data, it did not contain data discrepancies and it did not require data transformation to resolve special characters not displaying correctly.

## Issues Found

During the initial data cleaning of the Human Resources dataset, one issue was identified and resolved:

- Column Removal: The “HR Data.xlsx” was opened in Excel. After opening the file, I noticed two new columns inside the worksheet. I removed the two columns because they did not provide any useful data. The columns were called “-2” and ”0”. All the data inside contained the same values of “-2” and ”0”.

You can find the clean “HR Data.xlsx” file [here](https://github.com/egaruba/Human-Resources-Analytics-Dashboard/blob/main/dataset/clean/HR%20Data.xlsx).

[Go to TOC](#table-of-contents)

## Exploratory Data Analysis

Exploratory Data Analysis is utilised when examining employee data in order to answer key questions, such as:

- What are the overall analytics trends?
- Which employees are most satisfied?
- What are the highest attrition rates?

### Questions To Be Explored

1. What is the aggregate count of employed personnel within the organization?
2. How many individuals have transitioned from employment within the organization?
3. What is the composite turnover rate or attrition quotient characterizing the organizational dynamics?
4. By what methodology can we discern the distinction between actively engaged and disengaged personnel?
5. What is the mean age, or alternatively, the median age, of the organization's workforce?
6. What discernible trends emerge in attrition delineated by gender within the organizational context?
7. Across the array of departments, what variance exists in attrition metrics?
8. How is the workforce stratified across distinct age cohorts?
9. What quantifiable metrics inform us of employee engagement and overarching job satisfaction levels?
10. How do attrition rates stratify across disparate educational backgrounds within the employee pool?
11. What nuanced patterns emerge in attrition rates predicated upon both gender and discrete age cohorts?

[Go to TOC](#table-of-contents)

## Functional Validation

| Test ID                 | Test Description                        | Query          | Test Result    | Remarks         |
| :---------------------- | :-------------------------------------- | :------------- | :------------- | :-------------
| 1                       | KPI Requirement - Employee Count        | ``` SELECT SUM(employee_count) AS Employee_Count FROM hrdata;  ``` | Pass           | Exact match    |
| 2                       | KPI Requirement - Attrition Count       | ```SELECT COUNT(attrition) AS Attrition_Count FROM hrdata WHERE attrition = “Yes";```    | Pass           | Exact match|
| 3                       | KPI Requirement - Attrition Rate        | ```SELECT ROUND(((SELECT COUNT(attrition) FROM hrdata WHERE attrition = "Yes")/SUM(employee_count)) * 100, 2) AS Attrition_Rate FROM hrdata;```   | Pass           | Exact match    |
| 4                       | KPI Requirement - Active Employee       | ```SELECT SUM(employee_count) - (SELECT COUNT(attrition) FROM hrdata WHERE attrition = “Yes") AS Active_Employees FROM hrdata;```    | Pass           | Exact match    |
| 5                       | KPI Requirement - Average Age           | ```SELECT ROUND(AVG(age), 0) AS Average_Age FROM hrdata;```       | Pass           | Exact match    |
| 6                       | Chart Requirement - Attrition by Gender | ```SELECT gender, COUNT(attrition) AS Attrition_Count FROM hrdata WHERE attrition = “Yes" GROUP BY gender ORDER BY COUNT(attrition) DESC;```   | Pass           | Exact match    |
| 7                       | Chart Requirement - Attrition by Department| ```SELECT department, COUNT(attrition) AS Attrition_Count, ROUND(((COUNT(attrition))/ (SELECT COUNT(attrition) FROM hrdata WHERE attrition = "Yes")) * 100, 2) AS Attrition_Rate FROM hrdata WHERE attrition = “Yes" GROUP BY department ORDER BY COUNT(attrition) DESC;```    | Pass           | Exact match    |
| 8                       | Chart Requirement - Number of Employees by Age Group| ```SELECT age, SUM(employee_count) AS Employee_Count FROM hrdata GROUP BY age ORDER BY age;```    | Pass           | Exact match    |
| 9                       | Chart Requirement - Attrition by Education| ```SELECT education_field, COUNT(attrition) AS Attrition_Count FROM hrdata WHERE attrition = “Yes" GROUP BY education_field ORDER BY COUNT(attrition) DESC;```   | Pass           | Exact match    |
| 10                      | Chart Requirement - Attrition Rate by Gender for Different Age Group| ```SELECT age_band, gender, COUNT(attrition) AS Attrition_Count, ROUND(((COUNT(attrition))/ (SELECT COUNT(attrition) FROM hrdata WHERE attrition = "Yes")) * 100, 2) AS Attrition_Rate_By_Gender FROM hrdata WHERE attrition = “Yes" GROUP BY age_band, gender ORDER BY age_band DESC;```    | Pass           | Exact match    |
| 11                      | Chart Requirement - Job Satisfaction    | ```SELECT job_role, job_satisfaction, SUM(employee_count) AS Satisfaction_Score FROM hrdata GROUP BY job_role, job_satisfaction ORDER BY job_role, job_satisfaction;```            | Pass           | Exact match    |
 
## Data Validation and Analysis

1. What is the total number of employees?
---

```SELECT SUM(employee_count) AS Employee_Count FROM hrdata;```

2. What is the total number of employees in the Sales Department?
```SELECT SUM(employee_count) AS Employee_Count FROM hrdata WHERE department = “Sales”;```

3. What is the total number of employees in the HR Department?
```SELECT SUM(employee_count) AS Employee_Count FROM hrdata WHERE department = “HR”;```

4. What is the total number of employees in the R&D Department?
```SELECT SUM(employee_count) AS Employee_Count FROM hrdata WHERE department = “R&D”;```

5. What is the total number of employees with a High School Diploma?
```SELECT SUM(employee_count) AS Employee_Count FROM hrdata WHERE education = "High School”;```

6. What is the total number of employees with a Bachelor’s Degree?
```SELECT SUM(employee_count) AS Employee_Count FROM hrdata WHERE education = “Bachelor’s Degree”;```

7. What is the total number of employees with a Doctoral Degree?
```SELECT SUM(employee_count) AS Employee_Count FROM hrdata WHERE education = “Doctoral Degree”;```

8. What is the total number of employees with an Associates Degree?
```SELECT SUM(employee_count) AS Employee_Count FROM hrdata WHERE education = “Associates Degree”;```

9. What is the total number of employees with a Master’s Degree?
```SELECT SUM(employee_count) AS Employee_Count FROM hrdata WHERE education = “Master’s Degree”;```

10. What is the number of employees who have left the organisation?
```SELECT COUNT(attrition) AS Attrition_Count FROM hrdata WHERE attrition = “Yes";```

11. What is the number of employees who have left the organisation in the Sales Department?
```SELECT COUNT(attrition) AS Attrition_Count FROM hrdata WHERE attrition = “Yes” && department = “Sales";```

12. What is the number of employees who have left the organisation in the HR Department?
```SELECT COUNT(attrition) AS Attrition_Count FROM hrdata WHERE attrition = “Yes" WHERE attrition = “Yes” && department = “HR";```

13. What is the number of employees who have left the organisation in the R&D Department?
```SELECT COUNT(attrition) AS Attrition_Count FROM hrdata WHERE attrition = "Yes" WHERE attrition = “Yes” && department = “R&D”;```

14. What is the number of employees who have not left the organisation?
```SELECT SUM(employee_count) - (SELECT COUNT(attrition) FROM hrdata WHERE attrition = “Yes") AS Active_Employees FROM hrdata;```

15. What is the overall turnover level or attrition rate of the organisation?
```SELECT ROUND(((SELECT COUNT(attrition) FROM hrdata WHERE attrition = "Yes")/SUM(employee_count)) * 100, 2) AS Attrition_Rate FROM hrdata;```

16. What is the difference between active and inactive employees?
```SELECT SUM(employee_count) - (SELECT COUNT(attrition) FROM hrdata WHERE attrition = “Yes") AS Active_Employees FROM hrdata; SELECT COUNT(attrition) AS Attrition_Count FROM hrdata WHERE attrition = "Yes" WHERE attrition = “Yes”;```

17. What is the average age of employees?
```SELECT ROUND(AVG(age), 0) AS Average_Age FROM hrdata;```

18. What are the attrition patterns based on gender?
```SELECT gender, COUNT(attrition) AS Attrition_Count FROM hrdata WHERE attrition = “Yes" GROUP BY gender ORDER BY COUNT(attrition) DESC;```

19. What are the attrition rates across the different departments?
```SELECT department, COUNT(attrition) AS Attrition_Count, ROUND(((COUNT(attrition))/ (SELECT COUNT(attrition) FROM hrdata WHERE attrition = "Yes")) * 100, 2) AS Attrition_Rate FROM hrdata WHERE attrition = “Yes" GROUP BY department ORDER BY COUNT(attrition) DESC;```

20. What are the distribution of employees across various age groups?
```SELECT age, SUM(employee_count) AS Employee_Count FROM hrdata GROUP BY age ORDER BY age;```

21. What are the employee engagement and overall job satisfaction ratings?
```SELECT job_role, job_satisfaction, SUM(employee_count) AS Satisfaction_Score FROM hrdata GROUP BY job_role, job_satisfaction ORDER BY job_role, job_satisfaction;```

22. What are the attrition rates based on educational background?
```SELECT education_field, COUNT(attrition) AS Attrition_Count FROM hrdata WHERE attrition = “Yes" GROUP BY education_field ORDER BY COUNT(attrition) DESC;```

23. What are the attrition rates based on gender and different age groups?
```SELECT age_band, gender, COUNT(attrition) AS Attrition_Count, ROUND(((COUNT(attrition))/ (SELECT COUNT(attrition) FROM hrdata WHERE attrition = "Yes")) * 100, 2) AS Attrition_Rate_By_Gender FROM hrdata WHERE attrition = “Yes" GROUP BY age_band, gender ORDER BY age_band DESC;```

[Go to TOC](#table-of-contents)

## Insights and Findings

The analysis results are summarized as follows:

1. The total number of employees hired by the company are 1,470. Knowing the exact employee count allows for better resource allocation and workforce planning.
2. The total number of males hired by the company is 882.
3. The total number of females hired by the company is 588.
4. The number of staff that have left the company is 237. Understanding attrition count helps in assessing the impact of turnover on the organization and identifying potential retention issues.
5. Fewer females have left the company. The number of females that have left the company is 87.
6. More males have left the company. The number of males that have left the company are 150.
7. The rate of attrition of the organisation stands at 16.12% for both sexes. A high attrition rate may indicate issues with employee satisfaction and engagement.
8. Females have a lower rate of attrition. The rate of attrition of the organisation for females stands at 14.80%.
9. Males have a higher rate of attrition. The rate of attrition of the organisation for males stands at 17.01%.
10. HR has the lowest attrition. The fact that the HR Department has a lower number of employees may be a direct correlation to this. The rate of attrition for the HR department is 5.06% with 12 staff leaving.
11. The R&D Department has the highest attrition rate. The fact that the R&D Department has a higher number of employees may be a direct correlation to this. The rate of attrition for the R&D department is 56.12% with 133 staff leaving.
12. The rate of attrition for the Sales department is 38.82% with 92 staff leaving.
13. The number of active employees at the company is 1,233. Understanding the proportion of active employees helps in assessing current workforce capacity.
14. The average age of a staff member at the organisation is 37. Deviations from industry norms in average employee age may signal potential issues in attracting and retaining younger talent.

[Go to TOC](#table-of-contents)

## Recommendations

Based on the analysis, I recommend the following actions:

1. Implement regular audits of employee data to ensure accuracy. By regularly updating this data, HR can accurately assess the current workforce size and plan for future growth or downsizing effectively.
2. Establish protocols for updating employee records promptly.
3. Implement a clear exit process for departing employees. Establishing a standardized method for tracking employee attrition will provide reliable data for analyzing turnover trends.
4. Regularly update the database to reflect changes in employee status. Accurately identifying active employees enables better workforce management and productivity assessment.
5. Conduct exit interviews to gather feedback from departing employees. Analyze attrition rates by department to identify areas needing improvement. Monitoring attrition rate over time allows for the assessment of turnover trends and comparison with industry benchmarks.
6. Implement performance reviews to assess employee productivity. Performance reviews enable organizations to recognize and reward employees and ensure legal compliance, contributing to overall organizational effectiveness and success.
7. Implement age-inclusive recruitment strategies. Understanding the average age of employees aids in evaluating workforce demographics and succession planning.
8. Offer professional development opportunities tailored to different age groups.

## Limitations

Based on the analysis, I discovered the following limitations:

1. Lack of detailed information on job satisfaction and engagement levels:
The available data doesn't provide a thorough understanding of how satisfied employees are with their jobs or how engaged they are in their work. Without this information, it's challenging to gauge their overall happiness and commitment to the organization.

2. Limited historical data for trend analysis:
There isn't enough past data available to analyze trends over time effectively. Historical data helps identify patterns and changes in employee behavior or performance, which can inform future strategies and decisions.

3. Absence of specific reasons for employee attrition:
The data doesn't specify why employees are leaving the company. Knowing the reasons behind attrition is crucial for addressing underlying issues and implementing retention strategies to reduce turnover.

4. Data may not capture employees on leave or temporary assignments effectively:
The data might not accurately reflect employees who are on leave or working in temporary roles. This could lead to incomplete insights into workforce capacity and productivity.

5. Limited diversity in educational backgrounds and job roles represented in the dataset:
The dataset lacks variety in terms of employees' educational backgrounds and the roles they hold within the organization. A more diverse dataset would provide a richer understanding of the workforce and could uncover insights that are currently overlooked.

[Go to TOC](#table-of-contents)

## Conclusion

> This study highlights the critical role of data analysis in optimizing workforce management strategies and fostering a supportive work environment. By leveraging insights from employee demographics and attrition rates, organizations can tailor their HR policies and practices to enhance employee engagement, retention, and overall organizational success.

The analysis of employee demographics, attrition rates, active employee numbers, and average age underscores the importance of data-driven decision-making in human resource management. In terms of employee demographics, the company currently employs 1,470 individuals, with a gender distribution of 882 males and 588 females. This understanding of gender representation is pivotal for fostering diversity and inclusion initiatives within the organization. Furthermore, the examination of attrition rates unveils that a total of 237 employees have left, resulting in a 16.12% attrition rate. Importantly, variations in attrition rates are observed between genders and departments, underscoring the necessity for targeted retention strategies tailored to specific groups. 

Regarding active employees, the current workforce capacity is reflected by 1,233 individuals, providing valuable insights into productivity levels and resource allocation. Additionally, with the average age of employees standing at 37, there exists a notable influence on recruitment practices and succession planning efforts. Future research could delve deeper into understanding the underlying reasons behind gender and departmental variations in attrition rates, enabling the development access to more effective employee retention strategies. Additionally, exploring the impact of age diversity on team dynamics and organizational performance could provide valuable insights for talent management practices going forward.

[Go to TOC](#table-of-contents)


 ## Special Characters
  After importing the data to power query editor in excel, I changed the file origin to UTF-8 encoding,this automatically removed the special characters and replaced 
  it with the appropriate letter.
  
   |Special character Before  | Special character After                           |                                 
  ---------------------------:|:-----------------------------------
  ![](Specialcharactersbefore.png)| ![](Specialcharacterafter.png)                                      
  
  
 
