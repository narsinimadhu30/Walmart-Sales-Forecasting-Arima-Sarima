# Walmart Weekly Sales Forecasting using Time Series

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Time Series](https://img.shields.io/badge/Model-ARIMA%20%7C%20SARIMA-orange)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## Project Summary:

This project analyzes **Walmart weekly sales** data to extract business insights and forecast future sales using **time series forecasting techniques.**

The dataset contains historical sales information of multiple Walmart stores along with economic and environmental factors such as `Temperature, CPI, and Unemployment`.

## Problem Statement:

A retail store that has multiple outlets across the country are **facing issues in managing the
inventory** - to match the demand with respect to supply

## Dataset Information:

| Feature Name     | Description                                                                  |
| ---------------- | ---------------------------------------------------------------------------- |
| **`Store`**        | `Store number`                                                                |
| **`Date`**         | `Week of sales`                                                                |
| **`Weekly_Sales`** | `Sales for the given store in that week`                                      |
| **`Holiday_Flag`** | `Indicates whether the week includes a holiday (1 = Holiday, 0 = Non-Holiday)` |
| **`Temperature`**  | `Temperature on the day of the sale`                                           |
| **`Fuel_Price`**   | `Cost of the fuel in the region`                                              |
| **`CPI`**          | `Consumer Price Index`                                                         |
| **`Unemployment`** | `Unemployment rate`                                                            |

## The project focuses on:

- Answering key business questions

- Performing exploratory data analysis

- Understanding the effect of external variables on sales

- Building `time series forecasting` models

- Predicting `next 12 weeks` of sales for `each store`.

## Business Problems Solved

The following business questions were analyzed:

1). If the weekly sales are affected by the `unemployment rate`, if yes - which stores
are suffering the most?

2). If the weekly sales show a seasonal trend, when and what could be the reason?

3). Does temperature affect the weekly sales in any manner?

4). How is the `Consumer Price index` affecting the weekly sales of `various stores`?

5). `Top performing stores` according to the historical data.

6). The `worst performing store`, and how significant is the difference between the
`highest and lowest performing stores`.


## Data Analysis:

The project includes detailed **`Exploratory Data Analysis (EDA)`**:

- `Data cleaning and preprocessing`

- `Handling missing values`

- `Feature analysis`

- `Correlation analysis`

- `Store-level performance analysis`

- `Visualizations using plots and charts`

**```Insights were generated to support business decision making.```**

## Time Series Forecasting:

To forecast future sales, the following time series models were implemented:

**```1️). ARIMA (AutoRegressive Integrated Moving Average)```**

**ARIMA** was used to model the trend and past patterns of weekly sales.

It produced:

- **`Lower RMSE`**

- **`Lower MAE`**

indicating better prediction accuracy.

**```2️). SARIMA (Seasonal ARIMA)```**

**SARIMA** captures seasonality patterns in time series data.

It was used to model:

- **Seasonal trends**

- **Periodic patterns in sales**

However:

- **SARIMA** produced `higher RMSE` and `MAE compared to ARIMA`.

- Although **SARIMA captured seasonality better, ARIMA performed better in prediction accuracy**

## Forecasting:

Using the trained models, the project predicts:

**Next 12 weeks of sales for each Walmart store**

This helps businesses with:

- Inventory planning

- Demand forecasting

- Resource allocation

- Promotional planning

## Model Performance Comparison:

  | Model  | Strength                      | Weakness                           |
| ------ | ----------------------------- | ---------------------------------- |
| `ARIMA`  | `Lower RMSE & MAE`            | `May not capture strong seasonality` |
| `SARIMA` | `Captures seasonality patterns` | `Higher prediction error`            |

**Final Conclusion:**
ARIMA performed better overall for this dataset.

## Business Recommendations:

Based on the analysis:

- Stores affected by temperature variations should adjust product inventory accordingly.

- Stores impacted by economic indicators (CPI & unemployment) should implement pricing and promotion strategies.

- Low-performing stores require operational improvements and better demand planning.

- Sales forecasting helps Walmart improve:

  - Inventory management

  - Supply chain planning

  - Promotional campaigns

## Tech Stack:

**Programming Language**
- `Python`

**Libraries Used**

- `Pandas`

- `NumPy`

- `Matplotlib`

- `Seaborn`

- `Statsmodels`
  
- `pmdarima`

- `Scikit-learn`

**Tools**

- `Jupyter Notebook`

- `GitHub`

## Project Structure:

```
walmart-sales-forecasting/
│
├── data/
│   └── walmart_sales.csv
│
├── notebooks/
│   └── walmart_sales_analysis.ipynb
│
├── src/
│   ├── data_preprocessing.py
│   ├── eda_analysis.py
│   ├── arima_model.py
│   └── sarima_model.py
│
├── outputs/
│   └── plots/
│
├── requirements.txt
├── .gitignore
├── LICENSE
└── README.md
```

## How to Run the Project:

### 1️). Clone the Repository

```bash
git clone https://github.com/yourusername/walmart-sales-forecasting.git
```

### 2️). Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️). Run the Notebook

Open the notebook:

```
notebooks/walmart_sales_analysis.ipynb
```

Run it using **Jupyter Notebook or Google Colab**.
notebooks/walmart_sales_analysis.ipynb

## Future Improvements

Possible improvements for this project:

- Implement **SARIMAX with external variables**

- Use **Facebook Prophet forecasting**

- Try **Deep Learning models (LSTM)**
  
- Build an **interactive dashboard**

## Conclusion

This project demonstrates how **time series forecasting models** can help retailers analyze historical sales patterns and predict future demand.

The analysis helps Walmart:

- Understand sales trends

- Identify factors affecting store performance

- Improve decision making through forecasting
