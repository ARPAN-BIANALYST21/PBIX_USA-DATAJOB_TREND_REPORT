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


This Power BI project analyzes data-related job trends across the United States, focusing on hiring demand, salary distribution, seniority levels, skill requirements, and ownership patterns.
The report emphasizes clarity, consistency, and insight-driven storytelling using simple but effective visuals.


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
| Ownership Dominance | Private Sector (~55% of total jobs)                 |
| Market Pattern      | Hiring concentrated in select states and industries |


💰 SALARY & PROFESSIONAL INSIGHTS
| Aspect               | Observation                               |
| -------------------- | ----------------------------------------- |
| Highest Paying Roles | Director, Machine Learning Engineer       |
| Top Paying Locations | Chicago (IL), California, Washington (DC) |
| Education Impact     | Postgraduates earn significantly more     |
| Most In-Demand Role  | Data Scientist                            |
| Satisfaction Trend   | Higher at senior levels                   |


🏢 HIRING TRENDS & OWNERSHIP INSIGHTS
| Ownership Type         | Trend                                     |
| ---------------------- | ----------------------------------------- |
| Private Sector         | Highest hiring volume                     |
| Public Sector          | Moderate opportunities                    |
| Government             | Limited openings                          |
| Education Institutions | Lowest hiring volume                      |
| Skill Demand           | Data Scientists & Data Engineers dominate |


📐 DATA MODEL & DESIGN APPROACH
| Design Aspect   | Implementation                  |
| --------------- | ------------------------------- |
| Data Model      | Single Table                    |
| Transformations | Power Query                     |
| Visual Strategy | KPI-driven, No slicers          |
| Layout          | Consistent sizing and alignment |
| Focus           | Trend clarity over complexity   |


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
| Job Market     | Concentrated and competitive    |
| Hiring Driver  | Private organizations           |
| Salary Driver  | Education & seniority           |
| Role Stability | Data Science & Data Engineering |
| Skill Focus    | Python, SQL, Analytics Tools    |


📄 FULL REPORT 
Download the complete Power BI report: 




