# Yoga Pose Detection System

This project is a deep learning-based yoga pose classification and evaluation system that processes pre-recorded videos. It uses **MediaPipe** for extracting 3D body keypoints and a hybrid **Conv1D + LSTM neural network** for classifying poses and evaluating their correctness.

---

## Features

- Classifies 5 common yoga poses from video sequences:
  - Anjaneyasana (Low Lunge Pose)
  - Bhujangasana (Cobra Pose)
  - Gomukhasana (Cow Face Pose)
  - Paschimottanasana (Seated Forward Bend)
  - Vyaghrasana (Tiger Pose)
- Uses 33 key body landmarks extracted via MediaPipe
- Evaluates pose correctness using Euclidean distance
- Categorizes posture alignment into risk levels: **Low**, **Moderate**, **High**
- Provides visualization of classification results and model performance

---

## Model Architecture

- **Conv1D Layer**: Extracts spatial features from pose sequences  
- **LSTM Layer**: Learns temporal relationships between frames  
- **Dense Layers**: Classifies into one of the five yoga poses  
- **Evaluation Layer**: Calculates correctness score vs. ideal reference poses


