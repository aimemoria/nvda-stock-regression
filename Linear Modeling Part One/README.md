# NVDA Stock Regression Analysis

## Overview
This project applies multiple linear regression to predict NVIDIA (NVDA) stock closing prices using historical technical indicators and trading volume data from Yahoo Finance (2021-2023).

## Authors
- **Aime Serge Tuyishime**
- **Nshuti Manzi Christian**
- **Nshuti Clay Bower**

**Course:** Data Mining and Machine Learning (AIT-104)  
**Instructor:** M. A. Manazir Ahsan

## Dataset
- **File:** `NVDA_Stock_Regression_Data.csv`
- **Records:** 1,256 trading days
- **Features:** 15 technical indicators including Open, High, Low, Volume, Moving Averages (10/20/50-day), Volume Ratio, Price-to-MA20 Ratio, and more
- **Target:** Close (closing price)

## Key Results

### Model Performance
- **R² Score:** 0.999974 (99.997% variance explained)
- **Test RMSE:** $11.24
- **Test MAE:** $5.26
- **Significant Features:** 11 out of 15 (p < 0.05)

### Significant Predictors
Open, High, Low, Volume, Stock Splits, Volume_MA_10, Volume_Ratio, Price_to_MA20_Ratio, High_Low_Pct, High_Low_Range, MA_10

## Requirements

### Python Packages
```bash
pip install pandas numpy matplotlib seaborn scikit-learn scipy
```

### Versions Used
- Python 3.9+
- pandas 2.3.3
- numpy 2.0.2
- scikit-learn 1.5+
- matplotlib 3.9+
- seaborn 0.13+
- scipy 1.14+

## Usage

### Running the Analysis
1. Open `NVDA_Stock_Regression_Analysis.ipynb` in Jupyter Notebook or VS Code
2. Ensure `NVDA_Stock_Regression_Data.csv` is in the same directory
3. Run all cells sequentially (Cell → Run All)

### Expected Outputs
- Statistical summaries and model performance metrics
- Three visualization files (optional):
  - `residual_diagnostics.png`
  - `actual_vs_predicted.png`
  - `feature_coefficients.png`

## Project Structure

```
NVDA_Stock_Regression_Analysis.ipynb    # Main analysis notebook
NVDA_Stock_Regression_Data.csv          # Dataset
README.md                                # This file
```

## Methodology

1. **Data Preprocessing:** Load data, compute descriptive statistics, train-test split (80-20)
2. **Model Training:** Multiple linear regression with all features
3. **Statistical Testing:** Identify significant variables using t-tests and p-values
4. **Model Improvement:** Retain only statistically significant features
5. **Validation:** Residual analysis, cross-validation, assumption verification
6. **Visualization:** Diagnostic plots and performance charts
7. **Error Analysis:** Confidence intervals and error sources
8. **Ethical Reflection:** Christian worldview perspective on algorithmic trading

## Key Findings

- Achieved exceptional predictive accuracy (99.997% R²)
- Reduced model complexity from 15 to 11 features with no performance loss
- Average prediction error of ±$5.26 per share
- Model explains price movements primarily through OHLC data, volume metrics, and moving averages

## Limitations

- Linear model may not capture all nonlinear market dynamics
- Does not account for external factors (news, macroeconomic events, sentiment)
- Performance may degrade during market regime changes
- Trained on 2021-2023 data; may require retraining for future periods

## Future Enhancements

- Add momentum indicators (RSI, MACD)
- Incorporate ensemble methods (Random Forest, Gradient Boosting)
- Include external market indices and economic indicators
- Implement time series models (ARIMA, LSTM)
- Add ESG metrics for ethical investment screening

## License
Academic project for educational purposes.

## Contact
For questions or collaboration, contact the authors through the course instructor.
