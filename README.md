# End-to-End Airbnb Data Analysis Project

## Project Overview

This project focuses on predicting the prices of Airbnb listings using machine learning regression models. The dataset contains various independent features, and the goal is to build an end-to-end pipeline, including data cleaning, exploratory data analysis (EDA), feature engineering, and regression modeling to make accurate price predictions.

## Dataset

- The dataset originally contained **75,000** records.
- After removing duplicates, **54,000** records remained.
- The target variable for this analysis is **Price**.

## Project Pipeline

### 1. Data Cleaning

- Removed duplicate records, reducing the dataset size from **75k to 54k**.
- Handled missing values using **central tendency (mean/median/mode)** and **K-Nearest Neighbors (KNN) imputation**.

### 2. Outlier Detection & Treatment

- Applied statistical techniques to identify outliers.
- Created two versions of the dataset:
  - **With Outliers** (Retains all values)
  - **Without Outliers** (Filters extreme values)

### 3. Exploratory Data Analysis (EDA)

- Visualized relationships between variables.
- Plotted correlation heatmaps and scatterplots to understand dependencies.
- Examined the distribution of features and target variable.


### 4. Data Modeling

- Built a **Regression Model** to predict the price.
- Evaluated model performance using metrics like RMSE and R-squared.


## Results & Insights

- Identified key factors influencing Airbnb pricing.
- Compared dataset variations with and without outliers.
- Developed a regression model to predict price effectively.

## Author

**Mirza Imaduddin**
