# Autonomous AI Drone Flood Rescue System

A complete IoT-enabled flood rescue project that combines drone hardware, computer vision, and autonomous flight control.

This system is built around a quadcopter platform controlled by NodeMCU / ESP8266, with an IMU for stabilization and a vision pipeline using YOLO for detection and U-Net for flood segmentation.

## Project Goal

- Build an autonomous drone for real-time flood monitoring and rescue assistance
- Maintain safe tracking distance (~5m) from detected subjects or targets
- Stabilize flight using MPU-based IMU feedback
- Enable WiFi-based remote control and telemetry data flow
- Demonstrate rapid rescue assessment capability in flood scenarios

## Project Demo

### Drone System Overview

<p align="center">
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/Drone(Hardware).jpg" width="250" />
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/Drone_working.jpg" width="250" />
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/drone-virtual-remote-camera.jpg" width="250" />
</p>

## Model Results

### Input vs Prediction

<p align="center">
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/Predicted%20Mask%20Color.png" width="300" />
</p>

### Segmentation Outputs

<p align="center">
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/Predicted%20Mask%20BW.png" width="280" />
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/Predicted%20Mask%20Color.png" width="280" />
</p>

---

## Key Capabilities

- Autonomous flood region segmentation from drone imagery
- Real-time person/target detection using YOLO
- Tracking control logic to maintain a target distance of about 5 meters
- IMU-based stabilization support for smoother flight
- WiFi command and telemetry interface for remote operation
- Web-based upload and visualization via Flask UI

## Hardware and Software Stack

- Python
- Flask
- OpenCV
- TensorFlow / Keras
- NumPy
- NodeMCU / ESP8266
- MPU IMU sensor
- ESC and LiPo-powered quadcopter

---

## System Architecture

```text
Drone Camera → YOLO Detection → U-Net Segmentation → Tracking Control → WiFi Command → Telemetry
```

---

## Core Modules

- `drone_control.py` — WiFi command client for NodeMCU / ESP8266 controlling takeoff, landing, hovering, velocity, attitude, and telemetry.
- `vision_pipeline.py` — YOLO-based detection, U-Net segmentation, and autonomous target tracking logic.
- `imu_module.py` — IMU signal smoothing and attitude adjustment helper for flight stabilization.
- `app.py` — Flask frontend and backend, image upload flow, processing, and remote command endpoints.
- `train_model.py` — U-Net training script for flood mask segmentation.

---

## Installation

```bash
git clone https://github.com/dinesh1115/Drone-Based-Flood-Segmentation-System.git
cd Drone-Based-Flood-Segmentation-System
pip install -r requirements.txt
```

---

## Usage

Start the web app:

```bash
python app.py
```

Train the segmentation model:

```bash
python train_model.py
```

Use the web interface to upload drone images and visualize flood mask output. The Flask app also exposes command and telemetry APIs for drone control.

---

## Achievements

- Developed a quadcopter with ESC and LiPo integration
- Created a vision pipeline combining YOLO detection and U-Net segmentation
- Implemented subject tracking logic with 5m distance control
- Integrated IMU data for flight stability
- Built WiFi-based control and telemetry system
- Awarded 1st Prize for IoT-based flood rescue innovation

---

## Future Improvements

- Real-time video stream segmentation and tracking
- Complete autonomous flight planning for rescue paths
- AI-based alert and rescue recommendation system
- Cloud deployment for remote monitoring and analytics

---

## Author

Dinesh Yadav
