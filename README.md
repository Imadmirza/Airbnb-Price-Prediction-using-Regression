# ✨ End-to-End Airbnb Data Analysis Project ✨

## 📅 Project Overview

This project focuses on predicting the prices of Airbnb listings using machine learning regression models. The dataset contains various independent features, and the goal is to build an end-to-end pipeline, including data cleaning, exploratory data analysis (EDA), feature engineering, and regression modeling to make accurate price predictions.

## 📚 Dataset

- The dataset originally contained **75,000** records.
- After removing duplicates, **54,000** records remained.
- The target variable for this analysis is **Price**.

## 📚 Project Pipeline

### 1. 🌐 Data Cleaning

- Removed duplicate records, reducing the dataset size from **75k to 54k**.
- Handled missing values using **central tendency (mean/median/mode)** and **K-Nearest Neighbors (KNN) imputation**.

### 2. ⚖️ Outlier Detection & Treatment

- Applied statistical techniques to identify outliers.
- Created two versions of the dataset:
  - **With Outliers** (Retains all values)
  - **Without Outliers** (Filters extreme values)

#### 📊 Dataset with Outliers
![With Outliers](https://raw.githubusercontent.com/Imadmirza/Airbnb-Price-Prediction-using-Regression/main/With%20Outlier.jpg)

#### 📊 Dataset without Outliers
![Without Outliers](https://raw.githubusercontent.com/Imadmirza/Airbnb-Price-Prediction-using-Regression/main/Without%20Outlier.jpg)

**🔍 Insights:**
- The dataset **with outliers** shows extreme variations in price, which may not be realistic or representative of the general pricing trends.
- The dataset **without outliers** removes extreme values, allowing the model to generalize better and avoid being overly influenced by anomalies.
- **🌟 Key Takeaway:** Removing outliers improved the performance of regression models by reducing the impact of highly deviating price values.

### 3. 🎨 Exploratory Data Analysis (EDA)

- Visualized relationships between variables.
- Plotted correlation heatmaps and scatterplots to understand dependencies.
- Examined the distribution of features and target variable.

#### 🔄 Correlation Heatmap
![Correlation Heatmap](https://raw.githubusercontent.com/Imadmirza/Airbnb-Price-Prediction-using-Regression/main/correlation%20heatmap.jpg)

**🔍 Insights:**
- The heatmap reveals how different features relate to each other and their impact on price.
- Strong correlations were found between:
  - **Number of bedrooms and price** (More rooms generally increase price).
  - **Number of reviews and price** (Higher-rated properties may charge more).
  - **Location-based attributes** also showed a significant impact.
- **🌟 Key Takeaway:** Features with strong correlations were prioritized in model training to improve predictions.

#### 🎯 Scatterplot Matrix
![Scatterplot Matrix](https://raw.githubusercontent.com/Imadmirza/Airbnb-Price-Prediction-using-Regression/main/scatterplot%20matrix.jpg)

**🔍 Insights:**
- The scatterplot matrix helped visualize the **relationship between numerical features** and their impact on price.
- Some features showed **linear trends**, which are ideal for regression models.
- Certain features had **non-linear relationships**, suggesting that advanced models (e.g., polynomial regression or tree-based models) might improve prediction accuracy.
- **🌟 Key Takeaway:** The scatterplot helped in **feature selection** and deciding whether transformations were needed to improve the model’s accuracy.

### 4. 📊 Data Modeling

- Built a **Regression Model** to predict the price.
- Evaluated model performance using metrics like RMSE and R-squared.

## 🏆 Results

- Identified key factors influencing Airbnb pricing.
- Compared dataset variations with and without outliers.
- Developed a regression model to predict price effectively.

## 🏆 Insights from Visualizations

### Correlation Analysis:

![Correlation Analysis](https://raw.githubusercontent.com/Imadmirza/Airbnb-Price-Prediction-using-Regression/main/Correlation%20Analysis.jpg)

**Strongest positive correlations with log_price:**
- accommodates (~0.49)
- bedrooms (~0.47)
- bathrooms (~0.45)
- beds (~0.41)

**Weaker correlation:**
- review_scores_rating has a very weak correlation with price, suggesting ratings don’t strongly impact pricing.
- Cleaning fee has low correlation (~0.2), meaning it doesn’t significantly affect the price.

### Categorical Feature Analysis:

![Categorical Feature Analysis](https://raw.githubusercontent.com/Imadmirza/Airbnb-Price-Prediction-using-Regression/main/Categorical%20Feature%20Analysis.jpg)

**Room Type:**
- Significant price variation between room types.
- Entire homes/apartments tend to have higher log_price compared to shared/private rooms.

**Cancellation Policy:**
- Stricter policies might have slightly higher prices, but the difference is not very strong.

**Instant Bookable:**
- No major price difference observed between instant bookable and non-instant bookable listings.

## 🎮 Author

**Mirza Imaduddin**
