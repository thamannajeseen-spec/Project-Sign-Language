# AI-based Sign Language Interpretation 🤟

This project is a real-time sign language interpretation system that uses a standard webcam to identify static Indian Sign Language (ISL) gestures. It leverages Google's Mediapipe for high-performance hand landmark extraction and a lightweight Deep Neural Network (DNN) for classification.

The repository also includes a second, comparative model (a Convolutional Neural Network) to demonstrate that the Mediapipe feature-extraction approach is significantly more efficient and effective than training on raw image pixels.

## 🌟 Features

* **Real-time Detection:** Interprets signs live via your webcam.
* **High Accuracy:** Achieves >95% accuracy on the test dataset.
* **Mediapipe Integration:** Uses Mediapipe to extract 63 (x, y, z) hand landmarks, making the model robust to different backgrounds and lighting.
* **Lightweight DNN Model:** The primary model is a simple Deep Neural Network trained on landmark data, resulting in a tiny file size (< 1MB) and extremely fast predictions.
* **Comparative Analysis:** Includes a secondary, traditional CNN model trained on raw images to prove the efficiency of the Mediapipe approach.
  ## 🚀 Demo


https://github.com/user-attachments/assets/167e9859-11d4-42f3-bac8-f34296204650


  
## 📊 Model Comparison

This project's core finding is that a feature-extraction approach (Mediapipe + DNN) is vastly superior to a raw-pixel (CNN) approach for this task.

<img width="828" height="251" alt="Screenshot From 2025-11-03 10-45-21" src="https://github.com/user-attachments/assets/e731fa51-6d5a-40d2-ac19-eb0dd2b27696" />

📂 Repository Structure
```Project-Sign-Language/
├── 01_sign_language.ipynb   # Script 1: Images -> Landmarks CSV
├── 02_sign_language2.ipynb          # Script 2: CSV -> DNN Model
├── 03_sign_language3.py                  # Script 3: Run live webcam demo
├── 04_sign_language_raw_image.ipynb      # (Optional) Script 4: Images -> CNN Model
|
├── sign_language_model.h5          # The trained DNN model
├── scaler.joblib                   # The saved StandardScaler
├── encoder.joblib                  # The saved LabelEncoder
|
├── data/
│   └── Indian-Sign-Language-ISL/   # (Must be downloaded from Kaggle)
|
└── README.md                       # This file
















# -Project-Sign-Language
