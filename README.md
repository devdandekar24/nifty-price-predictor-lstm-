# NIFTY Price Predictor using LSTM and Walk-Forward Analysis

This project uses deep learning models to predict future NIFTY50 stock index prices. The primary model is an LSTM-based neural network, with comparisons against a Bidirectional LSTM and a Walk-Forward Analysis (WFA) approach.

## 📊 Models Used

- **LSTM**: Basic Long Short-Term Memory model
- **Bidirectional LSTM**: Improved version for sequence learning
- **Walk-Forward Analysis (WFA)**: Used to simulate real-world prediction where the model is retrained incrementally

## ✅ Results (Evaluation Metrics)

| Model             | RMSE (in ₹) | R² Score |
|------------------|----------------|------------|
| LSTM             | 427.61         | 0.9778     |
| Bidirectional LSTM | 393.83         | 0.9812     |
| Walk-Forward Analysis | 265.39         | 0.9439     |

> Lower RMSE and higher R² indicate better performance.

## 🧠 Features Used

- Open, High, Low, Volume
- Moving Averages (MA10, MA20)
- Daily Return
- Lagged Close Prices (1-day, 5-day)
- Rolling Volatility

## 🔧 Tools & Libraries

- Python, Pandas, NumPy, Matplotlib
- TensorFlow / Keras (for LSTM)
- Scikit-learn (scalers, metrics)
- Yahoo Finance (for NIFTY data)

## 📈 Target

The models are trained to predict the **next day's closing price** of the NIFTY50 index.

## 💾 Model Saving

- Models are saved using `.keras` format
- Scalers are saved using `joblib`
- Supports reloading models and predicting unseen data (like future dates)

## 📅 Future Scope

- Hyperparameter tuning
- Incorporation of macroeconomic indicators
- Web-based dashboard deployment

---

**Made for educational and portfolio purposes.**

