# Xerox-Quadcopter-Image-Processing-and-Algorithm

A practical computer vision and control project for detecting rectangular windows (or similar targets) in a live video stream and autonomously aligning a **DJI Tello** drone using PID controllers and a Kalman filter.

---

## Overview

This project captures frames from the Tello camera, detects window-like rectangular shapes using HSV color segmentation and contour analysis, tracks the target robustly with smoothing and a Kalman filter, and commands the drone to align and approach the target automatically.

**Core capabilities:**

- Real-time window detection
- Stable target tracking
- Autonomous yaw / roll / throttle / forward control
- Search behavior when target is lost
- Visual debugging overlays
- Live parameter tuning via trackbars

---

## Features

- Multi-range HSV masking (3 adjustable color ranges)
- Morphological filtering for noise reduction
- Polygon approximation for rectangle detection
- Kalman filter for smoothing & prediction
- PID controllers for all movement axes
- Intelligent search pattern when detection fails
- Real-time GUI controls for tuning parameters
- Safety hover when alignment is achieved


