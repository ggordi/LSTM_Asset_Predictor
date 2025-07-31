# LSTM_Asset_Predictor
Time Series Modeling for Buy/Sell Prediction

This project is in-progress.

## Project Organization
Historical daily OHLCV (open, high, low, close, & volume) data from which technical indicators were derived are located in the .csv files in `/5_day_data`. This folder contains files whose target variables are determined by looking ahead 5 days for each data point - if there is at least a 1% price change between the entrypoint and the exitpoint 5 days ahead, the data point is labeled as a buy, sell, or neutral if there isn't at least a 1% movement. These labels are manifested as integers of either 1, -1, or 0 respectively. The notebook used to obtain this data is located in `/notebooks/asset_ohlc_data_collection.ipynb`. 
