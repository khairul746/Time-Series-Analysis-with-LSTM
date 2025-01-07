# Time Series Analysis with LSTM

## Project Overview
In the dynamic world of finance, the ability to accurately predict stock prices holds immense value for investors, traders, and financial institutions. This project delves into the realm of stock price forecasting using Long Short-Term Memory (LSTM) networks, a powerful class of neural networks capable of capturing long-term dependencies in time series data.

The trained LSTM model showed excellent performance in predicting stock prices, achieving a root mean squared error (RMSE) of 126.08. This metric indicates the model's ability to accurately track price trends and patterns. Visualization of predicted and actual prices reveals the model's effectiveness in capturing short-term fluctuations and long-term trends, even though some timescales appear less convincing.

## Data
The dataset used in this project is from Yahoo Finance. It includes historical stock price data, comprising:
- **Open, High, Low, Close Prices**
- **Volume Traded**
- **Date and Time Index**

## Methodology
- **Data Preprocessing** : Created sequences of past prices as input for the model.
- **Define the Model** : Built an LSTM network with the following structure:
  - input_size: Dimensionality of the input features.
  - hidden_size: Number of units in the hidden layer of the LSTM cell.
  - output_size: Dimensionality of the output (number of predicted values).
  - num_layers: Number of stacked LSTM layers.
- **Model Training** :
  - Loss function: Mean Squared Error (MSE)
  - Optimizer: Adam
  - Training split: 2/3 training, 1/3 testing
  - Epochs: 1000
- **Perfomance Evaluation** :
  - Metric: Root Mean Squared Error (RMSE)
  - Visual comparison between predicted and actual stock prices. 

## Results
**Model Performance:**
  - Achieved an RMSE of **126.08**, indicating strong predictive capabilities.
  
**Visualization:**
  - The predicted prices closely follow actual price trends and patterns.
  - Effectively captures short-term fluctuations and long-term trends.
  - Minor deviations observed in some time scales, highlighting areas for improvement.
    ![stock_price_result](https://github.com/user-attachments/assets/25e97bc4-81ea-4631-8921-5a105097c172)

## Future Scope
1. **Incorporating Additional Features:**
   - Include macroeconomic indicators such as interest rates and GDP data.
   - Integrate social sentiment analysis from platforms like X.

2. **Improving Model Performance:**
   - Experiment with advanced architectures such as Bidirectional LSTMs or Transformers.
   - Conduct hyperparameter tuning for optimization.

3. **Deployment:**
   - Develop a web application or dashboard for real-time stock price predictions.

4. **Exploring Other Markets:**
   - Apply the model to different markets, including cryptocurrency and forex.

---

## Conclusion
This project demonstrates the potential of LSTM networks for stock price forecasting. While the model shows strong predictive performance, there remains room for improvement, particularly in capturing less obvious patterns. Future iterations will focus on expanding the feature set and optimizing the model further.
