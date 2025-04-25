---
layout: default
title: SKIPTHESERVERS Capstone 
permalink: /projects/capstone/
---

# 🤖 Skip-the-Servers: Autonomous Food Delivery Robot

A capstone project built to tackle the challenges of modern restaurant staffing with robotics and intelligent automation.

---

## Overview

**Skip-the-Servers** is a semi-autonomous food delivery robot developed during my Bachelor of Technology in Automotive and Vehicle Engineering Technology at McMaster University. Designed to address hygiene and staffing challenges in restaurants, the robot navigates autonomously, avoids obstacles, and presents food via a hygienic revolving tray mechanism.

This project was completed during the COVID-19 pandemic with extremely limited resources—no access to manufacturing equipment—requiring creative use of everyday materials, hand tools, and low-cost electronics. It was a true test of engineering under constraint, pushing me to innovate across mechanical design, embedded programming, and control systems.

📄 **[Download the Full Report (PDF)](/sebastianriveraportfolio/docs/pdf/4TR3_Capstone_SKIPTHESERVERS_Final_Report_Sebastian_Rivera.pdf)**


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


