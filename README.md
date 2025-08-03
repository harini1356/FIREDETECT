
# Fire detection

This project focuses on detecting fire in real-time video streams using Python and OpenCV. By analyzing frames from a webcam or video file, the system identifies fire-like colors (such as red, orange, and yellow) and alerts the user if fire is detected.

The goal is to create a basic yet effective fire detection system that can be used for safety and monitoring purposes.


## Table of Contents

Introduction

Project Overview

Key Components and Libraries

System Requirements

How It Works

Code Overview

Output & Alerts

Future Scope


## Project Overview
The main goal of this project is to detect fire in real-time using a camera (USB or laptop webcam) and generate immediate alerts when fire is detected. It helps in early fire detection in homes, industries, and remote places where physical supervision is difficult.

This system is:

Lightweight

Easy to deploy

Open-source and extendable

Ideal for indoor surveillance




## Key Component and library
This is a software-only project, but it may optionally trigger hardware alerts (like buzzers) using additional modules.

🖥️ Software:
Python 3.x

PyCharm IDE (for development)

OpenCV (cv2) – for image processing

NumPy – for handling pixel arrays

playsound / smtplib (optional) – for audio alerts or email notifications

📷 Hardware:
USB Webcam or Laptop Camera (for live feed)

💻 System Requirements
OS: Windows/Linux/macOS

RAM: Minimum 2 GB

PyCharm IDE (Community or Professional)

Python 3.x



## How It Works
Each frame is converted to HSV or RGB for easier fire color detection.

The system scans for fire-colored regions (usually orange/yellow/red).

If a threshold of fire-like pixels is detected:

A warning is displayed on-screen.

Optionally, an alert sound or email is triggered.

Fire detection is based on color segmentation — detecting specific ranges of fire color in the HSV spectrum.

![1](https://github.com/user-attachments/assets/61f60126-a782-4e08-8fd2-7d2c1d5edb37)




## Code Overview

Detect fire in real-time from a camera feed using a trained YOLO model (fire.pt) and display detection with bounding boxes and confidence.

The video window will show a "Fire Detected!" message when fire-like regions are seen.


## Future And Scope
Integrate with IoT devices (like NodeMCU) for SMS or cloud alert

Use Deep Learning (CNN) for more accurate fire recognition



