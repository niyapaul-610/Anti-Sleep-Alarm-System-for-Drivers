# Anti-Sleep Alarm System for Drivers

A real-time driver drowsiness detection project using Python, OpenCV, Dlib, Firebase, and gTTS.  
It monitors the driver's eyes using a webcam and gives audio alerts + cloud updates if the driver appears sleepy.

---

## Features

- Eye tracking using Dlib face landmarks
- EAR (Eye Aspect Ratio) for drowsiness detection
- Voice alert using gTTS
- Sends alerts to Firebase for remote monitoring
- Real-time webcam feed

---

## Technologies Used

- Python  
- OpenCV  
- Dlib  
- SciPy  
- gTTS  
- Firebase (Realtime DB)  
- pyrebase  

---

## How It Works

1. Detects face & eyes using Dlib
2. Calculates EAR (Eye Aspect Ratio)
3. If EAR is below threshold for too long:
   - Shows “DROWSY ALERT!” on screen
   - Plays a voice message
   - Sends an alert to Firebase

---

## Requirements

Install the following Python packages:
```bash
pip install opencv-python dlib scipy gtts pyrebase4
### Download Dlib Model File

This project uses Dlib's 68-point face landmark detector model.

 Download here:  
[shape_predictor_68_face_landmarks.dat (official link)](http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2)

 After downloading:
1. Extract the `.bz2` file using WinRAR/7-Zip
2. Place `shape_predictor_68_face_landmarks.dat` in the same folder as your Python code
