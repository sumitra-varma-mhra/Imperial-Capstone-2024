# Model Card for K Nearest Neighbours : Vaping Sentiment Analysis

## Model Description 
The model predicts the sentiment of tweets related to vaping. The output classifies tweets as either Positive, Negative, or Neutral based on their content. The model will help in understanding public opinion about vaping, aiding regulators and public health officials in understanding sentiment trends.

KNN tends to be slower for large datasets since it computes distances between all points, so it’s not always the best option for very large datasets. However, it's a simple and interpretable model.

**Input:** Tokenized text of tweets, preprocessed to remove stop words including profanities, special characters, and URLs.

**Output:** Sentiment analysis labels of positive, negative, neutral

**Model Architecture:** 

Construct a dataframe of tweets
Preprocess tweets to analyse the text by converting text to lowercase, removing URLs, removing hashtags, removing special characters including punctuation, tokenization and removing stop words. 
Label all vape tweets using a sentiment analysis library, VADER
Split into training and testing datasets
Convert tweets to TF-IDF features
Apply K-Nearest Neighbours to classify vape tweets

## Performance

This algorithm doesn't perform well on large data sets as it is computationally expensive.

               precision    recall  
    negative       0.83      0.40     
     neutral       0.44      0.94     
    positive       0.87      0.31    

## Limitations

The model has been trained on a subset of data, which covers tweets from January - November 2022. This limitation may have led to a less diverse data set. 

The training data consists of English-language tweets and thus, excludes non-English sentiments for analysis. 

Sentiments may have varied since 2022 (eg. after regulatory changes that happened in this period) and so the analysis is only valid for that period. 

## Trade-offs

Advanced NLP techniques like topic modelling or word embeddings may be useful as an enhanced feature. 

Advanced interpretability methods to show how the analysis has categorised vape tweets