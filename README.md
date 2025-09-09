Description
This project uses Convolutional Neural Networks (CNN) to classify driver behaviors into five categories using the Revitsone-5classes dataset.
Dataset

The dataset contains 5 classes of driver behaviors:

safe_driving

texting_phone

talking_phone

turning

other_activities

The dataset can be downloaded from Kaggle: Revitsone-5classes.
Steps in the Notebook
1. Setup

Install Kaggle API and download the dataset

Unzip dataset in Colab

Automatically detect dataset folder

!pip install kaggle


Upload your kaggle.json API key, configure it, and download the dataset.
Dataset Splitting

The dataset is manually split into train, validation, and test sets using the following ratios:

70% train

15% validation

15% testData Preprocessing

Images are loaded using ImageDataGenerator with rescaling:
CNN Model Architecture

The CNN model consists of:

Conv2D + MaxPooling layers

Flatten layer

Dense layers

Softmax output for 5 classes
Model Training

The model is trained with:

Epochs: 10

Batch size: 32
