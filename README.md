# Visual-Quality-Control-System
## Dataset
Dataset link: https://drive.google.com/drive/folders/1KA5_0-u9NVzR5i_zlL2UOhSkkcrt2-5n?usp=sharing

# VisionSpec QC – AI-Based PCB Defect Detection System

## 📌 Project Overview

**VisionSpec QC** is a Computer Vision-based Visual Quality Control system designed to automatically detect defects in Printed Circuit Boards (PCBs).

The system uses Deep Learning (CNN + Transfer Learning) to classify PCB images into:

* ✅ Pass (No Defect)
* ❌ Defect

Additionally, the system integrates **explainable AI (Grad-CAM)** to visually highlight defect regions, making the model trustworthy for industrial use.

## 🎯 Problem Statement

Manual PCB inspection in manufacturing environments:

* Is time-consuming
* Is prone to human error
* Does not scale efficiently

VisionSpec QC provides:

* Automated inspection
* High accuracy classification
* Real-time inference capability
* Visual explanation of detected defects

## 🛠 Tech Stack

* Python
* TensorFlow / Keras
* OpenCV
* NumPy
* Matplotlib
* TensorFlow Lite (for optimized deployment)

## 🧠 Model Architecture

### 1️⃣ Baseline CNN

* Convolution layers
* ReLU activation
* MaxPooling
* Dense layers
* Sigmoid output (Binary Classification)

### 2️⃣ Transfer Learning

Pre-trained backbone used:

* MobileNetV2 / ResNet50

Custom classification head:

* Global Average Pooling
* Dense Layer
* Dropout
* Sigmoid Output

## 🔍 Defect Types Detected

The model is trained to detect common PCB defects such as:

* Solder bridges
* Missing joints
* Burn marks
* Surface abnormalities

## 🚀 Features

✔ Image preprocessing & normalization
✔ Data augmentation (rotation, zoom, brightness adjustment)
✔ Transfer learning for improved accuracy
✔ Grad-CAM for model explainability
✔ TensorFlow Lite conversion for faster CPU inference
✔ Real-time camera simulation

## 🔥 Grad-CAM Explainability

Grad-CAM (Gradient-weighted Class Activation Mapping) is used to:

* Highlight defect regions
* Ensure model is focusing on relevant areas
* Validate correct predictions
* Analyze misclassifications

This ensures the system is not learning spurious background patterns.

## ⚡ Inference Optimization

The trained model is converted to **TensorFlow Lite**:

* Reduced model size
* Faster inference
* Suitable for CPU deployment
* Near real-time performance


## 📈 End-to-End Workflow

1. Image acquisition
2. Preprocessing
3. Model prediction
4. Grad-CAM generation
5. Result display
6. Optimized deployment


## 🏭 Industrial Relevance

This system can be deployed in:

* PCB manufacturing plants
* Electronics assembly lines
* Automated quality inspection systems

It reduces:

* Manual inspection cost
* Human error
* Production delays


## 📚 Future Improvements

* Multi-class defect detection
* Edge device deployment (Raspberry Pi)
* Web-based monitoring dashboard
* Continuous learning with new defect data

