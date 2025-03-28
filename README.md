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

#### Correlation Heatmap
![Correlation Heatmap](EDA/correlation_heatmap.jpg)

#### Scatterplot Matrix
![Scatterplot Matrix](EDA/scatterplot_matrix.jpg)

#### Dataset with Outliers
![With Outliers](EDA/With_Outlier.jpg)

#### Dataset without Outliers
![Without Outliers](EDA/Without_Outlier.jpg)

### 4. Data Modeling

- Built a **Regression Model** to predict the price.
- Evaluated model performance using metrics like RMSE and R-squared.

## Folder Structure

```
📂 Project Root
├── 📂 code                   # Python scripts and Jupyter notebooks
├── 📂 Data ingestion and prep # Data collection & preprocessing scripts
├── 📂 Dataset                # Raw and processed dataset
├── 📂 EDA                    # Exploratory Data Analysis outputs
│   ├── correlation_heatmap.jpg
│   ├── scatterplot_matrix.jpg
│   ├── With_Outlier.jpg
│   ├── Without_Outlier.jpg
├── requirements.txt          # List of dependencies
├── End_to_end_air_bnb.ipynb  # Jupyter Notebook with full analysis
├── Air_BNB.xlsx              # Processed dataset
└── README.md                 # Project Documentation
```

## Requirements

To run this project, install dependencies from `requirements.txt`:

```bash
pip install -r requirements.txt
```

## How to Use

1. Open the Jupyter Notebook `End_to_end_air_bnb.ipynb`.
2. Run all cells sequentially to process data and build the model.
3. Check the results in the EDA and model evaluation sections.

## Results & Insights

- Identified key factors influencing Airbnb pricing.
- Compared dataset variations with and without outliers.
- Developed a regression model to predict price effectively.

## Author

**Mirza Imaduddin**
