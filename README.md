    <p style="text-align: center; font-size: 1.1em; color: #555;">
        A comprehensive Human Resources analytics solution that combines SQL database management with Power BI dashboarding to analyze workforce data, track employee attrition, and provide actionable insights into departmental performance, compensation trends, and employee demographics.
    </p>
    
    <h2><span class="emoji">📝</span>Description</h2>
    <p>
        The HR ANALYTICS is a comprehensive Human Resources analytics solution designed to provide actionable insights into workforce data. This project combines SQL-based data processing with an interactive Power BI dashboard to help HR professionals and business leaders make data-driven decisions about:
    </p>
    <ul>
        <li>Employee attrition rates and retention metrics</li>
        <li>Departmental performance analysis</li>
        <li>Compensation and salary trends</li>
        <li>Employee demographics and diversity metrics</li>
        <li>Turnover analysis and predictive insights</li>
        <li>Performance ratings and productivity metrics</li>
    </ul>
    <p>
        The project enables HR departments to identify patterns, predict potential issues, and optimize workforce planning strategies.
    </p>
    
    <h2><span class="emoji">✨</span>Features</h2>
    <div class="feature-list">
        <div class="feature-item">
            <strong>SQL Database Integration</strong>
            <p>Structured data queries and analysis using SQL</p>
        </div>
        <div class="feature-item">
            <strong>Interactive Dashboard</strong>
            <p>Visual representation of key HR metrics using Power BI</p>
        </div>
        <div class="feature-item">
            <strong>Real-time Analytics</strong>
            <p>Up-to-date workforce insights and KPIs</p>
        </div>
        <div class="feature-item">
            <strong>Attrition Analysis</strong>
            <p>Track and predict employee turnover</p>
        </div>
        <div class="feature-item">
            <strong>Department Insights</strong>
            <p>Department-wise performance and staffing analysis</p>
        </div>
        <div class="feature-item">
            <strong>Compensation Analysis</strong>
            <p>Salary trends and compensation insights</p>
        </div>
        <div class="feature-item">
            <strong>Employee Demographics</strong>
            <p>Detailed employee categorization and statistics</p>
        </div>
    </div>
    
    <h2><span class="emoji">⚒️</span>Stack</h2>
    <ul>
        <li><strong>Languages:</strong> SQL (T-SQL for SQL Server), Power BI scripting</li>
        <li><strong>Platform:</strong> Microsoft SQL Server 2019+ & Power BI Desktop</li>
    </ul>
    
    <h2><span class="emoji">⚒️</span>Notable Tools</h2>
    <ul>
        <li><strong>SQL Server Management Studio (SSMS)</strong> — database administration and query execution</li>
        <li><strong>Power BI Desktop</strong> — data visualization and interactive dashboarding</li>
        <li><strong>SQL Server</strong> — relational database for structured HR data storage</li>
    </ul>
    
    <h2><span class="emoji">🚀</span>How to Run It</h2>
    
    <h3><span class="emoji">✅</span>Prerequisites</h3>
    <ul>
        <li>SQL Server 2019 or higher</li>
        <li>Power BI Desktop</li>
        <li>Git (optional, for cloning)</li>
    </ul>
    
    <h3>Step 1: Clone the Repository</h3>
    <div class="git-link">
        git clone https://github.com/dna5421/HR-ANALYTICS-PROJECT.git<br>cd HR-ANALYTICS-PROJECT
    </div>
    
    <h3>Step 2: Setup SQL Server Database</h3>
    <div class="step-box">
        <ol>
            <li>Open SQL Server Management Studio (SSMS)</li>
            <li>Connect to your SQL Server instance</li>
            <li>Open the <code>HR ANALYTICS.sql</code> file</li>
            <li>Execute the script (F5 or Ctrl+E)</li>
        </ol>
    </div>
    
    <h3>Step 3: Connect to Power BI</h3>
    <div class="step-box">
        <ol>
            <li>Open Power BI Desktop</li>
            <li>Go to <strong>Home</strong> → <strong>Get Data</strong> → <strong>SQL Server</strong></li>
            <li>Enter Server: <code>(local)</code> or your-server-name</li>
            <li>Enter Database: <code>HR_Analytics</code></li>
            <li>Click <strong>Load</strong></li>
            <li>Create/Open <code>HR ANALYTICS DASHBOARD.pbix</code> for interactive visualizations</li>
        </ol>
    </div>
    
    <h3>What the SQL Script Does</h3>
    <div class="highlight-box">
        <ul>
            <li>Creates HR_Analytics database</li>
            <li>Creates Employees table with schema</li>
            <li>Inserts sample data (10 employee records)</li>
            <li>Handles NULL values with defaults</li>
            <li>Runs sample analytical queries</li>
        </ul>
    </div>
    
    <h2><span class="emoji">🧑💼</span>Usage</h2>
    
    <div class="role-section">
        <h3><span class="emoji">✅</span>For HR Professionals</h3>
        <ul>
            <li>Track employee attrition and retention metrics</li>
            <li>Identify departmental trends and compensation patterns</li>
            <li>Generate custom reports for management presentations</li>
            <li>Use data-driven insights for workforce planning</li>
        </ul>
    </div>
    
    <div class="role-section">
        <h3><span class="emoji">🎯</span>For Business Leaders</h3>
        <ul>
            <li>Make strategic decisions based on HR data</li>
            <li>Perform cost analysis on compensation and departmental expenses</li>
            <li>Monitor department performance and productivity</li>
            <li>Identify high-risk attrition areas before they escalate</li>
        </ul>
    </div>
    
    <h2><span class="emoji">📊</span>Key Metrics to Monitor</h2>
    <div class="metrics-grid">
        <div class="metric-card">
            <strong>Attrition Rate</strong>
            <p>% of employees leaving</p>
        </div>
        <div class="metric-card">
            <strong>Average Tenure</strong>
            <p>How long employees stay</p>
        </div>
        <div class="metric-card">
            <strong>Department Distribution</strong>
            <p>Headcount by department</p>
        </div>
        <div class="metric-card">
            <strong>Salary Analysis</strong>
            <p>Average by role/department</p>
        </div>
        <div class="metric-card">
            <strong>Performance Ratings</strong>
            <p>Employee productivity distribution</p>
        </div>
        <div class="metric-card">
            <strong>Age Demographics</strong>
            <p>Retirement planning</p>
        </div>
    </div>
</div>
