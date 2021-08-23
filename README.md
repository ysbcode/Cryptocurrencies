# Cryptocurrencies

## Overview
In this project we used unsupervised machine larning to anlayze a database of cryptocurrencies and create a report including the traded cryptocurrencies classified into clusters based on their features. This report could be used to categorize different currencies being traded in the market for further analysis. 

To accomplish our task, we processed the data to remove null values, filtered for only currencies which were traded and coins were mined. We then converted string variables into numeric variables using the "get_dummies" pandas function. After the data was processed, it was scaled using StandardScaler and data dimensions were reduced to three using PCA. 

Using the final PCA dataframe, we performed K-means clustering to categorize the data into 4 classes. We ended up at 4 clusters by utilizing the elbow curve. 

Finally we created visualizations of our machine learning results. We created a 3D scatter plot of the three PCA Dimensions
![](https://github.com/ysbcode/Cryptocurrencies/blob/main/Screenshots/3D%20-%20Scatter.PNG?raw=true)

We also created a 2D Scatter plot by going back to our original dataset (before applying scaling using StandardScaler). We extracted the two variables coins mined and coins supply and performed a second scaling using MinMaxScaler. We then plotted the data on a 2D Scatter plot

![](https://github.com/ysbcode/Cryptocurrencies/blob/main/Screenshots/2D%20-%20Scatter.PNG?raw=true)

## Summary

We have identified the classification of 532 tradable cryptocurrencies based on similarities of their features. Particularities of each group need to be analyzed to determine their performance and potential interest for further investment.
