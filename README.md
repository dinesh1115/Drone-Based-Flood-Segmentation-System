# Autonomous AI Drone Flood Rescue System

## Dashboard Interface

<p align="center">
  <img src="DashBoard.png" width="900" alt="Drone Control Dashboard" />
</p>

*Real-time drone control dashboard with live stream, telemetry, and autonomous tracking modes.*

---

A professional-grade flood rescue solution that blends robotics, computer vision, and embedded IoT control into one award-winning platform.

This project delivers an end-to-end drone system that detects flood victims, segments flood zones, and maintains stable flight while offering remote command and telemetry over WiFi.

---

## Executive Summary

This system is designed for rapid disaster response using:

- A quadcopter platform with ESC and LiPo power integration
- NodeMCU / ESP8266 WiFi control for flight commands
- MPU IMU-based stabilization for reliable flight
- YOLO-based object detection for identifying people and targets
- U-Net-based semantic segmentation for flood area mapping
- Flask web interface for remote image upload, processing, and telemetry

It achieves a strong balance of autonomy, accuracy, and real-world readiness for flood rescue applications.

---

## Project Highlights

- **Award-winning innovation:** 1st Prize for IoT-based flood rescue solution
- **Autonomous tracking:** maintains ~5m distance from detected subjects
- **Real-time vision:** combines detection and segmentation in one pipeline
- **Robust telemetry:** supports live control data via WiFi
- **Modular design:** separates drone control, IMU processing, and vision pipeline

---

## Drone System Overview

<p align="center">
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/Drone(Hardware).jpg" width="250" />
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/Drone_working.jpg" width="250" />
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/drone-virtual-remote-camera.jpg" width="250" />
</p>

---

## Vision Performance

### Input vs Prediction

<p align="center">
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/Predicted%20Mask%20Color.png" width="300" />
</p>

### Segmentation Output

<p align="center">
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/Predicted%20Mask%20BW.png" width="280" />
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/Predicted%20Mask%20Color.png" width="280" />
</p>

---

## What This Project Delivers

- **Flood zone segmentation** from aerial imagery
- **Target detection** for people and rescue subjects
- **Autonomous flight control** with distance-based tracking
- **IMU-assisted stability** for smoother maneuvers
- **Remote operation** over WiFi with telemetry feedback
- **Web-based interface** for easy deployment and testing

---

## Technology Stack

| Component | Description |
| --- | --- |
| Python | Core application and logic |
| Flask | Web server and UI |
| OpenCV | Image processing and computer vision |
| TensorFlow / Keras | Deep learning model training and inference |
| NumPy | Numerical computing |
| NodeMCU / ESP8266 | Drone control and WiFi connectivity |
| MPU IMU | Stabilization sensor data |
| ESC + LiPo | Quadcopter propulsion hardware |

---

## System Architecture

```text
Drone Camera → YOLO Detection → U-Net Segmentation → Target Tracking → WiFi Command → Telemetry
```

---

## Core Software Modules

- `drone_control.py` — WiFi-based command client for NodeMCU / ESP8266 with takeoff, landing, hover, velocity, attitude, and telemetry.
- `vision_pipeline.py` — Integrated YOLO detection and U-Net segmentation pipeline with tracking control logic.
- `imu_module.py` — IMU signal smoothing and flight stabilization helpers.
- `app.py` — Flask backend, image upload processing, and remote command / telemetry endpoints.
- `train_model.py` — U-Net training script for flood mask segmentation.

---

## Prerequisites

Before installation, ensure your environment includes:

- Python 3.10 or higher
- Git
- `pip` package manager
- A webcam / ESP32-CAM stream for live video
- NodeMCU / ESP8266 based flight controller for drone control

### Optional hardware

- MPU IMU sensor for stabilization
- ESC + LiPo battery powertrain
- GPS module for location tracking

---

## Project Setup

```bash
# Clone the repository
git clone https://github.com/dinesh1115/Drone-Based-Flood-Segmentation-System.git
cd Drone-Based-Flood-Segmentation-System

# Create and activate a Python virtual environment
python -m venv venv
venv\Scripts\activate

# Install required Python packages
pip install -r requirements.txt
```

### Required model files

Copy or download the following files before running the app:

- `unet_model.h5` — trained segmentation model
- `models/yolov3.cfg` — YOLO configuration
- `models/yolov3.weights` — YOLO weights
- `models/coco.names` — YOLO class labels

If you do not have `unet_model.h5`, train the model using the `train_model.py` script.

---

## Running the Application

### Start the Flask dashboard

```bash
python app.py
```

Open your browser at `http://127.0.0.1:5000` and log in to access the dashboard.

### Train the segmentation model

```bash
python train_model.py
```

Use this command when you want to retrain the flood mask model on your own dataset.

---

## Advanced Installation

### GPU acceleration

For faster model inference on compatible hardware, install a GPU-enabled TensorFlow package or environment specific to your platform.

### Model preparation

If you are deploying this project on a new machine:

1. Place `unet_model.h5` in the project root.
2. Place YOLO files under `models/`.
3. Configure `DRONE_HOST` and `DRONE_PORT` environment variables if your flight controller uses a different IP address.

---

## Usage Notes

- Use the dashboard to monitor live video, run segmentation, and issue drone commands.
- The `drone_control.py` module sends WiFi commands to the NodeMCU / ESP8266 controller.
- The `vision_pipeline.py` module performs detection and segmentation for autonomous tracking.
- The `imu_module.py` module smooths IMU data and supports flight stabilization.

---

## Achievement Summary

- Built a full-stack flood rescue drone with embedded control
- Implemented computer vision using YOLO and U-Net
- Designed active tracking to keep the drone at a safe following distance
- Added IMU-based stabilization for smoother flight behavior
- Built a WiFi telemetry and control framework for remote piloting
- Recognized with 1st Prize for IoT-based flood rescue innovation

---

## Future Roadmap

- Live video segmentation and target tracking
- Autonomous rescue path planning
- Adaptive control using sensor fusion
- Cloud-based monitoring and alerting
- Mobile-ready control dashboard

---

## Author

**Dinesh Yadav**
