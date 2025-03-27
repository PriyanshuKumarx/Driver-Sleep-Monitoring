# Driver Sleep Detection System

## Overview
The **Driver Sleep Detection System** is a Python-based application that uses computer vision techniques to monitor a driver's drowsiness level in real-time. The system detects signs of sleepiness by analyzing eye closure and yawning patterns using OpenCV, Dlib, and the SciPy library. If the system detects prolonged eye closure, it triggers an alert sound and captures an image of the driver.

## Features
- **Real-time Face and Eye Detection** using Dlib's 68 facial landmarks.
- **Eye Aspect Ratio (EAR) Calculation** to detect drowsiness.
- **Mouth Aspect Ratio (MAR) Calculation** to detect yawning.
- **Audio Alert System** to wake up the driver.
- **Automatic Sleep Detection Image Capture** for analysis.
- **Live Location Fetching** based on IP address.
- **Graphical Display with Status Updates** using OpenCV.

## Technologies Used
- Python
- OpenCV
- Dlib
- NumPy
- SciPy
- Pygame
- Requests

## Installation
### Prerequisites
Ensure you have the following installed:
- Python 3.x
- OpenCV
- Dlib (with pre-trained model `shape_predictor_68_face_landmarks.dat`)
- NumPy
- SciPy
- Pygame
- Requests

### Steps to Install
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/driver-sleep-detection.git
   cd driver-sleep-detection
   ```
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Download the Dlib shape predictor model and place it in the project directory:


## Usage
1. Run the script:
   ```bash
   python sleep_detection.py
   ```
2. The system will start detecting drowsiness in real time using the webcam.
3. If drowsiness is detected:
   - An alert sound will play.
   - An image of the driver will be saved in the `sleep_detections` folder.

## How It Works
1. The system captures video from the webcam.
2. It detects the driver’s face and extracts facial landmarks.
3. It calculates the Eye Aspect Ratio (EAR) and Mouth Aspect Ratio (MAR).
4. If EAR is below the threshold for a certain duration, it detects sleep and triggers an alert.
5. If MAR exceeds the yawn threshold, it detects yawning.
6. The system continuously updates the driver’s status and location.

## Contributing
Feel free to contribute by submitting pull requests.

License

This project is licensed under the MIT License. Unauthorized use, reproduction, or distribution of this project without proper permission is strictly prohibited and may result in necessary actions.

## Author
[Priyanshu](https://github.com/PriyanshuKumarx)

