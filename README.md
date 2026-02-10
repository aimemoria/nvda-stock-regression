# NVDA Stock Regression Analysis

A focused linear regression analysis that models NVIDIA (NVDA) closing prices using technical indicators and volume features from historical market data.

## Highlights
- Multiple linear regression with feature significance testing
- Clear diagnostic plots for residuals and prediction quality
- Reproducible notebook workflow

## Dataset
- File: Linear Modeling Part One/NVDA_Stock_Regression_Data.csv
- Records: 1,256 trading days
- Features: OHLCV, moving averages, and derived ratios
- Target: Close (closing price)

## Requirements
- Python 3.9+
- pandas, numpy, matplotlib, seaborn, scikit-learn, scipy

Install dependencies:
```
pip install pandas numpy matplotlib seaborn scikit-learn scipy
```

## Run the analysis
1. Open the notebook: Linear Modeling Part One/NVDA_Stock_Regression_Analysis.ipynb
2. Ensure the CSV file is in the same folder as the notebook
3. Run all cells

## Project structure
```
Linear Modeling Part One/
  NVDA_Stock_Regression_Analysis.ipynb
  NVDA_Stock_Regression_Data.csv
  README.md
```

## License
MIT
