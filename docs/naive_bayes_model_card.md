# Model Card for Multinomial Naive Bayes : Vaping Sentiment Analysis

## Model Description 
The model predicts the sentiment of tweets related to vaping. The output classifies tweets as either Positive, Negative, or Neutral based on their content. The model will help in understanding public opinion about vaping, aiding regulators and public health officials in understanding sentiment trends.

For text classification tasks, Multinomial Naive Bayes is often used, especially when the features are word frequencies or TF-IDF scores. The model assumes conditional independence, which makes it useful for sentiment analysis. 

**Input:** Tokenized text of tweets, preprocessed to remove stop words including profanities, special characters, and URLs.

**Output:** Sentiment analysis labels of positive, negative, neutral

**Model Architecture:** 

Construct a dataframe of tweets
Preprocess tweets to analyse the text by converting text to lowercase, removing URLs, removing hashtags, removing special characters including punctuation, tokenization and removing stop words. 
Label all vape tweets using a sentiment analysis library, VADER
Split into training and testing datasets
Convert tweets to TF-IDF features
Apply Logistic Regression to classify vape tweets

## Performance

Naïve Bayes is computationally efficient:
- Training involves simple counting of word occurrences.
- Prediction requires only the calculation of probabilities for each class.
- This efficiency allows it to handle large-scale datasets.

              precision    recall  

    negative       0.91      0.87   
     neutral       0.90      0.96   
    positive       0.91      0.90    

## Limitations

The model has been trained on a subset of data, which covers tweets from January - November 2022. This limitation may have led to a less diverse data set. 

The training data consists of English-language tweets and thus, excludes non-English sentiments for analysis. 

Sentiments may have varied since 2022 (eg. after regulatory changes that happened in this period) and so the analysis is only valid for that period. 

Naive Bayes treats assumes conditional independence but this may not always be true. 

## Trade-offs

Advanced NLP techniques like topic modelling or word embeddings may be useful as an enhanced feature. 

Advanced interpretability methods to show how the analysis has categorised vape tweets