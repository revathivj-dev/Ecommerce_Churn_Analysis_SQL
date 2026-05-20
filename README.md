Readme
Getting Started
E Commerce Customer Churn Analysis
Overview
This project analyzes customer churn patterns in the e commerce domain using SQL based data cleaning, transformation, and exploratory analysis. It provides dashboard ready views for integration with BI tools like Power BI and Tableau, enabling stakeholders to identify churn drivers and design targeted retention strategies.
Project Objective
To uncover the key drivers of customer churn and provide actionable insights that help 
Problem Statement
Customer churn erodes profitability and loyalty in e commerce. Without structured analysis, businesses struggle to identify why customers leave — whether due to poor onboarding, dissatisfaction, payment trust issues, or regional delivery challenges. This project builds a data driven churn analysis framework to highlight vulnerable segments and recommend retention strategies.
Scope
•	Data Cleaning: Handle missing values, impute mean/mode, remove outliers.
•	Data Transformation: Standardize categorical values, rename columns, create derived fields (ComplaintReceived, ChurnStatus).
•	Exploratory Analysis: SQL queries for churn rate by payment mode, tenure, satisfaction, complaints, city tier, and high risk segments.
•	Dashboard Integration: SQL views for BI tools (vw_churn_summary, vw_churn_by_payment, etc.).
•	Executive Insights: Narrative synthesis of churn drivers with recommendations.
E commerce businesses reduce attrition, improve customer loyalty, and maximize lifetime value.
Deliverables
1.	Cleaned Dataset – standardized and imputed values.
2.	SQL Scripts – for cleaning, transformation, and analysis queries.
3.	Dashboard Views – modular SQL views for BI integration.
4.	Executive Insights – churn drivers and retention playbook.
5.	Presentation Deck Outline – 10 slide executive summary.
Methodology
1.	Data Collection – transactional and behavioral attributes.
2.	Data Cleaning – imputation of missing values, outlier removal.
3.	Data Transformation – standardization, renaming, derived fields.
4.	Exploratory Analysis – churn queries across multiple dimensions.
5.	Dashboard Integration – BI ready SQL views.
6.	Insight Synthesis – executive recommendations.
7.	Action Plan – lifecycle engagement, payment promotions, complaint resolution, regional logistics, segment specific campaigns.
Key Insights
•	COD customers churn more; UPI/Wallet users are more loyal.
•	Early tenure customers churn quickly; long tenure churn signals dissatisfaction.
•	Low satisfaction scores strongly predict churn.
•	Complaint raising customers churn at higher rates.
•	Tier 2/3 cities show higher churn due to logistics challenges.
•	Male COD users in fashion categories are the most vulnerable segment.
Future Work
•	Predictive churn modeling (logistic regression, decision trees).
•	Advanced segmentation (clustering).
•	RFM analysis for loyalty measurement.
•	Dashboard enhancements with predictive scores.
•	A/B testing of retention strategies.
•	Expansion to Indian e commerce context (Flipkart/Amazon style datasets).
How to Use
1.	Run SQL scripts to clean and transform the dataset.
2.	Execute analysis queries to generate churn insights.
3.	Use dashboard views (vw_churn_summary, vw_churn_by_payment, etc.) in Power BI/Tableau.
4.	Present executive insights using the prepared deck outline.
Prerequisites
•	Database: MySQL or PostgreSQL (tested on MySQL 8.x)
•	BI Tool (optional): Power BI or Tableau for dashboard integration
•	Dataset: Place raw dataset in /data/customer_churn_raw.csv




Setup Instructions
1.	Clone the repository
bash
git clone https://github.com/yourusername/customer-churn-analysis.git
cd customer-churn-analysis
--- Create the database
CREATE DATABASE ecomm;
USE ecomm;
---Load the dataset
•	Import customer_churn_raw.csv into the customer_churn table.
•	Use MySQL Workbench, pgAdmin, or CLI tools.
----Run cleaning scripts
1.	SOURCE sql_scripts/data_transformation.sql;
2.	Run analysis queries
SOURCE sql_scripts/analysis_queries.sql;
---Create dashboard views
SOURCE views/vw_churn_summary.sql;
SOURCE views/vw_churn_by_payment.sql;
-- (and other views)
Quick Validation
SELECT * FROM vw_churn_summary;
SELECT * FROM vw_churn_by_payment;



