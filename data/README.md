
# Data Directory

This directory contains the datasets used in the Customer Churn Prediction project.

## 1. Raw Data

Location: `data/raw/`

File: `Telco-Customer-Churn.csv`

Description:
The original IBM Telco Customer Churn dataset downloaded from the public IBM repository.

Rules:
- Keep the original dataset unchanged.
- Do not perform data cleaning directly on this file.
- Preserve it as the source for all analysis.

Source:
https://github.com/IBM/telco-customer-churn-on-icp4d

## 2. Processed Data

Location: `data/processed/`

This folder will contain cleaned and transformed datasets created during the data preparation stage.

These files will be generated from the original raw dataset.

## 3. Data Management

Raw and processed datasets are excluded from Git using `.gitignore`.

This keeps the GitHub repository lightweight while maintaining the project code and documentation.

## 4. Cleaned Dataset

Location: `data/processed/`

File: `telco_churn_cleaned.csv`

Description:
The cleaned version of the IBM Telco Customer Churn dataset.

Cleaning performed:
- Converted TotalCharges to numeric.
- Filled 11 missing TotalCharges values for zero-tenure customers with 0.0.
- Preserved all 7,043 customer records.
- Preserved the original raw dataset.

Validation:
- 7,043 rows
- 21 columns
- No missing values
- No duplicate records
