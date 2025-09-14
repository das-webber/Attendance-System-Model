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
