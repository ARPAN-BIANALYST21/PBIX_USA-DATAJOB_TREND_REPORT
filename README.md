# 📊 USA Data Job Trend Report – Power BI Project

Comprehensive Analysis of U.S. Data Job Market (742 Records | 31 Fields)


📝 Project Overview

This Power BI project analyzes data-related job trends across the United States, using a clean single-table dataset of 742 job postings with 31 attributes. The goal is to understand hiring demand, salary benchmarks, industry trends, ownership patterns, and skill requirements within the modern data profession landscape.


The dashboard is structured into five interactive report pages, each designed to highlight specific market insights :


1.Project Brief

2.Market Overview

3.Salary & Professional Insights

4.Hiring Trends & Ownership Insights

5.Complete Insights

These pages visualize trends such as top hiring states, highest salaries, job counts by seniority, skill expectations by role, job ownership distribution, and more, as reflected in charts and tables found throughout pages 2–5 of the PDF. (e.g., Top 5 Hiring States, Salary Distributions, Skill Matrix) 


🎯 Objectives :

The primary objective of this report is to analyze the U.S. Data Job Market to answer:

1. Which States, Companies, and Industries hire the most?

2. What are the Top-Paying Locations and Job Roles?

3. How do Seniority Levels impact salary and job availability?

4. What Skills are most in demand across different roles?

5. How do Public, Private, Nonprofit, and Educational Institutions differ in their hiring patterns?

6. What strategic recommendations can be formed for Job Seekers and Decision-Makers?


🛠️ Tools & Technologies Used :

A. MySQL Workbench:	Data extraction & ad-hoc SQL analysis

B. Microsoft Excel:	Exploratory Data Analysis (EDA) using Pivot Tables

C. Microsoft Power BI:	Data modeling, DAX calculations, and dashboard creation

D. Power Query:	Data cleaning & transformation


📁 Dataset Summary :

Type: Single Table

Rows: 742

Columns / Features: 31



📌 Key Features of the Dashboard :


✔ Market Overview 


1. Top hiring states: California, New York, Massachusetts, Illinois  

2. Top industries: Biotech & Pharmaceuticals, Insurance, IT Services

3. Job distribution across ownership types (e.g., Private = 410, Public = 193)


✔ Salary & Professional Insights  


1. Highest salary locations: Chicago IL, San CA, Washington DC

2. Seniority analysis showing Intermediate roles dominate job openings (519)

3. Average salary differences by education level

4. Employee satisfaction by role


✔ Hiring Trends & Ownership Insights 

1. Ownership-Wise job role demand (e.g., Private sector demands 24% Data Scientists)

2. Skills Distribution across job roles (full matrix shown in report)

3. Education vs. Salary insights
   


✔ Complete Insights  


1. Target high-demand states

2. Focus on Biotech, Insurance & IT Services

3. Data Science & Machine Learning roles show highest long-term potential

4. Postgraduate degree significantly boosts earning potential


📐 Data Modeling :

1. Single table schema, optimized with Power Query transformations

2. 13 DAX Measures created for cleaner KPI computation and reusable metrics




📊 DAX Measures Table :

Measure Name	                               DAX Code

1. Data_Scientists = COUNTROWS(FILTER(Data_Tab, Data_Tab[Job_Title] = "Data Scientist"))

2. Government_Jobs = COUNTROWS(FILTER(Data_Tab, Data_Tab[Type_of_Ownership] = "Government"))

3. Intermediate_Jobs = COUNTROWS(FILTER(Data_Tab, Data_Tab[Seniority] = "Intermediate"))

4. Junior_Jobs = COUNTROWS(FILTER(Data_Tab, Data_Tab[Seniority] = "Junior"))

5. Max_Salary = MAX(Data_Tab[Upper_Salary])

6. Min_Salary = MIN(Data_Tab[Lower_Salary])

7. Private_Jobs = COUNTROWS(FILTER(Data_Tab, Data_Tab[Type_of_Ownership] = "Private"))

8. Public_Jobs = COUNTROWS(FILTER(Data_Tab, Data_Tab[Type_of_Ownership] = "Public"))

9. Salary_Avg = AVERAGE(Data_Tab[Avg_Salary])

10. Senior_Jobs = COUNTROWS(FILTER(Data_Tab, Data_Tab[Seniority] = "Senior"))

11. Total_Companies = DISTINCTCOUNT(Data_Tab[Company_Name])

12. Total_Industries = DISTINCTCOUNT(Data_Tab[Industry])

13. Total_Jobs = COUNT(Data_Tab[Job_Title])
    



🧩 Key Insights :

✔ California & New York dominate hiring

✔ Biotech & Pharmaceutical Industries lead job demand (33.7%)

✔ Private Companies contribute 55% of total postings

✔ Data Scientists are the most-in-demand role (313 postings)

✔ Highest Salaries appear in Washington, California, Illinois

✔ Postgraduates earn ~22% more than Graduates

✔ Senior Roles bag the highest salaries but have fewer openings




🚀 Recommendations :

1. Target states like CA, NY, IL for high job density

2. Focus on Industries like Biotech, Insurance, IT Services

3. Enhance skills in Python, SQL, ML frameworks, as reflected in skill matrix

4. Consider Postgraduate Education for better salary prospects

5. Explore Nonprofit and Public Roles if seeking stability



🙌 Acknowledgements :

This project was developed using the dataset provided by Datamites Internship Team and Market Relevant BI tools to provide insights for job seekers, recruiters, and policy makers.


👉 Here is the complete PDF link of the report : https://github.com/ARPAN-BIANALYST21/PBIX_USA_DATAJOB_TREND_REPORT/blob/5bf8e994d99f48b39e65082c9b195ffc54581ea0/USA-DATAJOB_TREND_REPORT.pdf


