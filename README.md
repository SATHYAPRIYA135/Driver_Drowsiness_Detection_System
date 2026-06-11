# 🚗 Driver Drowsiness Detection System

## 📖 Project Overview

Driver fatigue is a major cause of road accidents worldwide. This project presents a **Real-Time Driver Drowsiness Detection System** that monitors a driver's eye movements through a webcam and detects signs of drowsiness using Computer Vision techniques.

The system uses **Dlib Facial Landmark Detection** and **Eye Aspect Ratio (EAR)** analysis to determine whether the driver's eyes remain closed for a prolonged period. When drowsiness is detected, an alert message is displayed, helping to prevent accidents and improve road safety.

---

## 🎯 Objective

The primary objective of this project is to develop a real-time driver monitoring system that:

* Detects driver drowsiness using eye movement analysis.
* Monitors eye closure continuously.
* Alerts the driver when signs of fatigue are detected.
* Enhances road safety through proactive monitoring.

---

## ✨ Features

* Real-time webcam monitoring
* Face detection using Dlib
* Facial landmark detection
* Eye Aspect Ratio (EAR) calculation
* Drowsiness detection based on eye closure
* Alert message generation
* Lightweight and easy-to-use system

---

## 🛠️ Technologies Used

* Python
* OpenCV
* Dlib
* Imutils
* SciPy
* NumPy
* Computer Vision

---

## 💻 Development Environment

* Python 3.x
* Python IDLE
* Windows Operating System
* Webcam

---

## ⚙️ Working Principle

1. Capture live video using a webcam.
2. Detect the driver's face.
3. Extract facial landmarks around both eyes.
4. Calculate the Eye Aspect Ratio (EAR).
5. Compare EAR with a predefined threshold.
6. Monitor eye closure across consecutive frames.
7. Display an alert when drowsiness is detected.

---

## 🔍 Eye Aspect Ratio (EAR)

The Eye Aspect Ratio (EAR) is used to determine whether the eyes are open or closed.

### Parameters Used

* EAR Threshold: **0.25**
* Consecutive Frames Threshold: **20 Frames**

If the EAR remains below the threshold for 20 consecutive frames, the system identifies the driver as drowsy and displays an alert message.

---

## 📦 Installation

Install the required libraries:

```bash
pip install -r requirements.txt
```

---

## ▶️ How to Run

### Step 1: Download Facial Landmark Model

Download the Dlib facial landmark model:

```text
shape_predictor_68_face_landmarks.dat
```

### Step 2: Create Folder Structure

```text
project/
│
├── driver_drowsiness_detection.py
└── models/
    └── shape_predictor_68_face_landmarks.dat
```

### Step 3: Run the Program

Using Python IDLE:

* Open `driver_drowsiness_detection.py`
* Click **Run → Run Module (F5)**

Or using Command Prompt:

```bash
python driver_drowsiness_detection.py
```

### Step 4: Exit Application

Press:

```text
q
```

to close the webcam window and terminate the program.

---

## 📊 Output

### Non-Drowsy State

* Eyes open
* EAR above threshold
* No alert displayed

### Drowsy State

* Eyes closed for consecutive frames
* EAR below threshold
* Alert message displayed on screen

---

## 🚀 Future Enhancements

* Audio alarm integration
* Yawning detection
* Mobile application deployment
* Night-time driver monitoring
* Deep learning based fatigue detection
* Vehicle safety system integration

---

## 📚 References

* OpenCV Documentation
* Dlib Facial Landmark Detection
* SciPy Distance Functions
* Eye Aspect Ratio (EAR) Based Drowsiness Detection Research

---
