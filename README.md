# CRM Promotion Targeting for a Limited-Time Grocery Promotion

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-purple)
![CRM Analytics](https://img.shields.io/badge/CRM-Analytics-success)
![RFM Analysis](https://img.shields.io/badge/RFM-Customer_Segmentation-orange)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

## About

This project identifies the 100 most promising customers for a limited-time grocery promotion using transactional, customer, product, and promotion data.

The solution combines RFM analysis with promotion engagement metrics to build an interpretable customer scoring model for campaign targeting.

Raw Data
    ↓
Data Cleaning
    ↓
Feature Engineering
    ↓
RFM Analysis
    ↓
Promotion Metrics
    ↓
Customer Scoring
    ↓
Top 100 Customers

---

## Business Problem

A grocery retailer plans a limited-time promotion but can target only 100 customers.

The objective is to identify customers who are most likely to deliver high business value based on historical purchasing behaviour and previous promotion engagement.

Rather than relying on a single metric, the project combines several behavioural indicators into a transparent customer ranking.

---

## Dataset

The analysis uses five datasets:

- Customer
- Sales
- Promotion
- Articles
- Account

---

## Methodology

The analysis consists of four main stages:

### 1. Data Preparation

- data cleaning
- duplicate removal
- missing value handling
- feature engineering
- data validation

### 2. Customer Behaviour Analysis

Customer purchasing behaviour is evaluated using the RFM framework:

- Recency
- Frequency
- Monetary

### 3. Promotion Engagement

Two additional CRM metrics are calculated:

- Promotion Transaction Ratio
- Promotion Value Ratio

### 4. Customer Scoring

All metrics are normalized and combined into a weighted customer score.

Customers are ranked according to the final score, and the Top 100 customers are selected for the promotion campaign.

---

## Results

The project produces:

- customer RFM metrics
- promotion engagement metrics
- final customer score
- ranked Top 100 customer list

Output:

```
outputs/
└── top_100_customers.csv
```

---

## Alternative Approaches Considered

Several alternative analytical approaches were considered.

**K-Means** and **Gaussian Mixture Models** could be used for customer segmentation. While valuable for long-term CRM strategy, they produce customer groups rather than a ranked list for a specific campaign.

**Linear Regression** and **XGBoost** could be applied to predict promotion response probabilities. However, supervised models require historical campaign response labels, which were not available in this case.

Given the business objective and available data, an interpretable scoring framework was selected as the most appropriate solution.

---

## Repository Structure

```
├── README.md
├── notebooks/
│   └── local_grocery_100customers_limitedOffer.ipynb
├── outputs/
│   └── top_100_customers.csv
├── requirements.txt
└── .gitignore
```

---

## Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

---

## Skills Demonstrated

- CRM Analytics
- Customer Analytics
- Customer Targeting
- RFM Analysis
- Feature Engineering
- Data Cleaning
- Data Validation
- Exploratory Data Analysis (EDA)
- Marketing Analytics
