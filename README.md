# Stock Price Prediction using RNN (LSTM)

This project demonstrates the use of Recurrent Neural Networks, specifically Long Short-Term Memory (LSTM) models, to predict stock prices of major technology companies. The model is trained on historical closing prices to learn time-dependent patterns and forecast future values.

## Project Overview
- ✅ Clean and preprocess stock data  
- ✅ Generate supervised learning sequences for training  
- ✅ Build and train an LSTM-based RNN model per company  
- ✅ Evaluate model using RMSE and visualize predictions  

The prediction task is performed independently for the following companies:
- **Google**
- **Amazon**
- **IBM**
- **Microsoft**

## Dataset Details
Each dataset contains daily stock data including:
- `Date`
- `Open`, `High`, `Low`, `Close`, and `Volume`

Only the `Close` price is used for training and prediction.

## Model Architecture
- Model: **LSTM-based Recurrent Neural Network**
- Layers:
  - 1–2 LSTM layers
  - Dense output layer
- Optimizer: `Adam`
- Loss Function: `Mean Squared Error`
- Evaluation Metric: Root Mean Squared Error (RMSE)

## Model Performance Summary

| Company     | Epochs | Validation Loss | RMSE (Approx) | Performance |
|-------------|--------|------------------|----------------|-------------|
| Google      | 50     | ~641.98          | ~25.33         | Moderate    |
| Amazon      | 50     | ~669.73          | ~25.88         | Moderate    |
| IBM         | 50     | ~11.23           | ~3.35          | High        |
| Microsoft   | 50     | ~9.65            | ~3.10          | High        |

> ✅ Microsoft and IBM models showed excellent alignment between predicted and actual values.

## Visual Insights
Each model includes a plot comparing actual vs predicted stock prices. These help visualize how closely the model tracks real-world trends. The IBM and Microsoft models demonstrate especially tight fits.

## How to Run

1. Clone this repository or download the notebook.  
2. Install required packages:  
   `pip install tensorflow pandas matplotlib numpy scikit-learn`  
3. Launch the notebook:  
   `jupyter notebook RNN_Assg_Stock_Price_Prediction_ProjeshKumarMondal_RajSrivastava.ipynb`  
4. Run cells sequentially. Switch the stock symbol to train models for different companies.

## Conclusion
The LSTM-based models effectively learned temporal patterns in stock price data. The results indicate strong predictive performance, particularly for IBM and Microsoft, with low validation loss and RMSE. In contrast, Google and Amazon showed moderate performance, likely due to greater volatility in their time series data.

This reinforces the power of LSTMs for time-series forecasting while also highlighting opportunities for further enhancement—such as incorporating additional financial indicators, longer lookback windows, or experimenting with hybrid or attention-based models.

## Contributors
- **Projesh Kumar Mondal**
- **Raj Srivastava**

---

**Onwards and Upwards 🚀**
