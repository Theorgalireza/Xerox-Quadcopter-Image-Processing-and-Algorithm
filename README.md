# Xerox-Quadcopter-Image-Processing-and-Algorithm

A practical computer vision and control project for detecting rectangular windows (or similar targets) in a live video stream and autonomously aligning a **DJI Tello** drone using PID controllers and a Kalman filter.

---

## Overview

This project captures frames from the Tello camera, detects window-like rectangular shapes using HSV color segmentation and contour analysis, tracks the target robustly with smoothing and a Kalman filter, and commands the drone to align and approach the target automatically.

The system integrates:
- **Computer Vision (OpenCV)**
- **Multi-stage HSV color segmentation**
- **Kalman filtering for robust tracking**
- **Multiple PID controllers** for stable flight control
- **Autonomous search behavior** when the target is lost

This project is designed for real-time operation using the onboard Tello camera and is fully tunable via GUI sliders.

---

##  Key Capabilities
- Real-time **window detection** using contour geometry and color filtering
- **4-DOF drone control**:
  - **Yaw** (horizontal alignment)
  - **Throttle** (vertical alignment)
  - **Roll** (window plane leveling)
  - **Pitch (forward/backward)** (distance control using contour area)
- **Kalman Filter–based tracking** for noise reduction and prediction
- **Autonomous search mode** when the target is not visible
- Live **HSV tuning interface**
- Safe termination and emergency land

---


