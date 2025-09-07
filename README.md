# 📊 E-Commerce Data Analysis

This repository contains an end-to-end **exploratory data analysis (EDA)** project on a synthetic e-commerce customer dataset. The project demonstrates data exploration, cleaning, filtering, and deriving business insights using **Python** and **Pandas**.

---

## 📌 Project Overview

Understanding customer behavior is crucial for e-commerce businesses.
This project analyzes a dataset of 30,000 customer records with attributes like **name, age, gender, profession, province, spending habits, credit card information, and purchase dates**.

Key objectives of the project:

* Explore customer demographics and spending behavior.
* Identify high-value customers and zero-spending customers.
* Examine popular professions, names, and email providers.
* Understand geographical distribution and patterns by province.
* Provide actionable insights for marketing campaigns.

---

## 🗂 Dataset

* **File Used:** `Cust_Purch_FakeData.csv`
* **Size:** 30,000 rows × 20 columns
* **Features Include:**

  * `prefix`, `first`, `last`, `email`, `gender`, `age`
  * `company`, `profession`, `province`
  * `price(CAD)` – amount spent
  * `cc_no`, `cc_type`, `cc_exp`
  * `weekday`, `date`

---

## 🔧 Tools & Libraries

The analysis is performed in **Python** using:

* **Pandas** – Data manipulation & analysis
* **NumPy** – Numerical operations
* **Matplotlib / Seaborn (optional)** – Visualization (can be added for future work)
* **Jupyter/Colab** – Notebook environment for step-by-step execution

---

## 📊 Analysis & Key Steps

### 1. Data Exploration

* Displayed first few rows using `df.head()`
* Checked data types and memory usage with `df.info()`
* Found:

  * **Max Age:** 65
  * **Min Age:** 18
  * **Average Age:** \~42

### 2. Customer Insights

* Top **3 first names:** Willie, Francis, Eula
* Top **3 last names:** Byrd, Morales, Luna
* Identified duplicate phone numbers.

### 3. Profession Analysis

* Counted total customers with profession = "Structural Engineer"
* Segmented by **gender** and **province**
* Found **87 Structural Engineers**, 43 of them male.

### 4. Spending Behavior

* **Max Spending:** 100 CAD
* **Average Spending:** \~50 CAD
* Identified:

  * **Zero spenders** → potential target for discounts
  * **High spenders (≥100 CAD)** → eligible for loyalty coupons

### 5. Credit Card & Email Insights

* Found customers with specific credit card numbers
* Counted cards expiring in 2019 (2684 customers)
* Counted Visa card users (1,721 customers)
* Found customers who spent 100 CAD using Visa

### 6. Popular Email Providers

* **Top 5:** gmail.com, me.com, outlook.com, live.com, hotmail.com
* Identified customers using educational emails (e.g., `am.edu`)

### 7. Temporal Patterns

* Found that **Saturday** has the highest number of customers visiting.

---

## 💡 Business Insights

* **Marketing Opportunity:** Target customers with `price(CAD)=0` with promotional offers.
* **Customer Loyalty:** Reward top spenders with personalized coupons.
* **Geographical Focus:** Alberta and Ontario have a significant number of professionals worth segmenting for campaigns.
* **Seasonal Trends:** Saturday is the busiest day, suggesting the ideal time for flash sales.

---

## 📁 Repository Structure

```
📦 E-commerce-Data-Analysis
 ┣ 📜 E-commerce Data Analysis.ipynb   # Jupyter/Colab notebook
 ┣ 📜 Cust_Purch_FakeData.csv          # Dataset (if shared)
 ┣ 📜 README.md                        # Project documentation
 ┗ 📜 requirements.txt                  # (Optional) Python dependencies
```

---

## 🚀 How to Run the Project

1. Clone this repository

   ```bash
   git clone https://github.com/your-username/ecommerce-data-analysis.git
   cd ecommerce-data-analysis
   ```

2. Install dependencies

   ```bash
   pip install pandas numpy
   ```

3. Open the notebook

   ```bash
   jupyter notebook "E-commerce Data Analysis.ipynb"
   ```

   or use **Google Colab** to run it directly.

---

## 📌 Future Work

* Add **visualizations** for spending distribution, gender vs spending, top provinces.
* Build a **predictive model** for customer spending behavior.
* Automate **customer segmentation** for targeted marketing.
