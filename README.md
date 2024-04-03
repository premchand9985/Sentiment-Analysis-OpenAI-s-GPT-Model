# Sentiment-Analysis

This repository contains a Python script for sentiment analysis of Reddit comments using OpenAI's GPT models. The script collects comments from specified subreddits, scores their sentiment, and visualizes the sentiment distribution across different subreddits.

## Overview

Sentiment analysis is a powerful tool for understanding the emotional tone of text data. By analyzing Reddit comments, we can gain insights into the sentiment of discussions across various topics, communities, and events. This analysis can be valuable for understanding public opinion, identifying trends, and informing decision-making processes.

## How it Works

- Data Collection: The script collects comments from specified subreddits using the Reddit API. It retrieves the top submissions from each subreddit and extracts comments from them.

- Sentiment Scoring: Each comment is scored for sentiment using OpenAI's GPT models. The sentiment score ranges from -1 (most negative) to 1 (most positive), providing a quantitative measure of the comment's sentiment.

- Visualization: The sentiment scores are visualized using seaborn and matplotlib, allowing for easy interpretation of the sentiment distribution across different subreddits.

## Dependencies

openai: OpenAI's Python library for accessing the GPT models.
pandas: Python Data Analysis Library for handling data.
praw: Python Reddit API Wrapper for accessing Reddit data.
seaborn: Python visualization library based on matplotlib.
matplotlib: Python plotting library.

## Setup

1. Install Dependencies: Install the required dependencies using pip:

pip install openai pandas praw seaborn matplotlib

2. Obtain API Keys:

Create a Reddit app to obtain your client_id, client_secret, and user_agent.

3. Set up an OpenAI account to get your OPENAI_API_KEY.

Configure Environment:

Create a .env file in the project directory and add your API keys:
OPENAI_API_KEY=<Your_OpenAI_API_Key>
REDDIT_CLIENT_ID=<Your_Reddit_Client_ID>
REDDIT_CLIENT_SECRET=<Your_Reddit_Client_Secret>

## Usage

Modify Parameters: Adjust the filename and subreddits variables in the script to specify the target subreddits and the filename for storing comments.

Run Script: Execute the script to collect comments, score their sentiment, and visualize the results:

python reddit_sentiment_analysis.py

## Files
reddit_sentiment_analysis.py: Main Python script for collecting Reddit comments, scoring sentiment, and visualizing the results.
.env: Configuration file for storing API keys.

## Acknowledgements
This script utilizes OpenAI's GPT models for sentiment analysis.
It relies on the praw library for accessing Reddit data.
Data visualization is done using seaborn and matplotlib.
