# BrTD as an Anomally Detection Problem

## Overview
This repository is an ongoing project that explores the capabilities of YOLOv8, a deep learning model, for the detection of brain tumors in medical images. It leverages computer vision and machine learning techniques to effectively identify and localize tumors in brain scans, with the ultimate goal of advancing tumor detection accuracy.

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
- The model successfully detects and localizes objects of interest in new images.
- The predictions are saved with confidence scores and bounding box coordinates.
## Detections (In Progress):

<p align="center">
  <img src="https://github.com/MHosseinHashemi/NBML_BrTD/assets/90381570/b973b6d4-754f-499b-b3c9-0142be9aec13" width="200" />
  <img src="https://github.com/MHosseinHashemi/NBML_BrTD/assets/90381570/6ca03316-0c35-4069-aa4c-9d358571109a" width="200" />
  <img src="https://github.com/MHosseinHashemi/NBML_BrTD/assets/90381570/351d0563-ab18-405b-a1f7-a73800aace22" width="200" />
  <img src="https://github.com/MHosseinHashemi/NBML_BrTD/assets/90381570/2a17250d-f6ba-4ce2-8e26-8e330c436717" width="200" />
</p>

Performance Metrics of the models will be released eventually ...


## License
This project is licensed under the Apache 2 License.

## Acknowledgements
- Ultralytics YOLO for the YOLO implementation.
- labelme2yolo for converting JSON labels to YOLO format.
- OpenCV for image processing and manipulation.
