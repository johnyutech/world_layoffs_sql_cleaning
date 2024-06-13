# Data Cleaning README

## Overview
This SQL script is designed to clean the layoffs data to ensure accuracy, consistency, and completeness. The cleaning process includes removing duplicates, standardizing data, handling null or blank values, and removing unnecessary columns.

## Steps

### Remove Duplicates:
- Identify and remove duplicate rows based on specific columns.
- Use `ROW_NUMBER()` to assign a unique identifier to duplicate rows.
- Delete rows with duplicate values.

### Standardize Data:
- Trim whitespace from the `company` column.
- Standardize industry names, such as combining variations of "Crypto" into a single category.
- Standardize country names, such as removing trailing periods from "United States".

### Handle Null or Blank Values:
- Identify and handle null or blank values in key columns.
- Fill missing industry values by matching other columns.
- Remove rows with null or blank values that are critical for analysis.

### Remove Unnecessary Columns/Rows:
- Identify and remove columns that are not needed for further analysis.
- Delete rows with critical null values.
