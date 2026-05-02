# Weather Forecasting Project

## Overview
This project analyzes global weather data and builds machine learning models to forecast next-day temperature.

## What I Did
- Cleaned and preprocessed weather dataset
- Performed exploratory data analysis (EDA)
- Engineered features including lag variables and time features
- Built and compared multiple models:
  - Linear Regression
  - Ridge Regression
  - Random Forest
- Evaluated model performance using RMSE
- Implemented a simple ensemble method
- Analyzed feature importance

## Dataset
Global Weather Repository (Kaggle)

## How to Run
1. Install required libraries:
   pip install -r requirements.txt

2. Open the notebook:
   weather-forecast-project.ipynb

3. Run all cells

## Results
- Ridge Regression achieved the lowest RMSE among tested models
- Linear models performed slightly better than Random Forest
- Temperature shows strong temporal dependency
- Weather variables improve prediction accuracy

## Notes
- The model predicts next-day temperature based on current weather conditions
- Time-based train/test split was used to preserve temporal order