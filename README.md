# 🧠 Alzheimer's Disease Detection Using Deep Learning

## 📖 Overview

Alzheimer's Disease is a progressive neurological disorder that affects memory, thinking, and behavior. Early detection plays a crucial role in improving patient care and treatment planning.

This project uses a **Convolutional Neural Network (CNN)** to classify MRI brain scans into different stages of Alzheimer's Disease. The model analyzes MRI images and predicts the severity of the disease automatically.

---

## 🎯 Objectives

- Detect Alzheimer's Disease from MRI brain scans.
- Classify patients into different disease stages.
- Assist healthcare professionals with AI-based diagnosis.
- Demonstrate the application of Deep Learning in medical imaging.

---

## 🏷️ Classes

The model classifies MRI scans into the following categories:

| Class | Description |
|---------|-------------|
| Non-Demented | Healthy brain |
| Very Mild Demented | Early stage Alzheimer's |
| Mild Demented | Moderate cognitive decline |
| Moderate Demented | Advanced Alzheimer's |

---

## 📂 Dataset Structure

```text
dataset/
│
├── NonDemented/
├── VeryMildDemented/
├── MildDemented/
└── ModerateDemented/
```

Dataset Source: Kaggle Alzheimer's MRI Dataset

---

## 🛠️ Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- OpenCV
- Scikit-Learn

---

## 🧠 CNN Architecture

```text
Input Image (128x128x3)
        │
Conv2D (32 Filters)
        │
Batch Normalization
        │
MaxPooling2D
        │
Conv2D (64 Filters)
        │
Batch Normalization
        │
MaxPooling2D
        │
Conv2D (128 Filters)
        │
Batch Normalization
        │
MaxPooling2D
        │
Conv2D (256 Filters)
        │
Batch Normalization
        │
MaxPooling2D
        │
Flatten
        │
Dense (256)
        │
Dropout (0.5)
        │
Dense (4, Softmax)
        │
Prediction
```

---

## ⚙️ Data Preprocessing

The following preprocessing techniques were applied:

- Image Resizing
- Normalization
- Data Augmentation
- One-Hot Encoding
- Train-Test Split

### Data Augmentation

- Rotation
- Zoom
- Width Shift
- Height Shift
- Horizontal Flip
- Brightness Adjustment

---

## 🚀 Installation

### Clone Repository

```bash
git clone https://github.com/your-username/alzheimers-disease-detection.git
cd alzheimers-disease-detection
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

Or install manually:

```bash
pip install tensorflow numpy pandas matplotlib opencv-python scikit-learn
```

---

## ▶️ Train the Model

```bash
python train.py
```

The training process:

1. Load MRI images
2. Preprocess data
3. Apply augmentation
4. Train CNN model
5. Validate model
6. Save best model

---

## 🔍 Make Predictions

```bash
python predict.py
```

Example Output:

```text
Predicted Class : Mild Demented
Confidence Score : 92.3%
```

---

## 📊 Performance

Metrics Used:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

Example Results:

```text
Training Accuracy  : 85%
Validation Accuracy : 84%
```

---

## 📈 Project Workflow

```text
MRI Brain Images
        │
        ▼
Data Preprocessing
        │
        ▼
Data Augmentation
        │
        ▼
CNN Model Training
        │
        ▼
Model Evaluation
        │
        ▼
Disease Prediction
        │
        ▼
Alzheimer's Stage Classification
```

---

## 💡 Applications

- Medical Imaging
- Healthcare Diagnostics
- Clinical Decision Support
- Alzheimer's Screening
- AI-Assisted Disease Detection

---

## 🔮 Future Enhancements

- Transfer Learning (EfficientNetB0, ResNet50)
- Web Application Deployment
- Mobile Application Support
- Explainable AI (XAI)
- Larger MRI Datasets
- Real-Time Prediction System

---

## 👨‍💻 Author

**Surya Pratap Verma**
**Shagun Chauhan**

B.Tech Computer Science & Engineering  
Galgotias University

---

## ⚠️ Disclaimer

This project is developed for educational and research purposes only. It should not be used as a replacement for professional medical diagnosis.
