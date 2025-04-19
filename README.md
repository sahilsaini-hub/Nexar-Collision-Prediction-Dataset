# Nexar-Collision-Prediction

# Collision Prediction from Dashcam Videos using Deep Learning

This project presents a complete deep learning pipeline to **predict vehicle collisions and near-miss incidents** from dashcam video footage. The model is trained on the [Nexar Collision Prediction Dataset](https://www.kaggle.com/competitions/nexar-collision-prediction) and is capable of making early predictions to warn drivers in real-time.

---

## Project Overview

The goal is to build a model that can:
- Analyze short video clips from dashcams
- Predict the **likelihood of a collision or near-collision**
- Raise an **audio alert** in real time if risk is detected
- Output a probability score per video for competition submission

---

## Features

-  Frame sampling and feature extraction with **ResNet18**
-  Temporal modeling using **Transformer Encoder**
-  Class imbalance handling using **weighted loss**
-  **Secondary classifier** (logistic regression) to learn dynamic thresholds
-  Real-time **audio alert system** using `pyttsx3`
-  Final submission ready for Kaggle competition format
