# A walk through Tokyo's Airbnb data

## Objective & Motivation

Airbnb had made it easier for people to rent their houses and apartements to tourists and visitors, and with a vibrant and relatively large city as Tokyo, a lot of factors can affect the price of such listings on Airbnb such as the neighbourhood, etc.. So the goal of this project is to find what factors play major role in determining the price. The specific questions answered in this project are:

1. What is the average price of neighbourhoods in Tokyo?
2. What is the average price of a room type in Tokyo neighbourhoods?
3. What percentage of AirBnb accomodations are of each room-type?
4. What is the average price of a room type in Tokyo neighbourhoods?

Predicting prices of Tokyo Airbnb using ML.

## Data
To answer these questions, AB_TYO_2019.csv is used (which is uploaded here) This dataset contains 11466 samples (number of rows) of different listings across Tokyo, with 14 different features (number of colomns) for these listings (eg. neighbourhood, price...etc.).

Some data preprocessing was necessary to utilize this available data in the best way, for example, dropping colomns with a lot of missing values, or that are irrlevant in answering above questions (you can learn more about this in the Notebook under data preprocessing).

## Models

In trying to answer question 6, I used 4 models in my analysis, first a linear regression model, then a ridge regression model (with different regularization paramters), then a Lasso Regression Model and lastly, an ElasticNet Regression Model. All the Models gave very similar accuracy results.

## Results

1. Using descriptive statistics, I was able to establish a sense of the most expensive and least expensive neighbourhoods around Tokyo, and the property types they have to offer.
2. For the prediction task, I achieved an R2 score of 0.27 on average using all the models. The low R2 score is also because of the lack of features available in this dataset.

You can read about the results in more details here:

## Libraries
Numpy, Pandas, Matplotlib, seaborn, datetime, sklearn

## Files
AB_TYO_2019.csv : The data in csv format airbnb_tokyo_2019.ipynb : Python Notebook, Main code and analysis

## To run the code
Make sure all necessary libraries are installed
Download the .ipynb file and the data file
Use Jupyter to open the .ipynb