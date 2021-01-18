# CP600-610: Practical Algorithm Design and Data Analytics

*Yash Shah*

*Master of Applied Computing - Wilfrid Laurier University*

A sentiment analysis job about the problems of each major U.S. airline. Twitter data was scraped from February of 2015 and contributors were asked to first classify positive, negative, and neutral tweets, followed by categorizing negative reasons (such as "late flight" or "rude service").

**Accuracy Results explored using SVM (support vector machine**
 
 
Columns used for analysis     | 
------------------------------| 
airline_sentiment             | 
airline_sentiment_confidence  | 
negativereason                |
negativereason_confidence     |
airline                       |
retweet_count                 |
text                          |

## Data Cleaning
1.	Filling numeric missing values with 0
2.	Filling Character missing values with “ ”
3.	One Hot Encoding – Columns “Airline” and “Negative Reason”

## Text Cleaning – Column “Text”
1.	Making text lower case
2.	Removing Stop Words 
3.	Lemmantization
4.	Replace @words with “ “
5.	Replace special characters with “ “

## Feature Engineering
1.	Length of text within Text column
2.	Syllable Count within Text column
3.	Lexicon Count within Text column

## Bag of Words – TF IDF
•	More Features added using Bag of Words – TF IDF and ngram range from 1: 3

#### Model Development
1.	Step 1 – Standardized the numerical data
2.	Step 2 – Train and Text split – 20% test size
3.	Step 3 – Model used to classify whether the sentiment of text is positive, negative or neutral using Random Forest Classification Algorithm
(Hyper parameter tuning to find the best model fit)
4.	Accuracy measure used for analyzing the prediction on test dataset = F1 Score

## Topic Modelling – LDA (Additional Data Viewing)
LDA model used to create topics and top terms within the topic


[Data Source](https://www.kaggle.com/crowdflower/twitter-airline-sentiment "Kaggle Link to DataSource")
