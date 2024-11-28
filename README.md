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

## MODEL 
The models used in this solution include : 
Classification of tweets based on positive/ negative classes
Naive Bayes 
K Nearest Neighbour implementation
Decision trees
Random forests
Support Vector Machines
Deep Learning Models 

## HYPERPARAMETER OPTIMISATION
Description of which hyperparameters you have and how you chose to optimise them. 

## RESULTS
A summary of your results and what you can learn from your model 

You can include images of plots using the code below:
![Screenshot](image.png)

