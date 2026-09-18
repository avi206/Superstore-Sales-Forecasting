# Superstore Sales Forecasting with Machine Learning

An end-to-end machine-learning project that explores Global Superstore sales data and uses a Random Forest regression model to estimate retail sales. The workflow combines data preparation, exploratory analysis, feature engineering, model evaluation, and prediction-error analysis.

## Project Overview

The goal is to turn historical retail transactions into practical sales insights and a reproducible baseline forecasting workflow. The analysis examines sales across product categories, locations, and other operational dimensions before training and evaluating a regression model.

## Tools and Libraries

- Python
- Pandas and NumPy
- Scikit-learn
- Matplotlib and Seaborn
- Jupyter Notebook

## Dataset

This project uses the **Global Superstore** dataset, which includes retail transaction details such as:

- Order and ship dates
- Product category and sub-category
- Sales, profit, quantity, and discount
- Region, customer segment, and shipping mode

## Workflow

1. Clean and prepare the source data.
2. Explore sales patterns and business performance.
3. Create features from date and categorical variables.
4. Split the prepared data into training and test sets (80/20).
5. Train a Random Forest Regressor.
6. Evaluate performance and inspect prediction errors.

## Model

### Random Forest Regressor

The final model estimates sales using historical transaction data and engineered features.

| Parameter | Value |
|---|---:|
| `n_estimators` | 50 |
| `max_depth` | 10 |
| `max_features` | `sqrt` |
| `random_state` | 42 |
| Train/test split | 80/20 |

## Evaluation

The model is evaluated on the test dataset using standard regression metrics:

| Metric | Result |
|---|---:|
| R² Score | 0.113 |
| RMSE | 491.99 |
| MAPE | 5.4990 |

The notebook also includes actual-versus-predicted visualizations, residual analysis, and a prediction-error distribution.

> The R² result indicates that this baseline model has limited predictive strength. It is useful as a starting point for further feature engineering, tuning, and validation.

## Key Insights

- **Technology** generated the highest total sales (approximately **4.74M**).
- **New York City** recorded the highest sales among the analyzed cities (approximately **256K**).
- Feature-importance analysis helps identify variables that contribute most to the model.
- The baseline model leaves room for stronger features and more robust validation.

## Recommendations

- Prioritize inventory and sales planning for high-performing product categories.
- Give additional attention to high-performing markets such as New York City.
- Improve future iterations with richer features, hyperparameter tuning, and stronger validation strategies.
- Use feature importance to focus refinement efforts on the most informative variables.

## Repository Structure

```text
Superstore-Sales-Forecasting/
├── data/                 # Source data
├── notebooks/            # Analysis and modeling notebook(s)
├── reports/              # Project report and presentation
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation
```

## Project Resources

- [Forecasting notebook](notebooks/superstore_forecasting.ipynb)
- [Project report](reports/Sales%20Forecasting%20using%20Machine%20Learning.docx)
- [Project presentation](reports/sales_forecasting_with_graph_slides.pptx)
- [Source dataset](data/superstore.csv)

## Getting Started

1. Clone this repository.
2. Create and activate a Python virtual environment.
3. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open the notebook in the `notebooks/` directory and run the cells in order.

## Author

**Avinash Madhu**  
Data Analyst | Business Analytics

- [GitHub](https://github.com/avi206)
- [LinkedIn](https://www.linkedin.com/in/avinash-madhu-847429203)
