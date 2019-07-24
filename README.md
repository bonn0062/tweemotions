# Capstone Project Proposal
## Udacity Machine Learning Engineer Nanodegree

This is the repository for the Machine Learning Nanodegree Capstone Project (Udacity)

The capstone project proposal can be found here: https://github.com/bonn0062/mlnd_capstone/blob/master/proposal.pdf

The random tweets dataset can be found from the Sentiment140 dataset readily available on Kaggle. (https://www.kaggle.com/kazanova/sentiment140)

The link to the dataset contains this information about the contents:

**"Context:**

This is the sentiment140 dataset. It contains 1,600,000 tweets extracted using the twitter api . The tweets have been annotated (0 = negative, 4 = positive) and they can be used to detect sentiment.

**Content:**

It contains the following 6 fields:

-target: the polarity of the tweet (0 = negative, 2 = neutral, 4 = positive)

-ids: The id of the tweet ( 2087)

-date: the date of the tweet (Sat May 16 23:58:44 UTC 2009)

-flag: The query (lyx). If there is no query, then this value is NO_QUERY.

-user: the user that tweeted (robotickilldozr)

-text: the text of the tweet (Lyx is cool)"


Tweets indicating depression will be retrieved using the Twitter scraping tool TWINT using linguistic markers indicitive of depression. The scraped tweets may contain tweets that do not indicate the user having depression, such as tweets linking to articles about depression or talking about loved ones who have depression. As a result, the scraped tweets will need to be manually checked for better testing results. A csv file of scraped tweets will be provided.


