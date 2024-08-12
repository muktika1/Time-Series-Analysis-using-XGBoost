# Time-Series-Analysis-using-XGBoost

This project involves the analysis and prediction of PJME (PJM Electric) energy consumption using time series data. The dataset contains hourly energy usage data, which is processed to identify patterns and make future predictions. The project implements XGBoost regression, feature engineering, and outlier removal to enhance model performance.
The dataset used in this project is sourced from the PJME hourly energy consumption records, which includes timestamped data representing energy usage in megawatts (MW). The data is indexed by datetime, enabling the extraction of various temporal features essential for forecasting.

## Part 1: Initial Analysis and Model Training
1. **Data Loading and Visualization**:
   - Load the PJME hourly energy consumption data from a CSV file.
   - Visualize the energy consumption trends over time.

2. **Train/Test Split**:
   - Split the dataset into training and testing sets, using data prior to January 1, 2015, for training.

3. **Feature Creation**:
   - Create time series features such as hour, day of the week, month, and year.

4. **Model Training**:
   - Train an XGBoost regressor model to predict energy consumption.
   - Evaluate the model performance using RMSE (Root Mean Square Error).

## Part 2: Outlier Removal, Feature Engineering, and Cross-Validation
1. **Outlier Detection**:
   - Visualize and remove outliers from the dataset.

2. **Feature Engineering**:
   - Add lagged features to the dataset for improved forecasting accuracy.

3. **Cross-Validation**:
   - Implement time series cross-validation using `TimeSeriesSplit` to validate the model's performance across different time frames.

4. **Future Predictions**:
   - Retrain the model using all available data and generate future energy consumption predictions.
