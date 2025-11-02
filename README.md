# Customer_Shopping_Behaviour_analysis
Analysis of 3,900 transactions revealed Male customers ($157K) and Young Adults as top revenue drivers. Key insights: 2,518 repeat buyers are non-subscribers—a prime conversion target. Strategy focuses on optimizing margins (reviewing 50% discounts on items like Hat) and targeted marketing to high-value segments like Express shipping users.
# 🛒 Customer Shopping Behavior Analysis

## 🌟 Project Overview

This project provides a comprehensive analysis of customer shopping behavior using transactional data. The goal was to uncover key insights into spending habits, loyalty segments, and product preferences to inform data-driven strategies for marketing and operations.

The analysis pipeline spanned from initial data cleaning and feature engineering in **Python** to structured querying in **SQL** and final visualization in **Power BI**.

---

## 💾 Dataset

* **Source:** Synthetic Transactional Data (3,900 Purchases)
* **Size:** 3,900 rows, 18 initial columns
* **Key Data Points:** Customer Demographics (**Age, Gender**), Purchase Details (**Purchase Amount, Category, Item Purchased**), and Behavioral Metrics (**Subscription Status, Discount Applied, Previous Purchases, Review Rating**).

---

## 🛠️ Tools and Technologies

| Category | Tool / Language | Purpose |
| :--- | :--- | :--- |
| **Data Processing** | Python (Pandas, NumPy) | Data cleaning, EDA, Feature Engineering |
| **Database** | MySQL / PostgreSQL | Structured data storage and complex querying |
| **Reporting** | Power BI | Interactive dashboard creation and visualization |
| **Presentation** | Gamma | Final report and presentation deck generation |

---

## 🚀 Key Steps and Methodology

1.  **Exploratory Data Analysis (EDA):** Initial inspection of the dataset structure and identification of 37 missing values in `Review Rating`.
2.  **Data Cleaning & Preprocessing:**
    * Missing values were imputed using the **median rating per product category**.
    * Column names were standardized (snake\_case).
    * Redundant column (`Promo Code Used`) was dropped.
3.  **Feature Engineering:** Created **`age_group`** (binned data) and **`purchase_freq_days`** columns for deeper segmentation.
4.  **Database Integration:** Cleaned data was loaded into a **MySQL/PostgreSQL** database.
5.  **SQL Analysis:** Executed queries to calculate revenue by gender/age, identify top-rated products, and classify customers into **Loyal/Returning/New** segments.
6.  **Visualization:** Designed and developed a dynamic **Power BI Dashboard** for presenting insights.

---

## 💡 Key Results & Business Insights

* **Revenue Driver:** **Male customers** contributed the highest total revenue (\$157K). The **Young Adult** age group was the highest-spending segment.
* **Conversion Opportunity:** The majority of **repeat buyers (2,518)** are not subscribed, presenting a clear target for high-priority subscription conversion campaigns.
* **Profitability Check:** Products like **Hat** had a significant **50% discount rate**, indicating a need to review pricing strategy for margin protection.
* **High-Value Segment:** Users opting for **Express Shipping** showed a higher average purchase amount, suggesting an opportunity for shipping-based upsells.

---

## 🖼️ Dashboard Preview

<img width="735" height="458" alt="image" src="https://github.com/user-attachments/assets/8757220f-4977-4772-accb-e897d9c03b08" />
---

## ⚙️ How to Run

1.  **Clone the Repository:**
    URL :https://github.com/Ramthu-info/Customer_Shopping_Behaviour_analysis
    ```
2.  **Run the Python Notebook:** Execute the `Customer_sales_data.ipynb` notebook to clean the data and load it into your local MySQL/PostgreSQL instance.
3.  **Connect Power BI:** Open the Power BI file and ensure the data source connection is correctly pointing to your local database.
4.  **Review SQL Queries:** All analytical SQL scripts are available in the repository for review.
