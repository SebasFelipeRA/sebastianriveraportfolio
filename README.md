# Sebastian Rivera

Welcome to my personal portfolio! I'm a passionate Mechatronics Engineer with a strong background in AI, autonomy, electric motors, and robotics. Below you'll find a selection of my featured projects and background.

---

 🚀 Projects

# 🔍 Autonomous Vehicle Perception System (GoWrench Project)

A Master’s-level engineering project focused on solving real-world mobility challenges using an autonomous off-road robot. Developed in collaboration with GoWrench Inc., this initiative integrates GNSS, ROS, and YOLO-based vision systems to support Level 4 autonomous navigation.

---

## Overview

In collaboration with GoWrench Inc., we developed a **Level 4 autonomous off-road navigation system** using ROS, GNSS localization, and real-time camera-based segmentation. The system enables robots to follow preplanned routes while navigating around obstacles with high precision using Jetson Orin and Oak-D cameras.

The project used the Husky UGV as a research platform and simulated GNSS and IMU data to validate algorithms before real-world deployment. Visual perception was enhanced using YOLOv8 and YOLOP models, which provided both semantic segmentation and depth estimation via stereo vision.

📄 **[Download Final Report (PDF)](./docs/pdf/SEP_799_Final_Report_GoWrench.pdf)**  
🖼️ **[Download Project Poster (PDF)](./docs/pdf/SEP_799_Final_Digital_Project_Poster.pdf)**

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


# 🤖 Skip-the-Servers: Autonomous Food Delivery Robot

A capstone project built to tackle the challenges of modern restaurant staffing with robotics and intelligent automation.

---

## Overview

**Skip-the-Servers** is a semi-autonomous food delivery robot developed during my Bachelor of Technology in Automotive and Vehicle Engineering Technology at McMaster University. Designed to address hygiene and staffing challenges in restaurants, the robot navigates autonomously, avoids obstacles, and presents food via a hygienic revolving tray mechanism.

This project was completed during the COVID-19 pandemic with extremely limited resources—no access to manufacturing equipment—requiring creative use of everyday materials, hand tools, and low-cost electronics. It was a true test of engineering under constraint, pushing me to innovate across mechanical design, embedded programming, and control systems.

📄 **[Download the Full Report (PDF)](./docs/pdf/4TR3_Capstone_SKIPTHESERVERS_Final_Report_Sebastian_Rivera.pdf)**


---

## Key Features

- 🦾 **Obstacle Avoidance** using ultrasonic sensors for real-time pathfinding  
- ⚙️ **PID Motor Control** for smooth and precise velocity adjustments  
- 🍽️ **Revolving Tray Mechanism** keeps meals covered and ready for delivery  
- 🔋 **Battery Optimized** for ~1h45m continuous operation  
- 🛠️ Constructed using IKEA VESKEN frame, 3D-printed shafts, and low-cost materials  

---

# 🛠️ Engineering Breakdown

### 🧠 Control & Navigation
- Encoder-based feedback using rotary magnetic encoders (64 CPR)  
- PID tuning (`Kp = 0.75`, `Kd = 0.045`) for zero steady-state error  
- Modular Arduino codebase for motor control and sensor logic  

### ⚙️ Powertrain & Chassis
- Dual 12V Pololu 100:1 Metal Gearmotors (34 kg-cm torque)  
- Target velocity: **0.16 m/s** at ~39% efficiency  
- Custom 3D-printed shafts (2 iterations) to reduce failure risk  
- CAD chassis planning via Fusion 360 and SolidWorks  

### 📡 Sensor System
- Six ultrasonic sensors (front, rear, corners)  
- Real-time collision detection using Arduino `pulseIn()`  
- Adaptive movement logic based on distance thresholds  

---

## 📊 Testing & Calibration

- Calibrated PWM-to-RPM performance for motor synchronization  
- Real-time speed monitoring using encoders and Arduino Serial Plotter  
- Analyzed gear ratio variation and adjusted motor voltage accordingly  

---

## 💡 Skills Applied

- Mechatronics and embedded control (DC motors, encoders, PID control)  
- Arduino programming and PWM regulation  
- Mechanical design and prototyping (CAD, 3D printing, woodworking)  
- Sensor integration and feedback-based navigation  

---

## 🔮 Future Enhancements

- Implement camera-based SLAM and AI-based mapping  
- Upgrade to all-wheel-drive for better maneuverability  
- Add low-pass filters for clean velocity data  
- Explore ROS integration for higher-level autonomy  

---

### 📍 Project Year: 2021  
### 🎓 Institution: McMaster University  
### 🔗 Advisor: Dr. Timber Yuen

---

