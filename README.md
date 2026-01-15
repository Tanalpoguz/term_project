# DengueAI: Disease Spread Prediction

This repository contains the code and experiments for the [DengueAI: Making Predictions for Today](https://www.drivendata.org/competitions/44/dengue-disease-spread-prediction/) competition on DrivenData. The goal involves predicting the number of dengue fever cases reported each week in San Juan, Puerto Rico and Iquitos, Peru, using environmental data such as temperature, precipitation, and vegetation indices.

## Project Structure

- **`code/`**: Contains Jupyter notebooks with various modeling approaches and experiments.
  - `xgboost.ipynb`: Implementation of XGBoost models.
  - `xgboost_lag.ipynb`: XGBoost with prediction horizon.
  - `xgboost_pca.ipynb`: XGBoost using PCA for dimensionality reduction.
  - `ensemble_xgb_lstm_svm.ipynb`: Ensemble method combining XGBoost, LSTM, and SVM.
  - `first_method_k_degree_poly.ipynb`: Baseline approach using polynomial regression.
- **`data/`**: Dataset files provided by the competition.
  - `dengue_features_train.csv`, `dengue_labels_train.csv`, `dengue_features_test.csv`
- **`requirements.txt`**: List of Python dependencies.