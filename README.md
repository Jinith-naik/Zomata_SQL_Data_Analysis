# 🍽️ Zomato Data Exploration & Analysis – SQL Project

## 📌 Project Overview
This project showcases **end-to-end SQL-based data exploration and analysis** on the **Zomato Restaurants Dataset**.  
It demonstrates my ability to perform **data cleaning, transformation, and advanced analytical queries** to extract actionable business insights for the food & restaurant industry.

The dataset contains **9,000+ records** across multiple countries, with attributes like `RestaurantID`, `Name`, `City`, `Locality`, `Cuisines`, `Rating`, `Votes`, `Average Cost for Two`, and more.

---

## 🎯 Objectives
1. **Explore** the dataset to identify structural details, missing values, duplicates, and data inconsistencies.
2. **Clean & transform** the data to ensure accuracy and readiness for analysis.
3. **Analyze** restaurant trends, customer preferences, and service offerings.
4. **Generate insights** to support strategic decision-making in the restaurant and food delivery space.

---

## 🛠️ Tech Stack
- **Database:** SQL Server
- **Language:** T-SQL
- **Tools:** SQL Server Management Studio (SSMS), Windows Functions, Views, CTEs
- **Dataset:** Zomato Restaurants Data (`.csv`)

---

## 📂 Project Workflow

### **1. Data Exploration** ([ZOMATO_DATA_EXPLORATION.sql](ZOMATO_DATA_EXPLORATION.sql))
- Checked **column names, data types, and constraints**.
- Identified **duplicate records** using `GROUP BY` & `COUNT`.
- Removed **irrelevant rows** and **unwanted columns** (`Address`, `LocalityVerbose`, `Switch_to_order_menu`).
- Merged **country details** from a separate mapping table using `JOIN` & `UPDATE`.
- Fixed **misspelled city names** using `REPLACE` functions.
- Created **rolling/moving counts** of restaurants by city & locality.
- Calculated **min, max, avg** for key numerical fields: `Votes`, `Rating`, `Average_Cost_for_two`.
- Created a **rating category column** (`Poor`, `Good`, `Great`, `Excellent`) using `CASE WHEN`.

---

### **2. Data Analysis** ([ZOMATO_DATA_ANALYSIS.sql](ZOMATO_DATA_ANALYSIS.sql))
- **Market share by country:** Found that **India holds 90.67%** of restaurants in the dataset.
- **Online delivery penetration:** Only **28.01%** of Indian restaurants and **46.67%** of UAE restaurants offer online delivery.
- **Top restaurant localities:**  
  - Connaught Place, New Delhi → 122 restaurants  
  - Rajouri Garden → 99 restaurants  
  - Shahdara → 87 restaurants  
- **Popular cuisines:** In Connaught Place, **North Indian food** is the most common.
- **Table booking insights:**  
  - In Connaught Place, only 54/122 restaurants offer table booking.  
  - Restaurants with table booking average **3.9★**, vs **3.7★** without.
- **Best value pick:**  
  - *India Restaurant* (Kolkata, ID: 20747) — Offers **table booking + online delivery**, `rating > 4`, `votes > 1000`, cost for two `< ₹1000`, serves **Indian cuisine**.
- **Pricing insights:** Found the price range distribution for restaurants with `rating >= 4.5` that also offer table booking.

---

## 📊 Key Insights
- **India dominates** Zomato's dataset presence, showing potential for domestic market strategies.
- **Online delivery services** are still underutilized in many regions.
- **High-rated restaurants** often align with **moderate pricing** and **service options** like booking & delivery.
- **Cuisine preference** varies sharply by locality, with North Indian dominating prime locations.

---

## 📈 Skills Demonstrated
- Advanced **SQL joins, CTEs, and window functions**.
- **Data cleaning** & standardization techniques.
- **Aggregations & ranking** for business KPIs.
- **Creating and using views** for modular analysis.
- **Deriving actionable business insights** from raw data.

---

## 📁 Repository Structure
```
📦 Zomato-SQL-Analysis
┣ 📜 Zomato_Dataset.csv              # Raw dataset
┣ 📜 ZOMATO_DATA_EXPLORATION.sql     # Data cleaning & exploration queries
┣ 📜 ZOMATO_DATA_ANALYSIS.sql        # Data analysis queries & insights
┗ 📜 README.md                       # Project documentation
```

---

## 🚀 How to Run This Project
1. Download the dataset (`Zomato_Dataset.csv`) and SQL scripts.
2. Import the dataset into **SQL Server**.
3. Execute **ZOMATO_DATA_EXPLORATION.sql** for cleaning & preparation.
4. Execute **ZOMATO_DATA_ANALYSIS.sql** to generate insights.
5. Use **SSMS** or any SQL IDE for execution.

---

## 💡 Future Enhancements
- Create **interactive dashboards** using Power BI/Tableau.
- Build **predictive models** for restaurant ratings & pricing using Python.
- Integrate **geo-visualization** for locality-wise restaurant mapping.

---

## 📬 Contact
**Author:** Jinith Naik  
📧 Email: [jinithnaikcareer@gmail.com](mailto:jinithnaikcareer@gmail.com)  
💼 LinkedIn: [www.linkedin.com/in/jinithnaik](https://www.linkedin.com/in/jinithnaik)  
🌐 Portfolio: [https://jinith-naik.github.io/JinithNaik/](https://jinith-naik.github.io/JinithNaik/)

---
> *This project reflects my expertise in SQL-based data analysis, transforming raw data into meaningful business intelligence. Perfect for roles in Data Analytics, Business Intelligence, and Data Engineering.*
