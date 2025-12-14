# 🧠 Alzheimer Detection Using DL Models on MRI Images with PET Scans

## 📌 Overview
Alzheimer’s disease is a progressive neurodegenerative brain disorder that gradually destroys memory and cognitive abilities. Early diagnosis plays a crucial role in slowing disease progression and improving the quality of life of patients.

Manual analysis of MRI brain scans is time-consuming and requires expert interpretation. This project leverages Deep Learning (DL) techniques to automatically classify MRI brain images into different stages of Alzheimer’s disease. PET scan integration is also explored to further enhance diagnostic accuracy.

---

## 🏫 Academic Information
- Institute: Dr. B. R. Ambedkar National Institute of Technology, Jalandhar
- Department: Information Technology
- Project Type: Minor Project

---

## 👨‍🎓 Project Team
- Shreyans Jaiswal (23124103)
- Abhinoor Tayal (23124003)
- Parav Sharma (23124072)

---

## 👨‍🏫 Project Supervisor
- Dr. Mohit Kumar Saini  
  Assistant Professor, Department of Information Technology

---

## 🧠 Stages of Alzheimer’s Disease
The system classifies MRI brain scans into the following stages:
- Non-Demented
- Very Mild Dementia
- Mild Dementia
- Moderate Dementia

---

## ❗ Problem Statement
- Manual interpretation of MRI scans is slow and complex
- Early Alzheimer’s symptoms are subtle and can be missed
- Limited automated diagnostic tools are available
- An AI-based system is required for early and accurate detection

---

## 🎯 Objectives
- Preprocess MRI images to improve quality and remove noise
- Build and train deep learning models for Alzheimer’s stage classification
- Optimize models to improve accuracy, precision, recall, and F1-score
- Compare different models to identify the best-performing approach
- Visualize results using confusion matrices and performance metrics
- Prepare a detailed technical report with future improvements

---

## 📂 Dataset Used
- OASIS Dataset (Open Access Series of Imaging Studies)  
  https://drive.google.com/drive/folders/1GMJ50JF6zc7TyXNWuXzkr7siypdqodo8

- Augmented Alzheimer MRI Dataset (Kaggle)  
  https://www.kaggle.com/datasets/uraninjo/augmented-alzheimer-mri-dataset

---

## 🛠️ Model Implementation

### Model 1: ResNet-18 (CNN)
Hyperparameters:
- Batch Size: 32
- Learning Rate: 1e-4
- Epochs: 18
- Weight Decay: 1e-5
- Number of Classes: 4

Performance (Original Dataset):
- Accuracy: 87.45%
- Precision (Weighted): 86.78%
- Recall (Weighted): 87.45%
- F1-Score (Weighted): 86.83%

Performance (Augmented Dataset):
- Accuracy: 99.84%
- Precision: 99.84%
- Recall: 99.84%
- F1-Score: 99.84%

---

### Model 2: Vision Transformer (ViT – vit_base_patch16_224)
Configuration:
- Image Size: 224 × 224
- Batch Size: 32
- Learning Rate: 5e-5
- Epochs: 30

Performance (MRI Only):
- Validation Accuracy: 96.28%
- Validation Loss: 0.1089

Performance (MRI + PET Integration):
- Initial Accuracy (Before Training): 15%
- Validation Accuracy: 99.97%
- Validation Loss: 0.0279

---

## ⚠️ Challenges
- Limited data for some Alzheimer’s stages
- Subtle visual differences in early-stage MRI images
- Variations in MRI image quality and resolution
- Risk of overfitting due to model complexity
- Challenges in real-world hospital deployment

---

## 🚀 Future Scope
- Multi-modal learning using combined MRI and PET scans
- Federated learning for privacy-preserving hospital collaboration
- Explainable AI (XAI) to highlight critical brain regions
- Training on larger and more diverse datasets
- Integration into real-time clinical decision-support systems

---

## 📚 References
- Research Paper: https://www.biorxiv.org/content/10.1101/070441v4.full.pdf
- OASIS Dataset
- Augmented Alzheimer MRI Dataset (Kaggle)
- CNN Google Colab Notebook
- Vision Transformer Google Colab Notebook

---

## ⚠️ Disclaimer
This project is developed strictly for academic and research purposes.
It is not intended for clinical diagnosis without medical professional validation.
