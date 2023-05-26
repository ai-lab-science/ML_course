# Description of Assignment 6
### Author: [Fotios Lygerakis](https://github.com/ligerfotis)
### Implementing Gaussian Processes in Python

In this assignment, your task is to implement the Gaussian Processes algorithm as a class in Python. Gaussian Processes are a powerful tool for probabilistic regression and can be used for various machine learning tasks. The goal of this assignment is to gain a deeper understanding of Gaussian Processes and their implementation.

#### GaussianProcess class
Implement the class that can perform the following tasks:

* Fit the model: The class should be able to fit the model to a given training data set (X, y), where X is an n x d matrix representing the input features, and y is an n-dimensional vector representing the target values

* Predict the output: The class should be able to predict the output for a given test data set X*, where X* is an m x d matrix representing the input features of the test data. The predicted output is obtained by using the training data and the estimated covariance structure to infer the most likely target values for the test data points.

* Compute log marginal likelihood: The class should be able to compute the log marginal likelihood of the training data set. The log marginal likelihood measures how well the model with its estimated hyperparameters explains the observed training data. It is used as an optimization objective for finding the best hyperparameters(no need to do that).

* Compute predictive mean and variance: The class should be able to compute the predictive mean and variance for a given test data set X*. The predictive mean represents the expected value of the target variable for each test data point, while the predictive variance indicates the uncertainty associated with the predictions.


#### Kernel Functions
You need to implement the following kernel functions:

* Linear kernel: The linear kernel computes the dot product between the input features. It is defined as k(x, x') = x.T @ x', where x and x' are input feature vectors.

* Polynomial kernel: The polynomial kernel computes the dot product between the input features raised to a certain power. It is defined as k(x, x') = (x.T @ x' + 1)^d, where x and x' are input feature vectors, and d is the degree of the polynomial.

* Periodic kernel: The periodic kernel captures the periodic patterns in the data. It is defined as k(x, x') = exp(-2 * sin^2(π * ||x - x'|| / p) / σ^2), where x and x' are input feature vectors, p is the period, and σ controls the smoothness of the periodicity.

* Gaussian kernel: The Gaussian kernel captures the similarity between data points based on their distance. It is defined as k(x, x') = exp(-||x - x'||^2 / (2 * σ^2)), where x and x' are input feature vectors, and σ controls the width of the Gaussian distribution.

#### Testing and Comparison
To validate your implementation, you should test it on 1D, 2D, and 3D data sets. Compare the results of your implementation with the scikit-learn Gaussian Processes implementation. Perform visual comparisons and analyze the performance metrics to evaluate the accuracy and efficiency of your implementation.

### Bonus Exercise

For the bonus exercise, utilize the Gaussian Process to fit any dataset of your choice. Provide a brief description of the dataset you have chosen, including the number of samples, the number of features, and the nature of the target variable. Explain why you believe the Gaussian Process is well-suited for modeling this particular dataset.



Note: It is recommended to break down your implementation into smaller functions to improve code modularity and readability.

Good luck with your implementation!