# Microsoft Stock Time Series Analysis

## Project Overview
This project focuses on analyzing Microsoft (MSFT) stock price trends from 1986 to 2025 using time series analysis. It includes various methods like decomposition,Heatmap, volatility analysis, and forecasting, with the aim to gain insights into stock price movements and make future predictions.

## Dataset Source
- Microsoft stock data (1986–2025)
- [Kaggle - Microsoft Stock Data](https://www.kaggle.com/datasets/umerhaddi/microsoft-stock-data-2025)

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
    pip install pandas numpy matplotlib seaborn plotly statsmodels mplfinance
    ```

2. **Download the dataset**:
   - Download the dataset from [Kaggle - Microsoft Stock Data](https://www.kaggle.com/datasets/umerhaddi/microsoft-stock-data-2025) or upload the CSV file locally.

3. **Run the analysis**:
   - Clone this repository or open the Jupyter Notebook.
   - Ensure the dataset is placed in the same directory as the notebook.
   - Run the cells to perform exploratory data analysis, time series decomposition, volatility analysis, and forecasting.

4. **Interactive Visualization**:
   - The project includes interactive charts created with Plotly for deeper insights into Microsoft stock trends and forecasts.

## Code Implementation

### Import Libraries
The following libraries are used for the analysis:

- **Core Libraries**: Pandas and NumPy for data manipulation and handling.
- **Visualization Libraries**: Matplotlib and Seaborn for static plots, Plotly for interactive visualizations.
- **Time Series and Stats Libraries**: Statsmodels for time series analysis and ARIMA forecasting.

### Load Data and Initial Exploration
The dataset is loaded from a CSV file. The first few rows, data types, and summary statistics are displayed. Missing values are checked, and the `Date` column is converted to a datetime format.

### Data Resampling and Date Range
Data is resampled to a monthly frequency and the average closing price is calculated for each month. A date range is also generated for the given time period.

### Handling Holidays
US federal holidays are generated using `USFederalHolidayCalendar`. These holidays are useful for understanding the market's performance around holidays.

### PeriodIndex for Monthly Aggregation
The data is aggregated by month using a `PeriodIndex` and the average closing price for each month is calculated.

### Timezone Handling
The data's timezone is localized to UTC and then converted to US Eastern time.

### Visualization and Analysis
Various visualizations are generated:
- **Closing Price Plot**: A plot showing the closing prices of MSFT stock over time.
- **Heatmap**: A heatmap showing the correlation between different stock features.
- **Daily Returns**: A plot showing daily percentage returns of the stock.
- **Moving Averages**: 50-day and 200-day moving averages are calculated and plotted along with the closing prices.

### ARIMA Forecasting
The ARIMA model is used to forecast the next 30 business days of Microsoft stock prices. The forecasted values are plotted along with the actual closing prices.

### Candlestick Chart Visualization
A candlestick chart is generated using `mplfinance` for the last 100 days of data, which provides insights into daily stock price movements.

### Interactive Charts
Interactive visualizations of the closing price and moving averages are created using Plotly. These charts allow users to zoom in and explore trends interactively.

## Conclusion
This analysis demonstrates how time series methods and statistical modeling techniques, such as ARIMA, can be applied to forecast stock prices. The interactive visualizations and insights provided offer a comprehensive view of Microsoft stock's historical trends, volatility, and future predictions.

---
This document provides a summary of the Microsoft Stock Time Series Analysis project. All code and data used in this analysis are available in the repository.
