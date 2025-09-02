# 📊 Credit Card Financial Dashboard

This project provides a **Credit Card Financial Dashboard** built using **Power BI**, with data sourced from CSV files and imported into **PostgreSQL** using SQL scripts.  
It delivers **customer insights, transaction analysis, and weekly financial performance tracking** for stakeholders to make data-driven decisions.

---

## 🚀 Project Objective
To develop a **comprehensive credit card weekly dashboard** that provides **real-time insights** into key performance metrics and trends, enabling stakeholders to monitor and analyze credit card operations effectively:contentReference[oaicite:0]{index=0}.

---

## Dashbaord Report <img width="1355" height="763" alt="Dashboard Report" src="https://github.com/user-attachments/assets/95182a03-60af-4a59-ab82-81caa665aa04" />


## 📂 Dataset Information
The project uses multiple CSV datasets:

- **credit_card.csv** → Credit card transaction details  
- **customer.csv** → Customer demographic details  
- **cc_add.csv** → Additional weekly credit card transaction data  
- **cust_add.csv** → Additional weekly customer data  

These datasets are processed and loaded into a **PostgreSQL database** before being visualized in **Power BI**.

---

## 🛠️ SQL Setup
Use the provided SQL script [`SQL Query - Financial Dashboard Data.sql`](./SQL%20Query%20-%20Financial%20Dashboard%20Data.sql) to create tables and import data into PostgreSQL.

### Steps:
1. Create database:
   ```sql
   CREATE DATABASE ccdb;
2. Create tables
3. Import CSVs using:
   ```sql
   COPY cc_detail FROM 'D:\credit_card.csv' DELIMITER ',' CSV HEADER;
   COPY cust_detail FROM 'D:\customer.csv' DELIMITER ',' CSV HEADER;
4. mport additional week data (cc_add.csv, cust_add.csv).

---

## Transaction Dashboard
- **Revenue by Expenditure Type**: Bills, Entertainment, Fuel, Grocery, Food, Travel  
- **Card Category Performance**:
  - Blue: **46.2M Revenue**  
  - Silver: **5.6M Revenue**  
  - Gold: **2.4M Revenue**  
  - Platinum: **1.1M Revenue**  
- **Quarterly Trends**:
  - Q1: **14.0M**  
  - Q2: **13.8M**  
  - Q3: **14.2M**  
  - Q4: **13.4M**  
- **Payment Channels**:
  - Swipe: **35M**  
  - Chip: **17M**  
  - Online: **3M**

---

##  Weekly Dashboard Report
- **YTD Overview**:
  - Revenue: **57M**  
  - Total Interest: **8M**  
  - Transaction Amount: **46M**  
  - Male Revenue: **31M**, Female Revenue: **26M**  
  - Blue & Silver cards: **93% of overall transactions**  
  - Top States: **TX, NY, CA → 68% contribution**  
  - Activation Rate: **57.5%**  
  - Delinquent Rate: **6.06%**  

- **WoW (Week 53 - Dec 31)**:
  - Revenue ↑ **28.8%**  
  - Transactions & customer count **increased**  

---

## ⚙️ Tech Stack
- **Database**: PostgreSQL  
- **Data Source**: CSV files (`credit_card.csv`, `customer.csv`, etc.)  
- **Visualization**: Power BI (Dashboards)  
- **Languages/Tools**: SQL, DAX  

---

