# 🛡️ FraudSight — Financial Fraud Intelligence & Risk Analytics Platform  

**Author:** Kamran Habib  
**Tools:** Azure Databricks (PySpark + SQL) | Delta Lake | Azure Data Factory | Power BI  
**Focus:** Data Engineering · Fraud Analytics · Business Intelligence  

---

## 📌 Business Objective  
Financial institutions face increasing losses due to transaction fraud, high-risk merchants, and account takeovers.  
**FraudSight** consolidates raw transaction, merchant, account, and login/device data to detect fraud patterns, identify risky entities, and support proactive fraud investigation through interactive dashboards.

---

## ⚙️ Technical Workflow  

| Stage | Platform | Key Tasks |
|-------|-----------|-----------|
| **Data Engineering** | Azure Databricks | Ingested raw transaction, merchant, account, and login/device datasets into Bronze layer with schema enforcement. |
| **Data Transformation** | PySpark + SQL | Cleaned and standardized Silver tables, merged fraud labels, handled nulls, derived fraud & behavioural indicators. |
| **Analytics Modeling** | Delta Lake | Built Gold tables (`FactTransactions`, `MerchantRisk`, `DailyAccountSummary`, `FactLoginRisk`, `DimAccount`, `DimMerchant`, `DimMCC`, `Date`). |
| **Pipeline Orchestration** | Azure Data Factory | Designed automated Bronze → Silver → Gold ETL pipelines. |
| **Visualization** | Power BI | Developed multi-page dashboards (Fraud Overview · Merchant Risk · Account Behaviour · Account Risk Summary). |

---

## 📊 Power BI Highlights  

- **Fraud Overview:** KPIs (Total Transactions, Fraud Transactions, Fraud Rate %, Fraud per 1,000), fraud vs transaction trend, country-wise fraud distribution.  
- **Merchant Risk:** Merchant fraud trend, MCC category fraud rates, chargeback ratios, high-risk merchant identification.  
- **Account Behaviour:** Daily spend vs transaction count, fraud 7-day moving average, behavioural anomaly analysis.  
- **Account Risk Summary:** Failed logins, MFA failures, unique devices/IPs, rooted device attempts, IP reputation scoring.

---

## 💡 Key Insights  

| Question | Finding |
|-----------|----------|
| Where is fraud concentrated? | Fraud is concentrated in specific countries and MCC categories with elevated fraud rates. |
| Which merchants are risky? | Certain merchants and MCC groups show recurring fraud and chargeback patterns. |
| Which accounts are suspicious? | Accounts with high failed logins, MFA failures, and multiple device/IP usage correlate strongly with fraud. |
| Are there signs of account takeover? | Yes — device/IP anomalies combined with authentication failures are strong indicators. |

---

## 📈 Business Impact  

- Enabled **early detection of fraudulent transaction patterns**  
- Improved **merchant risk monitoring** and MCC-level segmentation  
- Strengthened **account takeover detection** using behavioural and device/IP signals  
- Reduced manual fraud analysis through automated dashboards  

---

## 🧰 Skills Demonstrated  

- **Data Engineering:** PySpark, Databricks, Delta Lake, Medallion Architecture  
- **ETL Pipelines:** Bronze–Silver–Gold layering, Azure Data Factory orchestration  
- **Visualization:** DAX measures, time intelligence, multi-page Power BI reports  
- **Fraud Analytics:** Transaction anomalies, merchant & MCC risk analysis, account behaviour profiling  

---

## 🔗 Links  

- 📄 [FraudSight Final Report (PDF)](FraudSight.pdf)
- 📊 [Power BI Project File (.pbix)](Phase%202_Visualization%20Part_RECOVERY.pbix)
- 🧠 [SQL & PySpark Code (ZIP)](SQL_Python_codes.zip) 

---

## 📅 Next Steps  

- Add ML-based fraud prediction models (Isolation Forest / Gradient Boosting)  
- Enable real-time streaming ingestion  
- Introduce graph analytics for fraud ring detection  
- Publish dashboards to Power BI Service  

---

⭐ **If you like this project, star the repo!**
