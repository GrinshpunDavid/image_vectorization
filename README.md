## Project description:
The goal of this project is to improve the quality of data, used for the image classification model, by identifying and oversampling minority classes.

## Method:
- Vectorize images
- Kmean clustering the vectors
- Rebalance the clusters

## Conclusions:
- Images contain data that can be extracted as a way to differentiate them.
- Most features have a normal distribution, those that aren't can be log() transformed
- By finding a random seed that gives the lowest stats.ks_2samp(), we can decrease the maximum Kolmogorov-Smirnov between train-test features
- KElbowVisualizer is great tool for finding the optimal number of clusters for the dataset
- By placing each data point on a two-dimensional map, TSNE simplifies the comprehension of high-dimensional data
- As expected, each cluster has its own unique characteristics
- When re-sampling it is more efficient to undersample the majority class before oversampling
