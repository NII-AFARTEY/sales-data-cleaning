# Sales Data Cleaning Project Using Python.

## Overview
This project focuses on a data cleaning pipeline for a messy 20,000-row and 12-column sales dataset. The project identifies and resolves common data quality issues, including duplicates, inconsistent formatting, mixed data types, and missing values. The aim was to transform the dataset into a structured, analysis-ready format using Python.

## Objectives
* Identify data quality issues in the dataset
* Handle missing values appropriately
* Remove duplicate records
* Standardize column names and formats
* Correct data types
* Clean inconsistent text values
* Remove invalid and outlier values
* Create new derived features
* Produce a clean dataset ready for analysis

## Data Description
1. order_ID: Customer unique identification
2. order_Date: Date a customer placed an order
3. Sales_Rep: Sales representative who handled the order
4. Region: The location of the order
5. Product: The Item being purchased
6. Category: The category of item being purchased
7. Channel: Platform on which the order was made
8. Quantity: The quantity of items being purchased
9. Unit_Price: The price per item
10. Discount_%: The percentage discount on each item
11. Currency: The currency used for the purchase of each item
12. Status: The status of each order

## Data Cleaning Steps

### 1. Data Inspection
* Profiled the data to get an overall knowledge and identify some discrepancies
* Checked dataset shape
* Examined data types
* Identified missing values
* Identified duplicate records

### 2. Removing Duplicates
* Removed duplicate rows

### 3. Converting Numeric Columns
* Removed trailing percentage sign (%) from "Discount_%" column
* Converted numeric data types to float
* Got rid of negative and suspicious values

### 4. Standardizing Column Names
* Converted Currency codes into upper-case
* Converted all string fields into title case 
* Removed leading and trailing whitespaces

### 5. Handling Missing Values
* Dropped rows missing critical identifiers
* Filled categorical variables with "Unknown."
* Imputed numeric values using the median

### 6. Inspection of unique data values
* Checked for the number of unique values to gain insight into which data entries have typos,
 inconsistent casing, and casing variants.

### 7. Removing Header leaks
* Removed all column names that appeared as values

### 8. Fixing Common Typos and Standardizing Categories
* Fixed all typos 
* Standardized capitalization
* Fixed inconsistent labels

### 9. Standardizing Date Format
* Converted date columns to datetime

### 10. Handling Missing Values
* Dropped rows missing critical values
* Filled categorical variables with "N.A"
* Imputed numeric values using the median

### 11. Validation Checks
* Performed a validation check for the data entries to ensure validity\

### 12. Profiling and checking the cleaned data
* Checked for information and profile of the dataset

### 13. Saved the data
* The dataset was saved as an Excel file

### 14. Summary
* Showed brief steps on how the cleaning was done
* Provided a table to compare the state of the dataset before the cleaning and after the cleaning

## Tools and Libraries
* Python
* Pandas
* NumPy
* Ydata profiling

## Project Structure
data-cleaning-project/
│

├── messy_sales_data.xlsx

├── Data_Cleaning.ipynb

├── cleaned_sales_data.csv

└── README.md

## Use Cases
This cleaned dataset can now be used for:
* Exploratory Data Analysis
* Sales performance analysis
* Customer segmentation
* Forecasting
* Machine learning models
* Dashboard creation
