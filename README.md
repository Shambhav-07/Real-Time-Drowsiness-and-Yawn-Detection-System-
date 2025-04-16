# 💤 Real-Time Drowsiness and Yawn Detection System

This is a Python-based real-time drowsiness and yawn detection system using computer vision techniques. It detects if a person is getting drowsy or yawning by monitoring facial landmarks and alerts with an alarm sound.

---

## 🚀 Features

- Detects drowsiness based on Eye Aspect Ratio (EAR)
- Detects yawning by measuring lip distance
- Real-time video stream using webcam
- Alerts with sound (🔊 can be muted with `M` key)
- Uses pre-trained models for face and landmark detection

---

## 🧠 Tech Stack

| Technology     | Role                                 |
|----------------|--------------------------------------|
| Python         | Main programming language            |
| OpenCV         | Face detection and image processing  |
| Dlib           | Facial landmark detection (68 points)|
| Imutils        | Utility functions for OpenCV         |
| Scipy / Numpy  | Eye aspect ratio & distance math     |
| Pygame         | To play alert sound                  |
| Haarcascade XML| Fast face detection                  |

---

## 📁 Folder Structure
📁 Real-Time-Drowsiness-Detection-System/
│
├── drowsiness_yawn.py                 # 🧠 Main Python script for real-time drowsiness and yawn detection
├── shape_predictor_68_face_landmarks.dat  # 📌 Pre-trained dlib model to detect 68 facial landmarks
├── haarcascade_frontalface_default.xml    # 📷 Haar Cascade classifier for quick face detection (OpenCV)
├── Alert.WAV                          # 🔊 Alarm sound file played when drowsiness or yawn is detected
└── README.md                          # 📄 Project documentation explaining setup, usage, and features


---

## 🛠 Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/Real-Time-Drowsiness-Detection-System.git
cd Real-Time-Drowsiness-Detection-System

```
2. Install Requirements
```bash
pip install -r requirements.txt
```
Or install manually:
```bash
pip install opencv-python dlib imutils scipy numpy pygame
```
3. Download Required Files
✅ shape_predictor_68_face_landmarks.dat: Download

✅ haarcascade_frontalface_default.xml: Download

✅ Place them in your project folder.

## ▶️ Usage
```bash
python drowsiness_yawn.py
```
### Controls:

-Press Q to quit.
-Press M to mute/unmute sound.

## 📊 How It Works (High-Level Flow)
-Webcam feed starts.
-Face detected using Haar Cascade.
-Facial landmarks located using Dlib.
-Eye Aspect Ratio (EAR) & lip distance calculated.

### If:

-EAR falls below threshold → Drowsiness Alert
-Lip distance exceeds threshold → Yawn Alert
-Sound alert is played using Pygame.

## 🎯 Use Cases
--Driver drowsiness detection
--Monitoring workers/students
--Alerting system for prolonged inactivity

## 📌 Credits
-Dlib
-OpenCV
-Pygame


## 🙌 Contributing
Found a bug? Have a suggestion? PRs are welcome!


## 📞 Contact
For any questions, feedback, or collaboration, feel free to connect:

👤 Kumar Shambhav
📧 Email: kumarshambhav75@gmail.com
