# 😴 Drowsiness Detection System

A real-time computer vision system to detect driver drowsiness and prevent accidents by triggering an alert when eyes are closed for an extended period. This Python-based project utilizes OpenCV, Keras, and a pre-trained CNN model to monitor eye states and ensure road safety.

---

## 🎯 Objective

To reduce the risk of road accidents caused by drowsy driving by detecting prolonged eye closure and alerting the driver using an audible alarm.

---

## 🚗 Problem Statement

Drowsy driving is one of the leading causes of road accidents globally. According to global estimates, fatigue is a factor in 10–25% of all crashes. A system that continuously monitors the driver’s alertness can significantly reduce such incidents.

---

## 🧠 Technologies Used

- 🧾 **Python**
- 🎯 **OpenCV**
- 🧠 **Keras (CNN model)**
- 🎮 **Pygame (for playing alarm sound)**
- 📊 **NumPy**

---

## 🛠️ How It Works

1. Captures real-time video feed from webcam.
2. Detects **face**, **left eye**, and **right eye** using Haar cascades.
3. Passes cropped eye regions to a **CNN model** to classify as **open** or **closed**.
4. Maintains a **score** to track eye closure over time.
5. If eyes remain closed for a threshold duration, plays an **alarm sound** and flashes a red border on the screen.

---

## 🧪 Procedure

1. Take image input from camera.
2. Detect face and define Region of Interest (ROI).
3. Detect eyes within the ROI and process them.
4. Classify eyes as open or closed using the CNN model.
5. Calculate drowsiness score.
6. Trigger alarm if score exceeds the threshold.

---

## 🔔 Alert System

- An alarm is triggered when both eyes remain closed for multiple consecutive frames (threshold score > 10).
- A red border is drawn on the screen to grab the driver’s attention visually.

---
