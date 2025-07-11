# Bank-Customer-Churn-Analysis

## Table of Contents 
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning-and-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data analysis](data-analysis)
- [Visualisations and report](Visualisation-and-reports)
- [Results and Findings](#results-and-findings)
- [Conclusions](#conclusions)



### Project Overview
---
This Bank Customer Churn Analysis project demonstrates how Power BI was used to analyse customer retention patterns, clean and transform banking data, and apply DAX measures for insight generation. The dashboard highlights churn rates across customer segments, identifies high-risk profiles, and uncovers key factors contributing to customer attrition.

### Data Sources
The dataset was sourced from Kaggle and contains structured information on bank customers, including demographics, account activity, tenure, balance, and churn status. The data supports analysis of customer retention patterns and helps identify features linked to churn behavior in a banking context.

### Tools
---
- Excel: Data Cleaning
- Power BI: Data Analysis and Visualisation

### Data Cleaning and Preparation
---
The raw dataset from Kaggle was prepared using Excel for initial quality checks and Power Query in Power BI for transformation before building visualisations. The following steps were applied:
- Quality Check (Excel): Reviewed data structure, identified missing values, and validated column consistency.
- Column Removal: Dropped irrelevant or redundant columns to streamline analysis.
- Missing Values: Replaced blank values in numerical fields such as Age and Geography with average or most frequent values to maintain data completeness.
- Categorical Grouping: Created grouped columns for Credit Score, Age Range, Balance Range, and Tenure Range using conditional logic to support segment-based analysis.
- Conditional Columns: Added new fields to classify customers based on specific attributes (e.g., balance tier, tenure category).
- Churn Metrics: Created DAX measures to calculate the number and percentage of Churned vs. retained customers for comparative analysis.
- Data Architecture( Model Schema) was also created in support of filtering and analysis. The visual reference snapshot is attached below

  <img width="1018" height="568" alt="Screenshot 2025-07-11 135325" src="https://github.com/user-attachments/assets/f3a3670d-f508-4302-97c3-623ed39470e6" />


### Exploratory Data Analysis
---
The EDA phase focused on identifying patterns in customer churn across demographic and behavioural attributes. The dataset was reviewed to understand value distributions, missing entries, and outliers. Specific focus areas included:
- Distribution of customers by age, credit score, and tenure
- Categorical splits by gender, card ownership, and membership status
- Early identification of high-churn segments (e.g., specific age groups or tenure brackets

### Data Analysis
---
During the analysis phase, the following steps and metrics were implemented:

- Churn Rate Calculation: Percentage of customers marked as churned out of the total population
- Retention Rate: Percentage of customers who remained active
- Customer Segmentation: Grouped customers by age band, credit score range, balance, and tenure range for more targeted insights
- New Fields & Logic: Created categorical bins using conditional logic (e.g., Age Group, Credit Score Band)
- Defined DAX measures for churned and retained counts and percentages
- These metrics allowed for structured analysis across defined dimensions and enabled drill-down comparisons.

### Visualisations and Reports
This section outlines the Power BI dashboard built to analyze customer churn in a banking context. Each visual was designed to break down churn behavior across account features and demographics, allowing for precise identification of high-risk customer segments.

- Summary Cards: Key metrics are displayed using KPI cards:
1. Total Customers
2. Retained Customers
3. Churned Customers
4. Churn Rate (%)
These provide a clear, high-level view of the customer base and churn performance.
- Churn by Gender: A donut chart compares male and female churn proportions to assess if gender influences retention.
- Churn by Active Membership: This visual shows the distribution of churn among active and inactive members, helping assess engagement-related risk.
- Churn by Credit Card Ownership: Displays churn rates for customers who hold or don’t hold credit cards, offering insight into product linkage and behaviour.
- Churn by Age Group: A combined bar and line chart displays the number of customers per age group and their churn rate, highlighting high-risk age ranges (e.g., 41–60).
- Churn Table: A detailed table provides a segmented view of churn and retention counts, alongside churn percentages, across age bands. This format enables a clear comparison between segments.

The dashboard includes tab navigation for further breakdowns by balance, credit score, tenure, geography, and product holdings. These views support detailed, targeted analysis.

Below is the snapshot of an overview of the dashboard

<img width="1171" height="655" alt="Screenshot 2025-07-11 135714" src="https://github.com/user-attachments/assets/3ea6022c-8950-4daa-9f93-9acf4f407fcf" />



<img width="1174" height="662" alt="Screenshot 2025-07-11 135741" src="https://github.com/user-attachments/assets/8b878cb3-524a-4898-95fc-de13a2af43a6" />


<img width="1172" height="657" alt="Screenshot 2025-07-11 135806" src="https://github.com/user-attachments/assets/deb52ff2-b5bd-4555-b3b7-3dfdb940db9a" />


### Results and Findings
---
The analysis produced the following observations:
- Churn is highest in the 41–50 age group, with a churn rate of 33.99%, followed by the 51–60 age group at 56.21%
- Younger customers (<30) have low churn rates, with over 90% retention
- Customers with lower tenure and mid-level balances tend to churn more
- Card ownership and active membership status did not show extreme impact in isolation, but may compound when combined with tenure or age
These patterns point to risk concentration in older, mid-tenure customer segments with moderate balances.


### Conclusions
--- 
This project analysed customer churn across key demographic and account-based factors. The Power BI dashboard highlights where churn is most concentrated and provides breakdowns that support targeted retention planning.

By identifying high-risk segments—especially customers aged 41–60 with low tenure—the bank can prioritise outreach, adjust retention strategies, and improve customer lifecycle management. The structured visual layout allows for quick identification of trends without manual reporting effort.


