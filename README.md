# ArteFacto Machine Learning

Welcome to **ArteFacto Machine Learning**, where we are building a powerful image recognition model for the Prambanan Temple statues. Our goal is to enhance understanding and appreciation of the temple's rich cultural heritage through cutting-edge technology.

## Dataset

Our dataset, which includes high-quality images of the statues at Prambanan Temple, is available on our [Drive ](https://drive.google.com/drive/folders/1REQhQLxiZOUIh9l7CW7M9ALAsBwUllRa?usp=drive_link). It contains detailed labeled images for classification, which are crucial for training and improving the accuracy of our machine learning model.

The dataset has the following features:
- Consists of 8,061 color images in 10 classes
- Comprises 4,689 training images, 1,698 validation images, and 1674 test images.
- Classes: siwa, nandhi, wisu, brahma, gupolo, ganesa, durga, agastya, surya, candra.

Feel free to explore and contribute to the dataset as we continue to refine our approach.

## Convolutional Neural Networks - Image Classification

The objective of this project is to carry out supervised image classification on a collection of colored images. It employs a convolutional neural network design and applies data augmentation and transformations to recognize the category of images from a predefined set of 10 classes.

## Model Architecture and Training

### Convolutional Neural Network Design

We implemented a sophisticated image classification model using transfer learning with MobileNet as the base architecture. The key components of our approach include:

### Model Configuration
**Base Model:** MobileNet (pre-trained on ImageNet)
**Input Shape:** 224x224 pixels, 3 color channels
**Feature Extraction:**
 - Global Average Pooling layer
 - Dense layer with 256 neurons (ReLU activation)
 - Dropout layer (50% rate)
 - Output layer with 10 neurons (Softmax activation)

