# 🏠 House Price Prediction using Linear Regression

## 📌 Project Overview

This project aims to predict house prices using the California Housing Dataset. A Linear Regression model was trained to learn the relationship between housing characteristics and median house values.

The project covers the complete Machine Learning workflow, including data preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, and visualization.

---

## 🎯 Objective

Build a Machine Learning model that predicts the median house value of a district based on factors such as:

* Location
* Income
* Population
* Number of rooms
* Number of bedrooms
* Housing age
* Ocean proximity

---

## 📊 Dataset Information

The dataset contains housing information collected from districts in California.

### Features

| Feature            | Description                |
| ------------------ | -------------------------- |
| longitude          | Geographic longitude       |
| latitude           | Geographic latitude        |
| housing_median_age | Median age of houses       |
| total_rooms        | Total number of rooms      |
| total_bedrooms     | Total number of bedrooms   |
| population         | Total population           |
| households         | Number of households       |
| median_income      | Median income of residents |
| ocean_proximity    | Distance from the ocean    |

### Target Variable

| Target             |
| ------------------ |
| median_house_value |

---

## 🔍 Exploratory Data Analysis

The following analyses were performed:

### House Price Distribution

* Visualized the distribution of house prices.
* Identified a right-skewed distribution.
* Observed a value cap near $500,000.

### Income vs House Price

* Analyzed the relationship between median income and house value.
* Found a strong positive correlation between income and house prices.

### Correlation Analysis

Key findings:

| Feature            | Correlation with House Price |
| ------------------ | ---------------------------- |
| median_income      | 0.688                        |
| latitude           | -0.144                       |
| total_rooms        | 0.134                        |
| housing_median_age | 0.106                        |

Median income was identified as the strongest predictor of house prices.

---

## 🧹 Data Preprocessing

### Missing Values

The `total_bedrooms` column contained 207 missing values.

These values were replaced using mean imputation to preserve all observations.

### Categorical Encoding

The `ocean_proximity` feature was converted into numerical format using One-Hot Encoding.

---

## 🤖 Model Training

### Algorithm Used

* Linear Regression

### Train-Test Split

* Training Set: 80%
* Testing Set: 20%

The model was trained using Scikit-Learn's `LinearRegression()` implementation.

---

## 📈 Model Evaluation

### Results

| Metric   | Score  |
| -------- | ------ |
| MAE      | 50,701 |
| RMSE     | 70,031 |
| R² Score | 0.626  |

### Interpretation

* The model's average prediction error is approximately $50,701.
* RMSE indicates the presence of some larger prediction errors.
* The model explains approximately 62.6% of the variance in house prices.

---

## 📊 Visualizations

The following visualizations were created:

* House Price Distribution Histogram
* Income vs House Price Scatter Plot
* Correlation Analysis
* Actual vs Predicted Scatter Plot
* Residual Plot

---

## 🛠 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-Learn
* Jupyter Notebook

---

## 📂 Project Structure

```text
house-price-prediction-linear-regression/
│
├── Housing.csv
├── House_Price_Prediction.ipynb
├── README.md
│
├── images/
│   ├── house_price_distribution.png
│   ├── income_vs_house_price.png
│   ├── actual_vs_predicted.png
│   └── residual_plot.png
│
└── requirements.txt
```

---

## 🚀 Future Improvements

* Feature Engineering
* Random Forest Regressor
* XGBoost Regressor
* Hyperparameter Tuning
* Model Deployment using Streamlit

---

## 📚 Key Learnings

Through this project, I learned:

* Data Cleaning and Preprocessing
* Exploratory Data Analysis (EDA)
* Correlation Analysis
* Linear Regression
* Regression Evaluation Metrics
* Model Interpretation
* Machine Learning Workflow

---

## 👨‍💻 Author

**Lionel**

Machine Learning Engineer Roadmap – Day 1 Project
