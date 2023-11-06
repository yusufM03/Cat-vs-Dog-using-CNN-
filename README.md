# Cat vs. Dog Image Classification

This project implements a Convolutional Neural Network (CNN) to classify images as either a cat or a dog. The model is trained on a dataset containing labeled images of cats and dogs, and it can predict the class of unseen images.

## Dataset

The dataset used for training and testing consists of a large collection of cat and dog images. The dataset is split into training and testing sets, allowing the model to learn from a diverse range of cat and dog images.

## Model Architecture

The CNN model used for this classification task follows the following architecture:

```
Model Architecture:
-------------------
1. Conv2D layer with 32 filters, 3x3 kernel size, 'relu' activation, and input shape (150, 150, 3)
2. MaxPooling2D layer with 2x2 pool size
3. Conv2D layer with 64 filters, 3x3 kernel size, 'relu' activation
4. MaxPooling2D layer with 2x2 pool size
5. Conv2D layer with 128 filters, 3x3 kernel size, 'relu' activation
6. MaxPooling2D layer with 2x2 pool size
7. Conv2D layer with 128 filters, 3x3 kernel size, 'relu' activation
8. MaxPooling2D layer with 2x2 pool size
9. Flatten layer
10. Dense layer with 512 units and 'relu' activation
11. Output layer with 1 unit (sigmoid activation for binary classification)
