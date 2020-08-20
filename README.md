# Orderbook-price-prediction

Data:

  -1 second interval data logged on Ethereum over a roughly 18 hour period with volume weighted average price of all limit orders within 1% of current price as an input variable
  
Pre-processing:

  -Shift price forward by t+100 intervals and split train and test data (90% train, 10% test)
  
Model:

  -Two layered Bidrectional LSTM model with 50 nodes and dropout layers
  
Analysis:

  -Clearly cannot accurately predict the future price value 100 seconds in advance, however when compared against the current price, the predicted price realizes trends before they happen, although less than 100 seconds in advance.
