# Arvato customer analytics and response prediction
 Part of the Udacity Data Scientist Nanodegree Program
 Blog post for this project can be found [here]( ) on my medium platform
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
This is my cpastone project for the Udacity Data Science Nanodegree program. The goal of this projec is to analyze how can a client of Bertelsmann Arvato, a mail-order company in Germany that sells orgainic products, acquires new customers more efficiently.Instead of reaching out to the general propulatio, the client can reach out to people that we identified as being the most likely to become new customers

The dataset is provided by [Bertelsmann Arvato](https://www.bertelsmann.com/divisions/arvato),an internationally active services company that develops and implements innovative solutions for business customers from around the world.  The data is real-life data, and it is confidential, so I will not provide the dataset here.

## Dataset Description
There are four data files associated with this project:

1. Udacity_AZDIAS_052018.csv: Demographics data for the general population of Germany; 891 211 persons (rows) x 366 features (columns).\
2. Udacity_CUSTOMERS_052018.csv: Demographics data for customers of a mail-order company; 191 652 persons (rows) x 369 features (columns).\
3. Udacity_MAILOUT_052018_TRAIN.csv: Demographics data for individuals who were targets of a marketing campaign; 42 982 persons (rows) x 367 (columns).\
4. Udacity_MAILOUT_052018_TEST.csv: Demographics data for individuals who were targets of a marketing campaign; 42 833 persons (rows) x 366 (columns).

## Methods
1. Customer segmentation
I analyzed demographics data for customers, comparing it against demographics information for the general population. I used unsupervised learning techniques to perform customer segmentation, identifying the parts of the population that best describe the core customer base of the company. 

2. Response Prediction
Using the Udacity_MAILOUT_052018_TRAIN dataset, I made a model to predict which individuals are most likely to convert into becoming customers for the company. The column "RESPONSE" indicates whether or not each recipient became a customer of the company. 

## Results
There are 

## Licensing, Authors, and Acknowledgements
### Authors: 
Sara Sun

Blog post for this project can be found [here](https://sarasun97.medium.com/what-should-i-expect-when-considering-different-room-types-on-airbnb-35b3115a6574) on my medium platform
### Acknowledgements
I have learned a lot from [Data Scientist Nanodegree Program](https://classroom.udacity.com)

I downloaded the data from [Inside AirBnB](http://insideairbnb.com/get-the-data.html)

I learned a lot from [Matheus Vasconcellos's project](https://github.com/matheusvclls/airbnb_buenos_aires) and [Siddharth Sabat's project](https://github.com/SiddharthSabat/Data-Science-and-ML-Portfolio/tree/main/Write%20a%20Data%20Science%20Blog%20Post)

