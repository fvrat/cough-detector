# Cough Detection

This repo includes all training & evaluation code for classifying cough events using multimodal sensor data (audio + IMU). The selected model (XGBoost) achieves high accuracy and is optimized for real-time asthma monitoring.

---

## Dataset

- [Edge-AI Cough Counter](https://github.com/orlandic/edge-ai-cough-counter)
- 4,300+ labeled cough events
- Audio + IMU (sitting, walking, noisy environments)

---

## Preprocessing (Python)

- Removed incomplete subjects
- 1s window segmentation (cough & non-cough)
- Feature extraction:
  - **Audio**: MFCCs, ZCR, RMS, spectral features
  - **IMU**: Mean, Std, Min/Max, Energy, Entropy
- Normalized + saved as `.npz`

---

## Models Trained

- Logistic Regression
- Naive Bayes
- LDA
- Decision Tree
- Random Forest
- **XGBoost (Selected)**

---

##  Architecture


---![205b2d73-e260-47d6-a5d4-1ce90ad4e103](https://github.com/user-attachments/assets/b424697f-3b8e-4739-8418-2f2899c9cf51)
