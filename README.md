# Human Resources Analytics Dashboard

![](human_resources_department.png)
---
## Table of Contents

Project Overview
Background
Problem Statement
Entity Relationship Diagram
Tools Used
Skills Applied
Data Preparation
Data Cleaning
Issues Found
Exploratory Data Analysis 
Functional Validation
Data Validation/ Analysis
Insights & Findings
Conclusion


## Project Overview

This employee data analysis project aims to provide insights into the lack of clear trackable performance metrics for the Human Resources Department. By analysing various aspects of the employee data, I hope to identify trends, make data-driven recommendations and gain a deeper understanding of the Human Resources Department’s key performance metrics.

Disclaimer: All datasets and reports do not represent any company, institution or country. This is just a dummy dataset to demonstrate my capabilities in Tableau and SQL.

### Project Objectives

Assess the performance of different employees within the Human Resources Department, identifying areas of high attrition and opportunities for job satisfaction. 

Explore staff patterns, segmentations, and preferences through SQL queries, aiming to improve job satisfaction.

Analyse employee data to identify trends in staff performance, education based variations and gender preferences to make informed data driven decisions.

Generate actionable insights from the analysis, empowering decision-makers to make informed and strategic choices that improve the department’s employee satisfaction.

## Background

The Human Resources Department is responsible for monitoring and managing various aspects of employee data to ensure the organisation maintains a healthy workforce. However, there is a lack of clear performance indicators to track and analyse key Human Resource metrics. Therefore, there is a need to design and implement a set of KPIs to address the following issues: employee count at the company, attrition count of employees at the company, attrition rate of employees at the company, active employees at the company and average age of employees at the company.
 
### Dataset Overview

The raw dataset contains one .xlsx file named “HR Data.xlsx” and one CSV file titled “hrdata.csv”. Both of these files were used for this project.

## Dataset Description

hrdata: The primary dataset used for this analysis is the "hrdata.csv" file, containing detailed information about each employee at the company.
The raw dataset contains 1,470 records of employee data. The file has 1,470 rows and 15 columns. Each record represents a unique employee at the company. The records include various attributes such as gender, employee id number, marital status, age band, age, department, education, job role, education field, business travel, employee count, attrition, attrition label, job satisfaction and active employee.

HR Data: The alternative dataset provided for this analysis is the “HR Data.xlsx" file. It contains additional and more detailed information about each employee at the company.
The raw dataset contains 1,470 records of employee data. The file has 1,470 rows and 41 columns. Each record represents the same employee data as provided by the "hrdata.csv" file. 
The additional information not previously provided includes attributes such as over 18, training times last year, -2, 0, daily rate, distance from home, environment satisfaction, hourly rate, job involvement, job level, monthly income, monthly rate, number of companies worked, percent salary hike, performance rating, relationship satisfaction, standard hours, stock option level, total working years, work life balance, years at the company, years in current role, years since last promotion and years with current manager.

## Problem Statement

The Human Resources Department is responsible for monitoring and managing various aspects of employee data to ensure the organisation maintains a healthy workforce. However, there is a lack of clear performance indicators to track and analyse key departmental metrics. 

### KPI Requirements

There is a need to analyse and implement a set of KPIs to address the following issues:

Employee Count at the Company: The Human Resources Department lacks visibility into the total number of employees, making it challenging to assess workforce size and plan for future growth or downsizing effectively.

Attrition Count of Employees at the Company: The organisation lacks a standardised method to track employee attrition, resulting in incomplete and unreliable data on the number of employees who have left the organisation. 

Attrition Rate of Employees at the Company: Without a clear measure of attrition rate, the organization cannot assess the overall turnover level or compare it with industry benchmarks, hindering the ability to gauge employee satisfaction and engagement.

Active Employees at the Company: The organisation lacks a mechanism to differentiate between active and inactive employees, leading to difficulties in accurately assessing the current workforces’s productivity and capacity.

