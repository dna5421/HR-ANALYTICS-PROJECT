<body>
<div class="container">

  <h1>🎯 HR ANALYTICS</h1>

  <div class="card">
    <p>The <strong>HR Analytics Project</strong> is a data-driven solution that combines SQL database management with Power BI dashboarding to analyze workforce data. It provides actionable insights into employee attrition, departmental performance, compensation trends, and workforce demographics to support strategic HR decision-making.</p>
  </div>

  <h2>📝 Project Overview</h2>
  <ul>
    <li><strong>SQL Server</strong> for structured data management and analysis</li>
    <li><strong>Power BI</strong> for interactive visualization and real-time dashboarding</li>
    <li><strong>HR Data</strong> covering employee demographics, performance, compensation, and attrition</li>
  </ul>
  <p>The system enables HR departments to identify patterns, predict attrition risks, and optimize workforce planning strategies.</p>

  <h2>✨ Problem Statement</h2>
  <p><strong>Challenge:</strong> HR departments struggle to gain actionable insights from employee data scattered across multiple systems.</p>
  <p>✅ <strong>Goal:</strong> Create a unified analytics platform to:</p>
  <ul>
    <li>Track employee attrition and retention metrics</li>
    <li>Analyze departmental performance and compensation trends</li>
    <li>Identify high-risk turnover areas</li>
    <li>Support data-driven HR decision-making</li>
    <li>Provide real-time workforce visibility</li>
  </ul>

  <h2>📊 Dataset</h2>
  <p><strong>Employee Records Table (Employees)</strong></p>
  <table>
    <tr><th>Column</th><th>Type</th><th>Description</th></tr>
    <tr><td>EmpID</td><td>INT</td><td>Unique employee identifier</td></tr>
    <tr><td>Name</td><td>VARCHAR(50)</td><td>Employee full name</td></tr>
    <tr><td>Gender</td><td>VARCHAR(10)</td><td>Male/Female</td></tr>
    <tr><td>Age</td><td>INT</td><td>Employee age</td></tr>
    <tr><td>Department</td><td>VARCHAR(50)</td><td>IT, HR, Finance, Sales</td></tr>
    <tr><td>JobRole</td><td>VARCHAR(50)</td><td>Developer, Manager, Analyst, etc.</td></tr>
    <tr><td>Salary</td><td>FLOAT</td><td>Annual compensation</td></tr>
    <tr><td>Experience</td><td>INT</td><td>Years of work experience</td></tr>
    <tr><td>Attrition</td><td>VARCHAR(10)</td><td>Yes/No</td></tr>
    <tr><td>HireDate</td><td>DATE</td><td>Date of employment</td></tr>
    <tr><td>PerformanceRating</td><td>INT</td><td>1–5 scale rating</td></tr>
  </table>
  <p><em>Sample Data:</em> 10 employee records with various attributes and NULL value handling.</p>

  <h2>⚒️ Tools and Technologies</h2>
  <table>
    <tr><th>Category</th><th>Tools</th></tr>
    <tr><td>Database</td><td>Microsoft SQL Server 2019+</td></tr>
    <tr><td>Database Admin</td><td>SQL Server Management Studio (SSMS)</td></tr>
    <tr><td>Query Language</td><td>T-SQL (Transact-SQL)</td></tr>
    <tr><td>Visualization</td><td>Power BI Desktop</td></tr>
    <tr><td>Version Control</td><td>Git/GitHub</td></tr>
    <tr><td>Operating System</td><td>Windows</td></tr>
  </table>

  <h2>Ⓜ️ Methods</h2>
  <h3>✅ Data Processing Pipeline</h3>
  <ul>
    <li><strong>Data Creation</strong> — Create HR_Analytics database and Employees table</li>
    <li><strong>Data Insertion</strong> — Load 10 sample employee records</li>
    <li><strong>NULL Handling</strong> — Use <code>ISNULL()</code> function to handle missing values</li>
    <li><strong>Data Validation</strong> — Verify data integrity</li>
    <li><strong>Analytical Queries</strong> — Extract key metrics</li>
    <li><strong>Visualization</strong> — Create Power BI dashboard for visual representation</li>
  </ul>

  <h3>Key Analytical Queries</h3>
  <pre><code>-- Total Employee Count
SELECT COUNT(*) AS TotalEmployees FROM Employees;

-- Attrition Analysis
SELECT Attrition, COUNT(*) AS Count FROM Employees GROUP BY Attrition;

-- Department-wise Average Salary
SELECT Department, AVG(Salary) AS AvgSalary FROM Employees GROUP BY Department;

