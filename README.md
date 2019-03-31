# Twitter_US_Airline_Sentiment_Analysis
## Dataset
This data originally came from Crowdflower's Data for Everyone library: http://www.crowdflower.com/data-for-everyone which states: <br/>
A sentiment analysis job about the problems of each major U.S. airline. Twitter data was scraped from February of 2015 and contributors were asked to first classify positive, negative, and neutral tweets, followed by categorizing negative reasons (such as "late flight" or "rude service").<br/><br/>
It contains whether the sentiment of the tweets in this set was positive, neutral, or negative for six US airlines:<br/>
<img width="898" alt="Screen Shot 2019-03-31 at 5 50 43 PM" src="https://user-images.githubusercontent.com/31596604/55288975-8f62b780-53dd-11e9-9446-21243a9a8559.png">
### Features
The csv file has been added to the repo as Tweets_data.csv.It contains the following features (columns):<br/>
tweet_id<br/>
airline_sentiment<br/>
airline_sentiment_confidence<br/>
negativereason<br/>
negativereason_confidence<br/>
airline<br/>
airline_sentiment_gold<br/>
name<br/>
negativereason_gold<br/>
retweet_count<br/>
text<br/>
tweet_coord<br/>
tweet_created<br/>
tweet_location<br/>
user_timezone<br/>
Tweets<br/>

## Implementation
The data was cleaned using Natural Language Toolkit (NLTK).<br/>
For the analysis, Multinomial Naive Bayes and Supprt Vector Machine were used.

## Multinomial Naive Bayes Results
MultinomialNB classifier from sklearn was used.<br/>
Training Accuracy: 80.87%<br/>
Testing Accuracy: 77.18%<br/>
## Support Vector Machine Results
SVC classifier from sklearn was used.<br/>
Training Accuracy: 87.94%<br/>
Training Weighted Average F1-score: 0.88<br/>
Testing Accuracy: 78.79%<br/>
Testing Weighted Average F1-score: 0.79<br/>
