# Cryptocurrency Trading Simulator with Julia ML Integration

A sophisticated cryptocurrency trading simulator that integrates **Julia machine learning algorithms** with a **Python GUI interface** for real-time price prediction, risk analysis, and trading recommendations.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Julia](https://img.shields.io/badge/Julia-1.6+-purple.svg)
![PySide6](https://img.shields.io/badge/GUI-PySide6-green.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

## 🎯 Project Overview

This project demonstrates **advanced language interoperability** by connecting:
- **Julia ML Engine**: Advanced statistical analysis and prediction algorithms
- **Python GUI**: Professional trading interface with real-time updates
- **Real Market Data**: Integration with historical cryptocurrency prices

### Key Features
- ✅ **3-Coin Support**: Bitcoin (BTC), Ethereum (ETH), Tether (USDT)
- ✅ **Julia ML Predictions**: Advanced technical analysis algorithms
- ✅ **Real-time Risk Analysis**: Volatility-based risk scoring
- ✅ **Trading Signals**: BUY/SELL/HOLD recommendations
- ✅ **Portfolio Management**: Virtual trading with P&L tracking
- ✅ **Historical Data**: 13+ months of real cryptocurrency prices

## 🚀 Demo

![Crypto Trading GUI](screenshots/main_gui.png)

### Live Features
- **Price Predictions**: Julia-powered forecasting using MACD, RSI, Bollinger Bands
- **Risk Assessment**: Multi-factor risk analysis with visual indicators
- **Trading Simulation**: Execute virtual trades with portfolio tracking
- **Multi-coin Tabs**: Independent analysis for each cryptocurrency

## 🏗️ Architecture

```
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│   Python GUI    │◄──►│  Julia ML Bridge │◄──►│   Julia Engine  │
│  (PySide6/Qt)   │    │  (Async Comms)   │    │  (ML Algorithms) │
└─────────────────┘    └──────────────────┘    └─────────────────┘
        ▲                        ▲                        ▲
        │                        │                        │
        ▼                        ▼                        ▼
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│  User Interface │    │   Data Pipeline  │    │  ML Predictions │
│  3-Coin Tabs    │    │  CSV Integration │    │  Risk Analysis  │
│  Trading Logs   │    │  Price History   │    │  Trading Signals│
└─────────────────┘    └──────────────────┘    └─────────────────┘
```

## 📊 Machine Learning Algorithms

### Julia ML Engine (`enhanced_julia_ml.jl`)

**Price Prediction**:
- Moving Average Convergence Divergence (MACD)
- Relative Strength Index (RSI) 
- Bollinger Bands analysis
- Linear regression trend analysis

**Risk Analysis**:
- GARCH-like volatility modeling
- Value at Risk (VaR) calculation
- Skewness and kurtosis analysis

**Trading Signals**:
- Multi-timeframe analysis (short/medium/long term)
- Technical indicator convergence
- Momentum-based decision logic

## 🛠️ Installation & Setup

### Prerequisites
- Python 3.8+ with PySide6
- Julia 1.6+ with required packages
- Historical cryptocurrency data (CSV format)

### Quick Start

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/crypto-trading-julia-ml.git
   cd crypto-trading-julia-ml
   ```

2. **Install Python dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Install Julia packages**:
   ```bash
   julia -e 'using Pkg; Pkg.add(["CSV", "DataFrames", "Statistics", "LinearAlgebra"])'
   ```

4. **Run the application**:
   ```bash
   python run_gui.py
   ```

### Testing the System

1. **Run system validation**:
   ```bash
   python run_tests.py
   ```

2. **Test data integration**:
   ```bash
   python run_data_test.py
   ```

### Running from Source

If you prefer to run from the source directories:

```bash
# Main GUI
cd code && python crypto_gui_integration.py

# Data integration test
cd data && python real_data_integration.py

# System tests  
cd tests && python test_components.py
```

## 📁 Project Structure

```
crypto-trading-julia-ml/
├── 🎯 CORE APPLICATION
│   ├── crypto_gui_integration.py    # Main 3-coin GUI application
│   ├── julia_ml_bridge.py          # Python ↔ Julia ML bridge
│   └── enhanced_julia_ml.jl         # Advanced Julia ML algorithms
│
├── 📊 DATA INTEGRATION
│   ├── real_data_integration.py     # CSV data processing
│   ├── Bitcoin prices.csv          # BTC historical data
│   ├── Ethereum Prices.csv         # ETH historical data
│   └── USDT Prices.csv             # USDT historical data
│
├── 🧪 TESTING & VALIDATION
│   ├── test_components.py           # System validation
│   └── csv_julia_integration.py     # Integration testing
│
├── 📚 DOCUMENTATION
│   ├── README.md                   # This file
│   ├── Project_Analysis_Report.md   # Technical analysis
│   └── requirements.txt            # Python dependencies
│
└── 📸 ASSETS
    └── screenshots/                # GUI screenshots for demo
```

## 🔧 Key Components

### 1. Python GUI (`crypto_gui_integration.py`)
- **PySide6-based interface** with tabbed multi-coin layout
- **Real-time price updates** and portfolio tracking  
- **ML integration buttons** for predictions, risk, signals
- **Trading execution** with buy/sell functionality

### 2. Julia ML Bridge (`julia_ml_bridge.py`)
- **Async communication** between Python GUI and Julia engine
- **Error handling** with Python fallback algorithms
- **Data conversion** between Python/Julia formats
- **Callback system** for ML results

### 3. Julia ML Engine (`enhanced_julia_ml.jl`)
- **Advanced prediction algorithms** using multiple technical indicators
- **Professional risk analysis** with statistical modeling
- **Multi-timeframe trading signals** with threshold-based decisions
- **Optimized for cryptocurrency** volatility patterns

### 4. Data Integration (`real_data_integration.py`)
- **CSV processing** with timestamp sorting
- **Multi-coin data loading** from separate files
- **Data validation** and format standardization
- **Historical analysis** with 13+ months of real market data

## 📈 Technical Analysis Features

### Price Predictions
- **5-period forecasting** using trend analysis and momentum
- **Technical indicator synthesis** (MACD + RSI + Bollinger Bands)
- **Volatility adjustment** with realistic bounds
- **Confidence intervals** based on historical variance

### Risk Assessment  
- **Volatility clustering** detection using GARCH-like models
- **Value at Risk (VaR)** calculation for downside risk
- **Multi-factor scoring** combining volatility, skewness, kurtosis
- **Visual risk indicators** with color-coded displays

### Trading Signals
- **Moving average crossovers** with multiple timeframes
- **Momentum analysis** using RSI and price velocity
- **Support/resistance levels** via Bollinger Band positioning
- **Signal confidence** based on indicator convergence

## 🎓 Educational Value

This project demonstrates:
- **Language Interoperability**: Seamless Python-Julia integration
- **Financial ML Applications**: Real-world quantitative finance
- **GUI Development**: Professional desktop application design
- **Data Processing**: Time series analysis and CSV handling
- **Software Architecture**: Modular design with clear separation of concerns

## 🤝 Contributing

This project was developed as part of a collaborative team assignment with specialized roles:
- **Person E (This Role)**: Julia ML ↔ Python GUI Integration
- **Person A-D**: Blockchain, DEX, Smart Contracts, Data Integration

## 📊 Performance

**Data Processing**:
- Loads 398+ days of historical data in <2 seconds
- Julia ML predictions complete in <100ms
- Real-time GUI updates every 5 seconds

**Memory Usage**:
- Base application: ~50MB RAM
- With historical data: ~75MB RAM
- Julia engine: ~100MB RAM (when active)

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Historical cryptocurrency data from market APIs
- Julia community for excellent mathematical libraries
- PySide6 team for robust GUI framework
- Educational institution for project guidance

---

**Built with ❤️ using Python, Julia, and real cryptocurrency market data**
