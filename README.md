# Cryptocurrency Classification Project

## Purpose
The purpose of this project was to group cryptocurrencies that are trading on the market to segment the currencies for creating an investment portfolio for a bank.

The analysis began by importing data from this website, which contains data on all the cryptocurrencies. https://min-api.cryptocompare.com/data/all/coinlist

## Analysis
The analysis began by narrowing down the dataset - looking at currencies activly traded and mined and removing rows with null values.

In order to run machine learning models, I used the get_dummies method to create variables for two of the features and used the StandardScaler fit_transform method to standardize the data.

From there, I used the PCA algorithym to reduce the number of features analyzed to three. To identify the best K-value (for the K-means algorithm), I created an elbow curve using hvPlot. Then I applied that output (4 clusters ideal for this analysis) to hte KMeans model and added the output as a class to the dataframe with the coin names and other data. 

## Visualization
I created a few visualizations of the data including a 3-D scatter plot, and hvplot table and a 2-D plot with total coin supply/total coins mined scaled (normalized) data. 
