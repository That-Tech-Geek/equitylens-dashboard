# EquityLens 📊

A premium, interactive Equity Research dashboard built with Streamlit and Plotly. It provides composite Bull/Bear technical indicators, key price movement insights, NLP-based news sentiment analysis, and essential fundamental evaluation tools.

## 🌟 Features

- **🎯 Composite Bull/Bear Signal**: Combines 8 technical indicators (RSI, MACD, Moving Average trend, Bollinger Bands, Stochastic, ADX/Trend Strength, Volume, Williams %R) into a single unified signal with weightings.
- **📈 Price Performance & Statistics**: Displays daily changes, 52-week ranges, ATH drawdowns, returns (1D, 5D, 1M, 3M, 1Y), and annualized 30D volatility.
- **📰 News Sentiment Analyzer**: Analyzes recent headlines using TextBlob sentiment polarity with interactive gauge, donut, and chronological bar visualization charts.
- **💼 Fundamental Analysis**: Evaluates stocks using two robust valuation metrics: **PEG Ratio** and **EV/EBITDA**, alongside a full fundamental snapshot.
- **🎨 Premium Aesthetic**: Styled with a dark glassmorphism layout, custom typography (Inter & JetBrains Mono), and fully responsive Plotly graphics.

## 🚀 Installation & Running

1. **Clone the repository**:
   ```bash
   git clone <repo-url>
   cd equity-research-tool
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **(Optional) Add a NewsAPI Key**:
   Create a `.streamlit/secrets.toml` file to configure a NewsAPI key for live sentiment analysis:
   ```toml
   NEWSAPI_KEY = "your_newsapi_key_here"
   ```

4. **Launch the app**:
   ```bash
   python -m streamlit run app.py
   ```

## 🛠️ Tech Stack

- **Framework**: [Streamlit](https://streamlit.io/)
- **Charts**: [Plotly](https://plotly.com/)
- **Data Source**: [yfinance](https://github.com/ranaroussi/yfinance)
- **Technical Analysis**: [ta-lib python wrapper](https://github.com/bukosabino/ta)
- **Sentiment Analysis**: [TextBlob](https://textblob.readthedocs.io/)
