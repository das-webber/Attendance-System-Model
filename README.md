# Attendance-System-Model
 This project detects students in a classroom, marks their attendance, and also recognizes their emotions.   Attendance is only marked within a specific time window (default: 09:30–10:00 AM).   Results are stored in a CSV file.
 ---
 
##  Project Structure

- `data/faces_dataset/` → Student face dataset (5+ images per student)
- `models/` → Trained models (`face_id_svc.joblib`, `label_encoder.joblib`, `emotion_model_arch.json`, `emotion_model_weights.h5`)
- `train_face_id.py` → Train the face recognition model
- `run_attendance.py` → Run the attendance system
- `config.py` → Configuration paths and timing
- `requirements.txt` → Dependencies

---

##  How to Run

1. Install dependencies:
   ```bash
   pip install -r requirements.txt

2. Train the face recognition model:
   Run train_face_id.py

3. Run the attendance system:
   Run run_attendance.py

Notes:

Use real student face images (5+ per student).

Attendance only records between 09:30–10:00 AM (configurable in config.py).

# Emotion Detection Model 

This project is a **Facial Emotion Detection System** built using **TensorFlow/Keras**, **OpenCV**, and **Tkinter**.  
It detects human facial expressions and classifies them into seven categories:

**Angry, Disgust, Fear, Happy, Neutral, Sad, Surprise**


The model weights are too large to store in GitHub directly.  
You can download them here:

- [Download model.weights.h5 (Google Drive)]((https://drive.google.com/file/d/1CWN2ZbszU09mcc9TKfzS7T_5qmdMC9Iz/view?usp=drive_link))

And place this trained weighted file in models directory
---
Repository Structure

attendance-system/
│
├── data/
│   └── faces_dataset/                # student images dataset (real faces required)
│       ├── 001_Student1/
│       │   ├── img1.jpg
│       │   ├── img2.jpg
│       ├── 002_Student2/
│       │   ├── img1.jpg
│       │   ├── img2.jpg
│       └── ...
│
├── models/
│   ├── face_id_svc.joblib            # trained SVM model (face recognition)
│   ├── label_encoder.joblib          # trained label encoder
│   ├── emotion_model_arch.json       # emotion model architecture
│   ├── emotion_model_weights.h5      # emotion model weights
│
├── config.py                         # configuration paths
├── train_face_id.py                  # train face recognition model
├── run_attendance.py                 # main attendance system (face + emotion + csv)
├── requirements.txt                  # dependencies
└── README.md                         # documentation

