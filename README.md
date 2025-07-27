
# 🥑 Avocado Price Forecasting with Prophet

This project explores avocado prices in the United States and uses the **Prophet** library to forecast future price trends. The dataset used is from Kaggle and contains historical pricing and volume data for avocados sold across multiple regions.

---

## 📊 Dataset

- **Source**: [Avocado Prices | Kaggle](https://www.kaggle.com/datasets/neuromusic/avocado-prices)
- **Fields**: Date, AveragePrice, Total Volume, Region, Avocado Type (Conventional or Organic)

---

## 🎯 Project Objectives

- Perform time series forecasting on avocado prices
- Understand price behavior over time
- Forecast future average prices using Prophet
- Visualize trends and seasonality

---

## 🔍 What the Project Does

### 1. Data Loading & Exploration
- Loaded the avocado dataset into a Pandas DataFrame
- Checked for missing values and column types
- Explored unique values across regions and avocado types

### 2. Data Filtering & Preparation
- Focused on **Conventional avocados** in a specific region (e.g., "TotalUS")
- Renamed columns to match Prophet’s expected input format:
  - `ds`: Date
  - `y`: Average Price

### 3. Data Visualization
- Plotted historical price trends
- Used Seaborn and Matplotlib to visualize pricing over time
- Analyzed price seasonality and trends

### 4. Forecasting with Prophet
- Initialized and trained a Prophet model
- Generated a future dataframe (e.g., 365 days ahead)
- Forecasted avocado prices using Prophet’s `.predict()` method

### 5. Forecast Visualization
- Plotted:
  - Forecasted price curve with uncertainty intervals
  - Seasonality trends (weekly/yearly components)
- Interpreted insights from the model’s trend and seasonality

---

## 🛠️ Technologies Used

- Python 3
- pandas & NumPy
- matplotlib & seaborn
- Prophet

---

## 🚀 How to Run

1. Upload or clone the notebook into Google Colab or Jupyter.
2. Install Prophet (only needed once):

```python
!pip install prophet
