# SteamReviewClassifier

## Introduction
This project's objective is to predict if a certain game review will be positive or negative.
A dataset of Steam game reviews was used. The gaming community has been expanded very quickly over the past few years, and the peak period for Steam usage occurred during the pandemic.
Due to the large number of games that are linked to it, this dataset has a lot of potential for future advances. If we take into account one specific game and use the game's data, it will enable us to explore a bigger dataset and create models that can forecast how players will behave and the results of games based on the game's data. The Game Review Dataset has the Reviews, Recommendations which helped in training the model and build the classifier.
The process followed is Data Pre-processing --> Data Visualization --> Data Cleaning (Stemming) --> Building Classification Model
We looked for any null or duplicate values that would have impacted our classifier during the pre-processing stage and eliminated all of those rows. We were able to view the data from several angles throughout the visualisation process, which improved our comprehension of the data. We cleaned the data by making all the reviews in the datasets lower case, removing any special characters that would have an impact on the model, and assigning an integer to the recommendation column to make the next step easier. 

The reviews posted are text data, so we have to convert them into TFIDF form

tf-idf(t, d) = tf(t, d) * idf(t), and the idf is computed as

idf(d, t) = log [ (1 + n) / (1 + df(d, t)) ] + 1

## Model Building

We have used Multinomial Naive Bayes, Support Vector Machine, Random Forest Classifier and Ensembler of these three as these are text classifiers. Out of these SVM gave the best accuracy.

## Project Objective
As previously noted, Steam offers a wide range of applications, and this review classifier can assist us in developing the game recommender even further. People will be looking for recommendations so that this app can assist them in choosing the best game because Steam has millions of users who are always trying out new games. This classifier serves as the foundation for the recommender, which may then be further expanded into an entirely functional application.
