# README: Google Search Traffic Analysis

## Overview
This project aims to analyze Google search traffic data for MercadoLibre to identify unusual patterns, seasonal trends, and correlations with stock price movements. Additionally, a time series forecasting model is developed to predict future search traffic trends.

## Objectives
1. **Identify Unusual Patterns:** Explore the search traffic data for anomalies, particularly around May 2020 when MercadoLibre released its quarterly financial results.
2. **Seasonality Analysis:** Determine seasonal patterns in the search data to guide marketing efforts.
3. **Stock Price Correlation:** Examine the relationship between search traffic and stock price movements.
4. **Time Series Forecasting:** Develop a Prophet-based model to forecast search traffic.

---

## Prerequisites
To run this analysis, you need:
- Python 3.8 or above
- Libraries: `pandas`, `matplotlib`, `fbprophet` (or `prophet`), `numpy`
- Google search data and stock price data in CSV format

---

## Project Steps

### Step 1: Find Unusual Patterns
1. Load the search traffic data.
2. Slice the data to the month of May 2020.
3. Visualize hourly search traffic for May 2020.
4. Compare total search traffic for May 2020 to the median monthly traffic.

### Step 2: Analyze Seasonality
1. Group and analyze search traffic by:
   - **Hour of the day**
   - **Day of the week**
   - **Week of the year**
2. Visualize trends to identify peaks and patterns.

### Step 3: Relate Search Traffic to Stock Price
1. Load stock price data and merge it with the search traffic data.
2. Add derived metrics:
   - Lagged search traffic
   - Stock volatility (4-hour EWMA)
   - Hourly stock returns
3. Visualize trends to identify correlations.

### Step 4: Time Series Forecasting
1. Prepare the search traffic data for the Prophet model.
2. Fit the model and generate forecasts for the next 7 days.
3. Visualize the forecast and time series components to analyze patterns.

---

## Files
1. **google_search_data.csv:** Contains hourly Google search traffic data.
2. **stock_price_data.csv:** Contains hourly stock price data for MercadoLibre.
3. **analysis_script.py:** Python script for the entire analysis.
4. **README.md:** Documentation for the project.

---

## Usage
1. Clone the repository and place the required CSV files in the project directory.
2. Install the required Python libraries:
   ```bash
   pip install pandas matplotlib fbprophet
   ```
3. Run the analysis script:
   ```bash
   python analysis_script.py
   ```

---

## Results
1. **Unusual Patterns:** Insights into how search traffic changes around significant financial events.
2. **Seasonality:** Identification of peak hours, days, and weeks for search traffic.
3. **Stock Price Correlation:** Evidence of relationships between search trends and stock price movements.
4. **Forecasting:** Predictions for future search traffic to support decision-making.

---

## Authors
ESHUMAEL MANHANZVA
eshumaelm@yahoo.co.uk


