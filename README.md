# Sentiment analysis on the use of e-cigarettes or vapes in the UK based on social media 

Welcome to our repository for analysing sentiments on the use of e-cigarettes/ vapes in the UK based on social media tweets. 
We have developed and evaluated different machine learning models to analyse sentiment.

## Overview 
The rise of vapes and e-cigarettes has sparked significant debate and interest among health professionals, policymakers, and the public. My capstone project aims to perform a sentiment analysis on the use of vapes or e-cigarettes, analyzing emerging trends and trying to focus on their effectiveness in aiding smoking cessation. 
Currently e-cigarettes and vapes are treated as a medical device as they are a smoking cessation aid and thus, the sale of e-cigarettes/ vapes is regulated by the Medicines and Healthcare Regulatory products Agency. Sentiment analysis will involve extracting and analyzing subjective information from various sources. For this project, we will collect data from the social media platforms Twitter. The aim is to gauge public opinion, identify positive and negative sentiments, and understand the general perception of vapes and e-cigarettes.

## DATA
The data for this project is a subset of the Kaggle dataset : https://www.kaggle.com/datasets/bestgirl/vape-and-juul-tweet-dataset/data 
The Kaggle dataset contains over 8 million publicly available tweets scraped from X, known as Twitter at the time of data collection. Tweets in this dataset matched the following criteria:
- English language
- Posted between Jan 1st, 2015 and November 30th, 2022
- Contain JUUL or vaping related keywords: “juul", "juuls", "vape", "vapes", "juuling", "vaping", "juuled", "vaped", "juuler", "vaper", "juulers", and "vapers”
The data has the following fields : 
TweetID	- A unique integer ID for each tweet. Using the official Twitter API, it can be used to map each tweet with related quote tweets and retweets, or to rehydrate latent features such as likes.
TweetContent - Original tweet text content.
TweeterUsername	- Username of the tweeter. Using the official Twitter API, it can be used to map each tweet with the tweeter's profile (e.g. followers and following lists) and tweet history.
TweetDatetime - Tweet post datetime.

The subset used for this project contains data from the year 2022.

## MODEL 
The models used in this solution include : 

Logistic Regression Classification of tweets based on positive/ negative classes

Naive Bayes 

K Nearest Neighbour implementation


## HYPERPARAMETER OPTIMISATION

train_test_split 
- test_size=0.2:

TfidfVectorizer 
- max_features=5000
- max_df=1.0 and min_df=1 
- use_idf=True: 
- LogisticRegression 
- penalty='l2'
- C=1.0
- solver='lbfgs'
- max_iter=100
- multi_class='auto'

KNN model 
- n_neighbours = 3 

## RESULTS

KNN model had the least accuracy of 0.55325

Logistic Regression had the highest accuracy of 0.909133

Naive Bayes model had an accuracy of 0.807433
