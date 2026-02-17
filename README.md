# 🎬 Netflix Movies & TV Shows Data Analysis using SQL
![(logo.png)](https://github.com/Sakshi-Gaur01/netflix_sql_project/blob/b495488fca7bab170480238df9e09d5cca874be3/logo.png)

## 📌 Project Overview
This project presents a comprehensive data analysis of Netflix Movies and TV Shows using SQL (PostgreSQL).  
The objective is to extract meaningful business insights from the Netflix dataset by solving real-world analytical business problems using advanced SQL queries.

The analysis includes content distribution, ratings analysis, country-wise trends, genre insights, and content categorization.

---

## 🎯 Objectives
- Analyze the distribution of content types (Movies vs TV Shows)
- Identify the most common ratings for each content type
- Analyze content based on release year, country, and duration
- Extract genre-based and keyword-based insights
- Solve real-world business problems using SQL

---

## 🛠️ Tools & Technologies Used
- PostgreSQL (pgAdmin 4)
- SQL (CTE, Window Functions, Aggregations, Subqueries)
- Kaggle Netflix Dataset
- Data Cleaning & Transformation using SQL

---

## 📂 Dataset
- Source: Kaggle Netflix Movies and TV Shows Dataset  
- File Used: [netflix_titles](https://github.com/Sakshi-Gaur01/netflix_sql_project/blob/661105a3c32d55ccabf4758a2b8f921097fa4497/netflix_titles.csv)

The dataset contains information about:
- Movies and TV Shows
- Directors & Cast
- Country
- Release Year
- Rating
- Duration
- Genre (listed_in)
- Description

---

## 🧱 Database Schema
```sql
DROP TABLE IF EXISTS netflix;

CREATE TABLE netflix (
    show_id VARCHAR(5),
    type VARCHAR(10),
    title VARCHAR(250),
    director VARCHAR(550),
    casts VARCHAR(1050),
    country VARCHAR(550),
    date_added VARCHAR(55),
    release_year INT,
    rating VARCHAR(15),
    duration VARCHAR(15),
    listed_in VARCHAR(250),
    description VARCHAR(550)
);

