---
layout: default
title: Autonomous Vehicle Perception System
permalink: /projects/gowrench-autonomy/
---

# 🔍 Autonomous Vehicle Perception System (GoWrench Project)

A Master’s-level engineering project focused on solving real-world mobility challenges using an autonomous off-road robot. Developed in collaboration with GoWrench Inc., this initiative integrates GNSS, ROS, and YOLO-based vision systems to support Level 4 autonomous navigation.

---

## Overview

In collaboration with GoWrench Inc., we developed a **Level 4 autonomous off-road navigation system** using ROS, GNSS localization, and real-time camera-based segmentation. The system enables robots to follow preplanned routes while navigating around obstacles with high precision using Jetson Orin and Oak-D cameras.

The project used the Husky UGV as a research platform and simulated GNSS and IMU data to validate algorithms before real-world deployment. Visual perception was enhanced using YOLOv8 and YOLOP models, which provided both semantic segmentation and depth estimation via stereo vision.

📄 **[Download Final Report (PDF)](<a href="/sebastianriveraportfolio/docs/pdf/SEP_799_Final_Report_GoWrench.pdf" target="_blank"><strong>Download Final Report (PDF)</strong></a>)**  
🖼️ **[Download Project Poster (PDF)](<a href="/sebastianriveraportfolio/docs/pdf/SEP_799_Final_Digital_Project_Poster.pdf" target="_blank"><strong>Download Project Poster (PDF)</strong></a>)**

---

## Key Features

- 📍 GNSS-based localization fused with IMU using an Extended Kalman Filter (EKF)  
- 🧠 YOLOv8 with depth perception for real-time road and pedestrian detection  
- 🗺️ Google Maps API integration for real-world route planning  
- 💻 Dockerized deployment on NVIDIA Jetson Orin with ROS and DepthAI  
- 📡 Waypoint self-navigation tested in RViz and simulated environments  

---

# 🛠️ Engineering Breakdown

### 🧭 Navigation Stack
- Integrated ROS `move_base`, `navfn`, and `dwa_local_planner`  
- Simulated GNSS and IMU data using custom ROS nodes  
- Used static transforms and costmaps to test paths indoors  
- Tested route generation using real-world waypoints from Google Maps API

### 🧠 Visual Perception
- Oak-D cameras running YOLOv8 in Docker with DepthAI integration  
- Real-time XYZ depth estimation and road segmentation using YOLOP  
- Simulated driving scenarios using X, Y, Z bounding box calibration  
- Accuracy tested under varying distance thresholds (2–6% depth error)

---

## 📊 Testing & Validation

- Validated simulated paths in RViz and Google Earth  
- Achieved successful fusion of GNSS + IMU with reliable localization output  
- ROS architecture validated using bag files and static transforms  
- Achieved consistent XYZ output from stereo depth vision under test conditions

---

## 💡 Skills Applied

- Autonomous navigation in ROS (NavStack, costmaps, launch files)  
- Real-time segmentation and object detection (YOLOv8, YOLOP)  
- Depth sensing with Oak-D stereo cameras  
- Dockerized AI deployment on Jetson Orin  
- GNSS + IMU data fusion and localization (EKF)

---

## 🔮 Future Enhancements

- Merge YOLOP + YOLOv8 + depth data into a unified inference pipeline  
- Integrate live sensor feedback for real-time obstacle avoidance  
- Expand GNSS + move_base integration for fully dynamic self-navigation  
- Real-world deployment and fine-tuning of Z-axis predictions while in motion

---

### 📍 Project Year: 2024  
### 👥 Team: Haocun (Matt) Jing & Sebastian Rivera  
### 🧑‍🏫 Faculty Lead: Dr. Moein Mehrtash  
### 🤝 Partner: GoWrench Inc.  

---

> _"From simulated transforms to real-world path planning, this project demonstrated how ROS-based systems can drive robust, self-navigating autonomous platforms in partnership with industry."_


