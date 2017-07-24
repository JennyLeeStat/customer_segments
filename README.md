# Customer segments
This project is a part of the Udacity Machine Learning Nanodegree program.


### Dataset
The dataset was obtained from [UCI machine learning 
repository](https://archive.ics.uci.edu/ml/datasets/Wholesale+customers)

### Methods

##### Data preparation
##### Decorrelation and dimension reduction
![Alt text](https://github.com/JennyLeeStat/customer_segments/blob/master/assets/pca_biplot.png)


The Detergent_Paper is very nearly the same as the fist component in negative direction. Grocery and Milk, which are strongly correlated with the Detergent_Paper, are strongly projected on the first component. Fresh highly correlates with Frozen, and these two very strongly projects on to the negative direction of dimension 2. Delicatessan is weakly correlates with Frozen and Fresh. This observation is consistent with the pca_results plot obtained above. While biplot depicts only first two dimensions, it is more easily interpretable with feature axes and data points.

##### Clustering
![Alt text](https://github.com/JennyLeeStat/customer_segments/blob/master/assets/compare_clusters.png)

Three different clustering algorithms generally agree with each other.


### Conclustion
![Alt text](https://github.com/JennyLeeStat/customer_segments/blob/master/assets/channel_plot.png)

Surprisingly, the first component fairly well splits the data according to the the channel feature. 
Almost all of data points identified as Segment 1 actually fall into the retailers. 
Also, data points on the range [-5, -0] on the dimension 1 were clustered as segment 2, 
and identified as Hotel/Restausrants/Cafe. 
The range [0, 2] on the dimension has a mix of data points from both channels, and captured as segment 0.


### Conda environments
 you can find the Conda envoronment for MacOS at
 environment.yml file.