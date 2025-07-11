# House Price Prediction using Macroeconomic Indicators

## Project Overview

This project focuses on predicting future house prices by analyzing macroeconomic indicators such as interest rates, rental vacancy rates, and consumer price index (CPI). A Random Forest Classifier is trained to forecast whether adjusted home prices will rise in the next quarter, making this a classification-based forward-looking prediction system.

## Datasets Used

1. **Federal Reserve Data (FRED)**:
   - 30-Year Fixed Mortgage Rate
   - Rental Vacancy Rate
   - Consumer Price Index (CPI)

2. **Zillow Housing Market Data**:
   - Median Sale Price
   - Home Value Index (ZHVI)

## Key Steps and Methodology

- **Data Preparation**
  - Loaded and merged economic indicators from FRED and Zillow datasets.
  - Aligned dates, forward-filled missing values, and normalized prices using CPI.
  - Engineered features like Adjusted Price and Adjusted Value.

- **Label Engineering**
  - Defined the target variable as a binary classification (`Change`):  
    - `1` if adjusted price increases in the next quarter  
    - `0` otherwise

- **Model Training**
  - Used a Random Forest Classifier with backtesting logic.
  - Trained on past data and tested on future slices (mimicking real-world time series application).
  - Calculated prediction accuracy and visualized correct vs incorrect predictions.

- **Feature Enhancement**
  - Introduced rolling averages and yearly ratios to improve model robustness.
  - Computed feature importance using permutation importance.

## Tools and Libraries

- Python
- Pandas, NumPy
- scikit-learn (RandomForestClassifier, accuracy_score, permutation_importance)
- Matplotlib

## Results

- The model achieved high accuracy in classifying price trends.
- Visual analysis showed clear separation between correctly and incorrectly predicted outcomes.
- Important predictors included adjusted price, adjusted value, and interest rate trends.

## Conclusion

This project demonstrates how macroeconomic data can be effectively used to forecast housing market trends. It integrates financial datasets, performs time-aware backtesting, and builds a predictive system useful for buyers, sellers, and real estate analysts.
