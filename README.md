# disaster-tweets

This notebook is a submission for Week 4 of University of Colorado Boulder CSCA 5642: Introduction to Deep Learning. The assignment is a submission in the Kaggle competition Natural Language Processing with Disaster Tweets. It includes a dataset of 10,000 hand-classified tweets that either do or do not refer to real disasters in the world.

The goal is to predict whether a given tweet is about a real disaster or not (if yes, predict 1; if no, predict 0). Real disaster tweets are useful as a first indication that something serious may have gone wrong in some part of the world, but it's important to sort out the tweets that are just people exaggerating or using similar words in a non-urgent way.

(Side note: my day job is as a journalist and I use a program that does this kind of classification, Dataminr, often in my work!)

The test dataset has 3,263 rows and four columns (id, keyword, location and text of the tweet). The training set has 7,613 rows and those same four columns plus one more, target, which is the binary hand code for whether a tweet indicates a real disaster or not.

We can use natural language processing, a powerful strategy to impute meaning from text strings. We'll start by importing the data and some useful libraries.
