# Make Moons

Project usilising the Scikit-Learn `make_moons()` dataset to classify a binary dataset using a simple Neural Network built in TensorFlow 2.X.

## This project uses:
* TensorFlow 2.X to create, train and evaluate the performance of a binary classification dataset
* Sequential API to build a simple neural network composed of 3 fully-connected Dense layers with sigmoid activation
* Decision boundary plotting on the dataset

![image](https://github.com/DavAll22/make_moons/assets/124359152/9967767c-9732-49e5-bf4c-983738ff1f51)

The dataset is split in an 80:20 split of training data to test data. The model validates using the test data during the training of the model.

The labels used in the dataset are one-hot encoded by default [0, 1] but since it is binary data, `binary_crossentropy` is used in the loss function.


## Evaluation
* On the training data, the model achieves a loss of 0.019 and an accuracy of 99.62%
* On the test data, the model achieves a loss of 0.015 and an acucracy of 100.00%

![image](https://github.com/DavAll22/make_moons/assets/124359152/e2ff675f-2389-451a-82ea-0c0dbc08a18f)
![image](https://github.com/DavAll22/make_moons/assets/124359152/2a215168-fd14-4c3b-8c1d-d05f483511c0)

  * The results are dependent on the noise in generating the moons dataset: more noise in the dataset leads to a harder to fit decision boundary and more samples crossing the boundary, increasing loss and reducing accuracy.

## Predictions
* Prediction probabilities for each class is generated from the test data and the corresponding class label is assigned by rounding the value at the boundary of 0.5. 
* A confusion matrix is plotted from the predictions
