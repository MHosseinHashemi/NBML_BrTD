# Brain Tumor Detection as an Anomally Detection Probelm

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


## License
This project is licensed under the Apache 2 License.

## Acknowledgements
Ultralytics YOLO for the YOLO implementation.
labelme2yolo for converting JSON labels to YOLO format.
OpenCV for image processing and manipulation.
