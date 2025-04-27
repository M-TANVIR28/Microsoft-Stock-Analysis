# Microsoft Stock Time Series Analysis

## Project Overview
This project focuses on analyzing Microsoft (MSFT) stock price trends from 1986 to 2025 using time series analysis. It includes various methods like decomposition,Heatmap, volatility analysis, and forecasting, with the aim to gain insights into stock price movements and make future predictions.

## Dataset Source
- Microsoft stock data (1986–2025)
- [Kaggle - Microsoft Stock Data](https://www.kaggle.com/datasets/umerhaddii/microsoft-stock-data-2025)

## Tools & Libraries
This project uses the following tools and libraries:
- **Python**
- **Pandas**, **NumPy** for data manipulation
- **Matplotlib**, **Seaborn** for data visualization
- **Statsmodels** (ARIMA) for time series analysis
- **mplfinance** for candlestick chart visualization
- **Plotly** for interactive dashboards

## Key Features
- **Data cleaning & preprocessing**: Cleaning and preparing data for analysis.
- **Trend and moving average analysis**: Analysis of long-term trends using moving averages.
- **Time series decomposition**: Decomposing stock price into trend, seasonality, and residual components.
- **Heatmap visualization**: Visualizing the correlation between different stock features.
- **Daily returns analysis**: Calculating and plotting daily returns (percentage changes).
- **Volatility analysis**: Analyzing 30-day rolling volatility of the stock price.
- **ARIMA forecasting**: Using ARIMA to forecast the next 30 business days.
- **Interactive dashboards**: Using Plotly to create interactive charts for deeper insights.
- **Candlestick chart visualization**: Plotting Microsoft stock price movements with mplfinance for the last 100 days.

## How to Run
1. Install the required libraries:
    ```bash
    pip install pandas numpy matplotlib seaborn plotly statsmodels mplfinance prophet
    ```

2. **Download the dataset**:
   - Download the dataset from [Kaggle - Microsoft Stock Data](https://www.kaggle.com/datasets/umerhaddi/microsoft-stock-data-2025) or upload the CSV file locally.

3. **Run the analysis**:
   - Clone this repository or open the Jupyter Notebook.
   - Ensure the dataset is placed in the same directory as the notebook.
   - Run the cells to perform exploratory data analysis, time series decomposition, volatility analysis, and forecasting.

4. **Interactive Visualization**:
   - The project includes interactive charts created with Plotly for deeper insights into Microsoft stock trends and forecasts.

## Analysis Process
1. **Data Preprocessing**:
   - The raw stock data is cleaned and converted to a pandas DataFrame.
   - Date values are parsed and set as the index for time series analysis.

2. **Exploratory Data Analysis (EDA)**:
   - visualization of Microsoft stock's **Closing Prices** over time.
   - **Correlation heatmaps** and **daily returns** are calculated and plotted.
   - **Moving Averages** (50-day and 200-day) are computed and plotted to identify long-term trends.

3. **Time Series Decomposition**:
   - The time series is decomposed into **trend**, **seasonality**, and **residual** components to understand its underlying patterns.

4. **Volatility Analysis**:
   - A rolling **30-day volatility** is calculated and visualized to show periods of high market risk.

5. **ARIMA Forecasting**:
   - The ARIMA model is used to forecast Microsoft’s stock price for the next **30 business days**.
   - The **forecast** is plotted along with the actual data to visualize potential future trends.

6. **Advanced Visualization**:
   - **Candlestick charts** (using mplfinance) visualize Microsoft stock price movements over a short window of 100 days.
   - **Interactive charts** (using Plotly) are created to explore the **closing price**, **moving averages**, and other metrics interactively.

## Key Insights
- **Stock Price Trend**: The closing price has shown a consistent upward trajectory, reflecting Microsoft's growth.
- **Volatility**: Microsoft’s stock has shown varying levels of volatility, with certain periods experiencing more price fluctuations.
- **Moving Averages**: The 50-day and 200-day moving averages are useful for tracking long-term stock trends and identifying signals for potential buying or selling.
- **ARIMA Model**: The ARIMA model offers short-term forecasts, but future prices are highly influenced by external factors such as market events or sentiment.

## Conclusion
This project offers a detailed time series analysis of **Microsoft's stock price**, highlighting trends, volatility, and providing future forecasts based on statistical modeling. The combination of data visualization, moving averages, and time series forecasting offers actionable insights into stock price movements.
