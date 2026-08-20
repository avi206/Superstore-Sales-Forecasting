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

- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Feature engineering from date variables
- Encoding categorical variables
- Train-test split using an 80/20 ratio
- Training a Random Forest Regressor
- Model evaluation using R², RMSE, and MAPE
- Residual and prediction error analysis
  
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

##  Key Insights

* **Technology** generated the highest total sales at **4.74M**, followed by Furniture and Office Supplies.
* **New York City** recorded the highest sales among the cities analyzed, with approximately **256K** in sales.
* **Feature importance analysis** was used to identify influential variables and reduce the feature set for modeling.
* The final Random Forest model achieved an **R² score of 0.113** on the test data, indicating limited predictive strength.

##  Business Recommendations

* **Prioritize high-performing categories:** Technology generated the highest sales, so inventory and sales planning can give greater attention to this category.
* **Focus on high-performing markets:** New York City recorded the highest sales among the cities analyzed, making it a potential priority market for sales and inventory planning.
* **Improve model performance:** The final Random Forest model achieved an R² score of 0.113, so further feature engineering, hyperparameter tuning, and stronger validation strategies could improve predictive performance.
* **Use feature importance for model refinement:** The identified influential features can be used to simplify the model and focus future iterations on the variables contributing most to predictions.

##  Project Structure

```  
Superstore-Sales-Forecasting/
│
├── data/
├── notebooks/
├── reports/
├── requirements.txt
└── README.md
```  
## Author

Avinash Madhu
