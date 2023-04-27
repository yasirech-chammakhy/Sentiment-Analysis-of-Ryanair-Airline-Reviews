# Sentiment-Analysis-of-Ryanair-Airline-Reviews

## Overview
This project involves scraping and analyzing customer reviews of Ryanair airline to determine overall sentiment and identify common themes among customer complaints. The goal is to provide insights that can help Ryanair improve its customer service and attract more customers.

## Data Collection
To collect the data, we scraped reviews from the Skytrax website using BeautifulSoup and Selenium. We collected a total of 2252 reviews, which were stored in a CSV file.

## Data Cleaning
We cleaned the text data in the reviews column using various techniques such as removing special characters and numericals, converting all characters to lowercase, tokenizing each review, removing stopwords, and lemmatizing each word in each review. The resulting cleaned reviews were then saved in a new column called "cleaned reviews".

## Sentiment Analysis
We used the Vader SentimentIntensityAnalyzer from the NLTK library to generate sentiment scores for the cleaned reviews. We defined a function that took each review, applied the analyzer to it, and returned a compound score and sentiment label for the review. The compound score is a value between -1 and 1, where values closer to -1 indicate negative sentiment and values closer to 1 indicate positive sentiment. We used a threshold of 0.5 to classify reviews as positive, negative, or neutral. We then added the compound score and sentiment label to the dataframe for further analysis.

## Data Visualization
We visualized the distribution of sentiment categories in the dataset using a countplot and a pie chart. We also created a stacked bar plot to visualize the sentiment scores for each type of seat. We created a scatterplot to examine the relationship between review length and sentiment score.

## Conclusion
Overall, our analysis suggests that negative sentiment is more prevalent in airline reviews and that customers are becoming less satisfied with Ryanair's services. Whatever the reason for the decline in sentiment, it is clear that Ryanair needs to take steps to improve its customer service. This could include addressing the specific issues that customers are complaining about, such as delays, cancellations, and poor customer service. By taking steps to improve its customer service, Ryanair can improve the overall customer experience and attract more customers.

## Requirements
Python 3.9
Beautiful Soup 4
Selenium
Pandas
NLTK
Matplotlib
Seaborn

##License
This project is licensed under the MIT License. See the LICENSE file for more information.

