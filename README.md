## 📩 Contact

**Email:** [shreyans.jaiswal704@gmail.com](mailto:shreyans.jaiswal704@gmail.com)

---

## ⚠️ Important Note

While this model demonstrates strong predictive performance, actual clinical diagnosis of Alzheimer’s disease depends on multiple factors such as patient history, genetics, and professional medical evaluation.

This project is developed strictly for **research and educational purposes only** and should **not be used as a substitute for clinical diagnosis or medical advice**.


# 🧠 Alzheimer Detection Using Deep Learning on MRI & PET Scans

---

## 📌 Overview

Alzheimer’s disease is a progressive neurodegenerative disorder that affects memory and cognitive functions. Early diagnosis is crucial for slowing disease progression and improving patient outcomes.

Manual interpretation of MRI scans is time-consuming and requires expert knowledge. This project leverages **Deep Learning (DL)** techniques to automatically classify brain scans into different stages of Alzheimer’s disease. Additionally, **PET scan integration** is explored to enhance diagnostic accuracy.

---

## 🏫 Academic Information

* **Institute:** Dr. B. R. Ambedkar National Institute of Technology, Jalandhar
* **Department:** Information Technology
* **Project Type:** Minor Project

---

## 👨‍🎓 Project Team

* Shreyans Jaiswal (23124103)
* Abhinoor Tayal (23124003)
* Parav Sharma (23124072)

### 👨‍🏫 Supervisor

Dr. Mohit Kumar 
<br>
Assistant Professor, Department of IT

---

## 🧠 Alzheimer’s Disease Stages

The model classifies brain scans into four categories:

* Non-Demented
* Very Mild Demented
* Mild Demented
* Moderate Demented

---

## ❗ Problem Statement

* Manual MRI analysis is slow and complex
* Early-stage Alzheimer’s symptoms are subtle
* High dependency on expert radiologists
* Lack of scalable automated diagnostic systems

👉 This project aims to build an **AI-based classification system** for early and accurate detection.

---

## 🎯 Objectives

* Preprocess MRI images (resize, normalize, augment)
* Train deep learning models for classification
* Improve performance using optimization techniques
* Compare CNN and Transformer-based models
* Evaluate using Accuracy, Precision, Recall, and F1-score
* Analyze results using confusion matrices

---

## 📂 Dataset

### 🔹 OASIS Dataset - (Open Access Series of Imaging Studies)

https://drive.google.com/drive/folders/1GMJ50JF6zc7TyXNWuXzkr7siypdqodo8

### 🔹 Augmented Alzheimer MRI Dataset (Kaggle)

https://www.kaggle.com/datasets/uraninjo/augmented-alzheimer-mri-dataset

---

## 🧠 Models Implemented

### 🔹 ResNet-18 (CNN)

**Hyperparameters:**

* Batch Size: 32
* Learning Rate: 1e-4
* Epochs: 18
* Weight Decay: 1e-5

**Performance (Original Dataset):**

* Accuracy: 87.45%
* F1 Score: 86.83%

**Performance (Augmented Dataset):**

* Accuracy: 99.84%

---

### 🔧 Model Improvements

**Issue Identified:**

* Unrealistically high accuracy (~99%)
* Data leakage due to improper splitting

**Fixes Applied:**

* Stratified dataset splitting
* Removal of duplicate samples
* Proper train-test separation
* Weighted loss for imbalance

**Updated Performance:**

* Accuracy: ~95%
* Improved generalization

---

### 🔹 Vision Transformer (ViT)

**Configuration:**

* Image Size: 224×224
* Batch Size: 32
* Learning Rate: 5e-5
* Epochs: 30

**MRI Only:**

* Accuracy: 96.28%
* Loss: 0.1089

**MRI + PET (Multi-Modal):**

* Accuracy: **99.97%**
* Loss: 0.0279

👉 **Best Performing Model**

---

## 📈 Key Insights

* Data quality > model complexity
* Augmentation significantly improves performance
* Multi-modal learning (MRI + PET) gives highest accuracy
* Early-stage detection remains the most challenging

---

## 📂 Project Structure

```bash
Alzheimer-Detection/
│
├── app/                        # Streamlit app (UI)
│   └── app.py
│
├── models/                     # Trained models
│   ├── resnet18.pth
│   ├── vit_model.pth
│   └── capsnet.pth
│
├── notebooks/                  # Jupyter notebooks
│   ├── resnet_training.ipynb
│   ├── vit_training.ipynb
│   ├── evaluation.ipynb
│
├── utils/                      # Helper functions
│   ├── preprocessing.py
│   ├── model_loader.py
│   ├── inference.py
│
├── data/ (optional)            # Dataset (not included)
│
├── predict.py                  # Inference script
├── requirements.txt
├── README.md
└── .gitignore
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone Repository

```bash
git clone https://github.com/yourusername/alzheimer-detection.git
cd alzheimer-detection
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🚀 Usage

### ▶️ Run Prediction

```bash
python predict.py
```

---

## 💻 Demo (Optional)

```bash
streamlit run app/app.py
```

---

## ⚠️ Challenges

* Class imbalance in dataset
* Subtle differences in early-stage images
* Risk of overfitting
* Dataset variability
* Deployment in real-world clinical settings

---

## 🚀 Future Scope

* Capsule Networks (CapsNet)
* Grad-CAM (Explainable AI)
* 3D MRI analysis
* Federated learning
* Clinical integration

---

## 📚 References

* OASIS Dataset
* Kaggle Alzheimer MRI Dataset
* PyTorch Documentation
* Vision Transformer Research

---



