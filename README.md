<h1> USA Financial Data – Automated ETL & Dashboard</h1>

<h2> Project Overview</h2>
<p>
This project showcases a fully automated ETL pipeline and interactive dashboard built for analyzing U.S. financial survey data. The system replaces the previous manual workflow where approximately 25 daily files were emailed, downloaded, and manually processed. The new solution integrates Outlook, Power Automate, Google Drive API, Power Query, Python, and Power BI to automate data extraction, consolidation, and dashboard refresh.
</p>

<hr>

<h2> Problem Statement</h2>
<ul>
  <li>Manual downloading of ~25 files daily</li>
  <li>Strict processing deadlines (3 PM → 8 PM)</li>
  <li>Frequent manipulation errors</li>
  <li>Additional labor costs (~$12,000/month)</li>
  <li>Negative impact on other project workloads</li>
</ul>
<p>
The purpose of this automation was to reduce time, minimize errors, centralize processing, and improve dashboard reporting.
</p>

<hr>

<h2>Automated Workflow Architecture</h2>

<pre>
Email (Outlook)  
       ↓  
Power Automate → extract attachments  
       ↓  
Google Drive (cloud storage)  
       ↓  
Python script using Google Drive API (Google Cloud Platform)  
       ↓  
Consolidation in Power Query Editor  
       ↓  
Data Cleaning & Transformation  
       ↓  
Power BI Dashboard  
       ↓  
Auto Refresh → Published Dashboard 
</pre>

<hr>

<h2> Tools & Technologies Used</h2>
<ul>
  <li><strong>Microsoft Outlook</strong> – receives data files</li>
  <li><strong>Power Automate</strong> – extracts attachments & uploads to Google Drive</li>
  <li><strong>Google Cloud Platform</strong> – creates API credentials</li>
  <li><strong>Google Drive API</strong> – fetches files programmatically</li>
  <li><strong>Python Script</strong> – retrieves files from Drive to Power BI</li>
  <li><strong>Power Query Editor</strong> – consolidation & cleaning</li>
  <li><strong>Power BI Desktop</strong> – dashboard creation</li>
  <li><strong>Power BI Service</strong> – publishing & scheduled refresh</li>
</ul>

<hr>

<h2> Dashboard Visuals</h2>

<h3>Main Overview Dashboard</h3>
<img src="https://github.com/Nandan098/USA-FInancial-Data-Analysis-Power-BI/blob/main/Dashboard/Page-1.png"/>

<h3>Credit Mix, Payment Behaviour, Age Analysis</h3>
<img src="https://github.com/Nandan098/USA-FInancial-Data-Analysis-Power-BI/blob/main/Dashboard/Page-2.png"/>

<h3>LTV, Promotions, Loan Count, Age Groups</h3>
<img src="https://github.com/Nandan098/USA-FInancial-Data-Analysis-Power-BI/blob/main/Dashboard/Page-3.png"/>



<hr>

<h2> Dashboard Capabilities</h2>

<h3>Key Metrics</h3>
<ul>
  <li>Average annual income</li>
  <li>Average monthly balance</li>
  <li>Average credit utilization</li>
  <li>Average payment delays</li>
</ul>

<h3>Insights Delivered</h3>
<ul>
  <li>Age vs. credit limit change relation</li>
  <li>Payment behaviour vs credit mix</li>
  <li>Age demographic distribution</li>
  <li>Customer segmentation by age group</li>
  <li>LTV score calculation & promotion mapping</li>
  <li>Loan type distribution</li>
  <li>Potential customers and inquiries</li>
</ul>

<h3>LTV Formula</h3>
<pre>
LTV = (0.3 × Average Annual Income)
    - (0.15 × Average Delay Days)
    + (0.4 × Average Credit Score)
    + (0.075 × Average Amount Invested)
    + (0.075 × Average Monthly Balance)
</pre>

<hr>

<h2>Automatic Refresh & Publishing</h2>
<ul>
  <li>Python script connects Power BI to Google Drive API</li>
  <li>Data refresh triggers with new survey files</li>
  <li>Dashboard updates automatically</li>
  <li>Published to Power BI Service for stakeholder access</li>
</ul>

<hr>

<h2 Outcomes</h2>
<ul>
  <li>Eliminated manual processing</li>
  <li>Reduced costs & time</li>
  <li>Minimized human errors</li>
  <li>Improved reporting speed</li>
  <li>Provided actionable U.S. financial insights</li>
</ul>

<hr>


<h2> Data Automation Flowchart</h2>

```mermaid
flowchart TD
    A[Daily Files Received in Outlook Email] --> B[Power Automate Triggers Flow]
    B --> C[Extract Attachments Automatically]
    C --> D[Upload Files to Google Drive]
    D --> E[Python Script Accesses Drive via Google Drive API]
    E --> F[Load Data into Power Query Editor]
    F --> G[Clean, Transform & Consolidate Data]
    G --> H[Power BI Data Model & Visualizations]
    H --> I[Publish to Power BI Service]
    I --> J[Scheduled/On-Demand Auto Refresh]
    J --> K[Dashboard Updated with New Insights]
