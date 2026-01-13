📈 LLM-Enhanced Stock Price Predictor

Transformer + Local LLaMA-3 Reasoning

🔍 Overview

This project implements a Transformer-based time series model to predict stock prices using historical data and integrates a locally hosted LLaMA-3 model to generate explainable financial reasoning such as market trend, confidence, risks, and Buy/Sell/Hold decisions.

Unlike traditional LSTM-based approaches, this system leverages Transformer encoders for improved long-term dependency modeling and LLM-based interpretability without relying on external APIs.

🧠 Architecture
Historical Stock Prices
        ↓
Feature Scaling
        ↓
Transformer Encoder
        ↓
Price Prediction
        ↓
Evaluation (RMSE, MAE)
        ↓
LLaMA-3 Reasoning Layer

🛠️ Tech Stack

Python

PyTorch

Transformer Encoder

Yahoo Finance (yfinance)

HuggingFace Transformers

Meta LLaMA-3 (Local Inference)

Google Colab (GPU)

📊 Model Evaluation Results
Metric	Value (Typical)
RMSE	~2.0
MAE	~1.7

Results may vary slightly due to random initialization and data updates.

📉 Sample Prediction Output
Last Price: 192.53
Predicted Next Price: 194.11

🧠 LLaMA-3 Reasoning Output (Example)
Trend:
Short-term upward movement is expected.

Confidence:
Medium, based on recent stability and evaluation metrics.

Risks:
Market volatility and macroeconomic uncertainty.

Action:
HOLD

🚀 How to Run

Open llm_stock_predictor.ipynb in Google Colab

Enable GPU: Runtime → Change runtime → GPU

Install dependencies

Login to HuggingFace

Run all cells sequentially

📌 Key Features

Transformer-based stock prediction (LSTM-free)

Proper time-series evaluation (RMSE, MAE)

Local LLaMA-3 reasoning (no API usage)
