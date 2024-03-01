# 🏈 NFL Team Performance Predictor 🏆

## Overview 🌟

The goal of this project was to build an ML model that aims to predict the average total yards per season for every NFL team based on their points scored. My hypothesis is that there is a  correlation between the points scored by a team and their total yards, which can be used to predict future performance. Also referenced DataQuest

## Data Cleaning 🧹

I started with, `NFLdata.csv` which I found on Kaggle. That data was sorted by team and year to organize the data by team performance over time. My sorted dataset, `sortedNFLdata.csv`, was created from this.

## Feature Selection 📊

From the sorted data, only the columns I used for analysis were: 'year', 'team', 'wins', 'losses', 'points', and 'total_yards'.

## Correlation Analysis 🔍

A correlation matrix was generated to understand the relationship between the numeric features and identify strong predictors for total yards.

## Visualization 📈

Using Seaborn, scatter plots with regression lines were created to visualize the relationship between points and total yards, as well as wins and total yards to see something without as good of a correlation.

## Model Training and Evaluation 🚀

A linear regression model was trained using the 'points' feature to predict 'total_yards'. The model was used data from 2019 and onwards as a test set, while earlier years formed the training set. Pretty close to the suggested 80/20 split of train and test
