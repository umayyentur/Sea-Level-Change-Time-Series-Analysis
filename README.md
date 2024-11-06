# Sea Level Change Time Series Analysis
This project focuses on analyzing and forecasting global sea level changes using time series analysis techniques. By utilizing historical data on mean sea levels from regions worldwide, this study aims to identify seasonal patterns and trends over the years. The goal is to create an accurate forecast model that captures seasonal behaviors and provides insights into potential future sea level changes.

## Data
The data used in this project was sourced from Kaggle. It contains monthly observations of mean sea levels from various global regions, covering the period from December 1992 to August 2022.


## Objective

The primary objective is to:

* Analyze trends and seasonal patterns in global sea level data.
* Identify the most suitable time series model for forecasting.
* Create accurate forecasts that can help anticipate future sea level changes.


## Methods

* Data Cleaning: Unused columns and missing values were removed to improve data quality.
* Exploratory Analysis: Graphical methods, including time series and seasonal plots, were used to observe trends and seasonal patterns.
* Model Selection: Multiple forecasting models were tested, including mean and seasonal naive (snaive) models.
* Model Evaluation: The models were evaluated based on RMSE and MAPE values on both training and test sets, with additional residual analysis for model validation.
* Box-Cox Transformation: This transformation was applied to further optimize model performance and residual distribution.


## Results

Seasonal Naive Model: The seasonal naive model provided the most accurate forecast with the lowest error metrics, indicating strong alignment with seasonal patterns in the data.
Residual Analysis: Although the seasonal naive model performed well in predicting trends, residual analysis indicated some autocorrelation, suggesting that more advanced models might capture additional dependencies in the data.
Conclusion

The seasonal naive model was identified as the best-performing model for this dataset. It effectively captures seasonal variations in sea level changes over the years. However, residual patterns suggest that more complex models could be explored to improve forecasting accuracy further.

### Requirements

R Libraries: ggplot2, fpp2, dplyr, lubridate, GGally, olsrr
Install the required libraries:

install.packages(c("ggplot2", "fpp2", "dplyr", "lubridate", "GGally", "olsrr"))
Usage

To run the analysis, load the R script provided, ensuring the dataset path is correctly specified in the read.csv function. The script will clean, preprocess, and perform the time series analysis on the dataset.

### Future Work

Exploring more advanced models (e.g., ARIMA, Prophet) to further reduce residual autocorrelation.
Testing the model on additional regions and different time frames to validate generalizability.
