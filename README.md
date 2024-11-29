# ISM6562 Final Project: Fraud Detection and Analysis

This notebook serves as the final project for ISM6562. It focuses on building a pipeline for fraud detection by loading, merging, and analyzing data from multiple sources, followed by conducting exploratory data analysis (EDA) and implementing machine learning models. The goal is to identify fraudulent transactions based on provided datasets.

---

## Project Structure

### 1. Load Data
- **Objective:** Import and preprocess datasets related to transactions, users, credit cards, and fraud labels.
- **Details:**
  - CSV files for `transactions`, `cards`, and `users` are loaded using PySpark.
  - A JSON file containing fraud labels is transformed into a structured format.
  - Preprocessing includes removing special characters (e.g., `$`) and casting string columns to numeric types.

### 2. Merge Data
- **Objective:** Combine all datasets into a single view for analysis and modeling.
- **Details:**
  - Joins are performed between transactions, cards, users, and fraud labels.
  - The merged dataset includes fields such as transaction amount, merchant location, card details, user demographics, and fraud status.

### 3. Exploratory Data Analysis (EDA)
- **Objective:** Explore the data to understand patterns, distributions, and potential anomalies.
- **Details:**
  - EDA visualizations and statistics are generated to analyze fraud trends and correlations with other features.

### 4. Model Development (Planned)
- **Objective:** Train machine learning models to predict fraudulent transactions.
- **Details:** The notebook lays the foundation for implementing classification models, but the details of the implementation are not covered here.

---

## Data Sources
1. **Transactions:** Details about financial transactions, including amounts, dates, and merchant locations.
2. **Cards:** Information about credit cards, including brand, type, and credit limits.
3. **Users:** Demographic information such as age and per capita income.
4. **Fraud Labels:** A JSON file mapping transactions to fraud outcomes.

---

## Setup Instructions
1. Clone or download the repository.
2. Place all necessary datasets in the appropriate file paths as referenced in the notebook:
   - `/FileStore/transactions_data.csv`
   - `/FileStore/cards_data.csv`
   - `/FileStore/users_data.csv`
   - `/FileStore/train_fraud_labels.json`
3. Ensure PySpark and necessary libraries (e.g., `pyspark.sql`) are installed in your environment.
4. Run the notebook sequentially to process data, merge it, and perform exploratory analysis.

---

## Technologies Used
- **Databricks:** For distributed data processing and analysis.
- **PySpark:** To handle large datasets and perform preprocessing.
- **SQL:** For merging datasets and creating a unified view.
- **Python:** For additional data manipulation.

---

## Outputs
- **Merged Dataset:** A consolidated view of all data sources, ready for analysis and modeling.
- **EDA Insights:** Foundational insights into the dataset and fraud trends.

---

## Author
This project was developed as part of the ISM6562 coursework.

---
