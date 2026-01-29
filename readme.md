# BLINKIT SALES ANALYSIS

## Project Overview

* This project is an end-to-end data pipeline that transforms raw retail data into actionable insights. It covers the complete workflow from ETL (Extract, Transform,   Load) using Python to Database Management in MySQL and interactive dashboarding using Power BI.

## Tech Stack

* Language: Python 
* Database: MySQL 8.0 (Command Line Client)
* Libraries: PyMySQL, Pandas, NumPy
* Visualization: Power BI Desktop & Power BI Mobile Service

### Library Uses
* Pandas: Used for the core ETL process cleaning the raw Excel data and handling missing values.
* NumPy: Supported Pandas in performing mathematical operations like calculating the mean for imputation.
​* Openpyxl: The engine required to allow Python to read and extract data from the .xlsx source file.
​* PyMySQL: The database connector used to bridge Python with the MySQL 8.0 Command Line Client for data storage.

## Workflow
* Raw data ingestion from Excel
* Data cleaning and transformation using Python
* Structured data storage in MySQL
* Interactive dashboard creation in Power BI

### Data Preprocessing (Python)
* Handled missing values by filling NaNs with mean values.
* Corrected mismatched data types for accurate calculations.
* Structured and split data into logical segments:
 - Items
 - Outlets
 - Sales

### Database Management (DBMS)

* Automated the transfer of cleaned DataFrames into a MySQL database using PyMySQL.
* Ensured data integrity to support future CRUD operations and scalability.

### Data Visualization (Power BI)

* Developed a dynamic dashboard to track:
 - Total Sales 
 - Average Sales
 - No of Items
 - Average Ratings
* Analyzed sales distribution by:
 - Item Type
 - Fat Content
* Evaluated outlet performance based on:
 - Size
 - Location
 - Type
* Optimized the report for Power BI Mobile Service for on-the-go tracking.

## Key Insights

* Fruits and Snacks contribute the highest share of total sales.
* Tier 3 outlet locations generate the highest sales despite having fewer outlets. 
* Regular-fat products slightly outperform low-fat alternatives in overall sales.
* Supermarket Type 1 outlets show stronger performance compared to other outlet types.
* Outlets established in 2018 recorded the highest total sales, marking it as the peak-performing establishment year.
* Meat and Canned items received the highest average customer ratings, indicating strong customer satisfaction in these categories.
* Bread products showed comparatively lower average ratings, suggesting potential quality or preference gaps

## Images

![Dashboard Screenshot](images/ Powerbi_DashBoard_overView.JPG)
![Mobile Service Report Screenshot](images/ Powerbi_Mobile_Report.jpeg)
![MySQL CLC Screenshot](images/ MySQL_overView.JPG)


## Challenges & Solutions

* MySQL service stopping during development 
 - Manually managed the MySQL service to ensure stable database connections. 
* Handling missing and inconsistent data 
 - Applied data cleaning and standardization using Pandas. 
* Performance issues while inserting large datasets 
 - Used batch inserts with PyMySQL to improve efficiency.
* Power BI color and visual consistency 
 - Avoided random or extreme colors and aligned the dashboard theme with the Blinkit app for better UX. 
* Button links not working in edit mode 
 - Validated functionality after publishing in Power BI Service (read mode).

## CONCLUSION

* This project showcases an end-to-end data analytics workflow using Python, MySQL, and Power BI. It transforms raw retail data into structured insights through data cleaning, database management, and interactive visualization. The project reflects real-world problem solving and delivers meaningful business insights through a scalable and well-structured pipeline.

# Last Updated : JAN 2026

 