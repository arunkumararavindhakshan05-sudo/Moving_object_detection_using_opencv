# Moving Object Detection using OpenCV

A real-time moving object detection project using Python and OpenCV.
It captures live webcam feed, detects motion, and highlights moving objects
with a green bounding box.

## How It Works
- Captures the first frame as the background reference
- Converts each frame to grayscale and applies Gaussian Blur
- Finds the difference between the first frame and current frame
- Draws a bounding box around detected moving objects

## Requirements
- Python 3.x
- OpenCV
- imutils

## Installation

Install the required libraries using pip:

pip install opencv-python
pip install imutils

## How to Run

python cameraTest.py

## Controls
- Press **Q** to quit the camera feed

## Output
- Displays "Normal" when no motion is detected
- Displays "Moving Object detected" when motion is found
- Draws a green rectangle around the moving object