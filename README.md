# Disaster Response Pipeline

## by Liudmila Danilovskaya 

The goal of this project is to create a recommendation engine for the articles on the IBM Watson Studio Platform.

This is achieved by analyzing the past interactions that users had with articles and make recommendations to them about new articles you think they will like. This should improve user engagement on platform by providing users with articles that they are more likely to find interesting and relevant.

## Datasets 

1. articles_community.csv - a dataset containing information about articles such as document title and description.
	
1. user-item-interactions.csv - a dataset containing information on user interactions with articles

## Project structure

+ Recommendations_with_IBM.ipynb - a script that analyses data and build recommendation engines.
+ Recommendations_with_IBM.html - a html file for the recommendation engines.
+ data
	+ disaster_categories.csv: categories data to process
	+ disaster_messages.csv: messages data to process
+ .gitignore
+ README.md
+ requirements.txt
 

## Installation and running

This project requires Python 3.x and the following Python libraries installed:

pandas
scikit-learn
nltk
matplotlib
numpy

To install all libraries: pip install -r requirements.txt 


## Summary of Findings

The engine provides 4 types of recommendation engines:
1. Rank Based Recommendation:  a recommendation system that suggests articles to users based on their popularity and the number of times they have been interacted with by other users.

2. User-User Based Collaborative Filtering: a recommendation system that identifies the most similar users based on common articles read and recommends articles that the similar users have interacted with.

3. Content Based Recommendations: a recommendation system which recommends articles that are most similar in content to those that the user has interacted with in the past.

4. Matrix Factorization: decomposition of the user-article interaction matrix into two lower-dimensional matrices representing user and article characteristics. Decomposed matrices are used to calculate personalized recommendations for each user based on the articles they have interacted with in the past and the characteristics of the articles.

Flask app was created to give the training data overview and classify the messages the user entered. 


## Acknowledgments

This project was done as the part of Udacity learning. The data have been provided by [Appen](https://appen.com/).