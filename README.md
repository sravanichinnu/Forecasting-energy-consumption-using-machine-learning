# Forecasting-Energy-Consumption-Using-Machine-Learning

## Project Overview
This project uses historical time-series data to forecast energy consumption with machine learning models. Accurate energy demand forecasting helps power providers optimize operations, reduce costs, and support sustainability by minimizing overproduction.

## Research Questions
1. Can machine learning models predict future energy consumption with high accuracy using historical data?
2. How do different modeling approaches (RNN, LSTM, XGBosot) compare in terms of forecast error?

## Data Description
- Source: PJW (Eastern Interconnection grid, USA)
- Period: 2004 - 2018
- Granularity: Hourly energy consumtpion (MW)

## Methods & Statistical Analysis
### Exploratory Data Analysis
- Visualized long-term trends and seasonal patterns.
- Checked for missing values & outliers.

### Feature Engineering
- Created lag features to capture temporal dependencies.
- Extracted day of week, month, and hour as categorical predictors.

### Modeling & Evaluation
| Model   | Description                               | Evaluation Metric |
| ------- | ----------------------------------------- | ----------------- |
| RNN     | Captures sequential patterns              | RMSE              |
| LSTM    | Handles long-term dependencies            | RMSE              |
| XGBoost | Tree-based regressor with lagged features | RMSE              |

## Results
| Model   | RMSE      |
| ------- | --------- |
| **RNN** | **0.031** |
| LSTM    | 0.041     |
| XGBoost | 0.055     |

### RNN achieved the best performance, effectively capturing temporal dependencies.

## Visualization
### Energy Forecast Plot
- The plot shows actual vs predicted energy consumption.
- Predictions closely follow real trends, with minor deviations on sharp peaks.

## Interpretation & Implications
- Machine learning, especially RNNs, can reliably forecast energy demand.
- Power Utilities can use such models to:
  - Optimize grid operations by aligning production with demand.
  - Reduce operational costs by avoiding overproduction.
  - Advance environmental goals through efficient energy use.
 
## Technologies Used:
- Python: Pandas, NumPy, Matplotlib
- Machine learning: TensorFlow, Keras (RNN, LSTM), XGBoost, Scikit-learn
- EDA & Visualization: Matplotlib
- Evaluation: RMSE for regression accuracy.

## Conclusion
This project demonstrates how machine learning models- especially RNNs- can effectively predict energy demand, helping utilities improve planning, reduce costs, and meet environmental targets.
