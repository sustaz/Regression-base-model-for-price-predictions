# Bitcoin Price Prediction using Regression Models

A comprehensive machine learning project that implements **Linear and Polynomial Regression** models to predict Bitcoin (BTC-EUR) price movements. This project demonstrates how traditional regression techniques can be applied to cryptocurrency price forecasting.

## 📊 Overview

This project uses historical Bitcoin price data to build and evaluate regression models for price prediction. The implementation includes data preprocessing, model training, visualization, and performance evaluation using rolling window analysis.

## ✨ Features

- **Multiple Regression Techniques**: Implementation of both Linear and Polynomial Regression
- **Data Preprocessing**: Robust data cleaning and normalization pipeline
- **Outlier Detection**: Removal of volume outliers using statistical methods (3-sigma rule)
- **Multi-feature Analysis**: Analysis of Open, High, Low, Close, and Volume attributes
- **Rolling Window Validation**: Testing model reliability with 30-day rolling windows
- **SVR Comparison**: Comparison with Support Vector Regression for effectiveness evaluation
- **Comprehensive Visualizations**: Multiple plots for model performance and predictions
- **Future Price Prediction**: Capability to predict prices for n days ahead

## 📁 Dataset

The project uses historical Bitcoin to Euro (BTC-EUR) exchange rate data stored in `BTC-EUR.csv`. The dataset contains:

- **Date**: Trading date
- **Open**: Opening price
- **High**: Highest price of the day
- **Low**: Lowest price of the day
- **Close**: Closing price
- **Adj Close**: Adjusted closing price
- **Volume**: Trading volume

The dataset spans from September 2019 onwards and can be sourced from financial data providers like Yahoo Finance or Kaggle.

## 🛠️ Technologies Used

- **Python 3.x**
- **NumPy**: Numerical computations
- **Pandas**: Data manipulation and analysis
- **Matplotlib**: Data visualization
- **scikit-learn**: Machine learning models (SVR)
- **Jupyter Notebook**: Interactive development environment

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/sustaz/Regression-base-model-for-price-predictions.git
cd Regression-base-model-for-price-predictions
```

2. Install required dependencies:
```bash
pip install numpy pandas matplotlib scikit-learn jupyter
```

3. Launch Jupyter Notebook:
```bash
jupyter notebook Price_Regression_prediction.ipynb
```

## 🚀 Usage

1. Open `Price_Regression_prediction.ipynb` in your favorite Jupyter environment
2. Run the cells sequentially from top to bottom
3. The notebook will:
   - Load and preprocess the Bitcoin price data
   - Train Linear and Polynomial Regression models
   - Generate visualizations of predictions
   - Evaluate model reliability using rolling window analysis
   - Compare results with Support Vector Regression

### Using Custom Datasets

You can use your own cryptocurrency datasets! Just ensure they contain similar attributes:
- Date, Open, High, Low, Close, Adj Close, Volume

Replace `BTC-EUR.csv` with your dataset file and run the notebook. Check [Kaggle](https://www.kaggle.com/) for more cryptocurrency datasets.

## 📈 Model Details

### Linear Regression
Applied to individual features (High, Low, Open, Close) to establish baseline predictions.

### Polynomial Regression
Used for more complex price patterns, particularly for Open prices and overall price trends. This captures non-linear relationships in the data.

### Validation Methodology
- **Rolling Window Analysis**: 30-day windows to test model stability over time
- **Multi-day Prediction**: Function to predict prices for multiple days ahead
- **Comparative Analysis**: Performance compared against Support Vector Regression

## 📂 Project Structure

```
Regression-base-model-for-price-predictions/
│
├── BTC-EUR.csv                          # Historical Bitcoin price data
├── Price_Regression_prediction.ipynb    # Main Jupyter notebook with analysis
├── BitcoinRegressionReport.pdf          # Detailed analysis report
└── README.md                            # Project documentation
```

## 📄 Results

For a detailed analysis of the regression models, their performance metrics, and comprehensive findings, please refer to `BitcoinRegressionReport.pdf`.

## 🤝 Contributing

Contributions are welcome! If you'd like to improve the models or add new features:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes and commit (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Create a Pull Request

## 📝 License

This project is open source and available for educational and research purposes.

## 🔗 Acknowledgments

- Data sourced from cryptocurrency exchanges
- Built with Python and scikit-learn ecosystem
- Inspired by financial time series analysis techniques

---

**Note**: Cryptocurrency prices are highly volatile. This project is for educational purposes only and should not be used as financial advice for trading decisions.
