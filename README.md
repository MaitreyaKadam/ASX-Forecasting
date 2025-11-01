## ASX Time Series Forecasting 📈

Overview 🚀
This project presents a time series analysis of monthly averages from January 2004 onward, focusing on the ASX ALL Ordinaries, Price Index, Gold Price (AUD), Crude Oil, and Copper Price

Primary Objective
- Investigate non-stationarity in the time series
- Decompose and interpret time series components
- Built and Evaluated Distributed Lag Models to forecast the ASX Price Index using predictors.

📌 Key Insights
- To address high variance and shifting mean, a Box-Cox transformation followed by 1st Order differencing was applied. This improved stationarity and prepared the data for modelling.
- To capture the dynamic relation between ASX Index and Commodity Prices. The ARDLM model emerged as the most effective, which balances interpretability and predictive performance.
- The best performing model incorporated Gold Price as a Predictor, with lag orders of p=1 and q=5, achieving an adjusted R-square of 0.9478 which indicates strong explanatory power and alignment between the series.
- However, VIF checks revealed significant multi-collinearity which underscores the importance of cautious interpretation and potential refinement through variable selection or regularization

Tech Stack Used 🧰
- R for data cleaning, analysis and visualisation
- forecast package for time series forecasting and decomposition techniques
- tseries package for stationarity testing using ADF and related diagnostics
- dynlm package for contructing and evaluating distributed lag models.
