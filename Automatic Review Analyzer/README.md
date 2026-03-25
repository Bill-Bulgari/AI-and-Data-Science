# Automatic Review Analyzer

A sentiment analysis project using linear classifiers for text classification.

## Overview

This project analyzes review text and predicts whether a review is positive or negative.

It implements and compares several linear classification algorithms:

- Perceptron
- Average Perceptron
- Pegasos

The project also explores simple feature engineering techniques such as:

- stopword removal
- binary bag-of-words features
- count-based bag-of-words features

## Main goals

- build sentiment classifiers from scratch
- compare different linear learning algorithms
- tune hyperparameters
- inspect the most explanatory words
- study how feature engineering affects performance

## Files

- `project1.py` — core model and feature extraction code
- `main.py` — runs the experiments
- `utils.py` — helper functions for loading data, plotting, and tuning
- `stopwords.txt` — stopword list used for feature engineering

## Results

Key findings include:

- Pegasos performed best among the tested methods
- removing stopwords slightly improved test accuracy
- binary features outperformed count features in this project
- the most explanatory positive and negative words can be extracted from the learned weights

## Notes

This project is based on coursework that I adapted into a cleaner portfolio project for general audiences.
