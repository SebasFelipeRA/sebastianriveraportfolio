---
layout: default
permalink: /projects/pose-estimation/
---

# 🧍‍♂️ Human Pose Estimation Using Deep Learning (PoseNet Project)

A research-driven project focused on evaluating leading pose estimation models for real-time human keypoint detection using deep learning and computer vision.

---

## Overview

This project explored **human pose estimation** using four state-of-the-art models: **PoseNet**, **HRNet**, **MediaPipe**, and **OpenPose**. The primary goal was to detect and visualize human body keypoints in real-world scenarios using convolutional neural networks (CNNs).

We utilized the **Microsoft COCO val2017 dataset** with over 5,000 images annotated with 17 human keypoints. Each model was benchmarked using industry-standard metrics such as **Percentage of Correct Keypoints (PCK)** and **Mean Average Precision (mAP)**.

📄 **[Download the Full Report (PDF)](/sebastianriveraportfolio/docs/pdf/SEP740_Project_Report.pdf)**

---

## Key Features

- 📊 Compared accuracy, latency, and deployment ease across 4 top pose models  
- 🧠 Implemented PoseNet in **TensorFlow.js** for browser-ready inference  
- 🧮 Preprocessed and standardized over 5,000 images from the COCO dataset  
- 🎯 Visualized keypoints and skeletal structures using **OpenCV** overlays  
- 🔁 Evaluated both **single-person** and **multi-person** pose detection  

---

# 🛠️ Engineering Breakdown

### 🧠 Model Architecture & Training
- Evaluated four models: PoseNet, HRNet, MediaPipe, OpenPose  
- Benchmarked each model using PCK and mAP scores  
- Focused on generalization and robustness across varying poses  

### ⚙️ Deployment & Optimization
- PoseNet deployed in-browser using TensorFlow.js for lightweight applications  
- Tested models on both CPU and GPU environments for performance insights  
- MediaPipe leveraged for fast mobile-friendly inference  

### 🧪 Evaluation Pipeline
- Custom Python scripts for batch preprocessing of COCO dataset  
- Visual validation using OpenCV keypoint plotting  
- Quantitative evaluation via mAP and PCK metrics on COCO annotations  

---

## 📊 Testing & Results

- **PoseNet**: Lightweight, browser-deployable; ~63.9% PCK  
- **OpenPose**: Best for multi-person; ~72% PCK  
- **MediaPipe**: Balanced speed and accuracy; single-person only  
- **HRNet**: Highest accuracy (~74.4% mAP); computationally intensive  

---

## 💡 Skills Applied

- Deep learning for computer vision (CNNs, heatmaps, PCK/mAP)  
- Model benchmarking and evaluation metrics  
- Frontend integration using TensorFlow.js  
- Dataset handling and preprocessing (COCO API)  
- Visualization with OpenCV  

---

## 🔮 Future Enhancements

- Integrate real-time webcam feed for live pose tracking  
- Extend to action recognition using keypoint time series  
- Optimize model selection for mobile and embedded platforms  
- Explore transfer learning for custom gesture datasets  

---

### 📍 Project Year: 2022  
### 🧪 Dataset: Microsoft COCO val2017  
### 👥 Team Contribution: Multi-model evaluation, visualization scripting, web deployment  

---

> _"Exploring the balance between performance, accuracy, and deployability taught me how to approach deep learning projects with real-world usability in mind."_

