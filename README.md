# Grocery Retail Marketing Analytics

An end-to-end marketing analytics project that transforms customer transaction and behavior data into actionable campaign targeting strategies.

Built as part of *Marketing Analytics with R*, this project focuses on **prioritization under budget constraints**, not just prediction accuracy.

---

## 🔍 Business Problem

In grocery retail, mass marketing campaigns often waste budget and customer goodwill.
The key question is not:

> "Who *might* respond?"

but rather:

> "Who should we prioritize when outreach capacity is limited?"

This project reframes campaign targeting as a **resource allocation and ranking problem**, aligning analytics with real-world marketing operations.

---

## 📊 Dataset Overview

- **2,240 customers**
- Demographics: income, household composition
- Behavioral data: spending by category, recency, channel preference
- Digital engagement: website visits
- Campaign response (binary outcome)

---

## 🧠 Analytical Approach

### 1. Exploratory Data Analysis (EDA)
- Identified key behavioral drivers of response:
  - Historical spending
  - Purchase recency
  - Digital engagement
  - Channel preference
  - Household size

### 2. Customer Segmentation (K-Means)
- Clustered customers into **4 actionable segments**, including:
  - High-value loyal shoppers
  - Digitally engaged but low spenders
  - Browsers at high risk of churn

### 3. Predictive Modeling (Logistic Regression)
- Modeled probability of campaign response
- Interpretable coefficients aligned with marketing intuition

### 4. Lift-Based Targeting & Cutoff Selection
- Used **decile lift analysis** to select an optimal cutoff
- Evaluated performance using:
  - ROC AUC
  - Lift
  - Recall at workload
  - Business trade-offs (cost vs. reach)

---

## 📈 Key Results

Targeting only the **top 40%** of ranked customers:
- **24.3% response rate** (vs. 13.7% baseline → **1.78× lift**)
- **70.7% of all responders captured**
- **60% reduction in outreach volume**

This demonstrates how ranking-based targeting improves ROI without increasing marketing spend.

---

## 🧩 Business Recommendations

- Prioritize high-value, digitally engaged customers for premium campaigns
- Match channels to customer behavior (digital vs. in-store)
- Deploy predictive scores directly into campaign execution
- Launch automated win-back strategies for high-risk churn segments

---

## 🛠️ Tools & Methods

- R (tidyverse, ggplot2, stats)
- K-means clustering
- Logistic regression
- ROC & lift analysis
- Marketing-focused evaluation metrics

---

## 🚀 Key Takeaway

The real value of analytics lies not in complex models,
but in **turning messy customer behavior into clear prioritization and executable decisions**.

---

## 📁 Repository Structure
├── data/
│ └── customer_data.csv
├── notebooks/
│ ├── 01_eda.R
│ ├── 02_segmentation.R
│ └── 03_predictive_modeling.R
├── visuals/
│ └── charts/
├── report/
│ └── final_report.pdf
└── README.md

---

## 📌 Notes

This project uses an academic dataset.  
The methodology is designed to scale to real-world retail environments with larger volumes and richer operational signals.

