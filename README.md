# Anomaly Detection in Time Series Data: Catfish Company Dataset

## Overview
This project focuses on detecting anomalies in the sales data of a catfish company over time. Three different anomaly detection methods are employed: deviation model, seasonal model, and SARIMA model. The aim is to identify unusual patterns or outliers in the sales data that deviate significantly from the expected behavior.

## Dataset
The dataset used in this project contains historical sales data of the catfish company. It includes timestamps and corresponding sales figures over a certain period.

## Anomaly Detection Methods

### Deviation Model
The deviation model involves calculating deviations of observed data points from a baseline or expected value. An anomaly is detected when the deviation exceeds a certain threshold.

### Seasonal Model
The seasonal model takes into account the seasonal patterns in the data. Anomalies are identified based on deviations from the expected seasonal behavior.

### SARIMA Model (Seasonal Autoregressive Integrated Moving Average)
The SARIMA model is a more sophisticated approach that incorporates both seasonal and autoregressive components. It models the trend, seasonality, and noise in the data to forecast future values. Anomalies are detected based on significant deviations between observed and forecasted values.

## Implementation
The implementation involves the following steps:

1. **Data Preprocessing**: Load the dataset and preprocess it if necessary (e.g., handling missing values, resampling).

2. **Model Training**:
   - **Deviation Model**: Calculate deviations from the mean or median.
   - **Seasonal Model**: Decompose the time series into trend, seasonal, and residual components using techniques like seasonal decomposition.
   - **SARIMA Model**: Fit a SARIMA model to the data to capture its temporal patterns.

3. **Anomaly Detection**:
   - **Deviation Model**: Flag data points with deviations above a predefined threshold as anomalies.
   - **Seasonal Model**: Identify anomalies based on significant deviations in the seasonal component.
   - **SARIMA Model**: Detect anomalies by comparing observed values with forecasted values using the SARIMA model.

4. **Evaluation**: Evaluate the performance of each anomaly detection method using appropriate metrics (e.g., precision, recall, F1-score).

5. **Visualization**: Visualize the detected anomalies and their corresponding timestamps in the sales data.

## Results
The results of the anomaly detection process will provide insights into unusual patterns or outliers in the catfish company's sales data. By employing multiple anomaly detection methods, we can gain a comprehensive understanding of the data's behavior and identify potential issues or opportunities for further investigation.

## Conclusion
Anomaly detection in time series data is a crucial task for detecting abnormalities or irregularities that may indicate underlying problems or interesting phenomena. By leveraging deviation, seasonal, and SARIMA models, we can effectively identify anomalies in the catfish company's sales data and take appropriate actions based on the insights gained.
