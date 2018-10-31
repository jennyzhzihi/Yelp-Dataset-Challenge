# Yelp review data analysis

Natural Language Processing & Sentiment Analysis

## 1. Project Summary

This purpose of this project is to build a sentiment analysis model that predicts restaurant performance and construct a customer recomendation system based on the ratings

The restaurants reviewed are selected to be Las Vegas based, since Las Vegas is a popular touristy city, the time window is set to past two years,i.e, starting from 2016-01-01

The reviews are performed with NLP and split to traing and test data set.

Machine learning models, such as Logistic regression Naive Bayes and Random forest, are implemented to predict if the restaurant performance is good. The performance is measured by the restaurant average stars.

The result provides important insights to how the customers reviews reflect the restaurant performance and what business can focus on to improve their service.

The recommender systems is based on Collaborative filteringm based on the item-item similarity

## 2. Data Description

The data set can be downloaded from: https://www.yelp.com/dataset/challenge

The data set has size of 6.84 GB in total, over 1.8M reviews. Among those, _business, _review, _user are analyzed in this project.


## 3. Analysis Workflow

* Load the data, performed data cleaning and feature selection. 
Script see Yelp_Dataset_Preprocess_YL.ipynb

* Use NLP techniques, such as stemming, lemmatization and TF-IDF,to extract features from unstructured review text data. Script see Yelp_Dataset_NLP_YL.ipynb

* Build language understanding models to classify positive and negative reviews using NLP techniques, Logistic Regression and Random Forests, being able to understand business
performance based on user review text and comments. Script see Yelp_Dataset_NLP_YL.ipynb

* Use unsupervised learning to cluster users into groups. Identify and understand the common user preference within each of the group by inspecting the cluster centroid.
Script see Yelp_Dataset_-_Clustering_and_PCA-YL.ipynb

* Build a restaurant recommender system using collaborative filtering and matrix factorization based on user's past visits and ratings.
Script see Yelp_Dataset_-recommender_YL_fulldata.ipynb
