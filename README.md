# -Visualize-Activation-Maps


# 🎭 Emotion Detection Using CNN

This project is a deep learning-based **real-time emotion detection system** built using a custom-trained Convolutional Neural Network (CNN). The system captures facial expressions via webcam and classifies them into seven emotions using live video feed.

![Emotion Detector 12-04-2025 17_27_17](https://github.com/user-attachments/assets/f1a4a880-4d75-46d7-a92a-b6cee21f0cc8)

---

## 📁 Project Structure

. ├── model_training.ipynb # Model training & evaluation code (custom CNN) ├── emotion_model_best.h5 # Saved best model (download link below if large) ├── haarcascade_frontalface.xml # Face detector used in OpenCV ├── main.py # Real-time webcam emotion detection script ├── requirements.txt # List of required packages ├── confusion_matrix.png # Model evaluation heatmap └── README.md # Project documentation


---

## 😃 Emotions Detected

The model detects the following emotions:
- Angry
- Disgust
- Fear
- Happy
- Neutral
- Sad
- Surprise

---

## 🧠 Model Training

- **Model**: Custom CNN trained from scratch using FER2013 dataset
- **Input Size**: 48x48 grayscale images
- **Epochs**: 22 (Early Stopped at best epoch: 19)
- **Learning Rate**: Scheduled using `ReduceLROnPlateau`
- **Loss Function**: Categorical Cross-Entropy
- **Optimizer**: Adam
- **Activation**: Softmax in final layer

---

## 🧪 Evaluation

| Metric       | Value |
|--------------|-------|
| Training Accuracy | 76.5% |
| Validation Accuracy | 62.7% |
| Final Test Accuracy | **63%** |

### 📉 Confusion Matrix

![Confusion Matrix](![image](https://github.com/user-attachments/assets/ea59f2eb-a08d-4e2a-993a-42525279905a)
)

### 📋 Classification Report

| Emotion   | Precision | Recall | F1-Score |
|-----------|-----------|--------|----------|
| Angry     | 0.58      | 0.51   | 0.54     |
| Disgust   | 0.69      | 0.54   | 0.61     |
| Fear      | 0.56      | 0.32   | 0.41     |
| Happy     | 0.79      | 0.85   | 0.82     |
| Neutral   | 0.58      | 0.55   | 0.57     |
| Sad       | 0.45      | 0.61   | 0.52     |
| Surprise  | 0.74      | 0.80   | 0.77     |

> 🎯 **Overall Accuracy**: 63%  
> 🧪 **Macro Average F1-Score**: 0.60  
> ⚖️ **Weighted Average F1-Score**: 0.62

---

## 🎥 Run the Real-Time Emotion Detector

### 🔧 Step 1: Install dependencies

```bash
pip install -r requirements.txt
🎮 Step 2: Run the script
bash

python main.py
This will activate your webcam and start detecting emotions in real-time.

💾 Downloads
File Type	Download Link
🔗 Saved Model (emotion_model_best.h5)	Download via Google Drive
🔗 Trained Weights (if separate)	Download via Google Drive
📂 GitHub Repository	GitHub Repo Link
⚙️ requirements.txt


numpy
opencv-python
tensorflow
keras
matplotlib
seaborn
scikit-learn
✅ Checklist (As per Task Instructions)
 ✅ Custom CNN model trained from scratch

 ✅ No pre-trained models used

 ✅ Achieved over 60% accuracy (63%)

 ✅ Saved model & code added

 ✅ Used confusion matrix, precision, recall

 ✅ requirements.txt and .ipynb provided

 ✅ Real-time video detection using OpenCV

 ✅ Google Drive and GitHub links provided

🔮 Future Improvements
Improve performance for underrepresented classes like Fear and Sad

Data augmentation to handle imbalanced dataset

Try deeper CNN or add dropout layers for regularization

Deploy GUI-based application or web app for user interaction

👩‍💻 Developed By
Shwet Bhoyar
📧 shwetabhoyar04@gmail.com
🔗 LinkedIn
🔗 GitHub

