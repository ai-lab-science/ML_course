# Description of Assignment 5
### Author: [Fotios Lygerakis](https://github.com/ligerfotis)

### Implement the Perceptron algorithm for classification of the Iris dataset.
* Use load_iris() from sklearn.datasets to load the Iris dataset.
    * The Iris dataset is a multiclass classification dataset with 3 classes.
    * The Iris dataset has 4 features and 150 samples.
    * The Iris dataset is a balanced dataset with 50 samples per class.
* Split the dataset into train and test sets.
* Scale the features.
* Implement the Perceptron algorithm for classification.
    * Use the unit step function as the activation function.
* Evaluate the model on the test set.
    * Use accuracy_score() from sklearn.metrics to calculate the accuracy of the model.
* Do some hyperparameter tuning to improve the accuracy of the model.
    * Try different values of the learning rate and the number of iterations.
    * Print the accuracy of the model for different values of the learning rate and the number of iterations.
### Implement Non-linear feature transformation for regression of the Concrete Compressive Strength dataset.
* Use read_excel() from pandas to load the dataset.
* The Concrete Compressive Strength dataset
    * is a regression dataset with 1 target variable.
    * has 8 features and 1030 samples.
    * has 1 target variable.
* Split the dataset into train and test sets.
* Scale the features.
* **Polynomial feature transformation**
    * Implement the polynomial_features() function to transform the features.
    * Use LinearRegression() from sklearn.linear_model to train a linear regression model.
    * Evaluate the model on the test set.
        * Use mean_squared_error() from sklearn.metrics to calculate the mean squared error of the model.
        * Use r2_score() from sklearn.metrics to calculate the R2 score of the model.
    * Train a linear regression model on the polynomial features varying the degree of the polynomial from 1 to 4.
    * Evaluate the models trained on the polynomial features on the test set and compare the mean squared error of the models.
    * Discuss the results in the report.
* **Radial Basis Function (RBF) feature transformation**
    * Implement the rbf_features() function to transform the features.
    * Use LinearRegression() from sklearn.linear_model to train a linear regression model.
    * Evaluate the model on the test set.
        * Use mean_squared_error() from sklearn.metrics to calculate the mean squared error of the model.
        * Use r2_score() from sklearn.metrics to calculate the R2 score of the model.
    * Train a linear regression model on the RBF features varying the gamma parameter from 0.1 to 10.
    * Evaluate the models trained on the RBF features on the test set and compare the mean squared error of the models.
    * Discuss the results in the report.
### **(Bonus)** Implement the Multilayer Perceptron algorithm (2 layers) for regression of the Concrete Compressive Strength dataset.
* Use train_test_split() from sklearn.model_selection to split the dataset into train and test sets.
* Use StandardScaler() from sklearn.preprocessing to scale the features.
* Implement the Multilayer Perceptron algorithm for regression.
    * The Multilayer Perceptron algorithm is a neural network with 2 layers.
    * Implement the forward propagation algorithm.
    * Implement the backward propagation algorithm.
    * Use the tanh function as the activation function for the hidden layer.
    * Use the identity function as the activation function for the output layer.
* Evaluate the model on the test set.
* Do some hyperparameter tuning to improve the accuracy of the model.
    * Try different values of the learning rate and the number of epochs.
    * Plot the mean squared error of the model for different values of the learning rate and the number of epochs.
* Compare the performance of the Multilayer Perceptron algorithm with the Linear Regression algorithm.
    * Use LinearRegression() from sklearn.linear_model to train a linear regression model.
    * Use mean_squared_error() from sklearn.metrics to calculate the mean squared error of the linear regression model.
* Compare the mean squared error of the linear regression model with the mean squared error of the multilayer perceptron model.
]()