# Chest X-Ray Pneumonia Classification

## Project Overview
This project is about classifying chest X-ray images into two groups: **Normal** and **Pneumonia**.

The main goal was to build a CNN model that can look at an X-ray image and predict the correct class from the image itself.

## Problem Statement
As a data scientist in the healthcare field, the task is to develop a convolutional neural network (CNN) that can classify medical images accurately.

In this project, the model learns from chest X-ray images and predicts whether the image shows a normal chest or pneumonia.

## Dataset
The dataset contains **5,863 JPEG X-ray images**.

It is organized into three folders:
- `train`
- `val`
- `test`

Each folder has two subfolders:
- `NORMAL`
- `PNEUMONIA`

These are chest X-ray images taken in anterior-posterior view from pediatric patients aged **1 to 5 years**.

## Tools and Libraries
I used:
- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Method Used
First, I loaded the dataset from the folder structure and checked the number of images in each class.

Then I followed these steps:

1. Set a fixed random seed
2. Loaded and resized the images to `224 x 224`
3. Normalized the pixel values
4. Applied data augmentation on the training images
5. Used class weights to handle class imbalance
6. Built a custom CNN model
7. Compiled the model with Adam optimizer and Binary Crossentropy loss
8. Trained the model with Early Stopping, Model Checkpoint, and ReduceLROnPlateau
9. Evaluated the model on the test set
10. Checked the confusion matrix and classification report

## Why CNN
CNN is a strong choice for image classification because it can learn useful patterns from images, such as edges, shapes, and textures.

That makes it suitable for medical image classification tasks like this one.

## Model Evaluation
The model was evaluated using:

- Accuracy
- Recall
- AUC Score
- Confusion Matrix
- Classification Report

### Test Results
- **Test Accuracy:** 0.8974
- **Test Recall:** 0.9436
- **Test AUC:** 0.9504

## Result
The model performed well on the test data and was able to classify chest X-ray images with good accuracy.

## Key Findings
- The dataset is imbalanced, so class weights were useful.
- The model performed better on the pneumonia class than the normal class.
- Recall was strong, which is important in medical classification.
- The final test performance shows that the CNN model learned useful patterns from the X-ray images.
