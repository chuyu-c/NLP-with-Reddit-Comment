# NLP-with-Reddit-Comment

## Problem Statement
To help Reddit understand their topics, categorize comments attitude, and predict comments’ likes and dislike scores. We would like to conduct text analysis to better understand the current Reddit community through the subreddits. 
* Target popular topics using word clouds.
* Categorize the arritude based on the comments.
* Predict scores for each comment accordingly.

## Big Data Platforms
* Google Cloud Platform (BigQuery, Dataproc, Cloud SQL)
* UChicago Research Computing Center

## Data and Analysis
All analysis and data collection is found within *jupyter_notebooks* folder.
* Data Source:
  * https://www.kaggle.com/kaggle/reddit-comments-may-2015 
  * https://console.cloud.google.com/bigquery?project=fh-bigquery&page=table&t=2015_05&d=reddit_comments&p=fh-bigquery&redirect_from_classic=true 

## Modelling
#### Sentiment Analysis
* Understand people's opinions from a post
* Potentially help Reddit gain an overview of the wider public opinion behind certain topics
* Transformer pipeline:
  * Regular Expression Tokenizer
  * StopWords Tokenizer
  * CountVectorizer
  * StringIndexer
  * HashingTF
  * DF

#### Regression Analysis
* Based on the body of the post, predict a post’s success before it’s submitted
* Potentially help Redditors gain upvotes, and predict which posts will get popular enough to hit the front page

