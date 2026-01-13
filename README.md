# LLM-Enhanced Stock Price Predictor

Transformer + Local LLaMA-3 Reasoning

# Overview

This project implements a Transformer-based time series model to predict stock prices using historical data and integrates a locally hosted LLaMA-3 model to generate explainable financial reasoning such as market trend, confidence, risks, and Buy/Sell/Hold decisions.

Unlike traditional LSTM-based approaches, this system leverages Transformer encoders for improved long-term dependency modeling and LLM-based interpretability without relying on external APIs.

# Architecture

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

# Tech Stack

Python
PyTorch
Transformer Encoder
Yahoo Finance (yfinance)
HuggingFace Transformers
Meta LLaMA-3 (Local Inference)

# Model Evaluation Results
Metric	Value (Typical)
MSE : 131.91419982910156
RMSE: 11.485390712949279
MAE : 10.575881958007812

Results may vary slightly due to random initialization and data updates.

# Sample Prediction Output
Last Price: 249.292511
Predicted Next Price: 253.31201

# LLaMA-3 Reasoning Output (Demo)
Trend:
Short-term upward movement is expected.

Confidence:
Medium, based on recent stability and evaluation metrics.

Risks:
Market volatility and macroeconomic uncertainty.

Action:
HOLD

# Key Features

Transformer-based stock prediction (LSTM-free)
Proper time-series evaluation (MSE, RMSE, MAE)
Local LLaMA-3 reasoning (no API usage)
