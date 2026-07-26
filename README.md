## 🎯 HR ANALYTICS

The HR Analytics Project is a data-driven solution that combines SQL database management with Power BI dashboarding to analyze workforce data. It provides actionable insights into employee attrition, departmental performance, compensation trends, and workforce demographics to support strategic HR decision-making.

## 📝 Project Overview

 • SQL Server for structured data management and analysis
 • Power BI for interactive visualization and real-time dashboarding
 • HR Data covering employee demographics, performance, compensation, and attrition

 The system enables HR departments to identify patterns, predict attrition risks, and optimize workforce    planning strategies.

 ## ✨ Problem Statement

  • Challenge: HR departments struggle to gain actionable insights from employee data scattered across         multiple systems
  
 ✅ Goal: Create a unified analytics platform to:
   
  • Track employee attrition and retention metrics
  • Analyze departmental performance and compensation trends
  • Identify high-risk turnover areas
  • Support data-driven HR decision-making
  • Provide real-time workforce visibility

  ## 📊 Dataset

  Employee Records Table (Employees)

   Column	            Type	        Description
   EmpID	            INT	          Unique employee identifier
   Name	              VARCHAR(50)	  Employee full name
   Gender	            VARCHAR(10)	  Male/Female
   Age	              INT	          Employee age
   Department         VARCHAR(50)	  IT, HR, Finance, Sales
   JobRole	          VARCHAR(50)	  Developer, Manager, Analyst, etc.
   Salary	            FLOAT	        Annual compensation
   Experience	        INT	          Years of work experience
   Attrition	        VARCHAR(10)	  Yes/No
   HireDate	          DATE	        Date of employment
   PerformanceRating	INT	          1-5 scale rating
   Sample Data: 10 employee records with various attributes and NULL value handling

  ## ⚒️ Tools and Technologies

   Category	         Tools
   Database	         Microsoft SQL Server 2019+
   Database Admin	   SQL Server Management Studio (SSMS)
   Query Language	   T-SQL (Transact-SQL)
   Visualization	   Power BI Desktop
   Version Control	 Git/GitHub
   Operating System	 Windows

  ## Ⓜ️ METHODS
  
  ✅ Data Processing Pipeline:

   • Data Creation – Create HR_Analytics database and Employees table
   • Data Insertion – Load 10 sample employee records
   • NULL Handling – Use ISNULL() function to handle missing values
   • Data Validation – Verify data integrity
   • Analytical Queries – Extract key metrics
   • Visualization – Create Power BI dashboard for visual representation

   Key Analytical Queries:

   -- Total Employee Count
   SELECT COUNT(*) AS TotalEmployees FROM Employees;

   -- Attrition Analysis
   SELECT Attrition, COUNT(*) AS Count FROM Employees GROUP BY Attrition;

   -- Department-wise Average Salary
   SELECT Department, AVG(Salary) AS AvgSalary FROM Employees GROUP BY Department;

   -- Experience vs Salary Correlation
   SELECT Experience, AVG(Salary) AS AvgSalary FROM Employees GROUP BY Experience;

   ## 📊 Key Insights

   Based on the SQL queries and dashboard data:   

   Metric	                  Value	                  Insight
   Total Employees	        10	                    Small workforce sample
   Avg Experience	          4.40 years	            Moderate experience level
   Avg Salary	              ₹59,500	                Competitive compensation
   Avg Performance	        3.60/5	                Room for performance improvement
   Attrition Rate	          30% (3 out of 10)	      Moderate turnover risk
   Department Distribution	IT, HR, Finance, Sales	Balanced across departments

   ## 💨 Dashboard Overview
   
   ## 📊 Key Dashboard Components

   <img width="1003" height="403" alt="HR ANALYTICS DASHBOARD" src="https://github.com/user-attachments/assets/e8327ffc-3f85-474c-96e3-0f6e28632772"/>
