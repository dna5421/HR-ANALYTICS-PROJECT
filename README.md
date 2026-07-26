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

   Column	            Type	         Description
   EmpID	             INT	          Unique employee identifier
   Name	              VARCHAR(50)	  Employee full name
   Gender	            VARCHAR(10)	  Male/Female
   Age	               INT	          Employee age
   Department         VARCHAR(50)	  IT, HR, Finance, Sales
   JobRole	           VARCHAR(50)	  Developer, Manager, Analyst, etc.
   Salary	            FLOAT	        Annual compensation
   Experience	        INT	          Years of work experience
   Attrition	         VARCHAR(10)	  Yes/No
   HireDate	          DATE	         Date of employment
   PerformanceRating	 INT	          1-5 scale rating
   Sample Data: 10 employee records with various attributes and NULL value handling

  ## ⚒️ Tools and Technologies

   Category	         Tools
   Database	         Microsoft SQL Server 2019+
   Database Admin	   SQL Server Management Studio (SSMS)
   Query Language	   T-SQL (Transact-SQL)
   Visualization	    Power BI Desktop
   Version Control	  Git/GitHub
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

   Metric	                 Value	                   Insight
   Total Employees	        10	                      Small workforce sample
   Avg Experience	         4.40 years	              Moderate experience level
   Avg Salary	             ₹59,500	                 Competitive compensation
   Avg Performance	        3.60/5	                  Room for performance improvement
   Attrition Rate	         30% (3 out of 10)	       Moderate turnover risk
   Department Distribution	IT, HR, Finance, Sales	  Balanced across departments

   ## 💨 Dashboard Overview
   
   ## 📊 Key Dashboard Components

   <img width="1003" height="403" alt="HR ANALYTICS DASHBOARD" src="https://github.com/user-attachments/assets/e8327ffc-3f85-474c-96e3-0f6e28632772"/>

  1. KPI Cards (Top Row)

     • Avg Experience: 4.40 years
     • Avg Salary: ₹59.50K
     • Total Employees: 10
     • Avg Performance: 3.60/5

  2. Sum of Salary by Department (Bar Chart)

     • Displays departmental compensation costs
     • Identifies high-budget departments

  3. Attrition Rate by Job Role (Donut Chart)

     • JobRole, Executive, Analyst, Developer
     • Shows turnover risk by position

  4. Attrition Rate by Department and Year (Bar Chart)

     • Finance, Sales, IT departments tracked by year
     • Identifies temporal trends

  5. Active Employees by Name (Pie Chart)

     • Individual employee contribution
     • Workforce composition visualization

  6. Sum of Experience by Salary (Line Chart)

     • Relationship between experience and compensation
     • Trend analysis

  7. Attrition Rate by Gender (Stacked Bar)

     • Male vs Female attrition comparison
     • Diversity insights

   ## 🧑‍💼 Model / Output

   Output Files Generated:

   HR-ANALYTICS-PROJECT/
   ├── HR ANALYTICS.sql (Database & Query Script)
   ├── HR ANALYTICS DASHBOARD.pbix (Power BI Dashboard)
   ├── README.md (Documentation)
   └── Sample Data (10 employee records)

   ✅ Analytical Outputs:

   • Employee count reports
   • Attrition statistics
   • Departmental salary analysis
   • Experience vs. compensation reports
   • Performance distribution metrics

   ## 🚀 How To Run This Project
         
   📌 Step 1: Prerequisites
       ✅ SQL Server 2019 or higher
       ✅ SQL Server Management Studio (SSMS)
       ✅ Power BI Desktop
       ✅ Git (optional)

   📌 Step 2: Clone Repository

   git clone https://github.com/dna5421/HR-ANALYTICS-PROJECT.git
   cd HR-ANALYTICS-PROJECT

   📌 Step 3: Execute SQL Script
   
   • Open SQL Server Management Studio (SSMS)
   • Connect to your SQL Server instance
   • Open the file: HR ANALYTICS.sql
   • Execute the script using F5 or Ctrl+E
   • This creates HR_Analytics database
   • Creates Employees table
   • Inserts 10 sample records
   • Handles NULL values
   • Runs analytical queries

   📌 Step 4: Connect to Power BI
   
   • Open Power BI Desktop
   • Click Home → Get Data → SQL Server
   • Enter connection details:
   • Server: (local) or your server name
   • Database: HR_Analytics
   • Click Load
   • Open or create HR ANALYTICS DASHBOARD.pbix
   • Create visualizations and dashboards

   📌 Step 5: Generate Reports
   • Create custom reports for management
   • Export dashboard as PDF/image
   • Schedule data refresh

   ## 🎯 Results
   
   ✅ Successful Project Outcomes:

   ✓ Database successfully created and populated
   ✓ 10 employee records stored with proper schema
   ✓ NULL values handled with default values
   ✓ Key analytical queries executed successfully
   ✓ Interactive Power BI dashboard created
   ✓ Real-time workforce insights available
   ✓ Attrition tracking implemented
   ✓ Department-wise performance visible

   ## ✨ CONCLUSION
   
   The HR Analytics Project successfully demonstrates:

   📊 A complete HR data analytics pipeline from SQL to Power BI
   💡 Actionable insights for workforce management
   📈 Identification of attrition risks and departmental trends
   🎯 Data-driven decision-making capability
   🔄 Scalable framework for larger HR datasets

   ✅ Business Impact:

   • Enables proactive attrition management
   • Supports strategic workforce planning
   • Improves HR efficiency through automation
   • Provides transparency in compensation analysis

   ## 🏢 Future Work

  🚀 Potential Enhancements:

   1. Predictive Analytics

   • Machine Learning models to predict attrition
   • Employee churn prediction
   • Retention probability scoring

   2. Advanced Visualizations

   • Heat maps for departmental trends
   • Cohort analysis
   • Burndown charts for attrition

   3. Data Expansion

   • Include training and development data
   • Add performance review history
   • Integrate payroll details
   • Employee engagement surveys   

   4. Automation

   • Automated data refresh schedules
   • Email alerts for high attrition
   • Monthly/quarterly report generation

   5. Additional Metrics

   • Cost-per-hire analysis
   • Time-to-productivity metrics
   • Succession planning insights
   • Diversity & Inclusion analytics
   
   6. Integration

   • Connect with HRIS systems
   • API endpoints for real-time data
   • Mobile dashboard access
   • Cloud deployment

   ## 📡 Author & Contact

   👤 Author: DNA5421
   📧 GitHub Profile: @dna5421
   🔗 Repository: HR-ANALYTICS-PROJECT
