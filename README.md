# Customer Churn Decision Analytics
### Profit-Driven Retention Strategy with Cost-Sensitive Modeling

This project focuses on improving **business decision-making quality** rather than 
maximizing model accuracy. Instead of asking *“How well can we predict churn?”*, 
the analysis answers a more practical question:

> **“Who should we intervene on, and how much business value does that decision create?”**

By combining churn prediction models with cost-aware decision policies, this project 
demonstrates how analytics can directly translate into **measurable profit improvement**.

---

## 📌 Business Problem

Customer churn is costly, but **retention actions are also expensive**.  
In real-world settings, companies face limited budgets and operational constraints, 
making it impossible to intervene with every at-risk customer.

This project reframes churn modeling as a **decision optimization problem**, aiming to:

- Identify *which customers to target*
- Decide *when intervention is financially justified*
- Maximize **net business profit**, not predictive accuracy

---

## ❓ Key Business Questions

- Is a higher prediction accuracy always better for the business?
- At what churn probability does customer intervention become profitable?
- How do retention costs and expected benefits affect targeting decisions?
- Under limited budget or capacity, **who should be prioritized first?**

---

## 📊 Data

- **Dataset:** Telco Customer Churn dataset  
- **Target Variable:** Customer churn (Yes / No)
- **Features:** Customer demographics, contract information, service usage, and billing details

The dataset represents a realistic subscription-based business environment where 
churn decisions have direct financial implications.

---

## 🧠 Analytical Approach

### 1️⃣ Churn Prediction
Multiple classification models are trained and compared, including:
- Logistic Regression (interpretability-focused baseline)
- Tree-based models (to capture non-linear relationships)

Model evaluation emphasizes:
- ROC-AUC and PR-AUC (rather than accuracy alone)
- Probability calibration to support reliable decision-making

---

### 2️⃣ Cost-Sensitive Decision Framework

Instead of using a fixed probability threshold, the project introduces a 
**cost-aware decision rule** based on:

- Cost of customer intervention (e.g., retention offers, call center time)
- Expected value of saving a churned customer
- Assumed effectiveness of retention actions

This allows churn predictions to be converted into **expected profit calculations**.

---

### 3️⃣ Threshold & Budget Optimization

The project evaluates multiple decision policies:
- Probability threshold–based targeting
- Capacity-constrained Top-K targeting
- Profit comparison across different intervention strategies

Each policy is assessed using simulated business outcomes:
- Total intervention cost
- Expected customers retained
- Net profit and ROI

---

## 📈 Key Results (Example)

- Targeting only high-risk, high-value customers yields higher profit than 
  intervening broadly
- A small decrease in recall can result in **significant cost savings**
- Optimal decision thresholds differ depending on budget and intervention costs

> **Insight:**  
> A 1% improvement in model accuracy does not necessarily translate into higher business value,  
> while a well-designed decision policy can significantly improve profitability.

---

## 💡 Business Recommendations

- Use churn models as **decision-support tools**, not standalone predictors
- Align intervention thresholds with financial assumptions and capacity limits
- Continuously validate assumptions through controlled experiments (A/B testing)

---

## ⚠️ Limitations & Next Steps

- Retention success rates are assumed rather than experimentally validated
- Customer lifetime value is simplified and can be refined further

Future extensions include:
- Uplift modeling with experimental data
- Customer-level value–weighted decision policies
- Integration with A/B testing frameworks

---

## 🛠️ Tech Stack

- Python (pandas, scikit-learn, numpy)
- Jupyter Notebook
- Cost-sensitive evaluation & simulation
- GitHub for version control and documentation

---

## 🎯 Project Goal

This project is designed to showcase **Business Analytics–level thinking**, 
bridging predictive modeling with real-world decision-making and financial impact.

It is suitable for:
- MS Business Analytics / MBA applications
- Data Analyst / Analytics Consultant portfolios
- Decision-focused analytics case studies