-- Experience vs Salary Correlation
SELECT Experience, AVG(Salary) AS AvgSalary FROM Employees GROUP BY Experience;</code></pre>

  <h2>📊 Key Insights</h2>
  <table>
    <tr><th>Metric</th><th>Value</th><th>Insight</th></tr>
    <tr><td>Total Employees</td><td>10</td><td>Small workforce sample</td></tr>
    <tr><td>Avg Experience</td><td>4.40 years</td><td>Moderate experience level</td></tr>
    <tr><td>Avg Salary</td><td>₹59,500</td><td>Competitive compensation</td></tr>
    <tr><td>Avg Performance</td><td>3.60/5</td><td>Room for performance improvement</td></tr>
    <tr><td>Attrition Rate</td><td>30% (3 out of 10)</td><td>Moderate turnover risk</td></tr>
    <tr><td>Department Distribution</td><td>IT, HR, Finance, Sales</td><td>Balanced across departments</td></tr>
  </table>

  <h2>💨 Dashboard Overview</h2>
  <img class="dashboard-img" width="1003" height="403" alt="HR Analytics Dashboard" src="https://github.com/user-attachments/assets/e8327ffc-3f85-474c-96e3-0f6e28632772" />

  <h3>📊 Key Dashboard Components</h3>

  <p><strong>1. KPI Cards (Top Row)</strong></p>
<ul>
  <li><strong>Avg Experience:</strong> 4.40 years</li>
  <li><strong>Avg Salary:</strong> ₹59.50K</li>
  <li><strong>Total Employees:</strong> 10</li>
  <li><strong>Avg Performance:</strong> 3.60/5</li>
</ul>

  <p><strong>2. Sum of Salary by Department (Bar Chart)</strong></p>
  <ul>
    <li>Displays departmental compensation costs</li>
    <li>Identifies high-budget departments</li>
  </ul>

  <p><strong>3. Attrition Rate by Job Role (Donut Chart)</strong></p>
  <ul>
    <li>JobRole, Executive, Analyst, Developer</li>
    <li>Shows turnover risk by position</li>
  </ul>

  <p><strong>4. Attrition Rate by Department and Year (Bar Chart)</strong></p>
  <ul>
    <li>Finance, Sales, IT departments tracked by year</li>
    <li>Identifies temporal trends</li>
  </ul>

  <p><strong>5. Active Employees by Name (Pie Chart)</strong></p>
  <ul>
    <li>Individual employee contribution</li>
    <li>Workforce composition visualization</li>
  </ul>

  <p><strong>6. Sum of Experience by Salary (Line Chart)</strong></p>
  <ul>
    <li>Relationship between experience and compensation</li>
    <li>Trend analysis</li>
  </ul>

  <p><strong>7. Attrition Rate by Gender (Stacked Bar)</strong></p>
  <ul>
    <li>Male vs Female attrition comparison</li>
    <li>Diversity insights</li>
  </ul>

  <h2>🧑‍💼 Model / Output</h2>
  <p><strong>Output Files Generated:</strong></p>
 <pre><code>HR-ANALYTICS-PROJECT/
├── HR ANALYTICS.sql <em>(Database &amp; Query Script)</em>
├── HR ANALYTICS DASHBOARD.pbix <em>(Power BI Dashboard)</em>
├── README.md <em>(Documentation)</em>
└── Sample Data <em>(10 employee records)</em>
</code></pre>

  <p>✅ <strong>Analytical Outputs:</strong></p>
  <ul>
    <li>Employee count reports</li>
    <li>Attrition statistics</li>
    <li>Departmental salary analysis</li>
    <li>Experience vs. compensation reports</li>
    <li>Performance distribution metrics</li>
  </ul>

  <h2>🚀 How to Run This Project</h2>

  <p><span class="step-num">Step 1:</span> Prerequisites</p>
  <ul>
    <li>✅ SQL Server 2019 or higher</li>
    <li>✅ SQL Server Management Studio (SSMS)</li>
    <li>✅ Power BI Desktop</li>
    <li>✅ Git (optional)</li>
  </ul>

  <p><span class="step-num">Step 2:</span> Clone Repository</p>
