Experiment 2: Implement a Multi-Layer Perceptron (MLP) for multi-class image classification using TensorFlow/keras on the Fashion-MNIST dataset.

This experiment moves from the single perceptron in Experiment 1 to a full MLP with two hidden layers (128 and 64 neurons, ReLU) and a 10-way softmax output, trained on Fashion-MNIST after flattening each 28×28 image into a 784-length vector and normalizing pixel values to 0,1. The notebook covers the standard pipeline — loading the data, visualizing sample images and class distribution, building and training the model with Adam and categorical cross-entropy for 20 epochs, then evaluating it with accuracy, precision, recall, F1-score, a confusion matrix, and a full classification report.

Beyond the baseline model, the notebook also performs automated hyperparameter optimization using RandomizedSearchCV with the scikeras wrapper, searching over hidden layers, neuron counts, learning rate, batch size, optimizer, activation function, and epochs with 5-fold cross-validation. The best configuration found is then retrained and compared directly against the baseline model on accuracy, precision, recall, F1-score, and training time, with all the required plots (accuracy/loss curves, confusion matrix, search results, and the baseline-vs-optimized comparison) included alongside short inferences for each.

Datasets: Fashion-MNIST (60,000 training images, 10,000 testing images, 10 classes, 28×28 grayscale).

Instructions to run:

While viewing the .ipynb file, change the github in the link to githubtocolab.
Select restart and run all.

Note: there is a small section training a single-layer perceptron on the XOR gate, aka the notebook XORpart, carried over from the logic-gate work in Experiment 1, to demonstrate that a single perceptron cannot converge on a nonlinearly separable problem
