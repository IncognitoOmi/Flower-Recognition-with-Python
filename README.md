# Flower Recognition with Python

This project implements a flower recognition system using Python and deep learning. The dataset used consists of 4242 flower images divided into five categories: chamomile, tulip, rose, sunflower, and dandelion. The goal is to build a Convolutional Neural Network (CNN) that can classify images of flowers into their respective categories.

## Dataset

The dataset is collected from Flickr, Google Images, and Yandex Images. Each class contains approximately 800 images, with varying resolutions around 320x240 pixels.

## Requirements

To run this project, you need to install the following libraries:
pip install opencv-python-headless numpy scikit-learn tensorflow matplotlib

## Model Architecture
The CNN model consists of several layers:

Conv2D: Convolutional layers with ReLU activation
MaxPooling2D: Pooling layers to reduce the spatial dimensions
Flatten: Flattening the 2D arrays into a single long vector
Dense: Fully connected layers with softmax activation for classification

## Data Augmentation
To prevent overfitting, data augmentation techniques such as rotation, zoom, width shift, and height shift are applied using the ImageDataGenerator class from Keras.

## Training
The dataset is split into training (80%) and testing (20%) sets. The model is compiled using the Adam optimizer and categorical cross-entropy loss function. The training process includes validation on the test set to monitor performance.

## Results
The model's accuracy and loss are plotted to visualize the training process. The final accuracy on the test set is also reported.
