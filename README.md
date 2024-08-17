# TomatoSaviorAI

This project is a Tomato Disease Classification Model implements a deep learning model for identifying and classifying different diseases in tomato plants using images of their leaves. The model is built using TensorFlow and Keras and is capable of recognizing various tomato leaf diseases with 96.11% accuracy on the test dataset.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Predictions](#predictions)
- [Usage](#usage)



## Overview

The goal of this project is to accurately classify images of tomato leaves into various disease categories. The model was trained on a labeled dataset of tomato leaf images from Kaggle and can identify diseases such as Tomato Late Blight, Tomato Yellow Leaf Curl Virus, and others.

## Dataset

The dataset used for this project consists of labeled images of tomato leaves with various diseases. The data is divided into 80% training, 10% validation, 10% test sets to evaluate the model's performance accurately. The dataset initially consisted of Potatoes and Tomatoes but later removed to just focus on Tomatoes.
Dataset Link: https://www.kaggle.com/datasets/arjuntejaswi/plant-village


## Model Architecture

The model is based on a Convolutional Neural Network (CNN) architecture. Below is a summary of the model:

- **Input Layer:** Images of size 256x256 pixels.
- **Convolutional Layers:** Multiple layers with ReLU activation and max pooling.
- **Fully Connected Layers:** Dense layers for classification.
- **Output Layer:** Softmax activation for multiclass classification.

## Training

The model was trained using the Adam optimizer and Sparse Categorical Crossentropy loss function. The training was performed over 8 epochs, achieving a validation accuracy of over 90%. 

<img width="1512" alt="Screenshot 2024-08-17 at 12 53 28 AM" src="https://github.com/user-attachments/assets/c6a2dc7d-5ada-43d6-b2b9-f4d53e72517d">


## Predictions

Below are examples of predictions made by the model:

### Example 1: Tomato Late Blight
- **Actual Label:** Tomato Late Blight
- **Predicted Label:** Tomato Late Blight

<img width="1512" alt="Screenshot 2024-08-17 at 1 35 34 AM" src="https://github.com/user-attachments/assets/ab3d52cf-6c58-4545-89e6-dc4136d42bf6">


### Example 2: Tomato Yellow Leaf Curl Virus
- **Actual Label:** Tomato Yellow Leaf Curl Virus
- **Predicted Label:** Tomato Yellow Leaf Curl Virus

<img width="1512" alt="Screenshot 2024-08-17 at 1 35 45 AM" src="https://github.com/user-attachments/assets/e054d650-35c4-4ba4-bcae-515eea5c8b13">


## Usage

To use this model, clone the repository and run the Jupyter notebook provided:

```bash
git clone https://github.com/your_username/TomatoSaviorAI.git
cd TomatoSaviorAI
pip install -r requirements.txt
jupyter notebook tomato_model.ipynb
