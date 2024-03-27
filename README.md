website link from where data was extracted: [https://www.airlinequality.com/airline-reviews/british-airways].

Jupyter Notebook and Google Colab was used for this project.

Dataset was extracted from the skytrax and sentiment analysis was performed by following steps:

  1.Web scraping : 
        -> Packages used: BeautifulSoup ,Pandas and requests
        -> Data was extracted from the website and converted into a dataframe from list  using pandas and stored
           in a file in csv format
        -> 1000 reviews were scrapped as a sampling procees and stored into 10 pages (100 reviews in each page)

  2.Data preprocessing :
        -> Packages used: re,Pandas
        -> Text preprocessing and data manipulation was performed by removing unwanted words,
           Additionaly data cleaning can also be done ny removing stopwords(But was not done now but done when data visualized)

  3.Analysis :
        -> Packages used: nltk,requests and pandas
        -> 'vader_lexicon' was downloaded for using SentimentIntensityAnalyzer and sentiment score was generated
                ~ if score > 0 => positive review
                ~ elseif score < 0 => negative review
                ~ else => neutral review

  4.Data visualization :
        -> Packages used: Matplotlib and WordCloud
        -> A pie chart is plotted representing the Sentiment Analysis
        -> A barchart is plotted representing keywords count used in the reviews 
        -> A Wordcloud is displayed after removing stopwords from the dataset
