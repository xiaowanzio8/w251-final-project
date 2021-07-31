# Doorstep Package Recognition 
Team Members: John A, Jyoti K, Clayton M, Ming C

## Introduction

This project is about an automated doorstep package detection system that uses deep learning to identify multiple classes of packages in real time. Our team generated an object detection dataset and augmented that data to become robust to adverse weather, motion, and lighting conditions. We trained a YOLOv5 object detection model in AWS and deployed that model on a Kubernetes cluster on the edge. We then used the model to classify packages in a live webcam feed and broadcast the results using a MQTT broker.

## Data

Details about data collection, Annoation and Augmentation are available at: 
- [Data collection, Annotation and Augmentation](https://github.com/johnmandrus/w251-final-project/tree/main/1-data)

## Model Selection and Training Metrics

Model training details and metrics are available at: 
- [Model Selection and Training Metrics](https://github.com/johnmandrus/w251-final-project/tree/main/2-model)
- [data.yaml](https://github.com/johnmandrus/w251-final-project/blob/main/2-model/data.yaml)
- [training Yolov5s](https://github.com/johnmandrus/w251-final-project/blob/main/2-model/yolov5s.ipynb)

## Inference

- [Using NX](https://github.com/johnmandrus/w251-final-project/tree/main/3-architecture)
- [Container 1 - package-detector](https://github.com/johnmandrus/w251-final-project/tree/main/3-architecture/1-package-detector)
- [Container 2 - package-broker](https://github.com/johnmandrus/w251-final-project/tree/main/3-architecture/2-package-broker)
- [Container 3 - package-logger](https://github.com/johnmandrus/w251-final-project/tree/main/3-architecture/3-package-logger)
- [Inference](https://github.com/johnmandrus/w251-final-project/tree/main/3-architecture/inference)

## Reports
- [Reports and Presentation](https://github.com/johnmandrus/w251-final-project/tree/main/4-report-and-presentation)

