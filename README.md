Virtual Fence1 Project
Overview

The Virtual Fence project is designed to detect and count people entering a predefined zone within a crowded street video. The system processes an input video, tracks people, and counts those who enter a specified rectangular zone. The output video shows detected people with bounding boxes, highlights the predefined zone, and provides a real-time counter of people entering the zone.

This project compares the performance of three different detection methods: YOLOv5, VLM (Vision-Language Model), and Background Subtractor Detector (BG Subtractor).

Features

Person Detection: Detects people in the video frames.

Tracking: Tracks individuals across frames in the video.

Zone Monitoring: Defines and monitors a rectangular zone for counting people entering it.

Real-Time Counting: Displays the count of people entering the zone in real-time.

Comparison of Methods: Compares the performance of YOLOv5, VLM, and BG Subtractor methods.

Frameworks and Methods Used

PyTorch: Used for training and deploying models.

YOLOv5: A state-of-the-art object detection model that detects people in each frame.

VLM (Vision-Language Model): Used for enhanced detection capabilities, incorporating both visual and linguistic features.

BG Subtractor Detector: A background subtraction technique for detecting moving objects (people) in the scene.

These methods are compared to determine which one performs best for detecting and counting people entering the zone.

Datasets

In the next step, the project will utilize the CrowdHuman dataset along with additional data obtained from Pexels images as a supplementary dataset for fine-tuning the model. These datasets are available and will be used to improve the system's performance.

Installation
Prerequisites

Python 3.x

OpenCV

PyTorch

YOLOv5 dependencies

NumPy

Dataset Preparation

The additional dataset used for fine-tuning consists of images obtained from Pexels. These images need to be labeled before they can be used for training.

Labeling the Pexels Images:

First, you need to label the images using labeling tools like LabelImg. This involves manually drawing bounding boxes around people or objects of interest and assigning labels.

Splitting the Video:

After labeling the Pexels images, the input video (e.g., input.mp4) should be split into individual frames.

Labeling the Frames:

Once the video is split into frames, you will need to label these frames using LabelImg as well. This step helps in creating the necessary annotations for each frame.

Converting to YOLO Format:

After labeling, the annotations in XML format should be converted to the YOLO format. This is crucial for training the model with YOLOv5, as YOLO requires annotations in its own specific format.

Note: This part of the dataset preparation will be completed in the next step.

By following these steps, you can prepare the dataset for fine-tuning and ensure it is ready for model training.
