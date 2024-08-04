# soil-moisture-analysis
This model which predicts and automates to irrigate or drain water from field using Gradient Boosting Regressor model and linear regression model based upon the data of the water level or moisture level in soil.this system performs soil moisture analysis using synthetic datasets generated for three different scenarios: irrigation, drainage, and optimal conditions. It uses Gradient Boosting Regressor to model the relationship between temperature, humidity, and soil moisture. The system includes data generation, model training, and decision-making for soil moisture management.

## Contents

1. **Data Generation**:
   - Generates synthetic datasets for irrigation, drainage, and optimal conditions.
   - Saves datasets as CSV files (`irrigation_dataset.csv`, `drainage_dataset.csv`, `optimal_dataset.csv`).

2. **Data Analysis**:
   - Loads the irrigation dataset.
   - Splits the data into training and testing sets.
   - Performs hyperparameter tuning using GridSearchCV on a Gradient Boosting Regressor.
   - Evaluates model performance using Mean Squared Error (MSE) and R-squared metrics.
   - Makes decisions based on soil moisture thresholds for irrigation and drainage.

3. **Visualization**:
   - Plots actual vs. predicted soil moisture values.

4. **Decisions**:
   - Provides decisions based on predictions (whether to irrigate, drain, or maintain optimal soil moisture).

## Usage

1. **Run the Notebook**:
   - Ensure all dependencies are installed.
   - Execute each cell to generate data, train the model, and evaluate results.

2. **Modify Thresholds**:
   - Adjust `irrigationThreshold` and `drainageThreshold` as needed based on specific requirements.

## Dependencies

- `numpy`
- `pandas`
- `scikit-learn`
- `matplotlib`

## License

This notebook is licensed under the MIT License.
