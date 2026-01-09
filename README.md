# Customer Shopping Behavior Analysis

## 📌 Project Overview
This project analyzes customer shopping behavior using transactional data from **3,900 purchases** across multiple product categories. The objective is to uncover actionable insights related to **customer spending patterns, demographics, product preferences, discount usage, and subscription behavior** to support data-driven business decisions.

The project combines **Python for data cleaning & EDA**, **PostgreSQL for business-focused SQL analysis**, and **Power BI for interactive visualization**.

---

## 📊 Dataset Summary
- **Total Records:** 3,900
- **Total Columns:** 18
- **Key Features:**
  - Customer demographics (Age, Gender, Location, Subscription Status)
  - Purchase details (Item Purchased, Category, Purchase Amount, Season, Size, Color)
  - Shopping behavior (Discount Applied, Promo Code Used, Purchase Frequency, Review Rating, Shipping Type)
- **Missing Data:** 37 missing values in the *Review Rating* column

---

## 🧹 Data Cleaning & Preparation (Python)
The following steps were performed using **Python (Pandas, NumPy)**:

- Loaded and explored the dataset using `df.info()` and `df.describe()`
- Handled missing values by imputing **median review ratings per product category**
- Standardized column names to **snake_case**
- Performed **feature engineering**:
  - Created `age_group` by binning customer ages
  - Derived `purchase_frequency_days`
- Identified redundancy between `discount_applied` and `promo_code_used` and removed unnecessary columns
- Exported cleaned data into **PostgreSQL** for SQL-based analysis

---

## 🗄️ Data Analysis Using SQL (PostgreSQL)
Business-driven queries were written to answer key questions, including:

1. Revenue comparison by **gender**
2. Identifying **high-spending customers** who used discounts
3. Top 5 products by **average review rating**
4. Comparison of purchase amounts by **shipping type**
5. Spending patterns of **subscribers vs non-subscribers**
6. Products most dependent on **discounts**
7. Customer segmentation into **New, Returning, and Loyal**
8. Top 3 products per category
9. Relationship between **repeat purchases and subscriptions**
10. Revenue contribution by **age group**

---

## 📈 Power BI Dashboard
An interactive **Power BI dashboard** was created to visualize:
- Revenue trends
- Customer segmentation
- Subscription analysis
- Product performance
- Discount impact on sales

The dashboard enables stakeholders to quickly identify patterns and make informed decisions.

---

## 💡 Business Recommendations
Based on the analysis, the following insights were proposed:
- Promote **subscription benefits** to increase recurring revenue
- Implement **customer loyalty programs** for repeat buyers
- Optimize **discount strategies** to balance sales and profitability
- Highlight **top-rated and best-selling products**
- Focus marketing efforts on **high-revenue age groups** and **express shipping users**

---

## 🛠️ Tools & Technologies Used
- **Python** (Pandas, NumPy, Matplotlib, Seaborn)
- **PostgreSQL** (SQL for business analysis)
- **Power BI** (Dashboard & visualization)
- **Jupyter Notebook**
- **Git & GitHub**

---

## 📂 Project Structure
