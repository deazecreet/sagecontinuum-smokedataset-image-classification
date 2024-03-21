# sagecontinuum-smokedataset-image-classification

## Overview
This project focuses on developing a machine learning model for smoke detection using the Python programming language, primarily leveraging TensorFlow and Keras. The project utilizes a pre-trained VGG16 model as the backbone for feature extraction, demonstrating the application of transfer learning to achieve high accuracy in classifying images into smoke, cloud, or other categories.

## Dataset
The dataset used in this project is the `sagecontinuum/smokedataset` available on Hugging Face. It consists of images categorized into three classes: cloud, smoke, and other. The dataset is split into training, validation, and test sets, with an 80-20 split for training and testing.

## Preprocessing
Data preprocessing steps include:
- Downloading and organizing the dataset into respective folders.
- Applying image normalization to facilitate model training.
- Creating image datasets for training and validation using TensorFlow's `image_dataset_from_directory` method.

## Model Building and Training
The core of this project is building and training a convolutional neural network (CNN) model based on the VGG16 architecture. Modifications were made to the top layer to tailor the model to our specific dataset and classification goals. The training process is monitored using a custom callback to halt training once the model achieves a specified accuracy threshold, optimizing the training time and resources.

## Results
The model achieved over 94% accuracy on both training and validation sets, demonstrating its effectiveness in smoke detection from images. A detailed evaluation, including accuracy and loss plots, provides insights into the model's performance over epochs.

## Acknowledgments
Credit to the `sagecontinuum/smokedataset` creators and any other resources that significantly aided the project.
