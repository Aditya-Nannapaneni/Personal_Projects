# Quora Question Pair Similarity

Source:  https://www.kaggle.com/c/quora-question-pairs

## Quick Introduction 

Given a dataset containing question id's, 2 questions (text format) and a binary target variable we have to predict the target variable of new questions

| Target Variable               | Mapping                                    |
| ------------------------------| ------------------------------------------ |
| 0                             | not duplicates                             |
| 1                             | duplicates                                 |

## Problem Statement
  - Identify which questions asked on Quora are duplicates of questions that have already been asked.
  - This could be useful to instantly provide answers to questions that have already been answered.
  - We are tasked with predicting whether a pair of questions are duplicates or not.
  
  ### Real world business objectives and constraints: 
    - The cost of a mis-classification can be very high.
    - You would want a probability of a pair of questions to be duplicates so that you can choose any threshold of choice.
    - No strict latency concerns.
    - Interpretability is partially important.


## Approach

This problem can be formulated as a binary classification task. Since the only features given in our dataset are the 2 question given as text, we have to engineer features from this text data to serve as input to our classification model.

Performance Metrics: 
  - As specified in the Kaggle competition by Quora Log Loss would be our KPI.
  - We will also be looking at the Binary Confusion Matrix to get a better intuition of model performance

## Results
