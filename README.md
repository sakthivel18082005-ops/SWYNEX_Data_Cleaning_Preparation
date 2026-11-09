# SWYNEX – Data Cleaning and Preparation

## 1. Project Overview

This project focuses on cleaning and preparing a dataset using Python and Pandas in Google Colab.

The objective is to identify and handle missing values, duplicate records, inconsistent text values, and data types to prepare the dataset for further analysis.

## 2. Dataset Description

- **Dataset name:** Titanic Passenger Dataset
- **File name:** `titanic.csv`
- **Description:** Contains information about Titanic passengers, including passenger ID, survival status, passenger class, name, sex, age, family details, ticket, fare, cabin, and embarkation port.
- **Dataset source:** [https://www.kaggle.com/c/titanic/data?select=train.csv%2F&utm_source=chatgpt.com](https://www.kaggle.com/c/titanic/data?select=train.csv%2F\&utm_source=chatgpt.com)

## 3. Tools and Technologies

- Python
- Google Colab
- Pandas
- CSV

## 4. Data Quality Issues Identified

The initial dataset inspection found:

| Column   | Missing values |
| -------- | -------------: |
| Age      |            177 |
| Cabin    |            687 |
| Embarked |              2 |

The duplicate-row check found 0 exact duplicate rows.

## 5. Data Cleaning Process

1. **Load the dataset:** Imported the CSV file using Pandas.
2. **Inspect the dataset:** Checked the rows, columns, data types, and missing values.
3. **Remove duplicates:** Checked for and removed exact duplicate rows.
4. **Handle missing Age values:** Replaced missing values with the median Age.
5. **Handle missing Embarked values:** Replaced missing values with the most frequent Embarked value (mode).
6. **Handle Cabin values:** Created a `CabinKnown` column to indicate whether cabin information was available, then removed the original Cabin column because it contained many missing values.
7. **Clean text values:** Removed unnecessary leading and trailing spaces from text columns.
8. **Verify the cleaned dataset:** Checked missing values, duplicate rows, and data types again.

## 6. Output

The cleaned dataset is saved as:

`cleaned_dataset.csv`

The output file is prepared for further data analysis.

## 7. Conclusion

This project demonstrates the importance of data cleaning and preparation before performing data analysis or building machine learning models. Missing values, duplicate records, and text inconsistencies were reviewed and handled using Python and Pandas.

## 8. Author

**Name:** Sakthi Vel E

**Project:** SWYNEX – Data Cleaning and Preparation
