
# 🧠 Customer-Behavior-MySQL2Hive
*A Big Data Integration and Analytics Project using MySQL, Hive & Cloudera*

---

## 📘 Project Overview
The **Customer-Behavior-MySQL2Hive** project focuses on analyzing **e-commerce customer behavior** to understand purchasing patterns, satisfaction levels, and spending habits using **Big Data technologies**.  
It demonstrates how traditional databases like **MySQL** can be integrated with **Apache Hive** on a **Cloudera Hadoop environment** to efficiently handle and process large-scale datasets.  
By performing analytics in both MySQL and Hive, this project showcases the advantages of distributed processing for scalability, performance, and real-time insights.

---

## 🎯 Project Goals
1. **Analyze Customer Behavior Patterns** – Study spending, satisfaction, and engagement trends.  
2. **Integrate MySQL with Hive** – Enable seamless data migration using ETL.  
3. **Perform Comparative Analysis** – Compare SQL vs. HQL efficiency and scalability.  
4. **Identify Business Insights** – Find top spenders, active cities, and satisfaction correlations.  
5. **Implement ETL Process** – Demonstrate end-to-end data movement in Hadoop.  
6. **Enhance Decision-Making** – Support marketing and retention strategies through analytics.  
7. **Visualize Data** – Represent insights using charts for better interpretation.  
8. **Demonstrate Complete Big Data Workflow** – From ingestion to analysis and visualization.

---

## 🧩 Dataset Description
The dataset contains **e-commerce customer transaction data** with the following fields:

| Field Name | Description |
|-------------|-------------|
| Customer ID | Unique identifier for each customer |
| Gender | Male / Female |
| Age | Customer’s age |
| City | Customer location |
| Membership Type | Gold, Silver, or Bronze |
| Total Spend | Total amount spent by the customer |
| Items Purchased | Number of items bought |
| Average Rating | Product/service rating |
| Discount Applied | Whether discount was used |
| Days Since Last Purchase | Recency of last purchase |
| Satisfaction Level | Satisfied, Neutral, Unsatisfied |

**Purpose:** To understand customer segmentation, spending patterns, satisfaction distribution, and loyalty factors.

---

## ⚙️ Tools & Environment
### 🛠 Tools Used
- **MySQL** – Database for structured data storage & SQL analysis  
- **Apache Hive** – Big Data querying and analytics  
- **Cloudera** – Hadoop-based environment for Hive execution  
- **CSV Dataset** – Source file for importing data  
- **Command Line Interface (CLI)** – For Hive and MySQL commands  

### 💻 Environment Setup
- Cloudera VM running on Linux  
- MySQL database connected to Hive  
- Hive configured with MySQL as external source  

---

## 🧮 Analysis on MySQL
### 🔹 Steps:
1. **Login to MySQL and create database:**
   ```sql
   CREATE DATABASE project;
   USE project;
   ```
2. **Create and load table:**
   ```sql
   LOAD DATA INFILE 'path/customer_data.csv'
   INTO TABLE customer_data
   FIELDS TERMINATED BY ','
   LINES TERMINATED BY '\n'
   IGNORE 1 ROWS;
   ```
3. **Run SQL Queries:**
   - Total customers  
   - Average total spending  
   - City with highest spend  
   - Satisfaction distribution  
   - Top 3 high-value customers  
   - Average rating by gender  
   - Total revenue by membership type  
   - Customers using discounts & satisfaction levels  

---

## 🐝 Analysis on Hive
### 🔹 Steps:
1. **Load dataset from MySQL into Hive**  
2. **Create Hive table:**
   ```sql
   CREATE DATABASE project_hive;
   USE project_hive;
   CREATE TABLE customer_data (...);
   ```
3. **Perform HQL Queries:**  
   - Total customers  
   - Average total spending  
   - City with highest spend  
   - Customers by membership type  
   - Satisfaction level distribution  
   - Average rating by gender  
   - Top 3 high spenders  
   - Revenue by membership type  
   - Gender-based average spend  
   - Spend per item by membership  

---

## 📊 Key Insights
| Insight Area | Summary |
|---------------|----------|
| **Total Customers** | 10 sample records used for demonstration |
| **Average Spend** | ₹1,000 average spending per customer |
| **Top City** | San Francisco customers spend the most (~₹1,500+) |
| **Membership Type** | Gold members contribute over 60% of total revenue |
| **Satisfaction Levels** | High satisfaction among Gold members |
| **Gender Rating** | Females rate higher (avg 4.4) than males (avg 4.1) |
| **Top 3 Spenders** | Customers #110, #104, #107 (mostly metro cities) |
| **Discount Impact** | Discounts improve satisfaction among loyal members |
| **Days Since Purchase** | Satisfied customers buy again sooner (~18 days) |
| **Spending Pattern** | Males spend more per order; females shop more frequently |

---

## 📈 Data Visualization
Visualizations were created using **Python (Matplotlib / Seaborn)** and **Cloudera charts**:
- Bar Chart → Revenue by Membership Type  
- Pie Chart → Satisfaction Distribution  
- Scatter Plot → Spend vs. Rating  
- Line Chart → Purchase Recency Trends  

These visuals make analytical insights more interpretable and presentation-ready.

---

## 🚀 Project Workflow
```
📥 Dataset (CSV)
     ↓
🗄 MySQL (Data Storage & SQL Analysis)
     ↓
🔁 Data Transfer (ETL Process)
     ↓
🐝 Apache Hive (Big Data Analytics)
     ↓
📊 Visualization (Insights & Reporting)
```

---

## 🧑‍💻 Developed By
**Name:** Rajesh Chaurasiya  
**Course:** MCA in Data Science & Artificial Intelligence  
**Roll No:** 33  **University Roll No:** 1240259034  
**Faculty:** Mr. Harsh Gaur  

---

## 🌐 Repository Link
🔗 [GitHub Project Repository](https://github.com/Mr-Rajesh-108/Customer-Behavior-MySQL2Hive)
