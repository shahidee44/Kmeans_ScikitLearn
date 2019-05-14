# Kmeans_ScikitLearn
Implement Kmeans clustering using scikitlearn on the California housing price data.

## The Goal
1) To implement Kmeans clustering on a dataset and observe how the data would be classified in a binary classification situation
2) To observe the impact of normalisation on the way the data is divided between the classes
3) To calculate the probability of obtaining either a 0 or 1 based on the distances of the points from the centers

## The Insights
1) When fit to the training data with normalisation, it was noted that the centers of both classes were split along the median income feature. While the fit without normalisation was split along the median house value feature.
2) Another interesting observation is that the number of data points in either classes are rather similar, ignoring the permutation of the classes. For the normalised data, Class 0 had 4536 points while Class 1 had 12464. For the non-normalised data, Class 0 had 12526 points while Class 1 had 4474.
3) Once the kmeans algorithm was fitted with the relevant training data, a label prediction is applied to the test data. Since the centroids are not changed, we expect and get the same behaviours in the split along the axis for the features in point 1. 
4) The split between the classes for the test data are as follows: For normalised data, Class 0 has 750 points while Class 1 has 2250. For non-normalised data, Class 0 has 2224 points while Class 1 has 776.
5) Distance "probability" are placed after the labels column for the final test data. (If anyone has a better way to convert distance to probability do let me know)

## Dependencies
1) numpy
2) pandas
3) scikitlearn
4) matplotlib
