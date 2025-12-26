# 🛍️ H&M Customer Behavior Analysis

## 📘 Project Overview

This project dives deep into **customer shopping behavior** using real-world transactional data from **1000 purchases** across multiple product categories.
The objective is to uncover actionable insights into **spending habits, customer segments, product preferences, and subscription behavior**, helping drive **data-informed business decisions** for H&M.

---

## 📊 Dataset Summary

**Dataset Size:** 1,000 rows × 18 columns

### **Key Features**

* **Customer Demographics:** Age, Gender, Location, Subscription Status
* **Purchase Details:** Item Purchased, Category, Purchase Amount, Season, Size, Color
* **Behavioral Attributes:** Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type

**Missing Data:**

* 483 missing values in the `discount_applied` column handled through imputation.

---

## 🧹 Data Cleaning & Preparation (Python)

Performed in **Python (Pandas & NumPy)** to ensure clean, consistent, and enriched data.

**Steps:**

1. **Data Loading:** Imported dataset via `pandas.read_csv()`.
2. **Exploration:** Used `.info()` and `.describe()` for quick structure and statistical summary.
3. **Handling Missing Data:** Imputed missing values in `discount_applied` and `promo_code_used` using median per category.
4. **Standardization:** Converted all column names to snake_case for readability.
5. **Feature Engineering:**

   * Created `age_group` by binning age values.
   * Created `purchase_frequency_days` from transaction timestamps.
6. **Redundancy Check:** Found `promo_code_used` redundant with `discount_applied` and removed it.
7. **Database Integration:** Loaded the cleaned dataset into **PostgreSQL** for efficient querying and advanced SQL analytics.

---

## 🧠 SQL Analysis & Business Insights

SQL queries were used to answer strategic business questions and identify key behavioral trends:

1. **Revenue by Gender:** Compared total revenue between male and female shoppers.
2. **Subscriber vs Non-Subscriber Revenue:** Evaluated differences in purchase behavior.
3. **Top 5 Most Purchased Items:** Identified most popular products.
4. **Average Sales by Age Group:** Revealed how spending varies by age.
5. **Promo Code Performance:** Found the promo code yielding the highest revenue.
6. **Customer Distribution by Location:** Analyzed total customers and average purchase amounts by region.
7. **Shipping Type Comparison:** Compared spending habits across shipping methods.
8. **Top-Rated Items:** Identified items with the highest average review ratings.
9. **Purchase Frequency Impact:** Explored correlation between buying frequency and spending.

---

## 📈 Power BI Dashboard

A dynamic **Power BI Dashboard** was built to visualize insights across multiple dimensions:

* 👥 **Customer Segmentation:** By gender, age group, and location
* 💸 **Revenue Analysis:** Subscribers vs. non-subscribers
* 🌟 **Product Insights:** Top-performing items and best promo codes
* 📦 **Behavioral Trends:** Purchase frequency vs. average spending
* ⭐ **Customer Satisfaction:** Relationship between review ratings and purchase behavior

---

## 💼 Business Recommendations

Based on the findings, the following data-driven strategies are recommended:

1. **Boost Subscriptions:** Market exclusive offers to increase subscriber conversion.
2. **Enhance Loyalty Programs:** Reward repeat buyers to foster long-term engagement.
3. **Review Discount Strategy:** Balance discounts with profitability margins.
4. **Highlight Top Performers:** Feature best-rated and high-selling items in campaigns.
5. **Target High-Value Segments:** Focus marketing on profitable age groups and express shipping users.

---

## 🧰 Tech Stack

**Languages & Tools:**

* **Python** (Pandas, NumPy, Matplotlib, Seaborn)
* **SSDM** (for SQL analysis)
* **Power BI** (for visualization)
* **Git & GitHub** (for version control)

---

## 🚀 How to Use

1. Clone the repository:

   ```bash
   git clone https://github.com/dhimandipanshi/HM-customerAnalysis.git
   ```
2. Open the Jupyter Notebook or Python script to explore the data cleaning and EDA steps.
3. Use the included SQL queries for in-depth data analysis.
4. Open the Power BI file to interact with the visual dashboard.

---

## ✨ Author

👩‍💻 **Dipanshi Dhiman**
Data Analyst | Business Intelligence Enthusiast
📍 Toronto, Canada
📧 [dhimandipanshi713@gmail.com](mailto:dhimandipanshi713@gmail.com)

---

> “Turning data into strategy — because every purchase tells a story.” 💡