Average Age of Employees at the Company: The Human Resources Department lacks visibility into the average age of employees, making it difficult to evaluate workforce demographics, succession planning, and the organisation’s ability to attract and retain younger talent.

### Chart Requirements

There is a need to design and visualise charts and graphs to address the following issues:

Attrition by Gender at the Company: The Human Resources faces challenges in understanding the attrition patterns based on gender, making it difficult to identify any gender-related disparities and implement targeted retention strategies.

Attrition by Department at the Company: The Human Resources Department lacks visualisations to showcase attrition rates across different departments. This hinders their ability to identify departments with higher attrition rates and address any underlying issues or concerns effectively. 

Number of Employees by Age Group at the Company: The Human Resources Department requires visual representations to analyse the distribution of employees across various age groups. This helps in assessing workforce demographics, identifying any age-related gaps or imbalances, and implementing targeting Human Resource policies or programs.

Job Satisfaction Ratings at the Company: The Human Resources Department lacks visualisations to represent job satisfaction ratings, hindering their ability to measure employee engagement and overall job satisfaction.

Attrition by Education at the Company: The Human Resources Department requires visual representations to analyse attrition rates based on education fields. This helps identify specific educational backgrounds that may be associated with higher attrition, enabling the organisation to tailor retention strategies accordingly.

Attrition Rate by Gender for Age Groups at the Company:  The Human Resources lacks visualisations that display attrition rates based on gender and different age groups. This makes it challenging to identify any age and gender-related attrition trends, preventing the organisation from implementing targeted retention strategies for specific employee segments.

## Tools Used

Excel - Data Cleaning
MySQL - Data Analysis
Tableau - Creating Visualisations and Reports

## Skills Applied

Data Validation using SQL
Database Creation
SQL Functions: SELECT, INSERT, GROUP BY, WHERE, ORDER BY, etc.
Functional Validation
Aggregations

### Data Cleaning Process

The data cleaning process involves the following steps:

Data Preparation: This explains how I sourced the Human Resources department dataset for analysis, the structure and the key attributes of our dataset.

Data Cleaning: This involves steps taken to clean and preprocess the dataset to ensure its quality and reliability. The techniques used for handling missing values, standardising formats, and cleaning inconsistent data. The dataset was thoroughly examined to understand the structure, columns and their meanings. The data did not have a data dictionary attached.

Exploratory Data Analysis with SQL: Running SQL queries allows for the unveiling of employee trends, variations via education, employee behaviours and departmental insights. Exploratory Data Analysis is significant in understanding the dataset’s characteristics. The utilisation of more complex SQL techniques allows for deeper analysis, where the advanced SQL functions, window functions, will be used to derive insights beyond standard queries.

Insights and Recommendations: Summarise the key insights derived from the analysis. Discuss actionable recommendations based on SQL driven insights for enhancing employee satisfaction, optimising staff performance and improving employee experiences.

Dashboard Visualisation and Report: A dashboard visualisation that explains each segments and displays Key Performance Indicators to the client.

## Data Preparation

Field Name	Description	Data Type
EmployeeID	Unique identifier for each employee	VARCHAR(50)
Gender	Gender of the employee	VARCHAR(50)
MaritalStatus	Marital status of the employee	VARCHAR(50)
AgeRange	Age range of the employee	VARCHAR(50)
Age	Age of the employee	INT
Department	Department where the employee works	VARCHAR(50)
Education	Highest education level attained	VARCHAR(50)
EducationField	Field of education specialization	VARCHAR(50)
JobRole	Role of the employee within the company	VARCHAR(50)
BusinessTravel	Frequency of business travel	VARCHAR(50)
DistanceFromHome	Distance from home to workplace	INT
OverTime	Whether employee works overtime	VARCHAR(50)
EmploymentStatus	Current employment status	VARCHAR(50)
JobInvolvement	Level of job involvement	INT
PerformanceRating	Performance rating of the employee	INT

