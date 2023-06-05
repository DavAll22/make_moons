# Make Moons

Project usilising the Scikit-Learn `make_moons()` dataset to classify a binary dataset using a simple Neural Network built in TensorFlow 2.X.

## This project uses:
* TensorFlow 2.X to create, train and evaluate the performance of binary classification
* Sequential API to build a simple neural network composed of 3 fully-connected Dense layers with sigmoid activation
* Decision boundary plotting on the dataset

![image](https://github.com/DavAll22/make_moons/assets/124359152/9967767c-9732-49e5-bf4c-983738ff1f51)

## Evaluation
* On the training data, the model achieves a loss of 0.019 and an accuracy of 99.62%
* On the test data, the model achieves a loss of 0.015 and an acucracy of 100.00%
* The results are validated simultaneously when training the model

![image](https://github.com/DavAll22/make_moons/assets/124359152/e2ff675f-2389-451a-82ea-0c0dbc08a18f)
![image](https://github.com/DavAll22/make_moons/assets/124359152/2a215168-fd14-4c3b-8c1d-d05f483511c0)

  * The results are dependent on the noise in generating the moons dataset: more noise in the dataset leads to a harder to fit decision boundary and more samples crossing the boundary, increasing loss and reducing accuracy.
* The model is used t predict on the test data and a confusion matrix plotted
