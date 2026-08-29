Data-Driven Stock Analysis using Time Series Models
📈 Predictive Modeling & Quantitative Portfolio Allocation
Time Series Analysis 2026 Capstone Project
This repository contains the Jupyter Notebook and methodology used to construct a data-driven, risk-optimized ₹10,00,000 virtual portfolio on the StockGro platform. By leveraging historical daily stock data from the National Stock Exchange (NSE), this project implements a quantitative forecasting pipeline that bridges theoretical mathematical modeling with practical capital management.
🎯 Project Objective
To develop an empirical mathematical validation framework utilizing statistical time series models to predict short-term stock prices, evaluate underlying asset stability, and execute a mathematically optimized capital allocation strategy in a live virtual simulator arena.
🛠️ Tech Stack & Methodology
Data Sourcing: yfinance API (Daily 'Close' prices from Jan 1, 2021 – Dec 31, 2025).  
IPYNB
Preprocessing: Forward-fill (ffill) propagation to protect consecutive row sequences from non-trading intervals; Augmented Dickey-Fuller (ADF) tests for stationarity validation; first-order differencing (d=1) to stabilize variance boundaries. Feature scaling via MinMaxScaler.  
IPYNB
+ 1
Forecasting Architecture:
ARIMA (5, 1, 0): Standard stochastic classical framework capturing structural memory effects and filtering random innovations.  
IPYNB
Facebook Prophet: Additive regression system deployed to capture complex, non-linear variables and piecewise linear trends.  
IPYNB
Volatility & Trend Modeling: Log Return Mapping to minimize raw value skewness and Seasonal and Trend decomposition using Loess (STL) to extract isolated Trend, Seasonality, and Remainder noise residuals.  
IPYNB
Evaluation Metrics: Root Mean Squared Error (RMSE), Mean Absolute Percentage Error (MAPE), and Directional Accuracy.  
IPYNB
📊 Stock Universe (Diversification Strategy)
To establish a statistically diversified operational universe, assets were extracted across decoupled macroeconomic sectors to limit cluster-risk exposure:
Sasken Technologies Ltd (IT Sector): Selected via a Forecast-Guided framework. Long-term training windows isolated a strong underlying structural alpha trend.
Texmaco Rail & Engineering Ltd (Industrial Sector): Selected via a Volatility-Aware strategy. Rolling historical standard deviation filters isolated a predictable risk profile resistant to micro-structural drops.
Suryoday Small Finance Bank Ltd (Banking Sector): Selected via a Sector-Based rationale. STL decomposition verified positive sector momentum and expansionary macro phases.
⚖️ Portfolio Allocation Strategy
The ₹10,00,000 virtual capital base was actively deployed by combining two core allocation metrics:
Strategy A (Forecast-Guided Allocation Weighting): Capital target sizing favored tickers displaying the highest relative upward slope velocity inside the out-of-sample calculation bounds.
Strategy B (Volatility-Aware Inverse-Sizing): Asset weights were scaled inversely proportional to their estimated log conditional volatility boundaries to limit severe portfolio drawdown profiles.
Final Deployment: This hybrid approach resulted in a highly balanced capital distribution of Texmaco (33.30%), Sasken (33.30%), and Suryoday (33.40%).
🚀 Results & Forward Testing
Positions were deployed within the "Portfolio - Time Series Analysis 2026" event tracker arena on StockGro. To guarantee empirical validation, out-of-sample projections were analyzed against unseen, real-world NSE market data:
Model Benchmark: The ARIMA (5, 1, 0) baseline achieved the strongest overall statistical assessment, yielding significantly lower MAPE and RMSE values across the validation layer compared to Prophet.  
IPYNB
Live Execution Outcomes: While the linear statistical time series models excelled at capturing historical structures and forecasted positive momentum, all three core assets experienced minor downward trajectories (with absolute variances ranging from 2.74% to 4.06%).
Key Insight: Pure mathematical time series models require exogenous variables to successfully navigate intra-day microstructural liquidity shifts and real-time systemic market pressure.
🔮 Future Improvements
To transition this framework into a more robust financial tool, future iterations will focus on:
Multivariate Models (SARIMAX): Incorporating exogenous multi-variable components to capture real-time order book imbalances, trading volume profiles, and macroeconomic sentiment shifts.
Higher-Frequency Training: Shifting from daily interval data to hourly or minute-by-minute structures to better capture and react to intra-day price swings and stochastic shocks.
📁 Repository Contents
Data-Driven Stock Analysis.ipynb : The complete Python pipeline (Data Fetching ➔ Preprocessing ➔ Modeling ➔ Forecasting).  
IPYNB
Data-Driven Stock Analysis.pdf : Comprehensive documentation of the methodology, mathematical rationale, and StockGro execution results.
