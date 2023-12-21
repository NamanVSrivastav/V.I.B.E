# V.I.B.E: Virtual Intelligence for Business Enhancement 


Stock prediction using Neural Networks, specifically Long Short-Term Memory (LSTM) networks, involves applying advanced machine learning techniques to forecast future stock prices based on historical data. LSTMs, a recurrent neural network (RNN), are well-suited for time-series data like stock prices due to their ability to capture long-term dependencies and patterns in sequential information.

In this approach, historical stock price data, including relevant features such as Close price and Market Average for various intervals (e.g., 100 days, 200 days), is utilized. The data can be conveniently fetched by specifying a date range and an 80-20 split is employed for training and testing, respectively.

1. **Data Preprocessing:** Historical stock data is preprocessed to remove noise, handle missing values, and scale the data appropriately for input into the neural network.

2. **Model Architecture:** The LSTM neural network is designed with input layers, LSTM layers, and dropout layers to prevent overfitting and output layers. The architecture is configured to capture and learn temporal dependencies in the data.

3. **Training:** The model is trained on historical data, and during this process, it adjusts its internal parameters to minimize the difference between predicted and actual stock prices.

4. **Validation and Testing:** The trained model is validated on a separate dataset to ensure it generalizes well to new, unseen data. After validation, the model can be used to make predictions on future stock prices.

5. **Prediction:** The trained LSTM model can then be deployed to predict future stock prices based on new input data. These predictions provide insights that investors and traders can use to inform their decision-making processes.

*It's important to note that while neural networks, specifically LSTMs, have shown promise in capturing complex patterns in stock data, stock markets are inherently unpredictable, and predictions are subject to various uncertainties. Additionally, the success of the model depends on the quality and relevance of the input features, the amount of historical data available, and the continuous adaptation of the model to changing market conditions.*

---
*Database*
In this stock prediction model, the historical stock price data is sourced from the Yahoo Finance API (yfinance). Yahoo Finance provides a comprehensive and reliable database that includes a wealth of financial information. The data is retrieved by specifying a date range, allowing for the selection of a relevant time frame for training and testing the neural network.

The chosen parameters for the stock data include the Close price, which represents the final traded price of a stock within a given trading day, and the Market Average calculated over various intervals, such as 100 days and 200 days. These parameters play a crucial role in capturing trends and patterns in the stock market.

The utilization of yfinance simplifies the data acquisition process, providing a seamless interface to access historical stock prices and related financial metrics. It enables researchers and practitioners to focus on developing and evaluating predictive models without the complexity of manual data collection and preprocessing.

It's important to note that the accuracy of the model is not only dependent on the architecture of the neural network but also on the quality and representativeness of the historical data. The choice of an appropriate date range and relevant parameters is fundamental to ensuring the model's effectiveness in capturing the underlying patterns in the stock market dynamics.

*Accuracy Percentage*
The model's accuracy is assessed using metrics such as Mean Squared Error (MSE), providing insights into the predictive performance of the model. Additionally, an "Accuracy Percentage" is calculated for illustrative purposes, although it's important to note that this is not a standard metric for regression tasks.
*mean_squared_error(MSE)*: 14392428.855714077
