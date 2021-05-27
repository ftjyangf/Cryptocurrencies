# Cryptocurrencies
## Overview of Project
### In this project, Our dataset is a group of crypto currency, to better understand those currency and give some inside useful infomation to the investment department. we are tring to use unsupervised learning to find the patten or the classes each type of crypto currency belong to. In this project,Kmeans is the algorithm to cluster data points, and for purpose of visualization, Princple Component Analysis(PCA) also are used to decrease dimention data.

## Process
### There are categorical data and numerical data in this dataset.Onehotencoder are used to encoder categorical data,Standardscaler are used to scale data so that algorthm such as PCA and KMEANS can be minimum affected by outliers. After induced 3 components PCA, the dimention of data is reduced significantly, but the variance left is only about 7 percent,which means there are lot of information lost. however for the purpose of visualization, this is not our concern in this case 

## Idea on in the process
### Taking 3 components PCA as the input to Kmeans, we decide the number of clusters by finding biggest distance change between data points, which can be obtained by kmeans.inertia_ attribute. Visualization of number of clusters versus inertia(distance) help us find the turning point(elbow) quick. In this case we find 4 clusters are the best for categorizing cryptocurrencies.

