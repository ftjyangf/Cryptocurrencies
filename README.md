# Cryptocurrencies
## Overview of Project
### In this project, Our dataset is a group of crypto currency, to better understand those currency and give some inside useful infomation to the investment department. we are tring to use unsupervised learning to find the patten or the classes each type of crypto currency belong to.

## Process
### data infomation, in this dataset, we have categorical data and numerical data. after using onehotencoder, technically the categroical data can be turned into numerical data and the Prinple Component analysis can be performed. In this process, 3 components are selected for visualization purpose, so each components can be plot in 3D space. The demensionality reducted data also is used to in cluster process(KMeans is the method to cluster data). then we scatter the 3 components in 3D plot with KMean prediction.


## Idea on in the process
### In the process, we tried different options of n_components parameter in PCA, with the increasing number of PCA, the best KMean cluster is change with the increase of PCA components, in other word, 'the elbow' point is positively coordinate with n_compponents. why this is happening? after checking the explained variance for each PCA components, 3 components PCA only includes very small amount of variance, so as we increase the amount of componenets, more and more infomation are preserved. Based on the additional information, kmeans elbow point become larger and larger, finally give us the best K. 

### Conclusion, for purpose of visualization, PCA can be a very good tool to reduce the dimension of dataset. On the other hand, it also means some infomation will lost. another problem is this technique can only be applied to numerical data. In our this case, Onhotenconder is used to turn categorical data into binary data, it's working in our case. but this only for visualization purpose, because PCA is not built for categorical data.
