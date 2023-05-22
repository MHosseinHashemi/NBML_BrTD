# Tensorflow Approach

This repository contains code for tumor detection and localization using Tensorflow. It includes data preprocessing, model creation, training, and evaluation.

## Features

- Preprocessing of image and annotation data
- Creation of a deep learning model for tumor detection and localization
- Training of the model using labeled data
- Evaluation of the trained model using test data

## Requirements

To run the code, you need the following dependencies:

- Python 3.6 or higher
- TensorFlow 2.0 or higher
- OpenCV
- NumPy
- Matplotlib
- tqdm

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/tumor-detection.git
   ```
   
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Prepare your image and annotation data by following the instructions provided in the Data directory.
4. Run the main script to preprocess the data, create the model, and train it:
   ```bash
   python main.py
   ```
5. Monitor the training progress and evaluate the model's performance.

## Data
The data required for tumor detection and localization consists of images and corresponding annotation files. The images should be in JPG format, and the annotation files should be in JSON format. The code provides functions to load and preprocess the data.

## Model
The model architecture used for tumor detection and localization is based on the ResNet152V2 model, a deep convolutional neural network. The model includes separate branches for bounding box regression and classification. The model architecture can be modified in the create_model function.

## Training
The training process involves splitting the data into training, validation, and test sets. The training data is used to train the model, and the validation data is used to monitor the model's performance and prevent overfitting. The test data is used to evaluate the trained model. The training progress and performance metrics are displayed during the training process.

## Evaluation
The trained model can be evaluated using the test data. Evaluation metrics such as accuracy, F1 score, and localization loss are calculated to assess the model's performance. The evaluation results can be used to determine the effectiveness of the model in tumor detection and localization.

