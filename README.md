🛡️ FraudSight — Financial Fraud Intelligence & Risk Analytics Platform

Author: Kamran Habib
Tools: Azure Databricks (PySpark + SQL) · Delta Lake · Azure Data Factory · Power BI (DAX)
Focus: Data Engineering · Fraud Analytics · Business Intelligence · Risk Monitoring

📌 Business Objective

Banks and payment processors face increasing fraud risk across transactions, merchant networks, and account behaviour.
FraudSight consolidates raw operational data, engineers a unified risk dataset, and delivers interactive dashboards that help fraud teams:

Detect unusual transaction patterns

Identify high-risk merchants & MCC categories

Analyse suspicious account behaviour

Surface device/IP anomalies indicating account takeover

⚙️ Technical Workflow
Stage	Platform	Key Tasks
Data Ingestion & Engineering	Azure Databricks	Loaded raw transaction, merchant, account, and login/device datasets into Bronze layer; applied schema enforcement.
Data Transformation	PySpark + SQL	Cleaned & standardized Silver tables; merged transactions with fraud labels; engineered behavioural & risk features.
Data Modeling	Delta Lake	Built Gold analytical tables: FactTransactions, MerchantRisk, DailyAccountSummary, FactLoginRisk, DimAccount, DimMerchant, DimMCC, Date.
Pipeline Orchestration	Azure Data Factory	Designed pipelines to automate Bronze → Silver → Gold transformations.
Visualization	Power BI	Built a 4-page fraud intelligence dashboard: Overview • Merchant Risk • Account Behaviour • Account Summary.
📊 Power BI Highlights
1️⃣ Fraud Overview

KPIs: Total Transactions, Fraud Transactions, Fraud Rate %, Fraud per 1,000

Trends: Fraud vs Total Transaction Timeline

Geographic Risk: Country-wise fraud distribution

Behavioural Indicators: High Amount Fraud · High Velocity Fraud · Night Fraud · New Device Fraud

2️⃣ Merchant Risk Analysis

Merchant Fraud Trend over time

MCC Category Fraud Rate

Merchant-level Fraud & Chargeback Rates

Slicers for MCC, Merchant, Country

Identifies persistently high-risk merchants

3️⃣ Account Behaviour Analysis

Daily Spend vs Transaction Count

Fraud 7-Day Moving Average

Behavioural anomaly detection

Account activity table with slicers

4️⃣ Account Risk Summary

Unique Devices

Unique IPs

Failed Logins

Failed MFA Attempts

Rooted Device Attempts

IP Reputation Score

High-level profile of compromised accounts

💡 Key Insights
Question	Finding
Where is fraud happening?	Concentrated in certain countries and MCC categories.
Which merchants are risky?	Several MCC groups show consistently elevated fraud rates.
Are accounts behaving abnormally?	Accounts with high failed login activity correlate with higher fraud.
Are there signs of account takeover?	Multiple devices, multiple IPs, and frequent failed MFA attempts are strong indicators.
📈 Business Impact

Early detection of transaction anomalies

Merchant risk segmentation for targeted reviews

Improved fraud investigation efficiency using consolidated dashboards

Account takeover detection using device/IP behaviour patterns

Enterprise-ready architecture suitable for scalable fraud systems

🧰 Skills Demonstrated
Data Engineering

PySpark transformations

Delta Lake Medallion Architecture

SQL-based feature engineering

ETL orchestration with Azure Data Factory

Business Intelligence

Power BI modeling (Star Schema)

40+ DAX measures (fraud KPIs, behaviour metrics, merchant risk)

Multi-page interactive dashboards

Fraud Analytics

Transaction risk indicators

Merchant & MCC fraud patterns

Behavioural anomalies

Device/IP risk scoring

Professional Practices

Modular data engineering approach

Clean semantic modeling

Appendix-style reporting

Executive-ready dashboards

🔗 Links

📄 FraudSight Final Report (PDF)
📊 Power BI Dashboard Screens (PDF)
🧠 Power BI Project File (.pbix)
🧾 Gold-Layer Analytical Dataset (CSV/Delta)
📁 Databricks Notebooks (ZIP)

📅 Next Steps

Add ML-based fraud prediction (Isolation Forest / XGBoost)

Introduce graph analysis for fraud ring detection

Publish dashboards to Power BI Service for real-time monitoring

Enable streaming ingestion for real-time fraud alerts