In the data preparation phase, I performed the following tasks:

Created a database, setup tables, and imported data.[PIC]
Navigate to MySQL to create a database. Simply click and name it as “hr_data”. PIC]
To create tables, open the hr_data database, then right-click on tables and select “Table Data Import Wizard”. PIC]
Select the file you would like to import.PIC]
At the “Select Destination,” choose to create a new table for the data. I named my table “hrdata”. Then click next to proceed. PIC] 
Proceed to define columns by specifying names and corresponding data types, and next once it’s done. PIC]
Continue to click next until the data completes its importation. PIC]
I observed that the import of the hrdata table failed. PIC]
I encountered issues importing my dataset. To rectify this, I reformatted the document into a new .csv file using Excel and reimported the new file into my database.
Following these modifications, successful importation of the dataset was achieved. [PIC]

## Data Cleaning

The objective of this data cleaning is to improve the data quality by ensuring the data is accurate, complete, valid, and consistent before the data analysis phase. 

### Data Observation

Check the first 5 rows to make sure it imported well. SELECT *FROM ordersLIMIT 5; [PIC]
Checking for missing values. SELECT *FROM ordersWHERE rowid IS NULL OR orderid IS NULL OR orderdate IS NULL OR shipdate IS NULL. It revealed blank this shows that we have no missing values. [PIC]
Checking for duplicate Row. SELECT *FROM ordersWHERE (rowid orderid, orderdate, shipdate, shipmode, customerid, customername, sIN ( SELECT rowid, orderid, orderdate, shipdate, shipmode, customerid, customerna FROM orders GROUP BY rowid, orderid, orderdate, shipdate, shipmode, customerid, customer HAVING COUNT(*) > 1)ORDER BY rowid, orderid; The query returns an empty table, showing there are no duplicate rows. [PIC]

I used MySQL to complete the cleaning task. Fortunately for me the data was relatively clean and only required minimal cleaning.
You can find the clean “hrdata.csv” file here.

### Data Transformation

As stated previously, my data was clean and did not require further cleaning. All the raw data in the “hrdata.csv” file was relevant. It did not contain messy data, it did not contain data discrepancies and it did not require data transformation to resolve special characters not displaying correctly.

## Issues Found

During the initial data cleaning of the Human Resources dataset, one issue was identified and resolved:

Column Removal: The “HR Data.xlsx” was opened in Excel. After opening the file, I noticed two new columns inside the worksheet. I removed the two columns because they did not provide any useful data. The columns were called “-2” and ”0”. All the data inside contained the same values of “-2” and ”0”.

You can find the clean “HR Data.xlsx” file here.

## Exploratory Data Analysis

Exploratory Data Analysis is utilised when examining employee data in order to answer key questions, such as:

What is the overall analytics trend?
Which employees are most satisfied?
What are the peak attrition rates?

### Questions To Be Explored

What is the aggregate count of employed personnel within the organization?
How many individuals have transitioned from employment within the organization?
What is the composite turnover rate or attrition quotient characterizing the organizational dynamics?
By what methodology can we discern the distinction between actively engaged and disengaged personnel?
What is the mean age, or alternatively, the median age, of the organization's workforce?
What discernible trends emerge in attrition delineated by gender within the organizational context?
Across the array of departments, what variance exists in attrition metrics?
How is the workforce stratified across distinct age cohorts?
What quantifiable metrics inform us of employee engagement and overarching job satisfaction levels?
How do attrition rates stratify across disparate educational backgrounds within the employee pool?
What nuanced patterns emerge in attrition rates predicated upon both gender and discrete age cohorts?

## Functional Validation

Test each feature work as per the requirement. To verify all the filters and Action Filters on the report work as per the requirements.

TEST TABLE
Test No.	Sheet Name	Query	Test Result	QA Remark
1	KPI- Employee Count	select sum(employee_count) as Employee_Count from hrdata;	Pass	Exact match
2	KPI- Attrition Count	select count(attrition) from hrdata where attrition='Yes';	Pass	Exact match
3	KPI- Attrition Rate	select 
round (((select count(attrition) from hrdata where attrition='Yes')/ 
sum(employee_count)) * 100,2)
from hrdata;	Pass	Exact match
4	KPI- Active Employee	select sum(employee_count) - (select count(attrition) from hrdata  where attrition='Yes') from hrdata;	Pass	Exact match
5	KPI- Average Age	select round(avg(age),0) from hrdata;	Pass	Exact match
6	Attrition by Gender	select gender, count(attrition) as attrition_count from hrdata
where attrition='Yes'
group by gender
order by count(attrition) desc;	Pass	Exact match
7	Department wise Attrition	select department, count(attrition), round((cast (count(attrition) as numeric) / 
(select count(attrition) from hrdata where attrition= 'Yes')) * 100, 2) as pct from hrdata
where attrition='Yes'
group by department 
order by count(attrition) desc;	Pass	Exact match
8	No of Employee by Age Group	SELECT age,  sum(employee_count) AS employee_count FROM hrdata
GROUP BY age
order by age;	Pass	Exact match
9	Education Field wise Attrition	select education_field, count(attrition) as attrition_count from hrdata
where attrition='Yes'
group by education_field
order by count(attrition) desc;	Pass	Exact match
10	Attrition Rate by Gender for different Age group	select age_band, gender, count(attrition) as attrition, 
round((cast(count(attrition) as numeric) / (select count(attrition) from hrdata where attrition = 'Yes')) * 100,2) as pct
from hrdata
where attrition = 'Yes'
group by age_band, gender
order by age_band desc;	Pass	Exact match
11	Job Satisfaction Rating	SELECT * FROM 
crosstab('SELECT job_role, job_satisfaction, sum(employee_count)
   FROM hrdata
   GROUP BY job_role, job_satisfaction
   ORDER BY job_role, job_satisfaction'
	) AS ct(job_role varchar(50), one numeric, two numeric, three numeric, four numeric)
ORDER BY job_role;	Pass	Exact match 

## Data Validation/ Analysis

What is the total number of employees? SELECT SUM(employee_count) AS Employee_Count FROM hrdata;
What is the total number of employees in the Sales Department? SELECT SUM(employee_count) AS Employee_Count FROM hrdata WHERE department = “Sales”;
What is the total number of employees in the HR Department? SELECT SUM(employee_count) AS Employee_Count FROM hrdata WHERE department = “HR”;
What is the total number of employees in the R&D Department? SELECT SUM(employee_count) AS Employee_Count FROM hrdata WHERE department = “R&D”;
What is the total number of employees with a High School Diploma? SELECT SUM(employee_count) AS Employee_Count FROM hrdata WHERE education = "High School”;
What is the total number of employees with a Bachelor’s Degree? SELECT SUM(employee_count) AS Employee_Count FROM hrdata WHERE education = “Bachelor’s Degree”;
What is the total number of employees with a Doctoral Degree? SELECT SUM(employee_count) AS Employee_Count FROM hrdata WHERE education = “Doctoral Degree”;
What is the total number of employees with an Associates Degree? SELECT SUM(employee_count) AS Employee_Count FROM hrdata WHERE education = “Associates Degree”;
What is the total number of employees with a Master’s Degree? SELECT SUM(employee_count) AS Employee_Count FROM hrdata WHERE education = “Master’s Degree”;
What is the number of employees who have left the organisation? SELECT COUNT(attrition) AS Attrition_Count FROM hrdata WHERE attrition = “Yes";
What is the number of employees who have left the organisation in the Sales Department? SELECT COUNT(attrition) AS Attrition_Count FROM hrdata WHERE attrition = “Yes” && department = “Sales";
What is the number of employees who have left the organisation in the HR Department? SELECT COUNT(attrition) AS Attrition_Count FROM hrdata WHERE attrition = “Yes" WHERE attrition = “Yes” && department = “HR";
What is the number of employees who have left the organisation in the R&D Department? SELECT COUNT(attrition) AS Attrition_Count FROM hrdata WHERE attrition = "Yes" WHERE attrition = “Yes” && department = “R&D”;
What is the number of employees who have not left the organisation? SELECT SUM(employee_count) - (SELECT COUNT(attrition) FROM hrdata WHERE attrition = “Yes") AS Active_Employees FROM hrdata;
What is the overall turnover level or attrition rate of the organisation? SELECT ROUND(((SELECT COUNT(attrition) FROM hrdata WHERE attrition = "Yes")/SUM(employee_count)) * 100, 2) AS Attrition_Rate FROM hrdata;
What is the difference between active and inactive employees? SELECT SUM(employee_count) - (SELECT COUNT(attrition) FROM hrdata WHERE attrition = “Yes") AS Active_Employees FROM hrdata; SELECT COUNT(attrition) AS Attrition_Count FROM hrdata WHERE attrition = "Yes" WHERE attrition = “Yes”;
What is the average age of employees? SELECT ROUND(AVG(age), 0) AS Average_Age FROM hrdata;
What are the attrition patterns based on gender? SELECT gender, COUNT(attrition) AS Attrition_Count FROM hrdata WHERE attrition = “Yes" GROUP BY gender ORDER BY COUNT(attrition) DESC;
What are the attrition rates across the different departments? SELECT department, COUNT(attrition) AS Attrition_Count, ROUND(((COUNT(attrition))/ 
(SELECT COUNT(attrition) FROM hrdata WHERE attrition = "Yes")) * 100, 2) AS Attrition_Rate FROM hrdata WHERE attrition = “Yes" GROUP BY department ORDER BY COUNT(attrition) DESC;
What are the distribution of employees across various age groups? SELECT age, SUM(employee_count) AS Employee_Count FROM hrdata GROUP BY age ORDER BY age;
What are the employee engagement and overall job satisfaction ratings? SELECT job_role, job_satisfaction, SUM(employee_count) AS Satisfaction_Score FROM hrdata GROUP BY job_role, job_satisfaction ORDER BY job_role, job_satisfaction;
What are the attrition rates based on educational background? SELECT education_field, COUNT(attrition) AS Attrition_Count FROM hrdata WHERE attrition = “Yes" GROUP BY education_field ORDER BY COUNT(attrition) DESC;
What are the attrition rates based on gender and different age groups? SELECT age_band, gender, COUNT(attrition) AS Attrition_Count, ROUND(((COUNT(attrition))/ (SELECT COUNT(attrition) FROM hrdata WHERE attrition = "Yes")) * 100, 2) AS Attrition_Rate_By_Gender FROM hrdata WHERE attrition = “Yes" GROUP BY age_band, gender ORDER BY age_band DESC;

## Insights & Findings

The analysis results are summarized as follows:

The total number of employees hired by the company are 1,470. Knowing the exact employee count allows for better resource allocation and workforce planning.
The total number of males hired by the company is 882.
The total number of females hired by the company is 588.
The number of staff that have left the company is 237. Understanding attrition count helps in assessing the impact of turnover on the organization and identifying potential retention issues.
Fewer females have left the company. The number of females that have left the company is 87.
More males have left the company. The number of males that have left the company are 150.
The rate of attrition of the organisation stands at 16.12% for both sexes. A high attrition rate may indicate issues with employee satisfaction and engagement.
Females have a lower rate of attrition. The rate of attrition of the organisation for females stands at 14.80%.
Males have a higher rate of attrition. The rate of attrition of the organisation for males stands at 17.01%.
HR has the lowest attrition. The fact that the HR Department has a lower number of employees may be a direct correlation to this. The rate of attrition for the HR department is 5.06% with 12 staff leaving.
The R&D Department has the highest attrition rate. The fact that the R&D Department has a higher number of employees may be a direct correlation to this. The rate of attrition for the R&D department is 56.12% with 133 staff leaving.
The rate of attrition for the Sales department is 38.82% with 92 staff leaving.
The number of active employees at the company is 1,233. Understanding the proportion of active employees helps in assessing current workforce capacity.
The average age of a staff member at the organisation is 37. Deviations from industry norms in average employee age may signal potential issues in attracting and retaining younger talent.

## Recommendations

Based on the analysis, I recommend the following actions:

Implement regular audits of employee data to ensure accuracy. By regularly updating this data, HR can accurately assess the current workforce size and plan for future growth or downsizing effectively.
Establish protocols for updating employee records promptly.
Implement a clear exit process for departing employees. Establishing a standardized method for tracking employee attrition will provide reliable data for analyzing turnover trends.
Regularly update the database to reflect changes in employee status. Accurately identifying active employees enables better workforce management and productivity assessment.
Conduct exit interviews to gather feedback from departing employees. Analyze attrition rates by department to identify areas needing improvement. Monitoring attrition rate over time allows for the assessment of turnover trends and comparison with industry benchmarks.
Implement performance reviews to assess employee productivity. Performance reviews enable organizations to recognize and reward employees and ensure legal compliance, contributing to overall organizational effectiveness and success.
Implement age-inclusive recruitment strategies. Understanding the average age of employees aids in evaluating workforce demographics and succession planning.
Offer professional development opportunities tailored to different age groups.

## Limitations

Lack of detailed information on job satisfaction and engagement levels.
Limited historical data for trend analysis.
Absence of specific reasons for employee attrition.
Data may not capture employees on leave or temporary assignments effectively.
Limited diversity in educational backgrounds and job roles represented in the dataset.

## Conclusion

This study highlights the critical role of data analysis in optimizing workforce management strategies and fostering a supportive work environment. By leveraging insights from employee demographics and attrition rates, organizations can tailor their HR policies and practices to enhance employee engagement, retention, and overall organizational success.

My data analysis results are summarized as follows:

The analysis of employee demographics, attrition rates, active employee numbers, and average age underscores the importance of data-driven decision-making in human resource management. In terms of employee demographics, the company currently employs 1,470 individuals, with a gender distribution of 882 males and 588 females. This understanding of gender representation is pivotal for fostering diversity and inclusion initiatives within the organization. Furthermore, the examination of attrition rates unveils that a total of 237 employees have left, resulting in a 16.12% attrition rate. Importantly, variations in attrition rates are observed between genders and departments, underscoring the necessity for targeted retention strategies tailored to specific groups. 

Regarding active employees, the current workforce capacity is reflected by 1,233 individuals, providing valuable insights into productivity levels and resource allocation. Additionally, with the average age of employees standing at 37, there exists a notable influence on recruitment practices and succession planning efforts. Future research could delve deeper into understanding the underlying reasons behind gender and departmental variations in attrition rates, enabling the development access to more effective employee retention strategies. Additionally, exploring the impact of age diversity on team dynamics and organizational performance could provide valuable insights for talent management practices going forward.


 ## Special Characters
  After importing the data to power query editor in excel, I changed the file origin to UTF-8 encoding,this automatically removed the special characters and replaced 
  it with the appropriate letter.
  
   |Special character Before  | Special character After                           |                                 
  ---------------------------:|:-----------------------------------
  ![](Specialcharactersbefore.png)| ![](Specialcharacterafter.png)                                      
  
  
  ## Name,Long_name and ID
  The dataset does not consist of duplicate data, so the next line of action was to check the data types of each column. Beginning with the ID,Name, and Long_name 
  columns respectively, these columns had the right data type and didn't contain inconsistent data so it was left in its original state.
 
