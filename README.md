# Vehicle Price Predictor: Linear Regression Analysis

## Project Overview
This project applies statistical modeling to real-world automotive data to determine the strongest driving factors behind a vehicle's market price. By leveraging linear regression, this analysis evaluates multiple vehicle characteristics to identify which metric provides the most accurate price prediction.

## Business Application
Understanding the variables that impact depreciation and market value is critical for dealership pricing strategies, insurance valuation, and consumer financing. This script automates the exploratory data analysis (EDA) process, instantly identifying the most statistically significant variable to optimize pricing models.

## Technical Stack
* **Language:** Python
* **Libraries:** Pandas (Data manipulation), SciPy (Statistical modeling/Regression), Matplotlib (Data visualization)
* **Environment:** Jupyter Notebook

## Methodology
The script runs a comparative linear regression analysis on four distinct independent variables against the dependent variable (`car_price`):
1. Engine Displacement
2. Mileage
3. Top Speed
4. Maintenance Interval

For each model, the program calculates the **R-squared value, P-value, Slope, and Intercept**, generates a scatter plot with a line of best fit, and predicts the price for a sample input. 

## Key Findings
* The script programmatically evaluates all models and returns the strongest predictor based on the highest R-squared value.
* Missing data points (`NaN`) are dynamically handled and dropped per-variable to ensure high-integrity regression outputs without breaking the dataset.

## How to Run
1. Clone this repository.
2. Ensure you have the required libraries installed: `pip install pandas scipy matplotlib`.
3. Verify that the `car_data.csv` file is located in the `/data` directory.
4. Run the Jupyter Notebook. The outputs will print to the console, and visualization plots will automatically save to the `/images` directory.
