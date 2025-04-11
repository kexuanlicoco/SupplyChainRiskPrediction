# News Sentiment Prediction for Supply Chain Logistics Risk

## Overview

This project leverages natural language processing (NLP) to analyze news sentiment as an indicator of potential disruptions in the supply chain. Using BERT for sentiment analysis, summarization, and topic modeling, the system fetches news articles using the News API, processes them to extract key information, and stores the results for further analysis.

The core functionality includes:

- Fetching news articles based on location
- Summarizing article content
- Performing sentiment analysis using BERT
- Clustering articles based on topics
- Storing results in a local SQLite database
- Calculating sentiment scores for each state in the U.S.

## Features

- **Summarization**: Summarizes news articles for easier consumption.
- **Sentiment Analysis**: Analyzes the sentiment of news content to determine the tone (positive, neutral, or negative).
- **Topic Modeling**: Uses KMeans clustering to identify topics within a set of news articles.
- **Location-Based News Fetching**: Fetches news articles related to specific locations using the News API.
- **Sentiment Aggregation**: Computes an average sentiment score for each state based on analyzed articles.
- **Data Storage**: Stores the analyzed articles and results in a SQLite database.
- **CSV Export**: Exports sentiment data to a CSV file for further analysis.

## Setup

### Requirements

- Python 3.x
- Install dependencies:

```bash
pip install torch transformers sentence-transformers scikit-learn requests pandas sqlite3
```
- API Key
To fetch news articles, you will need an API key from The News API. Replace the api_key variable in the script with your personal API key.

