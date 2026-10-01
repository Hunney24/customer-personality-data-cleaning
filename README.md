# Customer Personality Analysis – Data Cleaning & Preprocessing

## Project Overview

This project focuses on cleaning and preprocessing the Customer Personality Analysis dataset to improve data quality and prepare the dataset for further analysis.

The objective was to identify and handle missing values, duplicate records, inconsistent categorical values, date formats, column naming conventions, and data-type issues.

## Dataset

The dataset contains customer demographic information, purchasing behaviour, campaign responses, and customer activity information.

- Original records: 2,240
- Original columns: 29
- Final records: 2,240
- Final columns: 29

## Data Cleaning Performed

### 1. Missing Values

The `Income` column contained 24 missing values.

The missing values were replaced using the median income because median imputation is less affected by extreme values.

### 2. Duplicate Records

The dataset was checked for duplicate rows.

- Duplicate rows found: 0

### 3. Categorical Standardization

An inconsistent education label was identified:

`2n Cycle` → `2nd Cycle`

### 4. Date Formatting

The `Dt_Customer` column was converted from text format to a proper datetime format.

No invalid dates were found after conversion.

### 5. Numerical Data Validation

Numerical columns were checked for negative values.

No negative values were identified.

### 6. Binary Data Validation

The campaign response and complaint fields were checked to ensure that they contained valid binary values.

The relevant fields contained only `0` and `1`.

### 7. ID Validation

Customer IDs were checked for uniqueness.

- Total records: 2,240
- Unique IDs: 2,240

### 8. Column Name Standardization

Column names were standardized to lowercase format with underscores for consistency.

Examples:

`Year_Birth` → `year_birth`

`Marital_Status` → `marital_status`

`Dt_Customer` → `dt_customer`

## Final Data Quality

After preprocessing:

- Missing values: 0
- Duplicate rows: 0
- Invalid dates: 0
- Unique customer IDs: 2,240
- Dataset size: 2,240 × 29

## Tools Used

- Python
- Pandas
- Google Colab
- GitHub

## Conclusion

The dataset was successfully cleaned and validated. The resulting dataset has consistent column naming, standardized categorical values, properly formatted dates, no missing values, no duplicate rows, and validated numerical and binary fields.

The cleaned dataset is now ready for further exploratory data analysis and visualization.
