# Financial-Time-Series-Anomaly-Detection
The Jupyter notebook implements a partial solution for financial time-series anomaly detection using Yahoo Finance stock price data. It focuses on Apple (AAPL) stock from January 1, 2020, to January 1, 2024, and performs the following:

Data Acquisition: Downloads historical closing prices for AAPL, Google, and Microsoft using yfinance, but only processes AAPL. Missing values are handled using forward fill.
Financial Indicators: Calculates 20-day SMA, 20-day EMA, 14-day RSI, and 20-day Bollinger Bands using the ta library, providing technical indicators for anomaly detection.
Anomaly Detection: Applies an Isolation Forest model with a 5% contamination rate to detect anomalies based on RSI and Bollinger Bands. Detected anomalies are printed, showing potential unusual activities during volatile periods (e.g., early 2020).
Missing Components: The notebook does not include a time-series forecasting model (e.g., LSTM or Prophet) or visualizations of anomalies on stock price trends, which are critical for a complete solution.
Limitations:

The analysis is limited to AAPL, ignoring other tickers.
The absence of forecasting and visualization hinders the ability to identify deviations or present results effectively.
Redundant library installations and deprecated code reduce efficiency and compatibility.
Recommendations:

Extend the analysis to include all tickers (AAPL, GOOG, MSFT).
Implement a Prophet or LSTM model to forecast prices and detect anomalies based on residuals.
Add visualizations using matplotlib to plot stock prices with marked anomalies.
Streamline library usage and update deprecated code.
Comparison with Provided Script
The script I provided earlier (in the first response) addresses these gaps:

It processes multiple tickers (AAPL, MSFT, GOOGL).
Includes both Isolation Forest and Prophet for anomaly detection.
Visualizes results with plots showing stock prices, RSI, Bollinger Bands, and marked anomalies.
Generates a summary report with anomaly counts.
The notebook, while functional for the implemented steps, requires significant enhancements to meet the full scope of the task, which the provided script already fulfills.

Conclusion
The notebook provides a foundation for financial time-series anomaly detection but is incomplete due to missing forecasting and visualization steps. The implemented components are correct, but the outcomes do not fully align with the task's requirements. By incorporating the missing steps and addressing the identified issues, the notebook can be enhanced to deliver a comprehensive anomaly detection tool.
