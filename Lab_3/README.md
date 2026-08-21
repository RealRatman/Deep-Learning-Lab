Experiment 3: Implement a Convolutional Neural Network (CNN) for multi-class image classification using TensorFlow/Keras on the CIFAR-10 dataset.

This experiment implements a full CNN that preserves spatial structure, with two Conv2D+ReLU+MaxPool blocks followed by a flatten, a dense hidden layer, and a 10-way softmax output, trained on CIFAR-10 after normalizing pixel values to [0,1]. This pipeline consists of loading the data, visualizing sample images and class distribution, studying how kernel size, stride, and padding affect output feature-map dimensions, visualizing learned filters and feature maps from the first convolutional layer, building and training the model with Adam and sparse categorical cross-entropy for 20 epochs with batch size 32, then evaluating it with accuracy, precision, recall, F1-score, a confusion matrix, and a full classification report.

Beyond the baseline model, theres hyperparameter ablation studies, training a fresh model for each setting and comparing test accuracy: max vs. average pooling, ReLU vs. sigmoid activation, and 16 vs. 64 convolutional filters (accuracy and training time both measured).
Datasets: CIFAR-10 (50,000 training images, 10,000 testing images, 10 classes, 32×32 RGB).

Instructions to run:
While viewing the .ipynb file, change the github in the link to githubtocolab. Select restart and run all.
