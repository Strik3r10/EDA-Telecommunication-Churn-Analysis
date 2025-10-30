# 🧠 Customer Churn Analysis Using Python

A detailed exploratory data analysis project aimed at understanding **customer churn behavior** and identifying key factors influencing churn in a telecom dataset using **Python’s Pandas framework**.

---

## 📋 Table of Contents
- [Goals of the Project](#goals-of-the-project)
- [Dataset Overview](#dataset-overview)
- [Libraries Used](#libraries-used)
- [Key Business Questions](#key-business-questions)
- [Project Workflow](#project-workflow)
- [Important Visualizations](#important-visualizations)
- [Key Findings](#key-findings)
- [Installation & Usage](#installation--usage)
- [Project Structure](#project-structure)
- [Future Improvements](#future-improvements)

---

## 🎯 Goals of the Project

1. **Explore and clean telecom churn data** for better interpretability.  
2. **Identify key customer segments** more likely to churn.  
3. **Visualize churn patterns** across demographics, services, and payment behaviors.  
4. **Generate actionable insights** for retention and strategy optimization.

---

## 📊 Dataset Overview

- **Source:** Kaggle – Customer Churn Dataset  
- **Records:** 7,043 observations  
- **Features:** 21 (Demographic, Contract, Service, and Payment features)  
- **Target:** `Churn` (Yes/No)  
- **Missing Values:** Present in `TotalCharges`, handled via numeric conversion.  

---

## 🛠️ Libraries Used

- **NumPy** – Numerical operations  
- **Pandas** – Data wrangling and exploration  
- **Matplotlib / Seaborn** – Data visualization  
- **Warnings / OS** – Code readability and performance  

---

## 💡 Key Business Questions

1. What is the overall churn rate and distribution?  
2. Do contract types and tenure length affect churn?  
3. Which payment methods are linked to higher churn?  
4. How do demographics (gender, partner, dependents) influence churn?  
5. How are `MonthlyCharges`, `TotalCharges`, and `tenure` related to churn?

---

## ⚙️ Project Workflow

1. **Data Import & Cleaning**
   - Handled missing values in `TotalCharges`.  
   - Converted columns to correct data types.  

2. **Feature Engineering**
   - Created `tenure_group` feature (1–12, 12–24, … months).  
   - Encoded categorical variables for correlation analysis.  

3. **EDA & Visualization**
   - Visualized churn patterns, demographic effects, and service dependencies.  

4. **Insights Generation**
   - Highlighted actionable factors for churn reduction.

---

## 📈 Important Visualizations

1. **Churn Distribution:** Horizontal bar chart showing churn vs non-churn ratio.  
2. **Tenure Groups:** Customers with tenure < 12 months churned the most.  
3. **Contract Type:** Monthly contracts had the highest churn rate.  
4. **Payment Method:** Electronic check users showed higher churn.  
5. **Correlation Heatmap:** Revealed weak positive correlation between monthly and total charges.  
6. **Demographics:** Female customers with partners exhibited higher churn probability.

---

## 🔍 Key Findings

- **Short-tenure customers (≤12 months)** churn significantly more.  
- **Monthly contracts** and **electronic payment methods** are key churn drivers.  
- **Low total charges** but **high monthly charges** → higher churn probability.  
- **Senior citizens and customers without dependents** are more likely to churn.  
- **Partner presence and gender** influence churn patterns unexpectedly.

---

## 💻 Installation & Usage

```bash
# Clone the repository
git clone https://github.com/<your-username>/Customer-Churn-Analysis.git

# Navigate to folder
cd Customer-Churn-Analysis

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook CaseStudy_ChurnAnalysis.ipynb
```

---

## 📁 Project Structure

```
Customer-Churn-Analysis/
│
├── CaseStudy_ChurnAnalysis.ipynb   # Main analysis notebook
├── CustomerChurn.csv               # Dataset
├── README.md                       # Project documentation
└── requirements.txt                # Dependencies
```

---

## 🚀 Future Improvements

- Implement predictive churn modeling (Logistic Regression, Random Forest).  
- Add dashboards using **Plotly** or **Power BI**.  
- Automate churn prediction pipeline for real-time use.  
- Extend analysis with feature importance ranking.
