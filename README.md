# Bitcoin Crash: Early Warning System (EWS)

This repository contains the source code and data analysis for a dual-layer predictive framework designed to identify Bitcoin market fragility and forecast extreme price drops.

- Project Overview

This research explores the feasibility of a dual-layer system to improve decision-making during periods of extreme volatility.
Layer 1: Price Forecasting (SARIMA): A regression approach to identify standard market trends.
Layer 2: Early Warning System (EWS): A behavioral classification model designed to detect "fragile" market regimes.

- Key Methodology

Operational Crash Definition: A significant price drop of 20% or more occurring over a future 7-day period.
Feature Engineering: Integration of Market Data (OHLCV), Sentiment (Fear & Greed Index), Social Interest (Google Trends), and Macroeconomic indicators.
Class Imbalance Strategy: Since crashes represent only 1.79% of the data, we implemented Inverse Class Weights in our Logistic Regression to prioritize crash detection.

- Results

EWS Performance: The model achieved a ROC AUC score of 0.70, successfully ranking high-risk days significantly better than a random guess.
Feature Importance: Google Search Interest was identified as the strongest predictor (+1.64), validating the Speculative Bubble Theory.
