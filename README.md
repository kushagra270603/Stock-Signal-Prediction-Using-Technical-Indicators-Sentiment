Stock Signal Prediction Using Technical Indicators & Sentiment

This repository contains the complete implementation of our research project titled:

**"Multimodal Stock Signal Prediction for Apple Inc.: A Hybrid Machine Learning Approach Integrating Technical Indicators and Social Media Sentiment"**

## 📘 Abstract

This project proposes a novel hybrid framework combining classical technical indicators and Twitter-based sentiment analysis for predicting Buy, Hold, or Sell signals for Apple Inc. (AAPL). The model integrates:

- Daily technical indicators (RSI, MACD, Bollinger Bands, etc.)
- Daily sentiment scores (calculated using the VADER model)
- Predictive models: **XGBoost**, **CNN-LSTM**, and **Gradient Boosting Classifier**
- Rule-based signal generation strategy

## 📁 Folder Structure

- `data/`: Contains the sentiment and stock price datasets
- `notebooks/`: Jupyter notebooks for data processing and modeling
- `figures/`: Plots for model performance and results
- `paper/`: PDF of the IEEE-style research paper

## 🔍 Dataset

- `Apple.csv`: Tweet-based sentiment scores (labels: -1, 0, +1)
- `Apple_dataset_technical_indicators.csv`: Historical stock prices and computed indicators

## ⚙️ Models Used

- **XGBoost Regressor** for stock price prediction
- **CNN-LSTM Hybrid** for deep learning-based price prediction
- **Gradient Boosting Classifier** for sentiment classification

## 📈 Evaluation Metrics

- Price Prediction: RMSE, MAE, MSE
- Sentiment Classification: Accuracy, Precision, Recall, F1-Score
- Signal Generation: Rule-based mapping of model outputs

## 📊 Results Summary

- XGBoost achieved lowest MSE
- CNN-LSTM yielded better RMSE/MAE
- Signals are realistically distributed across Buy/Hold/Sell

## 🧠 Future Work

- Add FinBERT sentiment model
- Incorporate news data (e.g., Reddit, financial headlines)
- Live backtesting with trading APIs

## 📦 Installation

```bash
git clone https://github.com/yourusername/FinSent-TI.git
cd FinSent-TI
pip install -r requirements.txt
