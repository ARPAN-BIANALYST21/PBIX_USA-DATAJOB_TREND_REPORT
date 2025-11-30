# 📊 USA Data Job Trend Report – Power BI Project

Comprehensive Analysis of U.S. Data Job Market (742 Records | 31 Fields)


📝 Project Overview

This Power BI Project analyzes data-related job trends across the United States, using a clean Single-Table Dataset of 742 Job Postings with 31 Attributes. The goal is to understand Hiring Demand, Salary Benchmarks, Industry Trends, Ownership Patterns, and Skill Requirements within the modern data profession landscape.


The Dashboard is structured into Five Interactive Slides, each designed to highlight Specific Market Insights :


1.Project Brief

2.Market Overview

3.Salary & Professional Insights

4.Hiring Trends & Ownership Insights

5.Complete Insights

These Slides visualize Trends such as top Hiring States, Highest Salaries, Job Counts by Seniority, Skill Expectations by Roles, Ownership Distributions, and more, as reflected in Charts and Tables found throughout pages 2–5 of the PDF. (e.g., Top 5 Hiring States, Salary Distributions, Skill Matrix) 


🎯 Objectives :

The primary objective of this report is to analyze the U.S. Data Job Market to answer:

1. Which States, Companies, and Industries hire the most?

2. What are the Top-Paying Locations and Job Roles?

3. How do Seniority Levels impact Salary and Job Opportunities?

4. What Skills are most in demand across different Roles?

5. How do Public, Private, Nonprofit, and Educational Institutions differ in their Hiring Patterns?

6. What Strategic Recommendations can be formed for Job Seekers and Decision-Makers?


🛠️ Tools & Technologies Used :

A. MySQL Workbench:	Data Extraction & Ad-Hoc SQL Analysis

B. Microsoft Excel:	Exploratory Data Analysis (EDA) using Pivot Tables

C. Microsoft Power BI:	DAX Calculations, Dasboard Preparation & Reporting

D. Power Query:	Data Preprocessing & Quality Assurance


📁 Dataset Summary :

Type: Single Table

Rows: 742

Columns / Features: 31



📌 Key Features of the Dashboard :


✔ Market Overview 


1. Top Hiring States: California, New York, Massachusetts, Illinois  

2. Top Industries: Biotech & Pharmaceuticals, Insurance, IT Services

3. Job Distributions across Ownership Types (e.g., Private = 410, Public = 193)


✔ Salary & Professional Insights  


1. Highest Salary Locations: Chicago IL, San CA, Washington DC

2. Seniority Analysis showing Intermediate Roles dominate Job Openings (519)

3. Average Salary differences by Education Level

4. Employee Satisfaction by Job Roles.


✔ Hiring Trends & Ownership Insights 

1. Ownership-Wise Job Role Demand (e.g., Private Sector demands 24% Data Scientists)

2. Skills Distribution across Job Roles (Full Matrix shown in the Report)

3. Education vs. Salary Insights
   


✔ Complete Insights  


1. Target High-Demand States

2. Focus on Biotech, Insurance & IT Services

3. Data Science & Machine Learning Roles show Highest Long-Term Potential

4. Postgraduate Degree significantly boosts Earning Potential


📐 Data Modeling :

1. Single-Table Schema, optimized with Power Query Transformations

2. 13 DAX Measures created for cleaner KPI Computation and Reusable Metrics




📊 DAX Measures Table :

| Measure Name          | DAX Code                                                                  |
| --------------------- | ------------------------------------------------------------------------- |
| **Data_Scientists**   | `COUNTROWS(FILTER(Data_Tab, Data_Tab[Job_Title] = "Data Scientist"))`     |
| **Government_Jobs**   | `COUNTROWS(FILTER(Data_Tab, Data_Tab[Type_of_Ownership] = "Government"))` |
| **Intermediate_Jobs** | `COUNTROWS(FILTER(Data_Tab, Data_Tab[Seniority] = "Intermediate"))`       |
| **Junior_Jobs**       | `COUNTROWS(FILTER(Data_Tab, Data_Tab[Seniority] = "Junior"))`             |
| **Max_Salary**        | `MAX(Data_Tab[Upper_Salary])`                                             |
| **Min_Salary**        | `MIN(Data_Tab[Lower_Salary])`                                             |
| **Private_Jobs**      | `COUNTROWS(FILTER(Data_Tab, Data_Tab[Type_of_Ownership] = "Private"))`    |
| **Public_Jobs**       | `COUNTROWS(FILTER(Data_Tab, Data_Tab[Type_of_Ownership] = "Public"))`     |
| **Salary_Avg**        | `AVERAGE(Data_Tab[Avg_Salary])`                                           |
| **Senior_Jobs**       | `COUNTROWS(FILTER(Data_Tab, Data_Tab[Seniority] = "Senior"))`             |
| **Total_Companies**   | `DISTINCTCOUNT(Data_Tab[Company_Name])`                                   |
| **Total_Industries**  | `DISTINCTCOUNT(Data_Tab[Industry])`                                       |
| **Total_Jobs**        | `COUNT(Data_Tab[Job_Title])`                                              |

    
🧩 Key Insights :

✔ California & New York dominate Hirings

✔ Biotech & Pharmaceutical Industries lead Job Demand (33.7%)

✔ Private Companies contribute 55% of all the Postings

✔ Data Scientists are the Most In-Demand Role (313 postings)

✔ Highest Salaries appear in Washington, California, Illinois

✔ Postgraduates earn ~22% more than Graduates

✔ Senior Roles bag the Highest Salaries but have fewer Openings




🚀 Recommendations :

1. Target states like CA, NY, IL for High Job Density

2. Focus on Industries like Biotech, Insurance, IT Services

3. Enhance skills in Python, SQL, ML frameworks, as reflected in Skill Matrix

4. Consider Postgraduate Education for Better Salary Prospects

5. Explore Nonprofit and Public Roles if seeking Stability



🙌 Acknowledgements :

This project was developed using the dataset provided by Datamites Internship Team and Market Relevant BI Tools to provide insights for job seekers, recruiters, and policy makers.


👉 Here is the complete PDF link of the Report : https://github.com/ARPAN-BIANALYST21/PBIX_USA_DATAJOB_TREND_REPORT/blob/5bf8e994d99f48b39e65082c9b195ffc54581ea0/USA-DATAJOB_TREND_REPORT.pdf


