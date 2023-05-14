# Tweet-Sentiment-Extraction
### Extract support phrases for sentiment labels

![](https://media.giphy.com/media/xUPGcEOEllmvFAvako/giphy.gif)

### **Description**

The aim of the  Kaggle competition project [Tweet Sentiment Extraction](https://www.kaggle.com/competitions/tweet-sentiment-extraction/overview) is to develop a machine learning model that can accurately identify the phrases within a tweet that support a particular sentiment label **(positive, negative, or neutral)**. The dataset contains tweets and their corresponding sentiment labels, and participants are tasked with predicting the support phrases for the sentiment labels. The competition is designed to help advance natural language processing and sentiment analysis techniques.


### Data

The [Dataset](https://www.kaggle.com/competitions/tweet-sentiment-extraction/data) contains a set of tweets in English, along with their corresponding sentiment labels (positive, negative, or neutral). Each tweet has a unique ID, and the task is to predict the support phrases (substrings within the tweet) that indicate the sentiment expressed in the tweet.

The training set contains around 27,000 tweets, while the test set contains 4,000 tweets. The tweets in both sets have been preprocessed, with mentions, hashtags, and URLs replaced with special tokens.

- `textID` - unique ID for each piece of text
- `text` - the text of the tweet
- `sentiment` - the general sentiment of the tweet
- `selected_text` - [train only] the text that supports the tweet's sentiment


In this Notebook, we explored the task of sentiment analysis on Twitter data and developed a solution to extract the support phrases for the sentiment labels. We performed exploratory data analysis and generated meta-features to gain insights into the distribution of sentiments and the characteristics of the data. We then cleaned the corpus by removing stopwords and most common words and examined unique words in each segment of positive, negative, and neutral tweets.

To train our model, we used spaCy and treated the task as Named Entity Recognition (NER) to predict the support phrases for each sentiment label. We also used WordClouds to visualize the most common words in our corpus and the unique words in each segment.

Overall, our solution achieved good performance on the test set and can be further improved by tuning the hyperparameters and exploring other NLP techniques. In conclusion, this project provides a useful approach to extract support phrases for sentiment labels in Twitter data and can be applied to various applications in social media analysis and customer feedback analysis.