> _"This project challenged me to combine hardware, code, and control theory into a working solution—laying the foundation for my continued work in robotics and intelligent systems."_


# 🧍‍♂️ Human Pose Estimation Using Deep Learning (PoseNet Project)

A research-driven project focused on evaluating leading pose estimation models for real-time human keypoint detection using deep learning and computer vision.

---

## Overview

This project explored **human pose estimation** using four state-of-the-art models: **PoseNet**, **HRNet**, **MediaPipe**, and **OpenPose**. The primary goal was to detect and visualize human body keypoints in real-world scenarios using convolutional neural networks (CNNs).

We utilized the **Microsoft COCO val2017 dataset** with over 5,000 images annotated with 17 human keypoints. Each model was benchmarked using industry-standard metrics such as **Percentage of Correct Keypoints (PCK)** and **Mean Average Precision (mAP)**.

📄 **[Download the Full Report (PDF)](./docs/pdf/SEP740_Project_Report.pdf)**

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

# 📡 AI-Based Anomaly Detection in MQTT Data Streams

A deep learning project developed to detect cybersecurity anomalies in IoT-based sensor data using time-series modeling and ensemble methods.

---

## Overview

This project tackled the detection of **duplication**, **interception**, and **modification** attacks in MQTT data streams — common vulnerabilities in connected industrial systems. Using the DAD (Dataset for Anomaly Detection), we implemented and evaluated multiple anomaly detection models, with a primary focus on **LSTM networks** due to their strength in modeling temporal dependencies.

An ensemble strategy combining **LSTM**, **Random Forest**, and **Isolation Forest** was used to boost classification performance via **majority voting**.

📄 **[Download Full Report (PDF)](./docs/pdf/SEP_769_Final_Project_Anomoly_Detection_Final_Report.pdf)**

---

## Key Features

- 🧠 LSTM RNN for time-series anomaly prediction  
- 🏗️ Majority voting ensemble of LSTM, Random Forest, and Isolation Forest  
- 📦 Preprocessing includes one-hot encoding, normalization, and SMOTE oversampling  
- 📊 ROC-AUC scores ~0.99 on unseen test data  
- 🛡️ Detected cybersecurity anomalies across 7-day MQTT traffic samples  

---

# 🛠️ Engineering Breakdown

### 🔍 Models & Dataset
- **Dataset**: [DAD - Dataset for Anomaly Detection](https://github.com/dad-repository/dad)  
- **Features used**: `ip.src`, `tcp.srcport`, `mqtt.clientid`, `mqtt.msgid`, and `label`  
- **Models implemented**:
  - LSTM with dropout layers
  - Random Forest (GridSearchCV tuned)
  - Isolation Forest
  - Feedforward Neural Network (FNN)
  - XGBoost

### 🧪 Training Strategy
- Data split: 60% Train / 20% Validation / 20% Test  
- Used **SMOTE** to balance classes  
- Trained for **100 epochs** with **early stopping**  
- Predictions consolidated via **majority voting**

### 📈 Performance Metrics
- **LSTM ROC-AUC**: 0.986 (test)  
- **FNN ROC-AUC**: 0.995 (test)  
- **Ensemble ROC-AUC**: 0.999 (train), 0.995 (validation)  
- Excellent **precision**, **recall**, and **F1-score** observed

---

## 💡 Skills Applied

- Deep Learning: LSTM, FNN, XGBoost  
- Ensemble Learning & Majority Voting  
- Cybersecurity anomaly detection  
- Feature encoding & time-series normalization  
- Python, Keras, scikit-learn, pandas, matplotlib

---

## 🔮 Future Enhancements

- Integrate model into a **real-time system**
- Test in cross-domain settings like healthcare or automotive  
- Improve adversarial robustness  
- Explore hybrid models (e.g., autoencoders + attention mechanisms)

---

### 📍 Project Year: 2024  
### 🧪 Dataset: DAD (Dataset for Anomaly Detection)  

---

> _"This project taught me how to design resilient deep learning systems capable of detecting subtle yet critical anomalies in real-world, time-sensitive environments."_


## 🎓 Education

- **Master of Engineering in Systems and Technology**, McMaster University (2025)  
- **Bachelor of Technology - Automotive Engineering**, McMaster University (2021)  
- **Ontario Secondary School Diploma**, Cathedral High School – *Awarded School Letter Award (2016)*

---

## 📫 Contact

Feel free to reach out via:

- **LinkedIn**: [linkedin.com/in/sebastianrivera](hwww.linkedin.com/in/sebasrivera)
- **Email**: [riveraas@mcmaster.ca](mailto:riveraas@mcmaster.ca)

---

Thanks for visiting!

---

