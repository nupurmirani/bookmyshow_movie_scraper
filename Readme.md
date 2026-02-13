# 🎬 BookMyShow Movie Data Scraper & ETL Pipeline

An end-to-end data pipeline built using Python that automates movie data extraction from BookMyShow, performs data transformation, and stores structured results in a MySQL database.

This project demonstrates practical experience in **web automation, data engineering, database design, logging, and ETL pipeline development**.

---

## 🚀 Project Overview

This application:

* Automates browser interaction using Selenium
* Extracts live movie listings from BookMyShow
* Parses and structures semi-structured web data
* Cleans and transforms data using Pandas
* Automatically creates and manages a MySQL database
* Inserts structured records into a relational schema
* Logs execution details for monitoring and debugging

The pipeline runs from **data extraction → transformation → database storage** in a single automated workflow.

---

## 🛠️ Technology Stack

* **Python**
* **Selenium** – Dynamic web scraping & browser automation
* **Pandas** – Data transformation and cleaning
* **MySQL** – Relational database storage
* **SQLAlchemy** – Database connectivity and ORM interface
* **webdriver-manager** – Automated ChromeDriver management
* **Python Logging Module** – Structured execution logging

---

## 🗄️ Database Schema

The script ensures automatic database and table creation with the following structure:

| Column     | Type     | Description               |
| ---------- | -------- | ------------------------- |
| id         | INT (PK) | Auto-increment identifier |
| city       | VARCHAR  | City of scraping          |
| movie_name | VARCHAR  | Movie title               |
| language   | VARCHAR  | Movie language            |
| format     | VARCHAR  | 2D / 3D / IMAX            |
| rating     | VARCHAR  | Rating or classification  |
| scraped_at | DATETIME | Timestamp of extraction   |

---

## 🔄 Data Processing & Transformation

The pipeline includes:

* Extraction of movie title from dynamic elements
* Intelligent parsing of rating and language fields
* Detection of format types (2D / 3D / IMAX)
* Handling edge cases (e.g., multi-language labels)
* Cleaning missing or malformed values
* Standardizing data before database insertion

---

## 📄 Logging & Reliability

All operations are logged to:

```
bms_scraper.log
```

Logs include:

* Script initialization and completion
* Database creation checks
* Number of movies scraped
* Per-movie extraction tracking
* Warning and exception handling

This ensures traceability and debugging capability similar to production systems.

---

## 🎯 Key Engineering Concepts Demonstrated

* Web scraping of dynamic content
* Automation of browser actions
* Data cleaning & preprocessing
* Relational database schema design
* ETL workflow implementation
* Error handling & logging best practices
* End-to-end pipeline development

---

## 🔮 Potential Enhancements

* Parameterized city input via CLI
* Scheduling using cron or task scheduler
* Docker containerization
* Cloud deployment (AWS / GCP)
* Historical data tracking & analytics dashboard
* API wrapper for serving data

---

## ⚠️ Disclaimer

This project is intended for educational purposes only. Please ensure compliance with BookMyShow’s terms of service before scraping.
