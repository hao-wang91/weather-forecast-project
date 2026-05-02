# Weather Forecasting Project

## Overview
This project uses global weather data to forecast next-day temperature using machine learning models.  
To ensure a valid time series structure, the analysis focuses on a single city with the most observations.

---

## What I Did
- Cleaned and preprocessed the weather dataset
- Converted time column to datetime format and sorted data chronologically
- Selected a single city to construct a consistent time series
- Removed irrelevant and non-numeric features
- Handled missing values

### Exploratory Data Analysis (EDA)
- Visualized temperature trends over time to observe seasonal patterns
- Created a correlation heatmap to examine relationships between variables
- Plotted the distribution of temperature to understand its shape

### Feature Engineering
- Created a prediction target by shifting temperature to represent next-day values
- Added lag-based feature (previous temperature)
- Extracted time-based features:
  - Hour
  - Day
  - Month

### Modeling
Built and compared multiple machine learning models:
- Linear Regression
- Ridge Regression
- Random Forest

### Evaluation
- Used time-based train/test split (80/20) to preserve temporal structure
- Evaluated performance using Root Mean Squared Error (RMSE)

### Additional Work
- Implemented a simple ensemble method
- Analyzed feature importance

---

## Dataset
Global Weather Repository (Kaggle)

---

## How to Run
1. Install required libraries: pip install -r requirements.txt
2. Open the notebook: weather-forecast-project.ipynb
3. Run all cells to reproduce the results

---

## Results
- Ridge Regression achieved the lowest RMSE among tested models
- Linear models performed slightly better than Random Forest
- Temperature shows strong temporal dependency
- Weather variables improve prediction accuracy

---

## Notes
- The model predicts next-day temperature based on current weather conditions
- A single city was used to preserve temporal consistency
- Time-based splitting was used instead of random splitting

---

## Future Improvements
- Extend to multiple cities with proper panel/time-series modeling
- Try more advanced time-series models (ARIMA, LSTM)
- Perform deeper hyperparameter tuning