🚗 Driver Sleep Detection System
📝 Overview
The Driver Sleep Detection System is a Python-based application that uses computer vision techniques to monitor a driver's drowsiness level in real-time. The system detects signs of sleepiness by analyzing eye closure and yawning patterns using OpenCV, Dlib, and the SciPy library. If prolonged eye closure is detected, it triggers an alert sound and captures an image of the driver.

🔹 Features
🛑 Real-time Face & Eye Detection using Dlib's 68 facial landmarks.

👀 Eye Aspect Ratio (EAR) Calculation for detecting drowsiness.

🗣 Mouth Aspect Ratio (MAR) Calculation for yawning detection.

🔊 Audio Alert System to wake up the driver.

📸 Automatic Image Capture upon sleep detection.

📍 Live Location Fetching based on IP address.

📊 Graphical Status Display using OpenCV.

⚙️ Technologies Used
Python

OpenCV

Dlib

NumPy

SciPy

Pygame

Requests

🛠 Installation
Prerequisites
Ensure you have the following installed:

Python 3.x

OpenCV

Dlib (shape_predictor_68_face_landmarks.dat)

NumPy

SciPy

Pygame

Requests

Steps to Install
1️⃣ Clone the repository:

bash
Copy
Edit
git clone https://github.com/yourusername/driver-sleep-detection.git
cd driver-sleep-detection
2️⃣ Install required dependencies:

bash
Copy
Edit
pip install -r requirements.txt
3️⃣ Download the Dlib shape predictor model and place it in the project directory.

🚀 Usage
Run the script:

bash
Copy
Edit
python sleep_detection.py
The system will start detecting drowsiness in real time using the webcam.

If drowsiness is detected:

🔊 An alert sound will play.

📸 An image of the driver will be saved in the sleep_detections folder.

🔍 How It Works
Captures video from the webcam.

Detects the driver’s face and extracts facial landmarks.

Calculates EAR and MAR for drowsiness detection.

Triggers an alert if EAR is below the threshold for a certain duration.

Detects yawning if MAR exceeds the set threshold.

Continuously updates the driver’s status and location.

🤝 Contributing
Feel free to contribute by submitting pull requests.

📜 License
This project is licensed under the MIT License. Unauthorized use, reproduction, or distribution of this project without proper permission is strictly prohibited.

👨‍💻 Author
Priyanshu

