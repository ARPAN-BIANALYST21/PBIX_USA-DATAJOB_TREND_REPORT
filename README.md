# 📊 USA DATA JOB TREND REPORT
Power BI Analysis of the U.S. Data Job Market


📌 PROJECT OVERVIEW
| Item              | Description                             |
| ----------------- | --------------------------------------- |
| Project Type      | Business Intelligence & Market Analysis |
| Domain            | Data & Analytics Job Market             |
| Geography         | United States                           |
| Dataset Structure | Single Table                            |
| Total Records     | 742                                     |
| Total Fields      | 31                                      |


This Power BI Project analyzes Data-Related Job Trends across the United States, focusing on Hiring Demand, Salary Distribution, Seniority Levels, Skill Requirements, and Ownership Patterns.

The Report emphasizes Clarity, Consistency, and Insight-Driven Storytelling using Simple but Effective Visuals.


📄 REPORT STRUCTURE
| Page No. | Report Page                        |
| -------- | ---------------------------------- |
| 1        | Market Overview                    |
| 2        | Salary & Professional Insights     |
| 3        | Hiring Trends & Ownership Insights |


🗂 DATASET INFORMATION
| Attribute        | Value                |
| ---------------- | -------------------- |
| Dataset Type     | Single Table         |
| Records          | 742                  |
| Columns          | 31                   |
| Data Scope       | U.S. Data Job Market |
| Data Granularity | Job-Level            |


Included Fields:
Job Title, Salary Ranges, Company Name, Industry, Location, Seniority, Ownership Type, Education Level, Skills, and Ratings.


🛠 TOOLS & TECHNOLOGIES
| Tool               | Usage                                         |
| ------------------ | --------------------------------------------- |
| MySQL Workbench    | Data Extraction & Ad-Hoc SQL Analysis         |
| Microsoft Excel    | Exploratory Data Analysis (Pivot Tables)      |
| Microsoft Power BI | Data Modeling, DAX Measures, Dashboard Design |
| Power Query        | Data Cleaning & Transformation                |


📊 MARKET OVERVIEW
| Key Metric          | Insight                                             |
| ------------------- | --------------------------------------------------- |
| Top Hiring States   | California, New York, Massachusetts, Illinois       |
| Leading Industries  | Biotech & Pharmaceuticals, Insurance, CS&H          |
| Ownership Dominance | Private Sector (~55% of Total Jobs)                 |
| Market Pattern      | Hiring Concentrated in Select States and Industries |


💰 SALARY & PROFESSIONAL INSIGHTS
| Aspect               | Observation                               |
| -------------------- | ----------------------------------------- |
| Highest Paying Roles | Director, Machine Learning Engineer       |
| Top Paying Locations | Chicago (IL), California, Washington (DC) |
| Education Impact     | Postgraduates Earn Significantly More     |
| Most In-Demand Role  | Data Scientist                            |
| Satisfaction Trend   | Higher at Senior Levels                   |


🏢 HIRING TRENDS & OWNERSHIP INSIGHTS
| Ownership Type         | Trend                                     |
| ---------------------- | ----------------------------------------- |
| Private Sector         | Highest Hiring Volume                     |
| Public Sector          | Moderate Opportunities                    |
| Government             | Limited Openings                          |
| Education Institutions | Lowest Hiring Volume                      |
| Skill Demand           | Data Scientists & Data Engineers Needed   |


📐 DATA MODEL & DESIGN APPROACH
| Design Aspect   | Implementation                  |
| --------------- | ------------------------------- |
| Data Model      | Single Table                    |
| Transformations | Power Query                     |
| Visual Strategy | KPI-Driven, No Slicers          |
| Layout          | Consistent Sizing and Alignment |
| Focus           | Trend Clarity over Complexity   |


📊 DAX MEASURES
| Measure Name      | DAX Code                                                                  |
| ----------------- | ------------------------------------------------------------------------- |
| Data_Scientists   | `COUNTROWS(FILTER(Data_Tab, Data_Tab[Job_Title] = "Data Scientist"))`     |
| Government_Jobs   | `COUNTROWS(FILTER(Data_Tab, Data_Tab[Type_of_Ownership] = "Government"))` |
| Intermediate_Jobs | `COUNTROWS(FILTER(Data_Tab, Data_Tab[Seniority] = "Intermediate"))`       |
| Junior_Jobs       | `COUNTROWS(FILTER(Data_Tab, Data_Tab[Seniority] = "Junior"))`             |
| Senior_Jobs       | `COUNTROWS(FILTER(Data_Tab, Data_Tab[Seniority] = "Senior"))`             |
| Private_Jobs      | `COUNTROWS(FILTER(Data_Tab, Data_Tab[Type_of_Ownership] = "Private"))`    |
| Public_Jobs       | `COUNTROWS(FILTER(Data_Tab, Data_Tab[Type_of_Ownership] = "Public"))`     |
| Max_Salary        | `MAX(Data_Tab[Upper_Salary])`                                             |
| Min_Salary        | `MIN(Data_Tab[Lower_Salary])`                                             |
| Salary_Avg        | `AVERAGE(Data_Tab[Avg_Salary])`                                           |
| Total_Jobs        | `COUNT(Data_Tab[Job_Title])`                                              |
| Total_Companies   | `DISTINCTCOUNT(Data_Tab[Company_Name])`                                   |
| Total_Industries  | `DISTINCTCOUNT(Data_Tab[Industry])`                                       |


🧠 KEY TAKEAWAYS
| Area           | Conclusion                      |
| -------------- | ------------------------------- |
| Job Market     | Concentrated and Competitive    |
| Hiring Driver  | Private Organizations           |
| Salary Driver  | Education & Seniority           |
| Role Stability | Data Science & Data Engineering |
| Skill Focus    | Python, SQL, Analytics Tools    |


📄 FULL REPORT 
Download the complete Power BI report: https://github.com/arpan-bisolution21/PBIX_USA-DATAJOB_TREND_REPORT/blob/1e69f43fd6b62b0d49a8d8d2f4b1951da2acfce5/USA-DATAJOB_TREND_REPORT.pdf




