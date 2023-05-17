## UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET

## INTRODUCTION

Data can be divided into groups, or clusters, using a variety of processes called clustering. In a broad sense, clusters are collections of data objects that share more similarities with one another than with those in other clusters. In the real sense clustering aids in identifying two characteristics of data significance. A range of methods known as clustering are used to divide data into groups or clusters. The term "clusters" refers to groups of data objects that have more similarities with one another than with data objects from other clusters.

This activity allows you to monitor changes in the attitude of a variable over time by detecting positive or negative sentiment from internal or external data sources.
For the purpose of this course work we would be using the K-Means clustering and the DBSCAN (Density-Based Spatial Clustering of Applications with Noise) clustering on our data set.

K-Means clustering is an unsupervised machine learning technique in clustering that is used to find groups of data objects in a dataset. Although there are many alternative clustering techniques, k-means is one of the most established and user-friendly.

Density-based spatial clustering of applications with noise (DBSCAN) is a data clustering algorithm which has the high-performance rate for dataset where clusters have the constant density of data points. One of the significant attributes of this algorithm is noise cancellation. The noise in this case is also known as outliers. Outliers are variables or observations that lies in an abnormal distance from the other values in within a given data set.

## EXPLANATION AND PREPARATION OF DATASET

![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/2c1ab6f4-1c1d-48f0-9f9f-3a8834e19edd)

The exported dataset is about the travel reviews from travelers within East Asia. Before the data set was exported into python the column names were changed. This was to ensure easy understanding of all the variables that would be considered when executing the task. The data set did not have empty cells or values hence there was no need to remove the empty cells or values.

## IMPLEMENTATION INTO PYTHON

The necessary libraries were imported into python.

![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/73237b5c-72fd-4d67-899e-e45e5674c110)


The file for this task was then imported into python.

![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/b57ef8aa-2b0e-4c4f-90e9-7f6888113e79)


![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/4dc944b9-5c9f-4058-947e-7f81fe0419b6)


![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/6e2f98fd-a26e-4ad5-bbad-a74c718384d7)


From the information derived, we can see that there is a total of 980 entries from the 10 different categories of entries in the data set.

![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/e2525fd3-284a-4f66-86fc-743d6061e67e)


![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/ba55d21f-01f5-45dd-88e1-299092b3ac81)


![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/abb9d52a-cf0a-4e31-90ce-eb3e4cf6a137)


![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/a6000f8e-a203-4202-8eb9-e51b984390b0)


This creates a nice visualization and helps us understand the data by summarizing a large amount of data in a single figure. This is essential when we are exploring our dataset and trying to become familiar with it. The seaborn pair plot above shows the relationships between the different variables within the data set. 
The elbow method is used in determining the number of clusters within the entire data set.

![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/82ac7005-6fbf-4ff4-a14f-6343ac43b370)


![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/eafb28e8-ad7f-44af-8484-5f90ee937ca0)


The curve in the elbow method of clusters is close to 2, we would therefore use 2 as the number of clusters within the given data set.

![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/8a28b57f-2377-4c38-ba59-b4edb2c95c03)


Because of the number of variables in the data set, we would be unable to visualize all the dimensions in the scatterplot. It is therefore important that we introduce that PCA technique. PCA means Principal Component Analysis. It is a linear dimension reduction technique that can be utilized in extracting information from a high-dimensional space by projecting it into a lower-dimensional sub-space.

![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/8372ddcc-c319-4e74-95bc-0fde04bd36bb)


From the result derived we would need to get the sum of the two arrays to arrive at the value of the principal component.

![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/a83f8f24-75e8-4043-af75-8a8b7b3fa9c1)


The result of the sum of both arrays is 42.40%. This therefore means that we would be using 42.40% of the entire data set to visualize when the scatter plot is being plotted.

![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/66b57e84-b309-43d4-8b9d-aae66f1953fb)


![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/a4126bdc-879b-462c-b935-887714bf05a4)

![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/7f9cc126-6007-4d35-b16f-6298cebd003c)

After the clusters within the data set has been classified into 2 clusters, we can see that cluster 1 has 606 counts while cluster 0 has 374 counts. We can also see that many clusters in cluster 2 lie directly above cluster 1.

![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/49393524-d74f-4fc8-824c-5d54684c6cea)


From the image above, can see that the different users within the data set have been put into two separate clusters.

![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/0c62dd8e-7c53-493f-a361-8ce239a8eac7)


![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/6cbc44f7-0a32-42ad-84f8-87c2166f50b8)


![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/e6d71a88-6494-41cc-9f14-3e2079f5e712)


From the image above we can see that the elbow method is between 1.8 and 2.0. We would therefore proceed with using 1.8 as the elbow method as the eps. The eps specify how close points should be to each other to be considered a part of a cluster. We would also use the minimum of 5 samples within the selected cluster.

![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/92b314b5-57f6-4d6d-86e3-c950056028e7)


![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/b25604f7-deb1-49c2-b95a-3524dedcaa13)


![image](https://github.com/Orlawlardey/UNDERSTANDING-THE-CLUSTERS-OF-ALL-THE-VARIABLES-WITHIN-THE-DATASET/assets/124607057/9ca32fb8-aa83-4cb7-b9bc-f6f040b2af2b)


After plotting the scatter plot, we can see that we most likely have more noise present than cluster one and cluster two. What this means is that there are lots of clusters that have not been assigned. 
