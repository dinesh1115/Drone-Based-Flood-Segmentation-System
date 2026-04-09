# 🚁 Drone-Based Flood Detection and Segmentation using Deep Learning

🚀 A deep learning-based system that detects and segments flood-affected regions from drone imagery using a U-Net model and a Flask web interface.

---

## 📌 Overview

This project focuses on automated flood detection using aerial images captured by drones. It leverages a U-Net convolutional neural network to perform pixel-wise segmentation and identify flooded regions accurately.

A user-friendly web application is developed using Flask, allowing users to:

* Register and log in
* Upload drone images
* View segmentation results in real time

This solution is useful for disaster response teams and environmental monitoring systems.

---

## 🚀 Features

* 🔐 User Authentication (Login & Registration)
* 📤 Upload aerial images
* 🤖 Deep learning-based segmentation (U-Net)
* 🖼️ Display original and segmented images
* 💾 SQLite database for user management
* 🌐 Interactive Flask web interface

---

## 🛠️ Tech Stack

| Category         | Technology         |
| ---------------- | ------------------ |
| Language         | Python             |
| Backend          | Flask              |
| Deep Learning    | TensorFlow / Keras |
| Image Processing | OpenCV             |
| Database         | SQLite             |
| Frontend         | HTML, CSS          |

---

## 🧠 Model Architecture

* Model: U-Net
* Input Size: 256 × 256 × 3
* Output: Binary segmentation mask
* Activation: Sigmoid
* Loss Function: Binary Crossentropy
* Optimizer: Adam

---

## 📂 Project Structure

```
Drone-Based-Flood-Segmentation-System/
│── app.py  
│── train_model.py  
│── README.md  
│── requirements.txt  
│── .gitignore  
│── screenshots/  
│── static/  
│── templates/  
│── Dataset/  
```

---

## 📸 Screenshots

### 🔐 Login Page

![Login](screenshots/loginscrnsht.png)

### 📝 Register Page

![Register](screenshots/registerscrnsht.png)

### 🖥️ Drone Capture Screen

![Capture](screenshots/dronepic.jpeg)

### 🎮 Remote Screen

![Remote](screenshots/droneremotescrnsht.png)

### 🤖 Segmentation Result

![Result](screenshots/resultscrnsht.png)

---

## 🎥 Demo Videos

### 🎬 Drone Capture Demo

[▶️ Watch Capture Video](screenshots/dronecapturescreen.mp4)

### 🎬 Drone Working Demo

[▶️ Watch Drone Video](screenshots/dronevideo.mp4)

---

## ▶️ How to Run

### 1️⃣ Clone the repository

```
git clone https://github.com/sudhakar123P/Drone-Based-Flood-Segmentation-System.git
```

### 2️⃣ Navigate to project folder

```
cd Drone-Based-Flood-Segmentation-System
```

### 3️⃣ Install dependencies

```
pip install -r requirements.txt
```

### 4️⃣ Run the application

```
python app.py
```

### 5️⃣ Open in browser

```
http://127.0.0.1:5000/
```

---

## 📦 Requirements

* Python 3.x
* Flask
* TensorFlow
* OpenCV
* NumPy

---

## 🌍 Use Cases

* 🌊 Flood Monitoring Systems
* 🚨 Disaster Management
* 🌱 Environmental Analysis
* 🛰️ Remote Sensing Applications

---

## ⚠️ Challenges Faced

* Handling large image datasets
* Training segmentation model efficiently
* Managing file uploads and processing
* Integrating ML model with web application

---

## 🔮 Future Enhancements

* Deploy on cloud platforms (Azure / AWS)
* Real-time drone video processing
* Improve model accuracy
* Add GIS/map visualization

---

## 👨‍💻 Author

** DINESH YADAV **

---

## ⭐ Conclusion

This project demonstrates how deep learning and drone technology can be combined to solve real-world problems like flood detection. It highlights the integration of machine learning models with web applications for practical deployment.
