Twitter Sentiment Analysis
This project performs sentiment analysis on tweets related to a specific topic, using the iPhone 15 as an example. It scrapes tweets, analyzes their sentiment, and visualizes the results.
Prerequisites
Python 3.x

Required libraries:

snscrape

pandas

matplotlib

seaborn

vaderSentiment

nltk

Install dependencies using:

bash


pip install snscrape pandas matplotlib seaborn vaderSentiment nltk
Usage
Run the Script:

The script sentiment_analysis.py scrapes up to 500 English-language tweets about "iPhone 15" from 2024.

Modify the query variable to change the topic (e.g., query = "Tesla").

Adjust max_tweets to change the number of tweets to scrape.

Output:

A bar plot showing the distribution of positive, negative, and neutral sentiments.

A time-series plot showing sentiment trends over time.

How It Works
Tweet Scraping:

Uses snscrape to collect tweets based on the query.

Stores tweet date and content in a pandas DataFrame.

Sentiment Analysis:

Uses the VADER sentiment analyzer to classify tweets as Positive, Negative, or Neutral based on compound scores.

Thresholds: ≥ 0.05 (Positive), ≤ -0.05 (Negative), else Neutral.

Visualization:

A bar plot shows the count of each sentiment category.

A time-series plot tracks sentiment changes over time.

Notes
Ensure an internet connection for tweet scraping.

The script downloads the NLTK punkt tokenizer on first run.

Visualizations are displayed using matplotlib and seaborn.
