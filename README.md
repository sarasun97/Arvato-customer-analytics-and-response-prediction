# Arvato customer analytics and response prediction
 Part of the Udacity Data Scientist Nanodegree Program
 A blog post for this project can be found [here]( ) on my medium platform
## Table of Contents
1. Installation
2. Project Motivation
3. Dataset Description
4. Methods
5. Results
6. Licensing, Authors, and Acknowledgements
## Installation
  [Install Anaconda](https://www.anaconda.com/products/individual#Downloads)
  [python (>=3.6)](https://www.python.org/downloads/)\
  [pandas](https://pandas.pydata.org/)\
  [numpy](https://numpy.org/)\
  [sklearn](https://sklearn.org/)

## Project Motivation
This is my capstone project for the Udacity Data Science Nanodegree program. This project aims to analyze how a client of Bertelsmann Arvato, a mail-order company in Germany that sells organic products, acquires new customers more efficiently. Instead of reaching out to the general population, the client can reach out to people that we identified as being the most likely to become new customers.

The dataset is provided by [Bertelsmann Arvato](https://www.bertelsmann.com/divisions/arvato), an internationally active services company developing and implementing innovative solutions for business customers from around the world.  The data is real-life data, and it is confidential, so I will not provide the dataset here.

## Dataset Description
There are five data files associated with this project:

1. Udacity_AZDIAS_052018.csv: Demographics data for the general population of Germany; 891 211 persons (rows) x 366 features (columns).
2. Udacity_CUSTOMERS_052018.csv: Demographics data for customers of a mail-order company; 191 652 persons (rows) x 369 features (columns).
3. Udacity_MAILOUT_052018_TRAIN.csv: Demographics data for individuals who were targets of a marketing campaign; 42 982 persons (rows) x 367 (columns).
4. Udacity_MAILOUT_052018_TEST.csv: Demographics data for individuals who were targets of a marketing campaign; 42 833 persons (rows) x 366 (columns).
5. DIAS Attributes - Values 2017.xlsx: A detailed mapping of data values for each feature in alphabetical order.

## Methods
1. Customer segmentation
I analyzed demographics data for customers, comparing it against demographics information for the general population. I used unsupervised learning techniques to perform customer segmentation, identifying the parts of the population that best describe the company's core customer base. 

2. Response Prediction
Using the Udacity_MAILOUT_052018_TRAIN dataset, I made a model to predict which individuals are most likely to convert into becoming customers for the company. The column "RESPONSE" indicates whether or not each recipient became a customer of the company. 

## Results
The general population is divided into 6 clusters; cluster 4 has the highest positive difference in proportion between customers and the general audience. Clusters 1 and 5 have the highest negative difference in proportion between customers and the general audience.

Among the four algorithms: Logistic Regression, Random Forest Classifier, Gradient Boosting Classifier and 
Support Vector Classification, Gradient Boosting Classifier gives the best result. The mean cross-validated auc score of the best_estimator is 0.656; the validation data auc score is 0.726.

In the Kaggle competition, the auc score I got is 0.782

## Licensing, Authors, and Acknowledgements
### Authors: 
Sara Sun

A blog post for this project can be found [here]() on my medium platform
### Acknowledgements
I have learned a lot from [Data Scientist Nanodegree Program](https://classroom.udacity.com)

The dataset is provided by [Bertelsmann Arvato](https://www.bertelsmann.com/divisions/arvato)

