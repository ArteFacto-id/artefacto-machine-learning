# ArteFacto Machine Learning

Welcome to **ArteFacto Machine Learning**, where we are building a powerful image recognition model for the Prambanan Temple statues. Our goal is to enhance understanding and appreciation of the temple's rich cultural heritage through cutting-edge technology.

## Dataset

Our dataset, which includes high-quality images of the statues at Prambanan Temple, is available on our Google Drive. It contains detailed, labeled images that are crucial for training and improving the accuracy of our machine learning model. After preprocessing the data, the processed dataset can be accessed here.

The dataset has the following features:

Consists of 8,061 color images categorized into 10 classes.
Includes 4,689 training images, 1,698 validation images, and 1,674 test images.
Classes: Siwa, Nandhi, Wisu, Brahma, Gupolo, Ganesa, Durga, Agastya, Surya, and Candra.

Feel free to explore and contribute to the dataset as we continue to refine our approach.

## Convolutional Neural Networks - Image Classification

The objective of this project is to carry out supervised image classification on a collection of colored images. It employs a convolutional neural network design and applies data augmentation and transformations to recognize the category of images from a predefined set of 10 classes.

## Model Architecture and Training

### Convolutional Neural Network Design

We implemented a sophisticated image classification model using transfer learning with MobileNet as the base architecture. The key components of our approach include:

### Model Configuration
**Base Model:** MobileNet (pre-trained on ImageNet) <br/>
**Input Shape:** 224x224 pixels, 3 color channels <br/>
**Feature Extraction:**
 - Global Average Pooling layer
 - Dense layer with 256 neurons (ReLU activation)
 - Dropout layer (50% rate)
 - Output layer with 10 neurons (Softmax activation)

### Training Parameters
**Optimizer:** [Adam](https://www.tensorflow.org/api_docs/python/tf/keras/optimizers/Adam) (learning rate: 0.00001) <br/>
**Loss Function:** [Categorical Crossentropy](https://www.tensorflow.org/api_docs/python/tf/keras/losses/categorical_crossentropy). <br/>
**Epochs:** 20 <br/>
**Early Stopping:** Monitored validation loss <br/>

### Performance Metrics
**Initial Training Accuracy:** 14.09% (Epoch 1) <br/>
**Final Training Accuracy:** 94.76% <br/>
**Final Validation Accuracy:** 98.41% <br/>
**Total Model Parameters:**
 - Trainable Parameters: 264,970
 - Non-trainable Parameters: 3,228,864

### Training Progression Highlights
- Rapid accuracy improvement in initial epochs
- Consistent reduction in loss
- Minimal overfitting
- Stable validation performance

### Class Distribution
The dataset shows a balanced distribution across 10 statue classes : <br/>
 - Most represented class: Statue 6 (634 training images)(
 - Least represented class: Statue 8 (415 training images)

## Visualization

![visualization-CNN](https://github.com/user-attachments/assets/afeed0f3-769a-4821-9369-20ca13d49216)
