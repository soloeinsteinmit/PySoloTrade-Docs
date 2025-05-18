# 🧰 PySoloTrade Tool Inventory

This document catalogs the various open-source libraries, APIs, and tools that PySoloTrade integrates or plans to integrate. The inventory is organized by category and includes information about each tool's purpose, features, and integration status.

**Legend:**

- ✅ Core Integration (already implemented)
- 🔄 Planned Integration (in progress)
- 🔍 Under Evaluation (being investigated)

## 📊 Market Data Sources

### Free & Open Data Sources

| Name                  | Description                                | Features                                                                                        | Integration Status | Documentation                                        |
| --------------------- | ------------------------------------------ | ----------------------------------------------------------------------------------------------- | ------------------ | ---------------------------------------------------- |
| **yfinance**          | Yahoo Finance data downloader              | Stock, ETF, mutual fund, index, currency, cryptocurrency data with OHLCV, dividends, and splits | ✅ Core            | [Link](https://github.com/ranaroussi/yfinance)       |
| **pandas-datareader** | Extract data from various Internet sources | Supports FRED, World Bank, Kenneth French's data library, and more                              | ✅ Core            | [Link](https://pandas-datareader.readthedocs.io/)    |
| **alpha_vantage**     | Free APIs for stock, forex, crypto data    | Intraday, daily, weekly data with technical indicators                                          | ✅ Core            | [Link](https://github.com/RomelTorres/alpha_vantage) |
| **FRED API**          | Federal Reserve Economic Data              | Macroeconomic indicators, interest rates, etc.                                                  | ✅ Core            | [Link](https://fred.stlouisfed.org/docs/api/fred/)   |
| **Quandl**            | Financial, economic, and alternative data  | Limited free data                                                                               | ✅ Core            | [Link](https://www.quandl.com/)                      |
| **IEX Cloud**         | Financial data platform                    | Limited free tier                                                                               | 🔄 Planned         | [Link](https://iexcloud.io/)                         |
| **Coinmarketcap API** | Cryptocurrency market data                 | Limited free tier                                                                               | 🔄 Planned         | [Link](https://coinmarketcap.com/api/)               |
| **CryptoCompare**     | Cryptocurrency data                        | Real-time and historical crypto data                                                            | 🔄 Planned         | [Link](https://min-api.cryptocompare.com/)           |
| **Finnhub**           | Financial data APIs                        | Limited free tier                                                                               | 🔄 Planned         | [Link](https://finnhub.io/)                          |

### Premium Data Sources (With Adapters)

| Name                   | Description             | Features                            | Integration Status | Documentation                                                                |
| ---------------------- | ----------------------- | ----------------------------------- | ------------------ | ---------------------------------------------------------------------------- |
| **Polygon.io**         | Financial data API      | Stocks, options, forex, crypto      | 🔄 Planned         | [Link](https://polygon.io/)                                                  |
| **Alpaca Market Data** | Market data APIs        | Real-time and historical stock data | 🔄 Planned         | [Link](https://alpaca.markets/data)                                          |
| **Tiingo**             | Financial data platform | End-of-day and intraday data        | 🔄 Planned         | [Link](https://api.tiingo.com/)                                              |
| **IBKR/TWS API**       | Interactive Brokers API | Comprehensive market data           | 🔄 Planned         | [Link](https://interactivebrokers.github.io/tws-api/)                        |
| **Refinitiv/Eikon**    | Market data platform    | Premium financial data              | 🔶 Future          | [Link](https://developers.refinitiv.com/en/api-catalog/eikon/eikon-data-api) |
| **Bloomberg API**      | Market data platform    | Premium financial data              | 🔶 Future          | [Link](https://www.bloomberg.com/professional/support/api-library/)          |

## 📈 Technical Analysis

### Indicator Libraries

| Name           | Description                         | Features                                  | Integration Status | Documentation                                  |
| -------------- | ----------------------------------- | ----------------------------------------- | ------------------ | ---------------------------------------------- |
| **TA-Lib**     | Technical Analysis Library          | 150+ indicators, pattern recognition      | ✅ Core            | [Link](https://ta-lib.org/)                    |
| **pandas-ta**  | Technical Analysis for pandas       | 130+ indicators with pandas integration   | ✅ Core            | [Link](https://github.com/twopirllc/pandas-ta) |
| **ta**         | Technical Analysis Library          | 80+ indicators implemented in pure Python | ✅ Core            | [Link](https://github.com/bukosabino/ta)       |
| **FinTA**      | Financial Technical Analysis        | Common technical indicators               | 🔄 Planned         | [Link](https://github.com/peerchemist/finta)   |
| **stockstats** | Technical indicators for stock data | Based on pandas                           | 🔄 Planned         | [Link](https://github.com/jealous/stockstats)  |

### Pattern Recognition

| Name                | Description             | Features                                      | Integration Status | Documentation                                    |
| ------------------- | ----------------------- | --------------------------------------------- | ------------------ | ------------------------------------------------ |
| **TA-Lib Patterns** | Pattern recognition     | 60+ candlestick patterns                      | ✅ Core            | [Link](https://ta-lib.org/function.html)         |
| **pennant**         | Chart pattern detection | Head and shoulders, triangles, etc.           | 🔄 Planned         | [Link](https://github.com/peraktong/pennant)     |
| **mplfinance**      | Financial plotting      | Candlestick charts with pattern visualization | ✅ Core            | [Link](https://github.com/matplotlib/mplfinance) |

## 🤖 Machine Learning and AI

### ML Libraries

| Name             | Description                | Features                               | Integration Status | Documentation                               |
| ---------------- | -------------------------- | -------------------------------------- | ------------------ | ------------------------------------------- |
| **scikit-learn** | Machine learning in Python | Classification, regression, clustering | ✅ Core            | [Link](https://scikit-learn.org/)           |
| **PyTorch**      | Deep learning framework    | Neural networks, GPU acceleration      | ✅ Core            | [Link](https://pytorch.org/)                |
| **TensorFlow**   | End-to-end ML platform     | Production-grade ML                    | 🔄 Planned         | [Link](https://www.tensorflow.org/)         |
| **XGBoost**      | Gradient boosting          | High-performance boosted trees         | ✅ Core            | [Link](https://xgboost.readthedocs.io/)     |
| **LightGBM**     | Gradient boosting          | Fast, distributed gradient boosting    | ✅ Core            | [Link](https://lightgbm.readthedocs.io/)    |
| **CatBoost**     | Gradient boosting          | Categorical feature support            | 🔄 Planned         | [Link](https://catboost.ai/)                |
| **sktime**       | Time series ML             | Forecasting, classification            | ✅ Core            | [Link](https://www.sktime.org/)             |
| **Prophet**      | Time series forecasting    | Robust forecasting with seasonality    | ✅ Core            | [Link](https://facebook.github.io/prophet/) |
| **pmdarima**     | ARIMA models               | Auto ARIMA, time series forecasting    | ✅ Core            | [Link](https://alkaline-ml.com/pmdarima/)   |
| **statsmodels**  | Statistical models         | Time series analysis, econometrics     | ✅ Core            | [Link](https://www.statsmodels.org/)        |

### Financial ML Models

| Name                  | Description                        | Features                                   | Integration Status | Documentation                                          |
| --------------------- | ---------------------------------- | ------------------------------------------ | ------------------ | ------------------------------------------------------ |
| **FinRL**             | Reinforcement learning for finance | Portfolio optimization, trading strategies | 🔄 Planned         | [Link](https://github.com/AI4Finance-Foundation/FinRL) |
| **PyPortfolioOpt**    | Portfolio optimization             | Mean-variance optimization, risk parity    | ✅ Core            | [Link](https://pyportfolioopt.readthedocs.io/)         |
| **ffn**               | Financial functions                | Performance analysis, returns analysis     | ✅ Core            | [Link](https://github.com/pmorissette/ffn)             |
| **FinBERT**           | NLP for financial text             | Sentiment analysis for financial news      | 🔄 Planned         | [Link](https://github.com/ProsusAI/finBERT)            |
| **QuantConnect LEAN** | Algorithmic trading engine         | Backtesting, live trading                  | 🔶 Future          | [Link](https://github.com/QuantConnect/Lean)           |

## 📰 News and Sentiment Analysis

### News APIs

| Name                   | Description       | Features                         | Integration Status | Documentation                                                     |
| ---------------------- | ----------------- | -------------------------------- | ------------------ | ----------------------------------------------------------------- |
| **NewsAPI**            | News articles API | Headlines, full articles, search | ✅ Core            | [Link](https://newsapi.org/)                                      |
| **Finnhub News**       | Financial news    | Company news, press releases     | 🔄 Planned         | [Link](https://finnhub.io/docs/api/company-news)                  |
| **Alpha Vantage News** | Financial news    | News sentiment, trending topics  | 🔄 Planned         | [Link](https://www.alphavantage.co/documentation/#news-sentiment) |
| **Benzinga**           | Financial news    | Real-time newsfeed               | 🔶 Future          | [Link](https://docs.benzinga.io/benzinga/newsfeed-v2.html)        |

### Social Media and Alternative Data

| Name              | Description            | Features                  | Integration Status | Documentation                                 |
| ----------------- | ---------------------- | ------------------------- | ------------------ | --------------------------------------------- |
| **Reddit API**    | Reddit data            | Subreddit data, comments  | 🔄 Planned         | [Link](https://www.reddit.com/dev/api/)       |
| **Twitter API**   | Twitter data           | Tweets, trends            | 🔄 Planned         | [Link](https://developer.twitter.com/en/docs) |
| **GDELT Project** | Global events database | News events, tone, themes | 🔶 Future          | [Link](https://www.gdeltproject.org/)         |

### Sentiment Analysis Tools

| Name             | Description                  | Features                                  | Integration Status | Documentation                                     |
| ---------------- | ---------------------------- | ----------------------------------------- | ------------------ | ------------------------------------------------- |
| **VADER**        | Sentiment analysis           | Rule-based sentiment                      | ✅ Core            | [Link](https://github.com/cjhutto/vaderSentiment) |
| **TextBlob**     | NLP processing               | Sentiment, noun phrase extraction         | ✅ Core            | [Link](https://textblob.readthedocs.io/)          |
| **spaCy**        | NLP library                  | Text processing, named entity recognition | ✅ Core            | [Link](https://spacy.io/)                         |
| **Transformers** | Hugging Face library         | State-of-the-art NLP models               | 🔄 Planned         | [Link](https://huggingface.co/transformers/)      |
| **FinBERT**      | Financial sentiment analysis | Pre-trained model for financial text      | 🔄 Planned         | [Link](https://github.com/ProsusAI/finBERT)       |

## 📊 Visualization

### Chart and Plot Libraries

| Name           | Description               | Features                               | Integration Status | Documentation                                    |
| -------------- | ------------------------- | -------------------------------------- | ------------------ | ------------------------------------------------ |
| **Matplotlib** | Visualization library     | Static charts, publication quality     | ✅ Core            | [Link](https://matplotlib.org/)                  |
| **mplfinance** | Financial charts          | Candlestick, OHLC, volume              | ✅ Core            | [Link](https://github.com/matplotlib/mplfinance) |
| **Plotly**     | Interactive visualization | Web-based interactive charts           | ✅ Core            | [Link](https://plotly.com/python/)               |
| **Bokeh**      | Interactive visualization | Web-based visualization                | 🔄 Planned         | [Link](https://bokeh.org/)                       |
| **seaborn**    | Statistical visualization | Statistical charts based on matplotlib | ✅ Core            | [Link](https://seaborn.pydata.org/)              |
| **altair**     | Declarative visualization | Grammar of graphics                    | 🔄 Planned         | [Link](https://altair-viz.github.io/)            |

### Dashboard Tools

| Name          | Description        | Features                           | Integration Status | Documentation                         |
| ------------- | ------------------ | ---------------------------------- | ------------------ | ------------------------------------- |
| **Dash**      | Web dashboards     | Interactive dashboards for Python  | ✅ Core            | [Link](https://dash.plotly.com/)      |
| **Streamlit** | Data apps          | Quick interactive data apps        | ✅ Core            | [Link](https://streamlit.io/)         |
| **Panel**     | Dashboard tools    | High-level app and dashboard tools | 🔄 Planned         | [Link](https://panel.holoviz.org/)    |
| **Voilà**     | Jupyter dashboards | Convert notebooks to dashboards    | 🔄 Planned         | [Link](https://voila.readthedocs.io/) |

## 📋 Backtesting and Simulation

### Backtesting Frameworks

| Name            | Description            | Features                       | Integration Status | Documentation                                 |
| --------------- | ---------------------- | ------------------------------ | ------------------ | --------------------------------------------- |
| **Backtrader**  | Backtesting library    | Strategy testing, optimization | ✅ Core            | [Link](https://www.backtrader.com/)           |
| **PyAlgoTrade** | Algorithmic trading    | Event-driven trading           | 🔄 Planned         | [Link](https://gbeced.github.io/pyalgotrade/) |
| **Zipline**     | Backtesting library    | Quantopian's engine            | 🔄 Planned         | [Link](https://github.com/quantopian/zipline) |
| **bt**          | Backtesting            | Flexible backtesting           | 🔄 Planned         | [Link](https://github.com/pmorissette/bt)     |
| **vectorbt**    | Vectorized backtesting | High-performance backtesting   | 🔄 Planned         | [Link](https://vectorbt.dev/)                 |

### Risk Analysis

| Name          | Description                  | Features                      | Integration Status | Documentation                                   |
| ------------- | ---------------------------- | ----------------------------- | ------------------ | ----------------------------------------------- |
| **PyRisk**    | Risk metrics                 | Various risk metrics          | ✅ Core            | [Link](https://github.com/PyRisk)               |
| **empyrical** | Performance and risk metrics | Returns analysis              | ✅ Core            | [Link](https://github.com/quantopian/empyrical) |
| **pyfolio**   | Portfolio analysis           | Performance and risk analysis | 🔄 Planned         | [Link](https://github.com/quantopian/pyfolio)   |

## 🏦 Broker APIs and Trading

### Broker Integrations

| Name                    | Description                 | Features                        | Integration Status | Documentation                                         |
| ----------------------- | --------------------------- | ------------------------------- | ------------------ | ----------------------------------------------------- |
| **Alpaca**              | Commission-free trading API | US stocks, ETFs                 | ✅ Core            | [Link](https://alpaca.markets/)                       |
| **Interactive Brokers** | Global broker API           | Stocks, options, futures, forex | 🔄 Planned         | [Link](https://interactivebrokers.github.io/tws-api/) |
| **TD Ameritrade**       | Trading API                 | US markets                      | 🔄 Planned         | [Link](https://developer.tdameritrade.com/)           |
| **ccxt**                | Cryptocurrency exchange     | 100+ crypto exchanges           | ✅ Core            | [Link](https://github.com/ccxt/ccxt)                  |
| **Oanda**               | Forex trading API           | Forex and CFDs                  | 🔄 Planned         | [Link](https://developer.oanda.com/)                  |
| **Binance**             | Crypto exchange API         | Crypto trading                  | 🔄 Planned         | [Link](https://binance-docs.github.io/apidocs/)       |

### Paper Trading

| Name                            | Description         | Features                | Integration Status | Documentation                                              |
| ------------------------------- | ------------------- | ----------------------- | ------------------ | ---------------------------------------------------------- |
| **Alpaca Paper Trading**        | Paper trading       | Realistic simulation    | ✅ Core            | [Link](https://alpaca.markets/docs/trading/paper-trading/) |
| **Backtrader Paper Trading**    | Paper trading       | Event-driven simulation | ✅ Core            | [Link](https://www.backtrader.com/docu/live/)              |
| **Custom Paper Trading Engine** | In-house simulation | Configurable rules      | ✅ Core            | PySoloTrade Docs                                           |

## 🧩 Fundamental Analysis

### Financial Statement Data

| Name                        | Description                | Features                                   | Integration Status | Documentation                                             |
| --------------------------- | -------------------------- | ------------------------------------------ | ------------------ | --------------------------------------------------------- |
| **Financial Modeling Prep** | Financial statements API   | Income statement, balance sheet, cash flow | ✅ Core            | [Link](https://financialmodelingprep.com/developer/docs/) |
| **SimFin**                  | Financial data             | Fundamentals, standardized format          | 🔄 Planned         | [Link](https://simfin.com/)                               |
| **Intrinio**                | Financial data             | Fundamentals, market data                  | 🔶 Future          | [Link](https://intrinio.com/)                             |
| **yfinance fundamentals**   | Yahoo Finance fundamentals | Basic fundamental data                     | ✅ Core            | [Link](https://github.com/ranaroussi/yfinance)            |

### Financial Ratios and Metrics

| Name         | Description            | Features                | Integration Status | Documentation                                  |
| ------------ | ---------------------- | ----------------------- | ------------------ | ---------------------------------------------- |
| **PyRatio**  | Financial ratios       | Common financial ratios | ✅ Core            | Custom PySoloTrade component                   |
| **finquant** | Portfolio optimization | Risk/return metrics     | 🔄 Planned         | [Link](https://github.com/fmilthaler/FinQuant) |

## 🧮 Core Financial Tools

### Pricing and Valuation

| Name                | Description              | Features                          | Integration Status | Documentation                                      |
| ------------------- | ------------------------ | --------------------------------- | ------------------ | -------------------------------------------------- |
| **QuantLib-Python** | Quantitative finance     | Derivatives pricing, yield curves | 🔄 Planned         | [Link](https://github.com/lballabio/QuantLib-SWIG) |
| **PyQL**            | Python QuantLib wrappers | Modern Pythonic interface         | 🔄 Planned         | [Link](https://github.com/enthought/pyql)          |
| **pyfin**           | Financial mathematics    | Option pricing, term structure    | 🔄 Planned         | [Link](https://github.com/google/pyfin)            |

### Calendar and Date Tools

| Name                        | Description        | Features                        | Integration Status | Documentation                                                     |
| --------------------------- | ------------------ | ------------------------------- | ------------------ | ----------------------------------------------------------------- |
| **pandas_market_calendars** | Market calendars   | Trading calendars for exchanges | ✅ Core            | [Link](https://github.com/rsheftel/pandas_market_calendars)       |
| **trading_calendars**       | Exchange calendars | Calendar for global exchanges   | 🔄 Planned         | [Link](https://github.com/quantopian/trading_calendars)           |
| **pandas**                  | Date functionality | Date range, offsets, etc.       | ✅ Core            | [Link](https://pandas.pydata.org/docs/user_guide/timeseries.html) |

## 📦 Core Infrastructure

### Data Management

| Name       | Description          | Features                       | Integration Status | Documentation                                 |
| ---------- | -------------------- | ------------------------------ | ------------------ | --------------------------------------------- |
| **pandas** | Data manipulation    | DataFrames, Series             | ✅ Core            | [Link](https://pandas.pydata.org/)            |
| **NumPy**  | Numerical computing  | Arrays, mathematical functions | ✅ Core            | [Link](https://numpy.org/)                    |
| **polars** | Data manipulation    | Fast DataFrames                | 🔄 Planned         | [Link](https://github.com/pola-rs/polars)     |
| **SciPy**  | Scientific computing | Statistics, optimization       | ✅ Core            | [Link](https://scipy.org/)                    |
| **Arrow**  | Data framework       | Fast data conversion           | 🔄 Planned         | [Link](https://arrow.apache.org/docs/python/) |
| **Dask**   | Parallel computing   | Scaled pandas operations       | 🔄 Planned         | [Link](https://dask.org/)                     |

### Storage and Persistence

| Name              | Description              | Features                 | Integration Status | Documentation                               |
| ----------------- | ------------------------ | ------------------------ | ------------------ | ------------------------------------------- |
| **SQLAlchemy**    | SQL toolkit              | Database ORM             | ✅ Core            | [Link](https://www.sqlalchemy.org/)         |
| **Arctic**        | Time series database     | High-performance storage | 🔄 Planned         | [Link](https://github.com/man-group/arctic) |
| **HDF5/PyTables** | Hierarchical data format | Efficient binary storage | ✅ Core            | [Link](https://www.pytables.org/)           |
| **Redis**         | In-memory data store     | Caching, pub/sub         | 🔄 Planned         | [Link](https://redis.io/)                   |

## 🔌 Financial APIs and Data Services Adapters

### Integration Status Legend

- ✅ Core: Included in initial release
- 🔄 Planned: Scheduled for inclusion in upcoming releases
- 🔶 Future: Considered for long-term roadmap

## 🧠 Trading Algorithms and Strategy Libraries

| Name                 | Description               | Features                        | Integration Status | Documentation                                         |
| -------------------- | ------------------------- | ------------------------------- | ------------------ | ----------------------------------------------------- |
| **PyQuant**          | Quantitative strategies   | Mean reversion, trend following | ✅ Core            | Custom PySoloTrade component                          |
| **AlphaPy**          | Machine learning pipeline | Algorithmic trading             | 🔄 Planned         | [Link](https://github.com/ScottfreeLLC/AlphaPy)       |
| **MlFinLab**         | ML for finance            | Financial feature engineering   | 🔄 Planned         | [Link](https://github.com/hudson-and-thames/mlfinlab) |
| **Strategy Library** | Strategy implementations  | Classic trading algorithms      | ✅ Core            | Custom PySoloTrade component                          |

## 🔄 Real-time Data Processing

| Name                 | Description           | Features                        | Integration Status | Documentation                                                |
| -------------------- | --------------------- | ------------------------------- | ------------------ | ------------------------------------------------------------ |
| **Redis Streams**    | Message broker        | Real-time data streams          | 🔄 Planned         | [Link](https://redis.io/topics/streams-intro)                |
| **Apache Kafka**     | Distributed streaming | High-throughput messaging       | 🔶 Future          | [Link](https://kafka.apache.org/)                            |
| **websocket-client** | WebSocket             | Real-time data connections      | ✅ Core            | [Link](https://github.com/websocket-client/websocket-client) |
| **socketio**         | WebSocket alternative | Real-time two-way communication | ✅ Core            | [Link](https://python-socketio.readthedocs.io/)              |

## 🛠️ Contribution Guidelines

### Adding New Tools to the Inventory

To suggest a new tool for inclusion in PySoloTrade, please submit a pull request with the following information:

1. **Tool Name**: The name of the library or API
2. **Category**: Which section it belongs in
3. **Description**: Brief explanation of what it does
4. **Features**: Key capabilities relevant to financial applications
5. **URL**: Link to the tool's documentation or GitHub repository
6. **License**: What license the tool is distributed under
7. **Integration Complexity**: Simple evaluation of integration difficulty
8. **Dependencies**: Major dependencies required
9. **Sample Code**: Optional small example of basic usage

### Tool Selection Criteria

Tools are selected for inclusion in PySoloTrade based on these criteria:

1. **Quality**: Code quality, documentation, test coverage
2. **Maintenance**: Active development, issue response time
3. **Community**: Size of user community, GitHub stars
4. **Performance**: Computational efficiency for financial workloads
5. **License Compatibility**: Must use an open-source compatible license
6. **Dependencies**: Minimal external dependencies preferred
7. **Stability**: API stability and backward compatibility

## 📝 Integration Notes

### Integration Levels

PySoloTrade offers different levels of integration for external tools:

1. **Core Integration**: Deep integration with consistent APIs and PySoloTrade data models
2. **Wrapped Integration**: Light wrapper with standardized interfaces
3. **Direct Access**: Direct access to the underlying library when needed
4. **Plugin Support**: Available as optional plugins

### Version Pinning

The specific versions of each integrated tool that are tested and supported are documented in the `requirements.txt` and `pyproject.toml` files.

## 🔍 Specialized Tools

### Alternative Data

| Name                        | Description          | Features                        | Integration Status | Documentation                               |
| --------------------------- | -------------------- | ------------------------------- | ------------------ | ------------------------------------------- |
| **Quandl Alternative Data** | Alternative datasets | Economic, real estate, etc.     | 🔄 Planned         | [Link](https://www.quandl.com/)             |
| **OpenSky API**             | Flight data          | Air traffic data                | 🔶 Future          | [Link](https://opensky-network.org/apidoc/) |
| **OpenWeatherMap**          | Weather data         | Historical and forecast weather | 🔄 Planned         | [Link](https://openweathermap.org/api)      |

### Market Microstructure

| Name                | Description           | Features                       | Integration Status | Documentation                    |
| ------------------- | --------------------- | ------------------------------ | ------------------ | -------------------------------- |
| **LOBster**         | Limit order book data | Order book reconstruction      | 🔶 Future          | [Link](https://lobsterdata.com/) |
| **Tick Data Suite** | High-frequency data   | Market microstructure analysis | 🔶 Future          | Custom PySoloTrade component     |

## 🔄 Regular Updates

This tool inventory is regularly updated as new tools are integrated, upgraded, or deprecated. The last update was made on 17th April, 2025.

---

This document serves as both a reference for users and a guide for development priorities. Tools marked as "Core" are already integrated or will be in the initial release, while "Planned" items are in the development pipeline.

_**Last updated:** 17th April, 2025_
