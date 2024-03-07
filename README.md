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

Check the first 5 rows to make sure it imported well. SELECT *FROM ordersLIMIT 5; [PIC]
Checking for missing values. SELECT *FROM ordersWHERE rowid IS NULL OR orderid IS NULL OR orderdate IS NULL OR shipdate IS NULL. It revealed blank this shows that we have no missing values. [PIC]
Checking for duplicate Row. SELECT *FROM ordersWHERE (rowid orderid, orderdate, shipdate, shipmode, customerid, customername, sIN ( SELECT rowid, orderid, orderdate, shipdate, shipmode, customerid, customerna FROM orders GROUP BY rowid, orderid, orderdate, shipdate, shipmode, customerid, customer HAVING COUNT(*) > 1)ORDER BY rowid, orderid; The query returns an empty table, showing there are no duplicate rows. [PIC]

I used MySQL to complete the cleaning task. Fortunately for me the data was relatively clean and only required minimal cleaning.
You can find the clean “hrdata.csv” file here.

 ## Special Characters

  ## Special Characters

   ## Special Characters

    ## Special Characters

     ## Special Characters


 ## Special Characters

  ## Special Characters

   ## Special Characters

    ## Special Characters

     ## Special Characters
 ## Special Characters
  After importing the data to power query editor in excel, I changed the file origin to UTF-8 encoding,this automatically removed the special characters and replaced 
  it with the appropriate letter.
  
   |Special character Before  | Special character After                           |                                 
  ---------------------------:|:-----------------------------------
  ![](Specialcharactersbefore.png)| ![](Specialcharacterafter.png)                                      
  
  
  ## Name,Long_name and ID
  The dataset does not consist of duplicate data, so the next line of action was to check the data types of each column. Beginning with the ID,Name, and Long_name 
  columns respectively, these columns had the right data type and didn't contain inconsistent data so it was left in its original state.
 
