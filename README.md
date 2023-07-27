# Drowsiness Detection with YOLOv5

In this project, we showcase the development of a Drowsiness Detection System using the YOLOv5 object detection model. The system is designed to classify a person's state in real-time as either 'awake' or 'drowsy'.

## Overview

The development process of the Drowsiness Detection system consists of several stages:

1. **Installing and Importing Dependencies:** Setting up the right environment with necessary packages is the first step.
2. **Loading the Pre-trained YOLOv5 Model:** We initially utilize the YOLOv5 model pre-trained on the COCO dataset. The model is loaded from the Torch Hub, a repository of pre-trained models.
3. **Real-time Detections with Pre-trained Model:** The pre-trained model is tested by performing real-time object detection on video stream captured from the webcam.
4. **Image Collection and Labeling:** To create a custom model for drowsiness detection, we collect and label images showcasing 'awake' and 'drowsy' states.
5. **Training the Custom Model:** The labeled images are then used to train our custom YOLOv5 model.
6. **Testing the Custom Model:** The final step involves loading the trained custom model and testing its performance on unseen images. We also test the model on real-time video stream for drowsiness detection.

## Custom Model Training

Training our custom model is crucial to achieve accurate drowsiness detection. This model is trained on a dataset containing images of people in 'awake' and 'drowsy' states. Training the model on such specific data allows it to learn features pertinent to these states, thereby aiding accurate detection. The image dataset is labeled appropriately to facilitate this learning.

## Real-Time Drowsiness Detection

The highlight of this project is the real-time drowsiness detection feature. After training our custom model, we utilize it to classify the state of a person in real-time. This is achieved by continuously feeding frames from the webcam video stream to the model and displaying the detections on screen.

## Potential Improvements

This project offers a beginner-level implementation of drowsiness detection. While the initial results are promising, there's always room for improvements:

- **Data Augmentation:** We can improve the model's performance by providing a larger, more diverse dataset for training.
- **Fine-Tuning:** Parameters like confidence thresholds can be tuned to achieve better detection accuracy.
- **Advanced Features:** Implementing additional features, such as yawning detection or eye closure detection, can enhance the overall accuracy and usefulness of the system.

## Conclusion

This Drowsiness Detection System, powered by YOLOv5, serves as a basic implementation of real-time state classification. The project provides an opportunity to explore object detection applications using the powerful YOLOv5 model. Despite the potential for improvements and additions, the existing system serves as an effective demonstration of the concept.
