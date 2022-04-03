The project:
=============
Secure investment recommendations across multiple categories of securities (stocks, bonds, currency, real estate, precious metals).
---------------
**Our ML models provide you with the safest investment options for the next 30 days based on price and volatility predictions.**

The price prediction model is based on an ensemble learning technique called stacking.
This technique uses predictions of multiple nodes (SVM, Decision Trees, RNNs etc.) and combines them to build a new, more robust model.
For our specific use case, we found that using a stacked LSTM model performs best. We fit this model on the adjusted closing price of the stocks because it's adjusted for factors like dividends, stocks splits and new stock offerings.

The volatility prediction model is based on an SVR-GARCH model with a linear kernel which is applying the Support Vector Regression method to the GARCH model. The model is performing decently since the data set is linearly separable.

Below, you can find some images on our price and volatility predictions for different stocks:

![Apple Stock Price Prediction](https://github.com/stefanzer0/hackaubg4.0/blob/73687e63b5e280d2deba7b229deaf1467d38648d/Apple%20Stock%20Price%20Prediction.png)
![Coca Cola Volatility Training](https://github.com/stefanzer0/hackaubg4.0/blob/f201cbd43b793c9f94ac324336eaab1d24c56fe6/Coca%20Cola%20Volatility%20Training.png)
![P&G Volatility Prediction](https://github.com/stefanzer0/hackaubg4.0/blob/f201cbd43b793c9f94ac324336eaab1d24c56fe6/P&G%20Volatility%20Prediction.png)
