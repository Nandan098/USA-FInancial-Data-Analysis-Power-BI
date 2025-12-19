<h1 align="center">📊 USA Financial Data – Automated ETL & Power BI Dashboard</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Power%20BI-Data%20Visualization-F2C811?style=for-the-badge&logo=Power%20BI&logoColor=black" />
  <img src="https://img.shields.io/badge/Python-Automation-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Power%20Automate-Workflow-0066FF?style=for-the-badge&logo=Microsoft%20Power%20Automate&logoColor=white" />
  <img src="https://img.shields.io/badge/Google%20Cloud%20Platform-API-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white" />
</p>

<hr>

<h2>🚀 Project Goal — <i>Automate → Consolidate → Analyze → Visualize</i></h2>
<p>
This project automates the entire lifecycle of processing daily U.S. financial survey data.
Over 25 files received every day via email are automatically extracted, stored in cloud, consolidated, cleaned,
modeled and visualized in Power BI. The dashboard refreshes automatically and is published for stakeholders. 
</p>

<hr>

<h2>🧠 Business Problem</h2>
<ul>
  <li>Manual file downloads & merges</li>
  <li>Time pressure — 3 PM to 8 PM turnaround</li>
  <li>High human errors</li>
  <li>₹10L+ yearly cost (~$12,000/month)</li>
</ul>

<p><strong>Solution:</strong> Full automation + Power BI analytics for error-free and fast reporting.</p>

<hr>

<h2>🛠 Tools & Technologies</h2>

<table>
<tr><td><b>📨 Outlook</b></td><td>Receive daily files</td></tr>
<tr><td><b>⚙ Power Automate</b></td><td>Extract & upload attachments</td></tr>
<tr><td><b>☁ Google Cloud + Drive API</b></td><td>Authenticated file access</td></tr>
<tr><td><b>🐍 Python</b></td><td>API integration & fetching</td></tr>
<tr><td><b>🧹 Power Query Editor</b></td><td>Data cleaning & consolidation</td></tr>
<tr><td><b>📊 Power BI</b></td><td>Visualizations & publishing</td></tr>
</table>

<p><strong>Skills demonstrated:</strong><br>
Automation • ETL • API Integration • Cloud • Data Cleaning • Modeling • Visualization • Reporting</p>

<hr>

<h2>📷 Dashboard Overview</h2>

<h3 align="center">Main Dashboard (Executive View)</h3>
<p align="center">
  <img src="images/Screenshot3302.png" width="85%" />
</p>

<h3 align="center">Payment Behaviour & Credit Mix Analysis</h3>
<p align="center">
  <img src="images/Screenshot3306.png" width="85%" />
</p>

<h3 align="center">LTV, Promotions, Loan Overview & Customers</h3>
<p align="center">
  <img src="images/Screenshot3307.png" width="85%" />
</p>

<p align="center"><i>(Ensure you upload screenshots to /images directory)</i></p>

<hr>

<h2>📌 Key Insights Delivered</h2>
<ul>
  <li>Average income, delays, utilization</li>
  <li>Age vs credit limit change</li>
  <li>Loan & credit card patterns by age</li>
  <li>Payment behaviour by credit mix</li>
  <li>Customer segmentation by age & inquiries</li>
  <li>LTV score to drive promotion strategy</li>
</ul>

<hr>

<h2>🔄 Automation Workflow</h2>

```mermaid
flowchart LR
    A[Outlook receives daily files] --> B[Power Automate extracts attachments]
    B --> C[Files uploaded to Google Drive]
    C --> D[Python retrieves via Google Drive API]
    D --> E[Power Query cleans & merges]
    E --> F[Power BI dashboard]
    F --> G[Published to Power BI Service]
    G --> H[Auto refresh enabled]
