# Superstore Sales Forecasting using Machine Learning

## Project Overview

This project predicts future retail sales using machine learning techniques on the Global Superstore dataset.

The objective is to analyze historical sales data, identify patterns influencing revenue, and build predictive models that help businesses forecast demand and improve decision-making.

## Tools Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Jupyter Notebook

## Dataset

Dataset: **Global Superstore Dataset**

The dataset contains retail transaction data including:

* Order Date and Ship Date
* Product Category and Sub-Category
* Sales, Profit, Quantity, Discount
* Region and Customer Segment
* Shipping Mode

## Key Analysis Performed

1. Data cleaning and preprocessing
2. Exploratory Data Analysis (EDA)
3. Feature engineering from date variables
4. Training machine learning models
5. Evaluating model performance

##  Machine Learning Model

### Random Forest Regressor

A Random Forest Regressor was used to predict sales based on historical transaction and engineered features.

The model was trained using an **80/20 train-test split**.

### Model Configuration

- **`n_estimators`:** 50
- **`max_depth`:** 10
- **`max_features`:** `sqrt`
- **`random_state`:** 42
  
##  Model Evaluation

The model was evaluated on the test dataset using:

- **R² Score:** 0.113
- **RMSE:** 491.99
- **MAPE:** 5.4990 (reported by scikit-learn as a ratio)

The notebook also includes:

- Actual vs. predicted sales visualization
- Residual analysis
- Prediction error distribution

## Key Insights

* Data cleaning and preprocessing
* Exploratory Data Analysis (EDA)
* Feature engineering from date variables
* Encoding categorical variables
* Train-test split using an 80/20 ratio
* Training a Random Forest Regressor
* Model evaluation using R², RMSE, and MAPE
* Residual and prediction error analysis

## Business Recommendations

* Focus inventory on high-performing product categories.
* Optimize discount strategies to protect profit margins.
* Use predictive models for demand forecasting.
* Improve inventory planning based on seasonal demand patterns.

  ## Dataset

The dataset used in this project is the Global Superstore dataset obtained from Kaggle.

It contains retail transaction data including:
- Order date
- Product category
- Sales
- Profit
- Discount
- Region and customer segment

## Project Structure

data/ → dataset used for training  
notebooks/ → Jupyter notebook containing analysis and ML model  
reports/ → project documentation and presentation  
README.md → project overview

## Author

Avinash Madhu
