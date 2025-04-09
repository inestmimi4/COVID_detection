# COVID-19 vs Healthy Lung Classification

This repository contains a deep learning model for classifying chest X-ray images as either **COVID-19** or **Healthy**. The model is built using a Convolutional Neural Network (CNN) with Keras.

## Overview

The objective of this project is to train a CNN model to distinguish between COVID-19 infected lungs and healthy lungs based on X-ray images. The model is trained using images that are augmented to improve its generalization capabilities.

## Features

- **Image Preprocessing**: 
  - Images are rescaled, rotated, zoomed, and flipped using Keras' `ImageDataGenerator` to create a more diverse training dataset and help prevent overfitting.
  
- **CNN Architecture**:
  - The model consists of Conv2D layers for feature extraction, MaxPooling2D layers for down-sampling, and Dense layers for classification.
  
- **Optimization**:
  - The model uses the Adam optimizer and binary cross-entropy loss function.
  - Early stopping is applied to prevent overfitting, saving the best model based on validation loss.
  
- **Metrics**:
  - The model's performance is monitored using accuracy and loss curves for both training and validation sets.
  - After training, the model's performance is evaluated using a confusion matrix and classification report.

## Dataset

The dataset is divided into three directories:
- `TRAIN/`: Contains the training images for both **COVID-19** and **Healthy** classes.
- `VAL/`: Contains the validation images for both **COVID-19** and **Healthy** classes.
- `TEST/`: Contains the test images (used for final evaluation).

### Dataset Structure:
