# Time Series Forecasting with `skforecast` and Random Forest

This Jupyter Notebook demonstrates a time series forecasting approach using the `skforecast` library in Python. The dataset used includes monthly sales quantities and other financial indicators. The workflow involves data preprocessing, model training, prediction, and evaluation using the Random Forest algorithm.

## 1. Data Preprocessing

The dataset is imported and checked for missing values. The data is then visualized to observe trends in the `Sales_quantity` over time. The time series data is split into training and test sets, where the last 12 months are reserved for testing the model.

## 2. Model Training

A forecasting model (`ForecasterAutoreg`) is created using a `RandomForestRegressor`. The model is trained on the training data, specifically focusing on predicting `Sales_quantity` based on previous values (lags).

## 3. Prediction and Evaluation

The model's predictions are generated for the test period and compared against the actual test data. The performance of the model is evaluated using the Mean Squared Error (MSE). A plot is generated to visually compare the training data, actual test data, and the model’s predictions.

## 4. Hyperparameter Tuning

To improve the model's performance, a grid search is conducted to find the optimal hyperparameters for the `RandomForestRegressor` and the best number of lags. The model is then retrained with these optimal settings using the entire dataset.

## 5. Final Prediction and Visualization

Finally, the retrained model is used to make predictions, which are compared with the actual data in a plot. This demonstrates the effectiveness of the model after optimization.

This notebook provides a complete workflow for time series forecasting, covering data preparation, model training, evaluation, and optimization using the `skforecast` library and Random Forest.

![descargar](https://github.com/user-attachments/assets/3b1758ca-0f6b-40b9-b9f7-e7a2458da265)
