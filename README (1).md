# House Price Prediction using Machine Learning

## Project Overview
This project focuses on predicting house prices using machine learning regression algorithms. I used the **House Prices - Advanced Regression Techniques** dataset from Kaggle.

The aim of this project is to understand how different house features affect selling prices and build a model that can predict prices for unseen properties.

## Dataset
Dataset: [Kaggle - House Prices: Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data)

The dataset contains information about residential properties in Ames, Iowa, USA.

- `train.csv` - 1460 records, including the target column `SalePrice`.
- `test.csv` - 1459 records, without the `SalePrice` column.

Download the dataset from Kaggle and place the CSV files in the project folder before running the notebook.

## Tools and Libraries
- Python
- Jupyter Notebook
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- YData Profiling

## Project Workflow
1. Loaded and explored the dataset.
2. Cleaned the data and handled missing values.
3. Removed selected columns with a large number of missing values.
4. Performed Exploratory Data Analysis (EDA).
5. Applied Ordinal Encoding and One-Hot Encoding.
6. Used StandardScaler for feature scaling.
7. Trained and compared different regression models.
8. Selected ElasticNet Regression as the final model.
9. Used GridSearchCV for hyperparameter tuning.
10. Evaluated the model using regression metrics.

## Models Tested
- Linear Regression
- Decision Tree Regression
- Ridge Regression
- Lasso Regression
- ElasticNet Regression

## Final Model Results
ElasticNet Regression gave the best result among the models I tested.

- Validation R² Score: 0.8646
- Cross-validation R² Score (GridSearchCV): 0.8193
- Mean Absolute Error (MAE): 19,222.31
- Root Mean Squared Error (RMSE): 32,227.66

Best parameters found using GridSearchCV:
- Alpha: 0.01
- L1 Ratio: 0.3

## How to Run
1. Clone or download this repository.
2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Download `train.csv` and `test.csv` from the Kaggle dataset link above.
4. Place the CSV files in the location expected by the notebook.
5. Start Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
6. Open the project notebook and run the cells.

## Future Improvements
- Try additional regression algorithms.
- Improve feature engineering and feature selection.
- Perform further hyperparameter tuning.
- Build a simple web interface using Flask or Streamlit.

## Author
**Mayukt Suthar**