<pre><code>git clone <a href="https://github.com/dna5421/HR-ANALYTICS-PROJECT.git" target="_blank">https://github.com/dna5421/HR-ANALYTICS-PROJECT.git</a>
cd HR-ANALYTICS-PROJECT</code></pre>

  <p><span class="step-num">Step 3:</span> Execute SQL Script</p>
  <ul>
    <li>Open SQL Server Management Studio (SSMS)</li>
    <li>Connect to your SQL Server instance</li>
    <li>Open the file: <code>HR ANALYTICS.sql</code></li>
    <li>Execute the script using <code>F5</code> or <code>Ctrl+E</code></li>
    <li>This creates <code>HR_Analytics</code> database</li>
    <li>Creates <code>Employees</code> table</li>
    <li>Inserts 10 sample records</li>
    <li>Handles NULL values</li>
    <li>Runs analytical queries</li>
  </ul>

  <p><span class="step-num">Step 4:</span> Connect to Power BI</p>
  <ul>
    <li>Open Power BI Desktop</li>
    <li>Click <strong>Home → Get Data → SQL Server</strong></li>
    <li>Enter connection details:</li>
    <li>Server: <code>(local)</code> or your server name</li>
    <li>Database: <code>HR_Analytics</code></li>
    <li>Click Load</li>
    <li>Open or create <code>HR ANALYTICS DASHBOARD.pbix</code></li>
    <li>Create visualizations and dashboards</li>
  </ul>

  <p><span class="step-num">Step 5:</span> Generate Reports</p>
  <ul>
    <li>Create custom reports for management</li>
    <li>Export dashboard as PDF/image</li>
    <li>Schedule data refresh</li>
  </ul>

  <h2>🎯 Results</h2>
  <p>✅ <strong>Successful Project Outcomes:</strong></p>
  <div class="result-item">✓ Database successfully created and populated</div>
  <div class="result-item">✓ 10 employee records stored with proper schema</div>
  <div class="result-item">✓ NULL values handled with default values</div>
  <div class="result-item">✓ Key analytical queries executed successfully</div>
  <div class="result-item">✓ Interactive Power BI dashboard created</div>
  <div class="result-item">✓ Real-time workforce insights available</div>
  <div class="result-item">✓ Attrition tracking implemented</div>
  <div class="result-item">✓ Department-wise performance visible</div>

  <h2>✨ Conclusion</h2>
  <p>The HR Analytics Project successfully demonstrates:</p>
  <ul>
    <li>📊 A complete HR data analytics pipeline from SQL to Power BI</li>
    <li>💡 Actionable insights for workforce management</li>
    <li>📈 Identification of attrition risks and departmental trends</li>
    <li>🎯 Data-driven decision-making capability</li>
    <li>🔄 Scalable framework for larger HR datasets</li>
  </ul>

  <p>✅ <strong>Business Impact:</strong></p>
  <ul>
    <li>Enables proactive attrition management</li>
    <li>Supports strategic workforce planning</li>
    <li>Improves HR efficiency through automation</li>
    <li>Provides transparency in compensation analysis</li>
  </ul>

  <h2>🏢 Future Work</h2>
  <p>🚀 <strong>Potential Enhancements:</strong></p>

  <h3>1. Predictive Analytics</h3>
  <ul>
    <li>Machine Learning models to predict attrition</li>
    <li>Employee churn prediction</li>
    <li>Retention probability scoring</li>
  </ul>

  <h3>2. Advanced Visualizations</h3>
  <ul>
    <li>Heat maps for departmental trends</li>
    <li>Cohort analysis</li>
    <li>Burndown charts for attrition</li>
  </ul>

  <h3>3. Data Expansion</h3>
  <ul>
    <li>Include training and development data</li>
    <li>Add performance review history</li>
    <li>Integrate payroll details</li>
    <li>Employee engagement surveys</li>
  </ul>

  <h3>4. Automation</h3>
  <ul>
    <li>Automated data refresh schedules</li>
    <li>Email alerts for high attrition</li>
    <li>Monthly/quarterly report generation</li>
  </ul>

  <h3>5. Additional Metrics</h3>
  <ul>
    <li>Cost-per-hire analysis</li>
    <li>Time-to-productivity metrics</li>
    <li>Succession planning insights</li>
    <li>Diversity &amp; Inclusion analytics</li>
  </ul>

  <h3>6. Integration</h3>
  <ul>
    <li>Connect with HRIS systems</li>
    <li>API endpoints for real-time data</li>
    <li>Mobile dashboard access</li>
    <li>Cloud deployment</li>
  </ul>

  <h2>📡 Author &amp; Contact</h2>
  <ul>
    <li>👤 Author: <strong>dna5421</strong></li>
    <li>📧 GitHub Profile: <a href="https://github.com/dna5421">github.com/dna5421</a></li>
    <li>🔗 Repository: <a href="https://github.com/dna5421/HR-ANALYTICS-PROJECT">github.com/dna5421/HR-ANALYTICS-PROJECT</a></li>
  </ul>

  <hr>
  <div class="footer">
    <p>Built with SQL Server &amp; Power BI · HR Analytics Project</p>
  </div>

</div>
</body>
