# SQL Layoffs Data Cleaning & Exploratory Data Analysis

## Project Overview

This project focuses on cleaning and analyzing layoffs data using MySQL. The objective is to transform raw layoffs data into a clean and analysis-ready dataset and explore meaningful patterns and trends using SQL.

The project demonstrates practical skills in data cleaning, data preparation, exploratory data analysis, aggregation, Common Table Expressions (CTEs), joins, and window functions.

## Tools & Technologies

* MySQL
* SQL
* Data Cleaning
* Data Preparation
* Exploratory Data Analysis
* CTEs
* Window Functions
* Aggregate Functions
* Data Transformation

## Dataset Description

The dataset contains information about company layoffs and includes:

* Company
* Location
* Industry
* Total Laid Off
* Percentage Laid Off
* Date
* Company Stage
* Country
* Funds Raised in Millions

## Project Workflow

### 1. Data Preparation

Prepared the layoffs dataset and created staging tables to perform the cleaning process while preserving the original data.

### 2. Data Cleaning

Cleaned and standardized the dataset by:

* Identifying and removing duplicate records
* Standardizing company names
* Standardizing industry values
* Cleaning country names
* Converting date values into the appropriate date format
* Handling NULL and blank values
* Filling missing industry values where possible
* Removing records where both total layoffs and percentage layoffs were unavailable
* Removing temporary columns used during the cleaning process

### 3. Exploratory Data Analysis

Performed exploratory analysis on the cleaned dataset to identify patterns and trends in layoffs.

The analysis includes layoffs by:

* Company
* Industry
* Country
* Year
* Month
* Company Stage
* Average layoffs
* Percentage of workforce laid off

### 4. Advanced SQL Analysis

Used CTEs and window functions to perform more advanced analysis, including:

* Monthly layoffs
* Rolling total of layoffs
* Company layoffs by year
* Ranking companies by yearly layoffs
* Identifying the top 5 companies by layoffs for each year

## Analysis Areas

The project explores layoffs based on:

* Company
* Industry
* Country
* Year
* Month
* Company Stage
* Total Layoffs
* Average Layoffs
* Percentage Laid Off
* Company Layoffs by Year
* Rolling Total
* Yearly Company Rankings

## Project Files

| **File**                        | **Description**                                           |
| ------------------------------- | --------------------------------------------------------- |
| `data_cleaning.sql`             | SQL queries used to clean and prepare the layoffs dataset |
| `exploratory_data_analysis.sql` | SQL queries used to perform exploratory data analysis     |
| `README.md`                     | Project documentation                                     |
| `data/layoffs.csv`              | Raw layoffs dataset                                       |

## SQL Concepts Used

This project demonstrates the following SQL concepts:

* SELECT
* WHERE
* GROUP BY
* ORDER BY
* UPDATE
* DELETE
* ALTER TABLE
* JOIN
* Common Table Expressions (CTEs)
* ROW_NUMBER()
* DENSE_RANK()
* Window Functions
* Aggregate Functions
* String Functions
* Date Functions
* TRIM()
* STR_TO_DATE()
* YEAR()
* SUBSTRING()

## Data Cleaning

The data cleaning process begins by creating staging tables to work with the layoffs data.

Duplicate records are identified using `ROW_NUMBER()` and partitioning across relevant columns.

The project also standardizes company names, industry values, country names, and date values.

NULL and blank values are investigated and handled where appropriate. Missing industry values are populated by comparing records belonging to the same company.

Records where both `total_laid_off` and `percentage_laid_off` are unavailable are removed from the cleaned dataset.

## Exploratory Data Analysis

The exploratory analysis examines total layoffs across companies, industries, countries, years, and company stages.

The analysis also calculates:

* Maximum total layoffs
* Maximum percentage laid off
* Total layoffs by company
* Total layoffs by industry
* Total layoffs by country
* Total layoffs by year
* Total layoffs by company stage
* Average layoffs by company
* Monthly layoffs
* Rolling total of layoffs
* Company layoffs by year

 ## Advanced Analysis

A rolling total is calculated using a window function to understand the cumulative number of layoffs over time.

Company rankings are also calculated using DENSE_RANK() to identify the top 5 companies by total layoffs for each year.

## Project Objective

To transform raw layoffs data into a clean and analysis-ready dataset and use SQL to explore patterns and trends in company layoffs.

## Key Skills Demonstrated
* SQL Data Cleaning
* Data Transformation
* Exploratory Data Analysis
* Data Quality Management
* Aggregate Functions
* CTEs
* Window Functions
* Ranking
* Date Analysis
* String Manipulation
* Joins
* Business Data Analysis

## Author

Shruti Ajit Khurpe

