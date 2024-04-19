# Bike Rental Prediction Project

This repository contains code and data for predicting bike rental counts based on various features like temperature, humidity, and more.

## Project Structure
├── data
│   ├── bike_rental_data.csv       # Raw data containing bike rental records
├── notebooks
│   ├── EDA.ipynb                   # Exploratory Data Analysis notebook
│   ├── Modeling.ipynb              # Model training and evaluation notebook
├── models
│   ├── random_forest_model.pkl     # Trained Random Forest regression model
├── src
│   ├── preprocessing.py            # Data preprocessing module
│   ├── model.py                    # Scripts for model training and evaluation
├── README.md                       # Project overview and guide

## Dataset Description

The dataset (`bike_rental_data.csv`) contains the following features:

- `Date`: Date of rental record
- `Hour`: Hour of the day
- `Temperature`: Temperature in Celsius
- `Humidity`: Humidity percentage
- `Windspeed`: Wind speed in meters per second
- `Visibility`: Visibility in meters
- `Dew_Point_Temperature`: Dew point temperature in Celsius
- `Solar_Radiation`: Solar radiation in MJ/m2
- `Rainfall`: Rainfall in millimeters
- `Snowfall`: Snowfall in centimeters
- `Seasons`: Season of the year (Winter, Spring, Summer, Autumn)
- `Holiday`: Holiday or No holiday
- `Functional_Day`: Functional or Non-functional day

The target variable is `Rented_Bike_Count`, representing the number of bikes rented at each hour.

## Exploratory Data Analysis (EDA)

The `EDA.ipynb` notebook contains exploratory data analysis steps, including:
- Data cleaning (removing outliers, handling missing values)
- Univariate, bivariate, and multivariate analysis
- Correlation analysis with VIF (Variance Inflation Factor)

## Model Training and Evaluation

The `Modeling.ipynb` notebook includes:
- Data preprocessing using `preprocessing.py`
- Model training and evaluation using various regression techniques:
  - Linear Regression
  - K-Nearest Neighbors (KNN) Regression
  - Random Forest Regression

The trained Random Forest model is saved as `random_forest_model.pkl` in the `models` directory.

## Running the Project

To run this project locally:
1. Clone this repository to your local machine.
2. Ensure you have Python installed (Python 3.6 or higher recommended).
3. Install the required packages using `pip install -r requirements.txt`.
4. Navigate to the `notebooks` directory and open Jupyter Notebook.
5. Run the `EDA.ipynb` notebook to perform data analysis.
6. Proceed to the `Modeling.ipynb` notebook for data preprocessing, model training, and evaluation.

