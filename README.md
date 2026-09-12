# [Project Title: SALES OPERATION ANALYSIS]

<!-- Add a project banner image or relevant dashboard screenshot here to capture attention -->
![Project Banner](path/to/banner_or_dashboard.png)

## 📊 Project Overview
ANALYSED 2022 RETAIL SALES DATA USING PIVOT TABLES AND CHARTS TO UNCOVER REVENUE TRENDS, CUSTOMER BEHAVIOUR, AND CHANNEL PERFORMANCE ACROSS MULTIPLE INDIAN STATES AND E-COMMERCE PLATFORMS. 

* **Objective:** To identify key drivers of customer churn and provide actionable recommendations to increase retention by 5%.
* **Tools Used:** MICROSOFT EXCEL | DOMAIN: RETAIL & E-COMMERCE
* **Key Insight:** DECEMBER DROVE THE HIGHEST SALES; MAHARASHTRA LED ALL STATES AT ₹2.99M FEMALE CUSTOMERS WERE THE DOMINANT BUYER DEMOGRAPHIC (32% VS 18% MALE) AMAZON ACCOUNTED FOR ~50% OF ALL ORDERS WITH A 92% DELIVERY
SUCCESS RATE

---

## ❓ Business Problem
What real-world problem initiated this project? Frame this from a business perspective rather than a technical one.
> "The marketing team noticed a steady decline in repeat purchases over the last three quarters. Without understanding why customers are leaving, budget is being wasted on generic acquisition campaigns instead of targeted retention efforts."

---

## 🗃️ Data Source & Inspection
Describe the data you used so anyone viewing the repository can understand its structure before opening the files.

* **Source:** Internal company transactional database / [Kaggle Dataset Link]([https://example.com](https://docs.google.com/spreadsheets/d/1QyWZMIV9GU5P6JnXCnGEGcKz0n-0ko-q/edit?usp=drivesdk&ouid=109050833589201869730&rtpof=true&sd=true))
* **Dataset Size:** 19 tables, 31,000+ rows spanning January 2025 to June 2026.
* **Database Schema:** 
  ![Schema Diagram](path/to/schema_image.png)
* **Recommendation:** PRIORITISE FESTIVE SEASON CAMPAIGNS AND FEMALE-FOCUSED MARKETING STRENGTHEN TOP-PERFORMING STATES AND DIVERSIFY BEYOND AMAZON DEPENDENCY

---

## 🛠️ Data Cleaning & Transformation
Outline the steps you took to prepare the data for analysis. This proves your attention to data integrity.

1. **Handling Missing Values:** Replaced missing `Discount_Code` nulls with 'None' and dropped rows with missing `Customer_ID`.
2. **Data Consistency:** Standardized date formats using `YYYY-MM-DD` and converted `Total_Amount` to a float data type.
3. **Outlier Removal:** Filtered out negative transaction amounts caused by system testing errors.

```sql
-- Example SQL snippet used during cleaning/joining
SELECT 
    customer_id,
    COUNT(order_id) AS total_orders,
    SUM(total_amount) AS total_spent
FROM sales_data
WHERE order_status = 'Completed'
GROUP BY customer_id;
```

---

## 📈 Exploratory Data Analysis (EDA) & Insights
Present your findings clearly. Use visual anchors like bullet points and embed charts directly into the text.

### 1. High Churn in Cohort Month 2
We found that **23% of users** who make a purchase do not return for a second purchase within 30 days. 
![Churn Chart](path/to/churn_chart.png)

### 2. Disproportionate Revenue from Premium Members
While Premium Members only make up **15% of the user base**, they generate **45% of total revenue**. Nurturing this segment is critical.

---

## 🖥️ Dashboard / Visualization
If your project includes a dashboard (Power BI, Tableau, Looker Studio), add a prominent screenshot here along with an interactive link.

[![Tableau Dashboard Screenshot](path/to/dashboard_screenshot.png)](https://tableau.com)
*Click the image above to view the interactive dashboard.*

---

## 💡 Recommendations & Actionable Insights
What should the business actually *do* with your findings? 

* **Implement a Month-2 Lifecycle Email:** Trigger an automated 15% discount code exactly 45 days after a user's first purchase to combat the Month-2 drop-off.
* **VIP Loyalty Program:** Create an exclusive tier for the top 15% spending customers to maintain their high lifetime value.
* **Fix the Checkout Bug:** Work with the engineering team to fix the high abandonment rate observed specifically on the Android mobile checkout screen.

---

## ⚠️ Challenges & Limitations
Demonstrate critical thinking by noting what could be improved or what constraints you faced.
* **Data Privacy:** PII (Personally Identifiable Information) was masked or removed prior to analysis.
* **Data Scope:** The dataset only contained digital transactions; offline retail store data was unavailable, which may limit the completeness of the customer profile.

---

## 📁 Repository Structure
```text
├── data/                  # Raw and cleaned data files (if size permits)
├── notebooks/             # Jupyter Notebooks for EDA and data cleaning
├── scripts/               # SQL queries or Python scripts
├── visuals/               # Charts, dashboard screenshots, and schema images
├── README.md              # Project documentation
```

---

## ✉️ Contact
* **Name:** KOLAWOLE AISHA
* **LinkedIn:** ([https://linkedin.com](https://www.linkedin.com/in/aisha-kolawole))
* **Email:** AishaDataAnalyst1@gmail.com
