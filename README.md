# .

📊 USA Data Job Trend Report
Power BI Analysis of the U.S. Data Job Market
Project Overview

This Power BI project presents an analytical view of data-related job trends across the United States, focusing on hiring demand, salary distribution, job seniority, skill requirements, and ownership patterns.

The report is built on a single-table dataset and designed with clean, minimal visuals to communicate trends clearly and effectively. The dashboard supports data-driven decision-making for job seekers, analysts, recruiters, and career planners.

Report Structure

The final Power BI report contains three analytical pages:

Market Overview

Salary & Professional Insights

Hiring Trends & Ownership Insights

Dataset Information
Attribute	Value
Dataset Type	Single table
Total Records	742
Total Fields	31
Geographic Scope	United States
Domain	Data and analytics job market

The dataset includes job titles, salary ranges, locations, industries, seniority levels, ownership types, education levels, and technical skill indicators.

Tools and Technologies Used

MySQL Workbench – Data extraction and ad-hoc SQL analysis

Microsoft Excel – Exploratory data analysis using Pivot Tables

Microsoft Power BI – Data modeling, DAX measures, and dashboard design

Power Query – Data cleaning and transformation

Market Overview
Key Highlights

California and New York lead hiring, with the highest concentration of job postings

Biotech and Pharmaceuticals dominate hiring demand, followed by Insurance, IT Services, and Healthcare

Private sector accounts for approximately 55% of total job openings

Hiring demand is concentrated within a limited number of high-impact industries

Salary and Professional Insights
Key Highlights

Senior-level roles command the highest salaries, with Directors earning the top averages

Chicago (IL), California, and Washington (DC) offer the highest maximum salaries

Postgraduates earn significantly more than graduates, indicating a strong education–salary relationship

Data Scientists are the most in-demand role, followed by Data Engineers and Other Scientist roles

Employee satisfaction is highest at senior levels and lowest among entry-level analyst roles

Hiring Trends and Ownership Insights
Key Highlights

Private organizations lead hiring, followed by the Public sector

Government roles remain limited in comparison to other ownership types

Data Scientists and Data Engineers are consistently required across ownership categories

Machine Learning Engineer roles remain relatively limited, despite higher compensation

Education-based institutions show the lowest hiring volumes, indicating reduced competition

Data Model and Design Approach

Single-table model optimized for clarity and performance

Data transformations handled using Power Query

KPI-driven layout with no slicers, emphasizing storytelling over interaction

Consistent visual sizing and alignment for professional presentation

DAX Measures Used
Measure Name	DAX Code
Data_Scientists	COUNTROWS(FILTER(Data_Tab, Data_Tab[Job_Title] = "Data Scientist"))
Government_Jobs	COUNTROWS(FILTER(Data_Tab, Data_Tab[Type_of_Ownership] = "Government"))
Intermediate_Jobs	COUNTROWS(FILTER(Data_Tab, Data_Tab[Seniority] = "Intermediate"))
Junior_Jobs	COUNTROWS(FILTER(Data_Tab, Data_Tab[Seniority] = "Junior"))
Senior_Jobs	COUNTROWS(FILTER(Data_Tab, Data_Tab[Seniority] = "Senior"))
Private_Jobs	COUNTROWS(FILTER(Data_Tab, Data_Tab[Type_of_Ownership] = "Private"))
Public_Jobs	COUNTROWS(FILTER(Data_Tab, Data_Tab[Type_of_Ownership] = "Public"))
Max_Salary	MAX(Data_Tab[Upper_Salary])
Min_Salary	MIN(Data_Tab[Lower_Salary])
Salary_Avg	AVERAGE(Data_Tab[Avg_Salary])
Total_Jobs	COUNT(Data_Tab[Job_Title])
Total_Companies	DISTINCTCOUNT(Data_Tab[Company_Name])
Total_Industries	DISTINCTCOUNT(Data_Tab[Industry])


Key Takeaways

The U.S. data job market is highly concentrated in select states and industries

Private organizations drive most hiring activity

Education level and seniority strongly influence compensation

Data Science and Data Engineering roles offer the strongest demand stability

Technical skill demand centers on Python, SQL, and analytics tools



👉 View or download the Power BI report (PDF)


