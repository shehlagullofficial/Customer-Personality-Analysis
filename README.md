# Customer Personality Analysis (RFM Segmentation & Marketing Insights)

## 📌 Project Overview
This project focuses on performing a comprehensive **Customer Personality Analysis** to help a business understand its ideal customer profiles. By analyzing historical data across demographics, purchasing behavior, family structures, and campaign histories, this project seeks to replace generic marketing initiatives with targeted, data-driven strategies that optimize engagement and drive revenue growth.

Through detailed exploratory data analysis (EDA), feature engineering, and **RFM (Recency, Frequency, Monetary) Segmentation**, over 2,200 customers are categorized into actionable groups to optimize marketing performance and maximize resource efficiency.

---

## ❓ Business Questions Addressed
1. **High-Value Customers:** Who are our most valuable customers, and what factors drive their high spending?
2. **Campaign Effectiveness:** Which marketing campaigns generated the highest acceptance and conversion rates?
3. **Channel Performance:** In which sales channels (Web, Catalog, Store, or Discounts) should the company invest more heavily?
4. **Impact of Household Structure:** Do customers with children or teenagers behave differently compared to those without?
5. **Product Contribution:** Which product categories generate the most revenue, and which specific customer cohorts purchase them?

---

## 📊 Dataset Structure & Key Variables
The dataset consists of **2,240 records** containing customer profiles with 29 underlying features:

### 🌐 Key Variable Groups:
* **Demographics:** `Age` (derived from `Year_Birth`), `Education`, `Marital_Status`, `Income`.
* **Household Structure:** `Kidhome`, `Teenhome` (combined into structural types).
* **Engagement & Activity:** `Dt_Customer` (enrollment date), `Recency` (days since last purchase).
* **Product Spending:** Amount spent on `Wines`, `Fruits`, `MeatProducts`, `FishProducts`, `SweetProducts`, and `GoldProds`.
* **Sales Channels:** Number of purchases via `Web`, `Catalog`, `Store`, and `NumDealsPurchases`.
* **Campaign History:** Acceptance indicators for campaigns 1 through 5 (`AcceptedCmp1–5`) and the latest marketing `Response`.

---

## 🛠️ Technical Toolkit & Libraries
The analysis was implemented entirely using Python inside a Jupyter Notebook environment, utilizing the following core stack:
* **Data Manipulation:** `pandas`, `numpy`
* **Static Data Visualization:** `seaborn`, `matplotlib`
* **Interactive Data Exploration:** `plotly.express`

---

## 🔄 Project Workflow & Roadmap

### 1. Data Cleaning & Handling Nulls
* Evaluated missing values (e.g., handling missing `Income` records).
* Assessed data shapes, data types, and filtered structural redundancies.

### 2. Feature Engineering
* Calculated precise customer age from `Year_Birth`.
* Aggregated individual product column values to establish a comprehensive `Total Spending` metric.
* Consolidated `Kidhome` and `Teenhome` to understand broader family behavior patterns.

### 3. Exploratory Data Analysis (EDA)
* Identified distributions, anomalies, and structural correlations across demographics and monetary outputs.
* Explored correlations between household income levels and categorical campaign acceptance.

### 4. RFM Segmentation Framework
* Engineered **Recency** (days since last transaction), **Frequency** (total purchase volume across channels), and **Monetary** (aggregate spending) scores to segment the database into high-value, active, slipping, or inactive cohorts.

---

## 📈 Key Findings & Strategic Insights

| Feature Category | Insights & Visual Discoveries | Strategic Impact |
| :--- | :--- | :--- |
| **Top Revenue Drivers** | Wines and meat products generated the absolute highest spending among premium customers. | Allocate larger budget portions toward cross-promoting and premium packaging for high-margin products. |
| **Education & Income** | High-income levels and advanced educational background strongly correlate with increased spending and campaign acceptance. | Focus premium marketing channels explicitly on responsive, high-income socioeconomic brackets. |
| **Household Impact** | Customers without children display significantly higher purchasing capacity and frequency than those with children. | Tailor targeted messaging: promote bulk/discounted family packs to households and premium experiences to child-free segments. |
| **Campaign Optimization** | Varying acceptance patterns across segments prove that a single, generic campaign framework fails to convert optimally. | Implement continuous A/B testing on smaller audiences before rolling out capital-intensive campaigns. |

---

## 🚀 How to Run the Project
1. Clone this repository to your local machine:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
