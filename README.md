# BrTD as an Anomally Detection Probelm

## Overview
This repository is an ongoing research project that explores the capabilities of YOLOv8, a deep learning model, for the detection of brain tumors in medical images. It leverages computer vision and machine learning techniques to effectively identify and localize tumors in brain scans, with the ultimate goal of advancing tumor detection accuracy.

## Features
- Convert JSON labels to YOLO format.
- Split data into training, validation, and test sets.
- Move images and labels to their respective folders.
- Train the YOLOv8n model on the custom dataset.
- Test the trained model on new images and save the predictions.
- Perform object detection on new images and save the output with bounding boxes.

## Preprocess the data:
- Set the image size and define the image_divider function.
- Call the image_divider function to collect the image paths.
- Split the data into train, validation, and test sets.
- Clean the labels and move the images and labels to their respective folders.
- Create dummy coordinates for images without tumors.
## Training:
- Initialize the YOLOv8n model.
- Train the model using the custom dataset.
## Testing:
- Predict the objects in new images using the trained model.
- Save the predictions with confidence scores and bounding box coordinates.
- Perform object detection on new images:
- Set the root and destination paths for new images.
- Call the perform_detection function to perform object detection.
- Save the output with bounding boxes in the patient's destination folder.
## Results
- The YOLOv8n model achieves an accuracy of XX% on the custom dataset.
- The model successfully detects and localizes objects of interest in new images.
- The predictions are saved with confidence scores and bounding box coordinates.
## Detections (In Progress):

<p align="center">
  <img src="https://github.com/MHosseinHashemi/NBML_BrTc/assets/90381570/0f8ee6df-852a-4c41-993b-3c14aa97b997" width="180" />
  <img src="https://github.com/MHosseinHashemi/NBML_BrTc/assets/90381570/8d7b86f2-2edf-4095-8342-725498865f1c" width="180" />
  <img src="https://github.com/MHosseinHashemi/NBML_BrTc/assets/90381570/6e589454-5b3d-4f42-be65-2d34e24fcf8e" width="180" />
  <img src="https://github.com/MHosseinHashemi/NBML_BrTc/assets/90381570/942bd66d-cd79-4002-9318-42c757b26791" width="180" />
  <img src="https://github.com/MHosseinHashemi/NBML_BrTc/assets/90381570/532cf001-50a4-474f-b392-51bc2c5fe62d)" width="180" />
</p>

Performance Metrics of the models will be released eventually ...








## License
This project is licensed under the Apache 2 License.

## Acknowledgements
- Ultralytics YOLO for the YOLO implementation.
- labelme2yolo for converting JSON labels to YOLO format.
- OpenCV for image processing and manipulation.
