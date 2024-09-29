# Human Body Detection using PoseNet

## Overview

This project demonstrates real-time human body detection using PoseNet and ml5.js libraries. The system utilizes the user's webcam to detect and analyze the keypoints of the human body, offering an interactive experience where detected keypoints are displayed on the screen.

PoseNet is a computer vision model used for estimating human poses by detecting key points in real-time. ml5.js is a high-level JavaScript library built on top of TensorFlow.js, which provides a simple API for using machine learning models, including PoseNet.

## Why PoseNet and ml5.js?

### PoseNet:
- PoseNet was developed by Google and was initially released as part of the TensorFlow.js library.
- PoseNet is a highly efficient pose estimation model capable of detecting keypoints in real-time. It is suitable for building human pose tracking applications.
- It provides a quick and accurate method to identify 17 key body parts such as elbows, wrists, and knees.

### ml5.js:
- ml5.js simplifies the usage of TensorFlow.js models. It abstracts complex machine learning tasks, allowing developers to easily integrate pose detection into web applications.
- The library is beginner-friendly and well-suited for creating interactive browser-based experiences.

## Project Structure

The project contains the following key files:

- `index.html`: The main HTML structure for the project, including layout for camera display and keypoints.
- `sketch.js`: JavaScript logic for loading PoseNet, detecting keypoints, and drawing them on the canvas.

## Code Functions

### `sketch.js`

- **`function setup()`**  
  - Initializes the canvas and webcam video feed.  
  - Loads the PoseNet model for keypoint detection.

- **`function modelLoaded()`**  
  - Callback function executed when PoseNet is successfully loaded.

- **`function gotPoses(poses)`**  
  - Receives the detected poses from PoseNet.  
  - Updates the list of keypoints detected on the screen.

- **`function draw()`**  
  - Continuously updates the canvas by rendering the webcam feed and overlaying keypoints detected by PoseNet.

## How to Run

1. Clone this repository to your local machine.
2. Open the `index.html` file in a browser.
3. Allow access to your webcam to see real-time body detection in action.

## Dependencies

- p5.js
- ml5.js

## Live Deployment

Click Here to Interact [Human Body Detection using PoseNet](https://nitinyadav1511.github.io/PoseNet-Human-Body-Detection/).
