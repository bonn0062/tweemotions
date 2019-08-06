# You Are What You Tweet: 

### Detecting Depression in Social Media via Twitter Usage

Anne Bonner 
August 3, 2019


More than 300 million people suffer from depression and only a fraction receive adequate treatment.  Depression is the leading cause of disability worldwide and nearly 800,000 people every year die due to suicide. Suicide is the second leading cause of death in 15-29-year-olds. Diagnoses (and subsequent treatment) for depression are often delayed, imprecise, and/or missed entirely.

It doesn’t have to be this way. 

[Read more...](https://github.com/bonn0062/mlnd_capstone/blob/master/capstone_report.pdf)


### Random Tweets
[The random tweets dataset can be found here](https://www.kaggle.com/ywang311/twitter-sentiment/data)

**This dataset is too large to include in the GitHub repo and must be downloaded in order to run the model.**

It was built from the [Sentiment140 dataset](https://www.kaggle.com/kazanova/sentiment140) available on Kaggle, but this dataset offers a binary classification of the classified sentiment. 

The link to the Sentiment140 dataset contains this information about the contents:

**"Context:**

*This is the sentiment140 dataset. It contains 1,600,000 tweets extracted using the twitter api . The tweets have been annotated (0 = negative, 4 = positive) and they can be used to detect sentiment.*

**Content:**

*It contains the following 6 fields:*

*-target: the polarity of the tweet (0 = negative, 2 = neutral, 4 = positive)*

*-ids: The id of the tweet ( 2087)*

*-date: the date of the tweet (Sat May 16 23:58:44 UTC 2009)*

*-flag: The query (lyx). If there is no query, then this value is NO_QUERY.*

*-user: the user that tweeted (robotickilldozr)*

*-text: the text of the tweet (Lyx is cool)"*


### Embedding 

[The Word2vec embedding file can be downloaded here](https://drive.google.com/file/d/0B7XkCwpI5KDYNlNUTTlSS21pQmM/edit)

**This dataset also too large to be made available on GitHub and must be downloaded separatedly in order to run the classifier.**


### Depressive Tweets

Tweets indicating depression were retrieved using the Twitter scraping tool TWINT using linguistic markers indicitive of depression. The scraped tweets may contain tweets that do not indicate the user having depression, such as tweets linking to articles about depression or talking about loved ones who have depression. As a result, the scraped tweets will need to be manually checked for better testing results. 

**The .csv of scraped and processed tweets is provided in the GitHub repository, however, because the file size is over the limit, it has been provided as a .zip file and must be unzipped before using.**

This can often be done within an ipynb with a command like `!unzip vader_processed_final.csv.zip`

In order to gather Tweets with TWINT, a command such as 

`twint -s "depression" --since 2019-07-20 -o depression —csv`

Can be run to scrape Tweets that contain the term “depression” on a specific day (or days) and save the information as a csv file. Make sure to adjust the date and/or search terms as necessary.

### Necessary Libraries

This model utilizes a number of libraries, including Matplotlib, NumPy, and more. These libraries can easily be downloaded and documentation is available on the official sites. Example pip installation commands included below.

This model utilizes:
* [Matplotlib](https://matplotlib.org/3.1.1/users/installing.html)
    `pip install matplotlib`
* [Pandas](https://pandas.pydata.org/pandas-docs/stable/install.html)
    `pip install pandas`
* [NumPy](https://numpy.org/)
    `pip install numpy`
* [Scikit-Learn](https://scikit-learn.org/stable/install.html)
    `conda install scikit-learn`
* [Keras](https://keras.io/)
    `pip install keras`
* [Gensim](https://radimrehurek.com/gensim/install.html)
    `pip install gensim`
* [NLTK](https://www.nltk.org/)
    `pip install --user -U nltk`
* [WordCloud](https://pypi.org/project/wordcloud/)
    `pip install wordcloud`
* [Ftfy](https://ftfy.readthedocs.io/en/latest/)
    `pip install ftfy`
