# Medicine Sales Forecasting

This project focuses on forecasting the sales of various medicines using the Prophet forecasting model. The goal is to provide accurate predictions to help pharmacies and healthcare providers manage their inventory more efficiently.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Training and Forecasting](#model-training-and-forecasting)
- [Results](#results)
- [Contributing](#contributing)


## Introduction
The accurate forecasting of medicine sales is crucial for maintaining adequate inventory levels and ensuring that patients have access to the medications they need. This project utilizes historical sales data to predict future sales using the Prophet forecasting model.

## Dataset
The dataset used for this project includes historical sales data from various pharmacies. The data includes information such as:
- Date of sale (`ds`)
- Medicine name (`medicine_name`)
- Total sales (`total_sales`)

The data should be grouped by medicine and date, summing up the total sales for each day per medicine.

## Installation
To run this project, you need to have Python installed along with the necessary libraries. You can install the required libraries using the following command:

```bash
pip install -r requirements.txt ```

## Usage
- Clone the repository
- Navigate to the project directory
- Ensure all dependencies are installed

## Model Training and Forecasting
The model training and forecasting process involves the following steps:

- Initializing dictionaries to store models and forecasts for each medicine.
- Getting the list of unique medicines from the dataset.
- Fitting the Prophet model for each medicine:
- Filtering the data for the current medicine.
- Initializing and fitting the Prophet model.
- Creating a DataFrame with future dates to make predictions.
- Making predictions and storing the model and forecast.

You can run the model training and forecasting script by executing:
```bash
python forecast_sales.py

## Results
The forecasts for each medicine, along with the corresponding plots, will be displayed. These plots include the sales forecast and the forecast components (trend, weekly, and yearly seasonality).

## Contributing
Contributions are welcome! If you have any ideas or suggestions to improve the project, please feel free to open an issue or submit a pull request.
