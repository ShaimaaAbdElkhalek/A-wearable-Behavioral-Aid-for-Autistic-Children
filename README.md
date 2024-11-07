# Wearable Behavioral Aid for Autistic Children

A graduation project from the Faculty of Engineering, Biomedical Engineering Department, designed to assist children with Autism Spectrum Disorder (ASD) in recognizing and interpreting emotions in social interactions. This wearable device, integrated with a deep learning model and mobile application, aims to enhance social communication skills by providing real-time feedback on the emotions of people around the wearer.



1. [Project Overview](#project-overview)
2. [Key Features](#key-features)
3. [Motivation](#motivation)
4. [System Architecture](#system-architecture)
5. [Data and Models](#data-and-models)
6. [Technologies Used](#technologies-used)
7. [Methodology](#methodology)
   - [Data Collection and Pre-processing](#data-collection-and-pre-processing)
   - [Model Development](#model-development)
   - [Mobile Application and Hardware Integration](#mobile-application-and-hardware-integration)
8. [Results and Findings](#results-and-findings)
9. [Future Work](#future-work)
10. [Contributors](#contributors)
11. [Acknowledgments](#acknowledgments)
12. [Full Documentation](#full-documentation)

---

## Project Overview

ASD affects social interaction, communication, and behavior, often making it challenging for individuals to interpret social cues. This project proposes a wearable device in the form of glasses equipped with a camera, integrated with a mobile app, that processes facial expressions through a predictive deep learning model. By identifying emotions in real-time, the system can provide immediate feedback to children with ASD, potentially improving their understanding and engagement in social situations.
# Table of Contents

## Key Features

- **Real-time Emotion Recognition**: Recognizes facial expressions and emotions in real-time using deep learning algorithms.
- **Wearable Device**: Glasses with a built-in camera to capture social cues.
- **Mobile Application Integration**: The application is designed to be user-friendly, allowing caregivers and individuals with ASD to receive emotion recognition data.
- **Transfer Learning Optimization**: Utilizes transfer learning with models like EfficientNetB7 and MobileNetV2 to enhance accuracy and reduce computational requirements.
- **Real-world Application**: Tested and validated in collaboration with professionals in autism research.
  
## Motivation
Autism Spectrum Disorder impacts individuals' ability to interpret nonverbal cues, such as facial expressions, which are essential for social interactions. This wearable aid aims to enhance independence and improve social communication skills for children with ASD, using deep learning and wearable technology.

## System Architecture
The project consists of three primary components:
1. **Emotion Recognition Model**: A CNN model with optimized transfer learning from MobileNetV2 and EfficientNetB7, achieving a high accuracy in emotion classification.
2. **Mobile Application**: A mobile app for Android devices that displays the detected emotions and offers educational resources.
3. **Smart Glasses Hardware**: Glasses equipped with an Esp32 camera module connected to the mobile app for real-time emotion analysis and feedback.

## Data and Models
- **Datasets**: The model is trained on FER2013, CK+, and AffectNet datasets, augmented and balanced to improve accuracy across diverse expressions.
- **Models Used**:
  - **Custom CNN**: Built for initial training.
  - **Transfer Learning**: Fine-tuned MobileNetV2 and EfficientNetB7 models for enhanced accuracy in real-world scenarios.

## Technologies Used

- **Machine Learning**: Convolutional Neural Networks (CNN) for image processing and emotion classification.
- **Deep Learning Models**: EfficientNetB7, MobileNetV2, VGG16, ResNet50.
- **Data Processing**: Dataset augmentation, balancing, and normalization for optimal performance.
- **Mobile Application Development**: Android-based mobile application with a Bluetooth interface for real-time updates from the wearable device.
- **Hardware**: ESP32 camera module, Arduino Uno for connecting the camera to the mobile app.

## Methodology

1. **Data Collection and Pre-processing**:
   - Data collected from CK+, AffectNet, and FER2013 datasets.
   - Pre-processed images through resizing, grayscale conversion, and data augmentation.

2. **Model Development**:
   - Trained several CNN models for emotion recognition, experimenting with different architectures and transfer learning techniques.
   - Evaluated models based on accuracy, loss, and real-time prediction performance.

3. **Mobile Application and Hardware Integration**:
   - Developed an Android application to interface with the glasses via Bluetooth.
   - The app provides real-time emotion feedback through visual cues.

## Results and Findings

- **Model Accuracy**: The EfficientNetB7 model achieved the highest accuracy of 91% in identifying emotions.
- **Real-time Performance**: MobileNetV2 demonstrated the best real-world application performance.
- **Impact**: This system offers ASD individuals greater independence in social situations by providing accessible emotional feedback.

## Future Work

- **Enhanced Hardware Integration**: Integrate more sensors for environmental awareness.
- **Expanded Emotion Categories**: Train models to recognize a wider range of emotions.
- **Generalization**: Test on a broader population and improve accuracy in diverse social settings.


## Contributors
- **Shaimaa Abd Elkhalek**  
- **Abdulrhman Nasser**
- **Merna Ahmed Mansour**
- **Supervisor**: Dr. Ibrahim Sadek

## Acknowledgments

This project was supported by the Information Technology Industry Development Agency (ITIDA) through the Graduation Projects Support program. Special thanks to our families and friends for their support throughout our studies.

---

*For more details, please refer to the full project documentation.*
