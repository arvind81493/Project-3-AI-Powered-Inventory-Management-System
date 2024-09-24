# Inventory Management Analysis


## Overview

This project focuses on inventory management using sales data to forecast future inventory needs. The main goal is to analyze historical sales data and predict future sales using various machine learning techniques. The dataset provides transactional information which is used to understand sales patterns and forecast inventory requirements.

## Table of Contents

1. [Dataset Overview](#dataset-overview)
2. [Machine Learning Techniques](#machine-learning-techniques)
3. [Tools Used](#tools-used)

## Dataset Overview

The dataset used in this project provides detailed transactional information necessary for inventory forecasting. The primary objective is to analyze sales data to predict future inventory needs. Below are the specifics of the dataset:

### Data File
- **File Name**: `Project.csv`
- **Location**: `https://github.com/Nikhil2349/Inventory-management-analysis/blob/main/Project.csv`

### Columns
1. **transaction_date**: 
   - **Description**: The date when the transaction occurred.
   - **Format**: `dd-mm-yyyy`
   - **Example**: `15-09-2023`

2. **Total_Bill**: 
   - **Description**: The total amount billed for the transaction.
   - **Data Type**: Numeric (float)
   - **Example**: `299.99`

3. **transaction_qty**: 
   - **Description**: The quantity of items purchased in the transaction.
   - **Data Type**: Numeric (integer)
   - **Example**: `5`

4. **store_location**: 
   - **Description**: The location of the store where the transaction was made.
   - **Data Type**: Categorical (string)
   - **Example**: `New York`

5. **product_category**: 
   - **Description**: The category to which the product belongs.
   - **Data Type**: Categorical (string)
   - **Example**: `Electronics`

6. **product_type**: 
   - **Description**: The specific type of product purchased.
   - **Data Type**: Categorical (string)
   - **Example**: `Smartphone`

7. **Size**: 
   - **Description**: The size of the product.
   - **Data Type**: Categorical (string)
   - **Example**: `Medium`

8. **season**: 
   - **Description**: The season during which the transaction occurred, derived from the transaction date.
   - **Data Type**: Categorical (string)
   - **Values**:
     - `Winter` (December, January, February)
     - `Spring` (March, April, May)
     - `Summer` (June, July, August)
     - `Fall` (September, October, November)

### Summary Statistics
The dataset contains various statistical summaries and characteristics:
- **Total Number of Records**: Number of rows in the dataset.
- **Missing Values**: Information on any missing or null values in the dataset.
- **Data Types**: The data types of each column (e.g., numeric, categorical).
- **Descriptive Statistics**: Mean, median, standard deviation, and other statistical measures for numeric columns.

### Example Data
Here are a few rows of the dataset for reference:

| transaction_date | Total_Bill | transaction_qty | store_location | product_category | product_type | Size  | season |
|------------------|------------|-----------------|----------------|------------------|--------------|-------|--------|
| 15-09-2023       | 299.99     | 5               | New York       | Electronics      | Smartphone   | Medium| Fall   |
| 22-09-2023       | 159.49     | 3               | Los Angeles    | Apparel          | Jacket       | Large | Fall   |
| 05-10-2023       | 499.99     | 2               | Chicago        | Electronics      | Laptop       | Small | Fall   |

### Data Preprocessing
- **Date Parsing**: `transaction_date` is converted to datetime format to facilitate time-based analysis.
- **Feature Engineering**: New columns such as `year`, `month`, and `season` are created to provide additional insights.
- **Column Removal**: Unnecessary columns such as 'Hour', 'Month', and 'Day of Week' are dropped.

## Machine Learning Techniques

In this project, various machine learning techniques are employed to analyze and forecast inventory needs. These techniques include:
- **Time Series Forecasting**: Using models like ARIMA and LSTM to predict future sales based on historical data.
- **Exploratory Data Analysis (EDA)**: Visualizing data to understand patterns and relationships.

## Tools Used

The following tools and libraries are utilized in this project:
- **Programming Language**: Python
- **Libraries**:
  - `pandas`: Data manipulation and analysis
  - `numpy`: Numerical computations
  - `matplotlib` & `seaborn`: Data visualization
  - `plotly`: Interactive plots
  - `tensorflow` & `keras`: Machine learning and deep learning
  - `scikit-learn`: Preprocessing and model evaluation
  - `statsmodels`: Statistical models and tests


