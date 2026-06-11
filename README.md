# 🚗 Driver Drowsiness Detection System

## 📖 Overview

Driver fatigue is one of the major causes of road accidents worldwide. This project presents a **real-time Driver Drowsiness Detection System** that continuously monitors a driver's eye movements using computer vision techniques and alerts the driver when signs of drowsiness are detected.

The system uses **OpenCV**, **Dlib Facial Landmark Detection**, and **Eye Aspect Ratio (EAR)** analysis to determine whether the driver's eyes remain closed for a prolonged period. If drowsiness is detected, the system displays an alert message to help prevent accidents.

---

## 🎯 Objective

To develop a real-time driver monitoring system capable of detecting drowsiness through eye closure analysis and providing timely alerts to improve road safety.

---

## 🛠 Technologies Used

* Python
* OpenCV
* Dlib
* Imutils
* SciPy
* Computer Vision

---

## ⚙️ Working Principle

The system follows these steps:

1. Capture live video using a webcam.
2. Detect the driver's face using Dlib's face detector.
3. Identify facial landmarks around both eyes.
4. Calculate the Eye Aspect Ratio (EAR).
5. Compare EAR with a predefined threshold.
6. Monitor consecutive frames for eye closure.
7. Trigger an alert when drowsiness is detected.

---

## 🔍 Eye Aspect Ratio (EAR)

EAR is calculated using six eye landmarks.

EAR decreases when the eyes are closed and increases when the eyes are open.

The system uses:

* EAR Threshold = **0.25**
* Consecutive Frames = **20**

When EAR remains below the threshold for 20 consecutive frames, the driver is considered drowsy.

---

## 📦 Requirements

Install dependencies using:

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Project

### Step 1

Download the Dlib facial landmark model:

```text
shape_predictor_68_face_landmarks.dat
```

Place it inside:

```text
models/
```

### Step 2

Run the Python file:

```bash
python driver_drowsiness_detection.py
```

### Step 3

Press:

```text
q
```

to quit the application.

---

## 📊 Features

* Real-time webcam monitoring
* Face detection
* Facial landmark detection
* Eye Aspect Ratio calculation
* Drowsiness detection
* Alert notification system
* Lightweight and easy to run

---

## 🔮 Future Improvements

* Audio alarm integration
* Yawning detection
* Mobile application support
* Night-time driver monitoring
* Deep learning based eye-state classification

---

## 📚 References

* OpenCV Documentation
* Dlib Facial Landmark Detection
* SciPy Distance Functions
* Eye Aspect Ratio (EAR) Based Drowsiness Detection Research

---
