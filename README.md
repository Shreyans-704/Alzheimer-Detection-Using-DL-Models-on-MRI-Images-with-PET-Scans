# Alzheimer-Detection-Using-DL-Models-on-MRI-Images-with-PET-Scans
🧠 Alzheimer Detection Using DL Models on MRI Images with PET Scans
📌 Overview

Alzheimer’s disease is a progressive neurodegenerative brain disorder that gradually destroys memory and cognitive abilities. Early diagnosis plays a crucial role in slowing disease progression and improving patients’ quality of life. However, manual analysis of MRI scans is time-consuming and requires expert interpretation.

This project presents an AI-driven deep learning system that automatically classifies brain MRI images into different stages of Alzheimer’s disease. Advanced CNN and Vision Transformer (ViT) models are used, and performance is further enhanced by multi-modal integration of MRI and PET scans.

🏫 Academic Details

Institute: Dr. B. R. Ambedkar National Institute of Technology, Jalandhar

Department: Information Technology

Project Type: Minor Project

👨‍🎓 Team Members

Shreyans Jaiswal (23124103)

Abhinoor Tayal (23124003)

Parav Sharma (23124072)

👨‍🏫 Supervisor

Dr. Mohit Kumar Saini
Assistant Professor, Department of IT

🧠 Stages of Alzheimer’s Disease

The system classifies MRI scans into four stages:

Non-Demented

Very Mild Dementia

Mild Dementia

Moderate Dementia

❗ Problem Statement

Manual MRI analysis is slow and highly dependent on expert radiologists

Early Alzheimer’s signs are subtle and often missed

Limited automated tools exist for quick and reliable diagnosis

There is a need for an AI-based system that can detect Alzheimer’s disease early and accurately

🎯 Objectives

Preprocess MRI images to improve quality and standardize size and format

Build and train deep learning models for Alzheimer’s stage classification

Optimize models for higher accuracy, precision, recall, and F1-score

Compare multiple models to identify the best-performing approach

Visualize results using confusion matrices and performance graphs

Prepare a complete technical report with results and future improvements

📂 Dataset

The project uses publicly available and augmented datasets:

OASIS Dataset (Open Access Series of Imaging Studies)
https://drive.google.com/drive/folders/1GMJ50JF6zc7TyXNWuXzkr7siypdqodo8

Augmented Alzheimer MRI Dataset (Kaggle)
https://www.kaggle.com/datasets/uraninjo/augmented-alzheimer-mri-dataset

🛠️ Models & Implementation
🔹 Model 1: ResNet-18 (CNN)

Batch Size: 32

Learning Rate: 1e-4

Epochs: 18

Weight Decay: 1e-5

Classes: 4

📊 Performance (Original Dataset)

Accuracy: 87.45%

Precision (Weighted): 86.78%

Recall (Weighted): 87.45%

F1-Score (Weighted): 86.83%

📊 Performance (Augmented Dataset)

Accuracy: 99.84%

Precision: 99.84%

Recall: 99.84%

F1-Score: 99.84%

🔹 Model 2: Vision Transformer (ViT – vit_base_patch16_224)

Image Size: 224×224

Batch Size: 32

Learning Rate: 5e-5

Epochs: 30

📊 Performance (MRI Only)

Validation Accuracy: 96.28%

Validation Loss: 0.1089

🧬 MRI + PET Fusion Results

Initial Accuracy (Before Training): 15%

Validation Accuracy (After PET Integration): 99.97%

Validation Loss: 0.0279

⚠️ Challenges

Limited data for some classes (e.g., Moderate Dementia)

Very subtle differences in early-stage MRI scans

Variations in MRI image quality and resolution

Risk of overfitting due to model complexity

Real-world deployment challenges in hospital environments

🚀 Future Scope

Full multi-modal learning using MRI + PET scans

Federated learning for privacy-preserving hospital collaboration

Explainable AI (XAI) to highlight critical brain regions

Training on larger, more diverse datasets

Real-time clinical decision-support integration

📚 References

Research Paper: https://www.biorxiv.org/content/10.1101/070441v4.full.pdf

OASIS Dataset

Augmented Alzheimer MRI Dataset (Kaggle)

CNN Google Colab Notebook

ViT Google Colab Notebook

⚠️ Disclaimer

This project is developed strictly for academic and research purposes.
It is not intended for direct clinical diagnosis without medical professional validation.
