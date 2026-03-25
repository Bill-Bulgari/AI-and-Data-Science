# Automatic Review Analyzer

A sentiment analysis project that classifies written reviews as positive or negative using linear machine learning algorithms implemented from scratch in Python.

## Overview

This project explores text classification through a review sentiment analysis task. Reviews are converted into bag-of-words representations, and several linear classifiers are trained and compared.

The implemented algorithms are:

- Perceptron
- Average Perceptron
- Pegasos

The project also includes basic feature engineering experiments to study how text representation affects performance.

## What this project demonstrates

- implementation of core linear classification algorithms from scratch
- text preprocessing and bag-of-words feature extraction
- hyperparameter tuning
- model comparison on validation and test data
- interpretation of learned model weights
- simple feature engineering for NLP

## Feature engineering explored

The project includes experiments with:

- stopword removal
- binary bag-of-words features
- count-based bag-of-words features

It also extracts the most explanatory positive and negative words according to the learned weights of the best classifier.

## Main findings

Key results from the project include:

- Pegasos performed best among the tested classifiers
- removing stopwords slightly improved test accuracy
- binary features performed better than count-based features in this task
- the learned weights provide interpretable sentiment-related words for both positive and negative reviews

## Project structure

The project currently uses the following folder structure:

```text
Automatic Review Analyzer/
├─ README.md
├─ sentiment analysis demo.ipynb
├─ Pegasos algorithm.pdf
└─ core/
   ├─ main.py
   ├─ project1.py
   ├─ utils.py
   └─ data/
      ├─ reviews_train.tsv
      ├─ reviews_val.tsv
      ├─ reviews_test.tsv
      ├─ toy_data.tsv
      └─ stopwords.txt
