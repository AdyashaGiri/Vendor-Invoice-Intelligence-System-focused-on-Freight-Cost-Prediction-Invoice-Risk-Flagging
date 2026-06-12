# Vendor Invoice Intelligence System 🚚💼

An end-to-end data science and machine learning solution designed to automate corporate invoice auditing. This project targets **Invoice Cost Leakage and Audit Risk** by combining relational data engineering, statistical analysis, and a dual-model predictive pipeline to identify overcharges and anomalies before payment processing.

## 🎯 Business Objectives
* **Predict Freight Cost:** A regression pipeline that estimates what a specific shipment *should* cost based on historical logistics metrics.
* **Flag Risky Invoices:** A classification pipeline that flags anomalous, suspicious, or highly irregular vendor submissions for human review.

## 🛠️ Tech Stack & Workflow
* **Database & Feature Engineering:** Structured relational tables managed via **SQLite** (`inventory.db`) with custom invoice-level SQL aggregations.
* **Exploratory Data Analysis (EDA):** Statistical validation (including T-Tests) to isolate cost patterns and distinct risk behaviors.
* **Machine Learning Pipelines:** 
  * **Regression:** Evaluated via MAE, RMSE, and R² to accurately forecast continuous freight charges.
  * **Classification:** Evaluated via Precision, Recall, and F1-Score to catch high-risk anomalies effectively.
* **Deployment:** Serialized model artifacts (`.pkl`) integrated into an interactive, real-time analytics dashboard built with **Streamlit** for business end-users.

## 📈 Key Deliverables
* Automated detection of financial leakage.
* Reduced manual auditing overhead through prioritized risk-flagging.
* Executive-ready dashboard featuring real-time insights and alerts.
