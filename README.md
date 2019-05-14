# Kmeans_ScikitLearn
Implement Kmeans clustering using scikitlearn on the California housing price data.

## The Goal
1) To implement Kmeans clustering on a dataset and observe how the data would be classified in a binary classification situation
2) To observe the impact of normalisation on the way the data is divided between the classes
3) To calculate the probability of obtaining either a 0 or 1 based on the distances of the points from the centers

## The Insights
1) When fit to the training data with normalisation, it was noted that the centers of both classes were split along the median income feature. While the fit without normalisation was split along the median house value feature.
2) Another interesting observation is that the number of data points in either classes are rather similar, ignoring the permutation of the classes. For the normalised data, Class 0 had 4536 points while Class 1 had 12464. For the non-normalised data, Class 0 had 12526 points while Class 1 had 4474.
3) Once the kmeans algorithm was fitted with the relevant training data, a label prediction is applied to the test data. While the non-normalised data kept the original axis split as observed with the training data, the normalised data seemed to exhibit a slightly different behaviour. From the graph of median house value vs median income, the clear axis split that is observable from the normalised training data was not observable in the testing data.
4) Distance probability measure used is not tested.
