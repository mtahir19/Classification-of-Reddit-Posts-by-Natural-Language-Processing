# Project 3 - Classifying Reddit Posts By Using Natural Language Processing

## Problem Statement
In this project, I am supposed to analyze posts from two subreddits with different classification models. Using Natural Language Processing, I worked on cleaning and dropping or engineering features and did exploratory data analysis. Then I trained different models to classify posts. I selected r/Conspiracy and r/TheOnion due to similarity between their title and content. The main aim is to find the accuracy score for these two subreddits.

## Executive Summary
I accessed and scraped the data from Reddit in the .json format:
1- Title, and unique ID were extracted into a Pandas Dataframe.
2- Deleted duplicate rows.
3- Did exploratory data analysis 
4- Train test split to split for models training and testing sets. 
5- CountVectorizer and TD-IDF Vectorizer to tokenize and count term frequencies.
6- With the help of Pipelines and GridSearch, optimal parameters were extracted
7- Models tested: 1) Logistic Regression, 2) K-Nearest Neighbors, 3) Multinomial Naive Bayes, and 4) Random Forest.

The better accuracy came from a CountVectorizer with logistic regression and Multinomial Naive Bayes. The highest accuracy in predicting the classification of posts based on their titles is the CountVectorizer with Multinomial Naive Bayes Classifier and Logistic regression, respectively:

A Train Accuracy Score: 0.93

A Test Accuracy Score: 0.82

and
A training set accuracy score of 0.94,

A testing set accuracy score of 0.81.

This is certainly overfit, however, less overfit than other models.

## Conclusion
Although predicted results are overfit, however,  logistic regression and Multinomial Naive Bayes are much better than baseline scores of 0.5. Due to some difficulties in distinguishing between these subreddits, it seems harder for models to accurately classify posts. I think by doing some further analysis and using different lemmatization or stemming of tokens may help to improve the score. Also one may try implementing boosting algorithms and support vector machines etc.
