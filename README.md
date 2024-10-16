# Waste Classification using Attention-Based Deep Learning Models

This project implements a custom deep learning model to classify waste into organic and recyclable categories. The project includes the development of a web app and an Android app, where the model is deployed using TensorFlow Lite (TFLite) for real-time waste classification.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Model Architecture](#model-architecture)
4. [Model Comparisons](#model-comparisons)
5. [Web App Flow](#web-app-flow)
6. [Android App](#android-app)
7. [Future Enhancements](#future-enhancements)
8. [Research Paper](#research-paper)


## Project Overview
Effective waste management is an increasingly critical global challenge. This project aims to address it by using machine learning to automate waste classification into organic and recyclable categories. We designed a custom Convolutional Neural Network (CNN) with Convolutional Block Attention Modules (CBAM) and compared its performance with popular architectures like VGG16 and ResNet50.

The model has been optimized and converted into TensorFlow Lite (TFLite) for real-time deployment in both web and Android applications, making it lightweight and efficient for use on devices with limited computational resources.

## Dataset
We used the **Waste Classification Dataset** sourced from Kaggle, which consists of 25,077 labeled images divided into two classes: Organic and Recyclable.

The dataset is evenly distributed between the two classes, with the following breakdown:

- Organic: 12,640 images
- Recyclable: 12,437 images

![Dataset Class Distribution](https://github.com/user-attachments/assets/e6621ada-3d93-43b4-b157-b57322a9615e)

![Dataset Class Distribution](https://github.com/user-attachments/assets/a3d2b917-031e-4358-a05b-e51199749b45)


## Model Architecture
Our custom CNN incorporates CBAM to enhance feature extraction. Below is a flowchart of the model’s architecture, showing how data flows from input to output, with attention mechanisms improving model performance:

![Model Architecture](https://github.com/user-attachments/assets/f281bab9-8be2-498b-9b63-46796ac2fde3)

The model was trained using various data augmentation techniques, achieving a test accuracy of **90.77%** on the Waste Classification Dataset.

## Model Comparisons
We compared our custom model with well-known architectures like VGG16 and ResNet50. Our model showed competitive performance, with the added benefit of lower computational requirements.

- **Custom Model Accuracy**: 90.77%
- **VGG16 Accuracy**: 87%
- **ResNet50 Accuracy**: 85%


## Web App Flow
The web app was developed using Flask and deployed on a cloud server. It allows users to upload waste images for classification, displaying results in real time.

Here’s a flowchart of the web app's architecture:

![Web App Flow](https://github.com/user-attachments/assets/bfe07187-ff95-4b32-9f73-50c95e3d2660)

## Android App
The Android app was developed using Flutter, integrating the TensorFlow Lite model for on-device waste classification. It provides an intuitive interface where users can capture or upload images, and receive classification results.

![App Flow](https://github.com/user-attachments/assets/0f740295-41e6-4d75-b3f5-d2a48ac8c09c)

![image](https://github.com/user-attachments/assets/554dabae-74ab-4673-934e-b4f97556137a)



# Usage
Web App: Upload an image to classify it as organic or recyclable.
Android App: Capture or select an image to classify, providing real-time feedback.

# Future Enhancements
IoT Integration: Implementing the model in smart bins using IoT devices to automatically classify and sort waste.
Improved Model: Further optimizing the model by experimenting with deeper layers and additional attention mechanisms.
Extended Dataset: Expanding the dataset to include more waste categories and improving the classification of mixed waste.



Research Paper
For a more detailed explanation of our methodology and results, please refer to our research paper:

[Attention Module-Based Waste Management: A Machine Learning Approach to Sorting Organic and Recyclable Materials](https://ieeexplore.ieee.org/document/10393702)
