# Credit Card Risk Analysis Project

## Overview
This project represents a comprehensive pipeline developed by the project team to analyze, segment, and predict customer risk levels in a credit card dataset.  
The workflow spans from **data cleaning** to **stress scoring**, **segmentation**, **risk prediction**, **profit analysis**, and **exploratory data analysis (EDA)** of risk levels.  

The goal is to provide actionable insights for business teams in **marketing, customer engagement, and risk management**.

---

## Project Workflow & Notebooks

### 1. [Data Cleaning](README_cc_data_cleaning.md)
- Checked for missing values and imputed them using skewness analysis.
- Imputed `CREDIT_LIMIT` and `MINIMUM_PAYMENTS` using the **median** due to right-skewness.
- Verified no duplicate records.

**Outcome:** A clean, consistent dataset ready for downstream analysis.

---

### 2. [Stress Scoring](README_cc_stress_scoring.md)
- Defined behavioral risk flags (cash advances, low payments, high utilization, irregular balances).
- Combined flags into a composite **Stress Score**.
- Created business-friendly **Risk Levels** (Low, Medium, High) and an **Attention Flag**.

**Outcome:** An interpretable scoring system to flag risky customer behaviors.

---

### 3. [Customer Segmentation](README_cc_customer_segmentation.md)
- Applied **KMeans clustering** on scaled features.
- Evaluated cluster quality with Silhouette Score and Davies–Bouldin Index.
- Compared k values and identified **k=3** (broad segmentation) and **k=7** (granular segmentation).

**Outcome:** Clear customer segments including **VIP spenders, low-risk full payers, revolvers, and dormant users**.

---

### 4. [Risk Prediction](README_cc_risk_prediction.md)
- Built predictive models to forecast whether a customer requires attention.
- Addressed multicollinearity via **correlation analysis** and **VIF**.
- Managed class imbalance concerns (2.7:1 ratio).
- Logistic Regression baseline achieved **83% F1** and **91% accuracy**; alternatives (MLP, RF, XGBoost) considered.

**Outcome:** Logistic Regression deemed sufficient for operational risk flag forecasting.

---

### 5. [Profit Analysis](README_cc_profit_analysis.md)
- Analyzed profitability of at-risk customers.
- Calculated profit contribution at customer level.
- Quantified potential total loss exposure from unprofitable at-risk customers.
- Estimated preventive impact of predictive risk detection (~**$7.52 million** safeguarded).

**Outcome:** Linked customer risk with financial outcomes and demonstrated the business value of predictive models.

---

### 6. [Risk Level EDA](README_cc_data_risk_level_EDA.md)
- Quantified attention-needed customers (~26.9%).
- Profiled three key at-risk groups: **Dormant/Casual Users (44%)**, **Heavy Credit Users (25%)**, and **Balanced Moderate Spenders (20%)**.
- Proposed conversion opportunities tailored for each group.

**Outcome:** Data-driven recommendations for **customer reactivation, debt management, and upselling opportunities**.

---

## Business Impact
- Provides a **risk management framework** to identify and monitor at-risk customers.
- Enables **personalized marketing** by segmenting customers into actionable groups.
- Supports **predictive analytics** to forecast customer behaviors.
- Links **financial performance** with **risk indicators** to quantify potential losses and preventive savings.

---

## Next Steps
- Deploy predictive models into a real-time monitoring system.
- Continuously update customer segmentation with new data.
- Test marketing and risk control interventions on prioritized customer segments.

---

## Repository Structure
- `cc_data_cleaning_revised.html` → Data preprocessing and cleaning  
- `cc_stress_scoring_revised.html` → Stress scoring and attention flagging  
- `cc_customer_segmentation_revised.html` → Customer segmentation via clustering  
- `cc_risk_prediction_revised.html` → Predictive modeling of risk flags  
- `cc_profit_analysis_revised.html` → Profitability analysis of at-risk customers  
- `cc_data_risk_level_EDA_revised.html` → EDA of customer risk levels  
- `README_cc_*` → Module-level READMEs  
- `README_MASTER.md` → This file (project overview)  

---

## Contributors
This work reflects a **collaborative effort by the project team** to transform raw customer data into actionable insights for business stakeholders.
