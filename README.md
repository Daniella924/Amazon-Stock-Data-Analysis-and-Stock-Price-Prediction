# 📈 Amazon Stock Data Analysis and Price Prediction

## 🌟 Project Overview
This project analyzes Amazon stock data and builds predictive models by combining quantitative financial analysis with external event impacts. The system integrates time-series stock data with event-driven features to enhance prediction accuracy.

## 🔥 Key Features

### 1. 🧠 Hybrid Feature Modeling with XGBoost
- **Integrated multi-source data**: Combines traditional OHLCV (Open/High/Low/Close/Volume) data with external event labels
- **Event types considered**:
  - 🚀 Product releases
  - 💰 Financial report announcements
  - � Epidemic policy changes
  - Other market-moving events

### 2. 📊 Event Impact Quantification Module
- **Statistical validation**: Uses t-test (p<0.05) to verify significance of price fluctuations
- **Event window analysis**: Examines ±3 trading days around each event
- **Impact scoring**: Quantifies how different event types affect stock movement

### 3. ⚙️ Rolling Feature Generator
- **Multiple time windows**: 30/60/90 day rolling calculations
- **12+ technical indicators** including:
  - 📉 Rolling Volatility
  - ➗ Moving Averages (MA)
  - 🎚️ Bollinger Bands
  - RSI, MACD, and more

### 4. 📊 Interactive Power BI Dashboard
- **Dynamic visualizations** of stock trends
- **Event correlation analysis**
- **Model performance metrics**

## 🗂️ Repository Structure

```
├── 📂 data_processing/       # Data cleaning and feature engineering
│   ├── event_processor.py   # Event impact analysis
│   └── feature_generator.py # Rolling feature creation
├── 📂 modeling/             # Predictive models
│   ├── xgboost_model.py     # Hybrid XGBoost implementation
│   └── evaluation.py        # Model performance metrics
├── 📂 visualization/        # Power BI dashboard files
├── 📂 tests/                # Unit and integration tests
├── 📜 requirements.txt      # Dependency list
└── 📜 README.md             # This file
```

## 🛠️ Technical Stack

- **Python 3.8+** 🐍
- Key Libraries:
  - `pandas` 🐼, `numpy` 🔢 for data processing
  - `xgboost` 🌳 for predictive modeling
  - `scipy` 📈 for statistical testing
  - `ta` 📊 for technical indicators
- **Power BI** 💹 for visualization

## 🚀 Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/amazon-stock-analysis.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the pipeline:
   ```bash
   python main.py
   ```
4. Open the Power BI dashboard:
   ```bash
   start visualization/amazon_stock_dashboard.pbix
   ```

## 📊 Sample Outputs

![Prediction Performance](screenshots/prediction_chart.png)
*Figure: Actual vs Predicted stock prices*

![Event Impact](screenshots/event_impact.png)
*Figure: Quantified impact of different event types*

## 🤝 How to Contribute

We welcome contributions! Please:
1. � Fork the repository
2. 🛠️ Create your feature branch
3. 💾 Commit your changes
4. 🔀 Push to the branch
5. 🎯 Open a Pull Request
