# Databases-and-MySQL-project-repository

# 🗄️ SQL Data Analysis Project 

## 📘 Overview
This project was completed during a **Data Technician Bootcamp**, focusing on developing core **SQL querying and data analysis skills**.

Using the **Northwind (retail/sales)** and **World (global demographics)** databases, the project demonstrates how to extract, transform, and analyse data to generate actionable insights for business and research scenarios.

---

## 🧰 Skills & Tools Used

### 💻 SQL & Database Skills
- Writing queries using:
  - `SELECT` – retrieving relevant data
  - `WHERE` – filtering records based on conditions
  - `ORDER BY` – sorting results
  - `GROUP BY` – aggregating and summarising data
- Performing **table JOINs**:
  - INNER JOIN
  - LEFT JOIN
  - RIGHT JOIN
- Combining data from multiple tables for reporting and analysis 

---

### 🔍 Data Analysis Skills 
- Data Extraction & Querying
- Data Cleaning & Filtering
- Aggregations & Grouping
- Relational Database Analysis
- Business Intelligence (BI)
- Data Exploration (EDA)
- Sales & Performance Analysis
- Query Optimisation (basic)

---

## 📊 Datasets Used

### 🛒 Northwind Database (Retail & Sales)
- Customers, Orders, Products, Suppliers, Categories
- Used to analyse:
  - Product performance
  - Customer behaviour
  - Order trends and sales data


### 🌍 World Database (Global Insights)
- Countries, Cities, Population, Life Expectancy
- Used to analyse:
  - Population trends
  - Urban distribution
  - Global demographics
 -  <img width="477" height="534" alt="image" src="https://github.com/user-attachments/assets/57d6379f-4a26-4baf-bd52-11999b6f0495" />
- <img width="452" height="324" alt="image" src="https://github.com/user-attachments/assets/c3b26551-50f3-43ed-9f3a-a0308d96dae5" />



---

## 🔍 Project Analysis

### 📌 Retail & Sales Insights (Northwind)
- Retrieved **customer and order data** using `SELECT` queries  
- Filtered **high-value products and targeted customers** using `WHERE`  
- Sorted data to analyse **recent orders and pricing trends** using `ORDER BY`  
- Combined tables (Customers, Orders, Products) using **JOINs** to create complete reports  
- Aggregated data using `GROUP BY` to calculate:
  - Number of products per category
  - Sales volume and product demand   

---

### 📌 Global Data Insights (World Database)
- Analysed **population distribution across cities and countries**
- Identified:
  - Most populated cities
  - Countries with highest life expectancy
- Used filtering and aggregation techniques to:
  - Compare demographic trends
  - Extract meaningful global insights  

---

## Queries :

- Select population, name FROM city ORDER BY population DESC LIMIT 10;

- Select name, lifeexpectancy FROM country ORDER BY lifeexpectancy DESC LIMIT 1;

- Filtering :
  select population, name FROM city WHERE population > 2000000;

- COUNT :
  Select count(*) AS total_number_of_cities FROM city WHERE countrycode = 'USA';

- LIKE Operator:
  Select name, countrycode FROM city WHERE name LIKE '%New%;

- JOIN:
  Select city.name, country.name, continent from city join country  on city.countrycode = country.code where continent = 'Europe'; 

- WHERE Clause:
  select ci.name as city, co.name as country, continent from city as ci join country as co on ci.countrycode = co.code where continent =    "Europe";

- GROUP BY:
 Select name, count(name) as frequency from city group by name order by frequency  asc , name asc; 

- OFFSET:
  Select name, population FROM city ORDER BY population DESC LIMIT 10 OFFSET 30;


