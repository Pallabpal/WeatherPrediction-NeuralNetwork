# Weather Forecasting of Kharagpur
## Overview
This project focuses on predicting future weather temperatures and classifying weather conditions for upcoming days using advanced neural networks. We have employed several models, including Recurrent Neural Networks (RNN), XGBoost, and ARIMA, to forecast weather temperature. After comparing their performance, we found that the RNN model provides the most accurate predictions.
## Dataset
Weather data is kept by numerous organisations, including the National Weather Service, Indian Space Research Organization, Indian Meteorological Department, and National Aeronautics and Space Administration (NASA). Storing weather data is important for various reasons other than Weather Forecasting. Weather data is also used to study long-term climate patterns, including trends in temperature, precipitation, and other me- teorological variables. This information is used to develop models of how the climate is changing over time and to understand the impacts of climate change on ecosystems, human health, and infrastructure. Energy companies also require such data to forecast demand for energy, such as electricity or natural gas, based on factors like temperature, humidity, and wind speed. This information is used to manage energy supply and demand more efficiently, which can help to reduce costs and improve reliability. The data for this project has been extracted from the NASA Power API. API stands for Application Programming Interface, which is a set of protocols, routines, and tools for building software applications. APIs allow different software systems to communicate with each other and share data in a standardized way, making it easier to integrate different software components into a cohesive application. Data extracted from this API had 4108 records and 31 features including the date of observation.


## Models
1. Recurrent Neural Network (RNN)
   
The RNN model was found to be the most effective for predicting future weather temperatures. We trained the RNN model on historical weather data and fine-tuned it for optimal performance.

2. XGBoost
   
We also implemented an XGBoost model for comparison. Although it didn't perform as well as the RNN, you can find the code and results in the models folder.

3. ARIMA
   
ARIMA (AutoRegressive Integrated Moving Average) is a traditional time series forecasting method. We included an ARIMA model to compare its performance with our machine learning models.

## RNN model Architecture
The weather prediction model utilizes the LSTM architecture, a type of RNN that is well-suited for sequence prediction tasks. The LSTM cells in the model help capture long-term dependencies in the weather data, allowing for accurate predictions. The model is implemented using the TensorFlow framework, a popular choice for deep learning projects. The follwing link provides a detail Architecture of LSTM model: https://colah.github.io/posts/2015-08-Understanding-LSTMs/

## Prediction
Once the model is trained, it can be used to make weather predictions for future dates. Given the current weather conditions as input, the model generates predictions for the next 15 days. The predicted weather data includes temperature, humidity, wind speed, and precipitation for each day.

![output](https://github.com/Pallabpal/WeatherPrediction-NeuralNetwork/assets/122145541/215b5dd8-898f-428e-8eab-ebb75e310977)
