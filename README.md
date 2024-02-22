# Diabetic-Retinopathy-GDSC-Solution-Challenge-2024
______________________________________________________
## Overview
This repository contains the code for our solution to the Diabetic Retinopathy GDSC Solution Challenge 2024. Our solution involves a Convolutional Neural Network (CNN) model integrated within a system for diagnosing diabetic retinopathy.


## Demo Video
Check out our system prototype in action! Watch the demo video below:
https://youtu.be/ec3B4SaQItE


## Dataset Source
We obtained the dataset used in this project from (https://www.kaggle.com/datasets/sovitrath/diabetic-retinopathy-224x224-gaussian-filtered)

 The dataset consists of retinal images annotated for diabetic retinopathy severity levels. It includes images from various sources and is labeled by expert ophthalmologists for training and evaluation of machine learning models for diabetic retinopathy diagnosis.


## Running the Code

To run the code, simply open the provided notebook file in Jupyter Notebook or Google Colab. All required libraries are already included in the notebook.

## Preprocessing

We performed preprocessing on the images before feeding them into our model. The preprocessing steps include applying Gaussian filters to enhance image quality and reduce noise, improving the model's ability to extract relevant features from the images.


## Model Architecture
Our model architecture is based on a pre-trained DenseNet121 convolutional neural network (CNN) model, which has been widely used for image classification tasks. The DenseNet121 model is pre-trained on the ImageNet dataset, allowing it to effectively extract high-level features from images.

We fine-tuned the DenseNet121 model by adding additional layers on top to adapt it to our specific task of diabetic retinopathy diagnosis. This involved adding a Flatten layer to convert the output of the DenseNet121 model into a one-dimensional tensor, followed by a fully connected dense layer with ReLU activation function to further process the features. Dropout regularization was applied to prevent overfitting, and a softmax activated dense layer with multiple units was used for multi-class classification of diabetic retinopathy severity levels.

This architecture enables our model to effectively learn and extract relevant features from retinal images, allowing it to make accurate predictions for diabetic retinopathy diagnosis.


### Gradio Interface

We created a Gradio interface for our solution, allowing users to interactively upload retinal images and obtain diagnostic predictions in real-time. The Gradio interface provides a user-friendly way to utilize our solution without requiring any programming knowledge.


