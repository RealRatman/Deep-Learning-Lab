Experiment 5: Comprehensive Study of CNN Training, Regularization, Optimization, Hyperparameter Tuning, Transfer Learning and Cross-Validation

This experiment studies how different training techniques and hyperparameters affect the performance of a CNN. MobileNetV2 is used as the main architecture, and the Oxford-IIIT Pet dataset is used for training and evaluation. The dataset contains images from 37 different pet breeds, which are resized to 224×224×3.

Different weight initialization methods such as Zero, Random, Xavier and He initialization are compared first. The experiment also tests different regularization techniques, including no regularization, L2 regularization, Dropout and Batch Normalization. Different optimizers such as SGD, Momentum, RMSProp and Adam are also compared using training and validation curves.

After this, hyperparameter tuning is performed by changing the learning rate, batch size and dropout rate to see how they affect model performance. Transfer learning with MobileNetV2 is also tested by comparing a model with the pretrained feature extractor frozen against a model where some layers are unfrozen and fine-tuned.

Finally, three different configurations are compared using 5-fold cross-validation. The mean accuracy and standard deviation, along with the training time, are used to select the final configuration. The selected model is then retrained using the complete training set and evaluated on the held-out test set.

The baseline configuration using Adam optimizer, Xavier initialization and no additional regularization achieved the best overall result. It obtained 90.60% test accuracy, with 91.72% precision, 90.60% recall and 90.58% F1-score. The baseline also provided a good balance between accuracy, variation across the cross-validation folds and training time. Two additional configurations were tested after this, but both performed worse than the baseline.

Dataset: Oxford-IIIT Pet —> 37 breeds, RGB images resized to 224×224×3.

Instructions to run: Open the .ipynb file, change github in the link to githubtocolab, open it in Google Colab, select Restart and Run All, and wait for all the cells to finish executing.
