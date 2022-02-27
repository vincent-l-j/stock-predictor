# LSTM Stock Predictor

![deep-learning.jpg](image/deep-learning.jpg)

Due to the volatility of cryptocurrency speculation, investors will often try to incorporate sentiment from social media and news articles to help guide their trading strategies.
One such indicator is the [Crypto Fear and Greed Index (FNG)](https://alternative.me/crypto/fear-and-greed-index/) which attempts to use a variety of data sources to produce a daily FNG value for cryptocurrency.
This project will build and evaluate deep learning recurrent neural network models using both the FNG values and Bitcoin closing prices to determine if the FNG indicator provides a better signal than the normal closing price data.
One model will use the FNG indicators to predict the closing price while the second model will use a window of closing prices to predict the nth closing price.

- - -

## Summary of Findings

> Which model has a lower loss?

The model that was fit using only the closing prices has a lower loss of 0.0882.
The fear and greed fitted model has a loss of 0.2833.

> Which model tracks the actual values better over time?

The closing prices model tracks the actual values better over time.
The fear and greed model predictions remain at less than $3600 even when the actual price reaches over $12000.

> Which window size works best for the model?

After testing window sizes from 1-10, the optimal model was found when the window size was 10.
