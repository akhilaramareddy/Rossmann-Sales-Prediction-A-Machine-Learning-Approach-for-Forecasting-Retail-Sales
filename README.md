# Rossmann-Sales-Prediction-A-Machine-Learning-Approach-for-Forecasting-Retail-Sales
Project Overview :

This project aims to predict sales for Rossmann stores using historical sales data. The objective is to build a machine learning model that accurately forecasts daily sales based on various factors such as promotions, store type, competition, holidays, and seasonality.

Dataset Description :

The dataset consists of sales records from Rossmann stores and includes the following key attributes:

Store:  Unique ID for each store.
DayOfWeek:  Day of the week (1 = Monday, 7 = Sunday).
Sales:  The daily sales for a store (Target variable).
Customers:  Number of customers visiting the store.
Open:  Indicates whether the store was open (1) or closed (0).
Promo:  Whether a store is running a promotion on a particular day.
StateHoliday:  Indicates if the day is a public holiday.
SchoolHoliday:  Indicates if the store was affected by a school holiday.
StoreType & Assortment:  Categorical variables representing store characteristics.
CompetitionDistance:  Distance to the nearest competitor store.
CompetitionOpenSince:  The month and year when a competitor store opened.
Promo2:  Continuous promotional campaigns, including start dates.
Data Preprocessing
Handling Missing Values: 
Filled CompetitionDistance with the mean distance.
Filled CompetitionOpenSinceMonth and CompetitionOpenSinceYear with mode values.
Feature Engineering:
Extracted Year and Month from the Date column.
Created additional time-based features for trend analysis.
Encoding Categorical Variables: Applied label encoding and one-hot encoding where necessary.
Scaling: Normalized numerical features for better model performance.
Model Selection and Training
Several machine learning models were evaluated:

Linear Regression: Baseline model for sales prediction.
Random Forest Regressor: Captures non-linear relationships and interactions.
XGBoost: Gradient boosting model optimized for performance.
Neural Networks (MLP): A deep learning approach for capturing complex patterns.
The models were evaluated using Root Mean Squared Error (RMSE) and Mean Absolute Percentage Error (MAPE).

Results & Insights
The XGBoost model performed the best with an RMSE of 2100 and an accuracy of 89.6%.
The model successfully captures trends related to promotions, store types, and seasonal variations.
Stores with active promotions show a significant increase in sales.
Libraries & Tools Used
Python: For data processing and model development.
Pandas, NumPy: Data manipulation and preprocessing.
Matplotlib, Seaborn: Data visualization.
Scikit-learn, XGBoost: Machine learning model implementation.
Conclusion
This project provides a robust framework for predicting sales using machine learning techniques. The insights can help Rossmann Stores optimize inventory management, staffing, and promotional strategies.

Future Improvements
Incorporate time-series forecasting models such as LSTM or Prophet.
Fine-tune hyperparameters using GridSearchCV or Bayesian Optimization.
Improve feature engineering to include external economic factors
