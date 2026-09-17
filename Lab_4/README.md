Experiment 4: Comparative Study of Deep CNN Architectures Using Transfer Learning

This experiment compares different CNN architectures including LeNet-5, AlexNet, VGG16, GoogleNet and ResNet. Transfer learning is performed on the CIFAR-10 dataset using a pretrained VGG16 model with ImageNet weights. Initially, the convolutional layers are frozen and a classification head consisting of Global Average Pooling, a Dense/ReLU layer and a softmax output is added. The model is trained using Adam with a learning rate of 0.001 for 10–20 epochs.

After this, the last convolutional block is unfrozen and the model is fine-tuned for another 5–10 epochs. Performance is evaluated using accuracy, precision, recall, F1-score, confusion matrix and classification report. Different hyperparameters such as learning rate, batch size, epochs, optimizer, dense units and number of frozen layers are also tested.

The fine-tuned VGG16 model achieved 90.41% test accuracy, compared to 82.89% when the convolutional base was kept frozen. It achieved a precision of 0.9075, recall of 0.9041 and F1-score of 0.9049. The models are also compared against LeNet-5, an AlexNet-style model, GoogleNet and ResNet50.

Dataset: CIFAR-10 — 50,000 training images and 10,000 test images across 10 classes, with images of size 32×32×3.

Instructions to run: While viewing the .ipynb file, change the github in the link to githubtocolab. Select restart and run all.
