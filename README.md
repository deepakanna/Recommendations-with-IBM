# Recommendations-with-IBM-
# Contents
## 1. [Introduction](Introduction)
## 2. [Exploratory Data Analysis](ExploratoryDataAnalysis)
## 3. [Rank Based Recommendations](RankBasedRecommendations)
## 4. [User-User Based Collaborative Filtering](User-UserBasedCollaborativeFiltering)
## 5. [Content Based Recommendations](ContentBasedRecommendations)
## 6. [Matrix Factorization](MatrixFactorization)


## Introduction
This project aims at analysing the interactions that users have with articles on the IBM Watson Studio platform, and make recommendations to them about new articles.

## Exploratory Data Analysis
The data is explored to gain insight into descriptive statistics of the data. 
### The graph shows the frequency(the number of times ) of the article. The article number 0 was accessed 14 times, the article 2 was accessed 58 times and so on. Only the first 25 articles are shown in the graph as the graph is too dense with all the articles.
![image](https://user-images.githubusercontent.com/110763030/205441554-79d12651-922a-4d51-9bbd-09740c8c0413.png)
### Taking only the first 100 records, the number of times an article was accessed is plotted in the graph below.
![image](https://user-images.githubusercontent.com/110763030/205441582-0c9b2ddc-416b-499f-90d1-60816a4a6aaa.png)
### Taking only the first 50 records, the number of articles each user has accessed is plotted in the graph below. The user with ID 2 has accessed 2 articles and user with ID 23 has accessed 3 articles.
![image](https://user-images.githubusercontent.com/110763030/205441607-b5f3424f-68d7-4bb4-b9de-49f95d977beb.png)


## Rank Based Recommendations
we don't actually have ratings for whether a user liked an article or not.  We only know that a user has interacted with an article.  In these cases, the popularity of an article can really only be based on how often an article was interacted with.

## User-User Based Collaborative Filtering
The similar users based on the article interaction is determined. The article recommendation is based on the closeness of a user with neighbor users and the article interaction of neighbor users are used. 

## Content Based Recommendations
The nltk package is used to generate tokens and CountVectorizer is used to transform a given text into a vector on the basis of frequency count.  Cosine similarity is used to determine similarity and recommendations are made based on the similarity of content. 

## Matrix Factorization
Matrix factorization is used to make article recommendations to the users on the IBM Watson Studio platform.
