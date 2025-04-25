# Sebastian Rivera

Welcome to my personal portfolio! I'm a passionate Mechatronics Engineer with a strong background in AI, autonomy, electric motors, and robotics. Below you'll find a selection of my featured projects and background.

---

 🚀 Projects

# 🔍 Autonomous Vehicle Perception System
- **Description**:  This Master’s-level engineering project focused on solving real-world challenges in collaboration with community partners in the Greater Toronto Area (GTA). We developed a road and sidewalk segmentation system using YOLOP on NVIDIA Jetson Orin to enhance autonomous navigation and pedestrian safety. The project spanned two academic terms and involved structured planning, technical implementation, and public impact considerations. Project coordination, planning milestones, and stakeholder engagement were managed using Microsoft Teams, while final deliverables and presentations were developed using Microsoft PowerPoint
Below are links to the final technical report and project poster.
- **Key Features**:
  - Real-time segmentation of road environments
  - Edge deployment on Jetson with GNSS and ROS integration
- **Tech Stack**: Python, YOLOP, ROS, NVIDIA Jetson Orin, GNSS, Microsoft Teams, PowerPoint
- **Links**:
  - [GitHub Repository](#)
  - [Live Demo / Video](#)

---

# 🤖 Skip-the-Servers: Autonomous Food Delivery Robot

A capstone project built to tackle the challenges of modern restaurant staffing with robotics and intelligent automation.

---

## 🚀 Overview

**Skip-the-Servers** is a semi-autonomous food delivery robot developed during my Bachelor of Technology in Automotive and Vehicle Engineering Technology at McMaster University. Designed to address hygiene and staffing challenges in restaurants, the robot navigates autonomously, avoids obstacles, and presents food via a hygienic revolving tray mechanism. 

This project was completed during the COVID-19 pandemic with extremely limited resources—no access to manufacturing equipment—requiring creative use of everyday materials, hand tools, and low-cost electronics. It was a true test of engineering under constraint, pushing me to innovate across mechanical design, embedded programming, and control systems.

## 🔧 Key Features

- 🦾 **Obstacle Avoidance** using ultrasonic sensors for real-time pathfinding
- ⚙️ **PID Motor Control** for smooth and precise velocity adjustments
- 🍽️ **Revolving Tray Mechanism** keeps meals covered and ready for delivery
- 🔋 **Battery Optimized** for ~1h45m continuous operation with low power draw
- 🛠️ Built using **IKEA VESKEN** frame, 3D-printed custom shafts, and low-cost materials

## 🛠️ Engineering Breakdown

### 🧠 Control & Navigation
- Implemented encoder-based feedback loops using rotary magnetic encoders (64 CPR)
- Tuned PID controller (`Kp = 0.75`, `Kd = 0.045`) for zero steady-state error
- Wrote modular Arduino code for sensor handling, motor PWM control, and path logic

### ⚙️ Powertrain & Chassis
- Motors: Dual 12V Pololu 100:1 Metal Gearmotors (34 kg-cm torque)
- Velocity target: **0.16 m/s** at optimal efficiency (~39%)
- Custom 3D-printed shaft designs (2 revisions) to prevent shear failure

### 📡 Sensor System
- 6 ultrasonic sensors (front, back, sides, and corners) for full-coverage obstacle detection
- Uses `pulseIn()` with speed-of-sound calculations for distance measurement

## 📊 Testing & Calibration

- ✅ Calibrated PWM vs RPM for both motors under load
- 🧪 Encoder-based velocity monitoring and real-time plotting
- 📉 Addressed gear ratio mismatches and voltage spikes
- 📐 Precision chassis and tray mount design via Fusion 360 and SolidWorks

## 💡 Skills Applied

- Mechatronics & motor control (DC motors, PID, power management)
- Embedded systems programming (Arduino IDE, real-time interrupts)
- Mechanical prototyping (hand tools, CAD, 3D printing, DIY home design)
- Sensor fusion for autonomous navigation

## 🔮 Future Enhancements

- Add **AI-based mapping** and camera-based navigation
- Introduce **AWD design** for tighter turning radius
- Upgrade to **ROS or SLAM-based architecture**
- Integrate **low-pass filters** for cleaner encoder signals

📍 **Project Year**: 2021  
🎓 **Institution**: McMaster University  
🔗 **Advisor**: Dr. Timber Yuen

---

> _"This project challenged me to combine hardware, code, and control theory into a working solution—laying the foundation for my continued work in robotics and intelligent systems."_

---

### 🧠 AI-Based Anomaly Detection in MQTT Data Streams
- **Description**: Created a deep learning model to detect anomalies in IoT sensor data for cybersecurity using LSTM networks.
- **Key Features**:
  - Identified duplication, interception, and modification anomalies
  - Applied time-series deep learning techniques
- **Tech Stack**: Python, PyTorch, LSTM, MQTT
- **Links**:
  - [GitHub Repository](#)

---

### 📄 Human Pose Estimation Using Deep Learning (PoseNet Project)

This project explored human pose estimation using four leading deep learning models: **PoseNet**, **HRNet**, **MediaPipe**, and **OpenPose**. The goal was to detect and visualize human body keypoints using convolutional neural networks (CNNs) and benchmark model performance across real-world scenarios.

We used the **COCO val2017 dataset**, which includes 5,000+ images annotated with 17 keypoints per person. Our team evaluated each model using industry-standard metrics such as **Mean Average Precision (mAP)** and **Percentage of Correct Keypoints (PCK)**.

---

### 🔧 Implementation Highlights
As part of the implementation, we:
- Preprocessed over 5,000 COCO images for input standardization
- Compared model accuracy and inference performance across CPU and GPU environments
- Visualized predicted poses using OpenCV keypoint skeletons
- Integrated **PoseNet** via TensorFlow.js for lightweight, browser-based inference
- Benchmarked single-person and multi-person detection scenarios

---

### 🔍 Key Observations
- **PoseNet**: Fast and browser-deployable with lower accuracy (~63.9% PCK)
- **OpenPose**: Strong performance in multi-person detection (~72% PCK)
- **MediaPipe**: Balanced speed and accuracy for single-person use
- **HRNet**: Highest precision (~74.4% mAP) but most computationally intensive

---

### 📊 Project Summary
- **Models Used**: PoseNet, HRNet, OpenPose, MediaPipe  
- **Dataset**: Microsoft COCO val2017  
- **Key Contributions**:
  - Trained and evaluated 4 advanced pose estimation models
  - Deployed PoseNet using TensorFlow.js and PyTorch
  - Rendered visual outputs with pose keypoints and skeletal structures

- **Tech Stack**: Python, PyTorch, TensorFlow, OpenCV, COCO API, MediaPipe, TensorFlow.js

---

### 📁 Project Files
- 📄 [Final Project Report (PDF)](./docs/pdf/SEP740_Project_Report.pdf)
- 🖼️ [Project Poster (PDF/Image)](./docs/pdf/PoseNet_Poster.pdf)

---

🖼️ **Add Pictures Here**  
*(Images to be included below each project or in a separate 'gallery' section if preferred.)*

---

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

## 📄 View My Resume (PDF)

To include a PDF in your GitHub repository and link to it here:

1. Upload your `resume.pdf` file into your GitHub repo (e.g., root folder).
2. Then link to it like this:

```markdown
[📄 View My Resume](./resume.pdf)
