# Steam Game Analytics and Recommendation Platform

This project is a **Dash-based web application** designed to analyze Steam game data, provide insights, and offer recommendations and predictions. It leverages machine learning models, statistical analysis, and data visualization to explore game ratings, pricing trends, success metrics, and more. The application is built with Python, using libraries like Pandas, Scikit-learn, Plotly, and Dash.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Dependencies](#dependencies)
- [Code Structure](#code-structure)
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
- [How to Run](#how-to-run)
- [Future Improvements](#future-improvements)

## Project Overview

The Steam Game Analytics and Recommendation Platform processes a dataset of Steam games (e.g., `games.csv`) to provide an interactive dashboard. Users can input a game title, price, and discount to explore:
- Rating distributions and statistical summaries.
- Historical price and discount trends.
- Game recommendations based on similarity.
- Predicted success metrics (positive review ratio).
- Impact of Steam Deck compatibility.
- Inferred game ratings/tags from titles.
- Suggested pricing based on game features.

The project combines data cleaning, machine learning, statistical testing, and time-series analysis into a user-friendly interface.

## Features

- **Data Cleaning**: Loads and preprocesses Steam game data, handling missing values and standardizing features.
- **Rating Analysis**: Visualizes rating distributions and computes statistical metrics (mean, std, confidence intervals).
- **Price Trends**: Analyzes average price and discount trends over time with seasonal decomposition.
- **Recommendation System**: Suggests similar games using cosine similarity on a feature matrix.
- **Success Prediction**: Predicts a game's positive review ratio using a Random Forest Regressor.
- **Steam Deck Impact**: Assesses the statistical impact of Steam Deck compatibility on game success.
- **Tag Prediction**: Infers game ratings from titles using TF-IDF and Random Forest classification.
- **Dynamic Pricing**: Suggests optimal pricing based on game attributes.
- **Interactive Dashboard**: Built with Dash, allowing users to input game details and view real-time analytics.

## Dependencies

The project relies on the following Python libraries:
- `dash`, `dash.dcc`, `dash.html`: For building the web application.
- `plotly.express`: For interactive visualizations.
- `pandas`, `numpy`: For data manipulation and numerical operations.
- `joblib`: For saving and loading machine learning models.
- `sklearn`: For preprocessing (LabelEncoder, StandardScaler), model training (RandomForest), and similarity computation (cosine_similarity).
- `scipy`: For sparse matrices (csr_matrix) and statistical tests (ttest_ind).
- `pingouin`: For computing effect sizes.
- `statsmodels`: For time-series decomposition.
- `typing`: For type hints.

Install dependencies using:
```bash
pip install dash plotly pandas numpy joblib scikit-learn scipy pingouin statsmodels
