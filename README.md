## 🧪 Results

## Results

### Input Images

<p align="center">
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/1753426585639.jpg" width="250"/>
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/YOUR_IMAGE_2.jpg" width="250"/>
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/YOUR_IMAGE_3.jpg" width="250"/>
</p>

---

### Segmentation Outputs

<p align="center">
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/output1.jpg" width="300"/>
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/output2.jpg" width="300"/>
  <img src="https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/output3.jpg" width="300"/>
</p>

### Segmentation Outputs

![Binary Mask](https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/Predicted%20Mask%20BW.png)

![Colored Mask](https://raw.githubusercontent.com/dinesh1115/Drone-Based-Flood-Segmentation-System/main/Predicted%20Mask%20Color.png)
Drone-Based Flood Detection and Segmentation

An IoT-based project where a drone was designed and built to capture aerial images, combined with a deep learning model to detect and segment flood-affected areas.

Abstract

This project presents an IoT-based drone system integrated with a deep learning model for detecting and segmenting flood-affected regions from aerial imagery. A drone is used to capture images, which are then processed using a U-Net convolutional neural network. The system performs pixel-level classification to distinguish flooded and non-flooded areas. A web interface is also developed to allow users to upload images and view results.

Introduction

Flood monitoring is an important part of disaster management. Traditional methods are often slow and require manual effort. This project aims to automate the process by combining drone-based data collection with deep learning techniques.

The system uses aerial images captured by a drone and applies segmentation to identify flood-affected regions. It provides a practical approach for real-world monitoring and analysis.

Objectives
Design and build a drone for aerial image capture
Develop a deep learning model for flood detection
Integrate the model with a web application
Provide clear visualization of results
Methodology

The drone captures aerial images of the environment. These images are preprocessed and passed to a trained U-Net model. The model analyzes each image and generates a segmentation mask highlighting flooded areas. The results are displayed through a web interface.

Model Details

The system uses a U-Net architecture for image segmentation. The model takes images as input and produces a binary mask as output, identifying flooded regions. It is trained using standard optimization and loss functions suitable for segmentation tasks.

Results
Input Images

Segmentation Outputs

Experimental Observations

The drone was tested in real-world conditions. During testing, some instability and failure cases, including crashes, were observed. These helped in understanding practical challenges and improving the system.

Applications
Flood monitoring
Disaster response
Environmental analysis
Remote sensing
Limitations
Depends on image quality and weather conditions
Limited real-time capability
Hardware constraints of the drone
Future Work
Real-time video processing
Cloud deployment
Improved model accuracy
Integration with mapping systems
Author

Dinesh Yadav

Conclusion

This project demonstrates how drone technology and deep learning can be combined to detect flood-affected areas automatically. It provides a practical solution for disaster monitoring and analysis.
