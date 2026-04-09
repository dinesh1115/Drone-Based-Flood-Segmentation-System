# Drone-Based Flood Segmentation System

AI-powered drone system for detecting and segmenting flood-affected areas using deep learning. Designed for disaster response, rescue planning, and environmental monitoring.

---

## Project Demo

### Drone System Overview

<p align="center">
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/Drone(Hardware).jpg" width="250"/>
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/Drone_working.jpg" width="250"/>
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/drone-virtual-remote-camera.jpg" width="250"/>
</p>

---

## Model Results

### Input vs Prediction

<p align="center">
  <b>Original Image</b> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <b>Segmented Output</b>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/Drone_working.jpg" width="300"/>
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/Predicted%20Mask%20Color.png" width="300"/>
</p>

---

### Segmentation Outputs

<p align="center">
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/Predicted%20Mask%20BW.png" width="280"/>
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/Predicted%20Mask%20Color.png" width="280"/>
</p>

---

## Features

- Real-time flood detection using drone imagery  
- Deep learning-based image segmentation  
- High accuracy water-body identification  
- Scalable for disaster management systems  

---

## Tech Stack

- Python  
- OpenCV  
- TensorFlow / PyTorch  
- NumPy  
- Flask (for deployment)  

---

## System Architecture

```
Drone Camera → Image Capture → Deep Learning Model → Segmentation Output → Visualization
```

---

## Installation

```bash
git clone https://github.com/dinesh1115/Drone-Based-Flood-Segmentation-System.git
cd Drone-Based-Flood-Segmentation-System
pip install -r requirements.txt
```

---

## Usage

Run the system:

```bash
python app.py
```

Train the model:

```bash
python train_model.py
```

---

## Applications

- Flood disaster management  
- Rescue and evacuation planning  
- Environmental monitoring  
- Smart surveillance systems  

---

## Future Improvements

- Real-time drone integration  
- Live video segmentation  
- AI-based alert system  
- Cloud deployment (AWS/GCP)  

---

## Author

Dinesh Yadav
