# Big Mart Sales Prediction

This project focuses on building a machine learning model to predict the sales of products in different Big Mart outlets using historical sales data. The model is trained using a Random Forest Regressor and includes essential preprocessing and feature engineering steps.

## Project Structure

```
Big_Mart_Sales_Predictions/

 ── Big_Mart_Sales_Predictions.ipynb   # Main Jupyter Notebook
 ── Train.csv                          # Training dataset
 ── Test.csv                           # Test dataset
 ── README.md                          # Project overview and setup
```

## Objective

To predict the sales of each product in a Big Mart outlet based on various features including product information and outlet characteristics.

## Model Used

* **Algorithm:** Random Forest Regressor
* **Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn

## Features Used

* Item\_Weight
* Item\_Fat\_Content
* Item\_Visibility
* Item\_Type
* Item\_MRP
* Outlet\_Establishment\_Year
* Outlet\_Size
* Outlet\_Location\_Type
* Outlet\_Type

## Workflow Overview

1. **Data Cleaning**

   * Handle missing values
   * Standardize inconsistent category labels

2. **Feature Engineering**

   * Encode categorical variables using `LabelEncoder`
   * Normalize text-based columns for consistency

3. **Model Training**

   * Train a Random Forest Regressor
   * Evaluate using metrics like R² and RMSE

4. **Prediction**

   * Use the model to predict sales on the test dataset
   * Optionally allow interactive user inputs for prediction

## Evaluation Metrics

| Metric        | Score    |
| ------------- | -------- |
| Training R²   | \~99.13% |
| Validation R² | \~90.91% |
| Test R²       | \~94.00% |

*Note: These values may change based on data splits and model tuning.*

## Possible Improvements

* Tune hyperparameters using GridSearchCV
* Try other regression models like XGBoost or LightGBM
* Build a frontend using Streamlit or Flask for deployment

## Requirements

Install the following libraries before running the notebook:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

## Running the Notebook

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/Big_Mart_Sales_Predictions.git
   cd Big_Mart_Sales_Predictions
   ```

2. Launch Jupyter Notebook:

   ```bash
   jupyter notebook Big_Mart_Sales_Predictions.ipynb
   ```



