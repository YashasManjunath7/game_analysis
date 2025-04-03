# Steam Game Analytics and Recommendation Platform

This project is an interactive **Dash web application** that analyzes Steam game data, offering insights into ratings, pricing trends, and game success while providing recommendations and predictive analytics. Built in Python, it integrates data preprocessing, statistical analysis, machine learning models, and visualizations using libraries like Pandas, Scikit-learn, Plotly, and Dash.

---

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Dependencies](#dependencies)
- [Detailed Code Breakdown](#detailed-code-breakdown)
  - [Imports](#imports)
  - [Data Preprocessing](#data-preprocessing)
  - [Rating Analysis](#rating-analysis)
  - [Price/Discount Trends](#pricediscount-trends)
  - [Recommendation System](#recommendation-system)
  - [Success Prediction](#success-prediction)
  - [Steam Deck Impact](#steam-deck-impact)
  - [Tag Prediction](#tag-prediction)
  - [Dynamic Pricing](#dynamic-pricing)
  - [Dash Application](#dash-application)
- [Setup and Usage](#setup-and-usage)
- [Potential Enhancements](#potential-enhancements)

---

## Project Overview

The Steam Game Analytics and Recommendation Platform is designed to process a Steam game dataset (e.g., `games.csv`) and deliver an interactive dashboard. Users can input a game title, price, and discount percentage to explore detailed analytics and predictions. The application combines robust data preprocessing with advanced analytics, including time-series decomposition, statistical hypothesis testing, and machine learning-based recommendations and predictions, all presented through a sleek Dash interface.

---

## Features

- **Data Preprocessing**: Cleans and standardizes game data for analysis.
- **Rating Analysis**: Provides statistical insights into game ratings and positive review ratios.
- **Price Trends**: Tracks historical pricing and discount patterns with trend analysis.
- **Recommendation System**: Suggests similar games using cosine similarity.
- **Success Prediction**: Forecasts game success (positive review ratio) with a Random Forest model.
- **Steam Deck Impact**: Evaluates the effect of Steam Deck compatibility using statistical tests.
- **Tag Prediction**: Infers ratings from game titles via text vectorization and classification.
- **Dynamic Pricing**: Recommends optimal prices based on game features.
- **Interactive Dashboard**: Allows real-time exploration of analytics via Dash.

---

## Dependencies

- `dash`, `dash.dcc`, `dash.html`: Web framework for the interactive dashboard.
- `plotly.express`: High-level API for creating interactive plots.
- `pandas`, `numpy`: Core libraries for data manipulation and computation.
- `joblib`: Serialization of machine learning models.
- `sklearn`: Tools for preprocessing, model training, and similarity metrics.
- `scipy`: Sparse matrix support and statistical functions.
- `pingouin`: Effect size calculations.
- `statsmodels`: Time-series analysis utilities.
- `typing`: Type annotations for better code clarity.

Install with:
```bash
pip install dash plotly pandas numpy joblib scikit-learn scipy pingouin statsmodels
