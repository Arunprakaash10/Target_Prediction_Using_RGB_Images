# Target Prediction Using RGB Images

## Project Overview

This repository contains the implementation of **Target Prediction Using RGB Images**, focusing on two key applications:
1. **Intrusion Detection**: Detect human presence in restricted areas using real-time object detection.
2. **Missile Guidance**: Detect and track targets such as battle tanks to guide missiles using precise angle calculations.

The system utilizes deep learning models, specifically **YOLOv3** and **YOLOv8**, to perform real-time object detection and prediction.

## Project Details

- **Project Title**: Target Prediction Using RGB Images
- **Institution**: Sri Sivasubramaniya Nadar College of Engineering
- **Team Members**:
  - Anjana Narayan Rao
  - Anuprapaa V R
  - Arun Prakaash C

## Features

- **Intrusion Detection**: Uses YOLOv8 to monitor live CCTV footage and detect unauthorized human presence in predefined restricted areas.
- **Missile Guidance**: Implements a guidance system using YOLOv3 to detect battle tanks and compute the necessary angles for missile maneuvering.
- **Custom Object Tracking**: Tracks detected objects across frames to ensure accurate movement prediction.

## Methodology

1. **Human Intrusion Detection**:
   - Detects intrusions using pre-trained YOLOv8 models.
   - Tracks objects across frames and triggers alarms when individuals cross into restricted zones.
   
2. **Missile Guidance**:
   - Uses YOLOv3 to detect targets (e.g., battle tanks).
   - Calculates angles to adjust missile trajectory based on object location relative to the center of the image.
   
3. **Model Training**:
   - Collected a custom dataset of battle tanks using Roboflow.
   - Preprocessed images to 640x640 pixels and trained the YOLOv8 model.

## Results

- **Intrusion Detection**: Achieved an accuracy of 88% on CCTV footage.
- **Missile Guidance**: Successfully predicted the correct missile maneuvering angles for 24 out of 29 images in the test dataset.
- **Battle Tank Detection**: The model exhibited 88.9% precision and 100% recall after 50 training epochs.
