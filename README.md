# medical-ml-classification
Deep learning project for classifying Alzheimer's disease from MRI scans using CNN, ViT, and other models.

# 🧠 Deep Learning Study for Image Classification of Alzheimer's MRI

**Author**: Simone Castelli  
**Email**: cstsmn.job@gmail.com  
**Date of Publication**: May 2025

This project investigates the use of deep learning architectures to classify Alzheimer's disease from MRI scans. The aim is to distinguish between **No Alzheimer** and **Early Alzheimer** cases by transforming a 4-class dataset into a binary classification problem.

---

## 📚 Project Overview

- **Language**: Python 3  
- **Dataset**: [Alzheimer MRI Disease Classification Dataset (Kaggle)](https://www.kaggle.com/datasets/borhanitrash/alzheimer-mri-disease-classification-dataset)  
- **Total Images**: 5,120 grayscale MRI scans (128×128 resolution)  
- **Preprocessing**: Original 4-class labels were consolidated into two:  
  - `No Alzheimer` → "Non-Demented"  
  - `Early Alzheimer` → Combined "Very Mild", "Mild", and "Moderate Demented"  
- **Data Split**: 60% Training, 20% Validation, 20% Testing (with oversampling applied to the training set)  
- **Frameworks**: TensorFlow, Keras  
- **Key Libraries**: NumPy, Pandas, Matplotlib, scikit-learn, TensorFlow, Keras  
- **Environment**: Google Colab (GPU)  
- **Workflow**: Structured using the CRISP-DM methodology

---

## 🔬 Models Implemented

- Convolutional Neural Network (CNN)  
- Artificial Neural Network (ANN)  
- Residual Network (ResNet50)  
- VGGNet16 (using transfer learning)  
- Vision Transformer (ViT)

---

## 📊 Evaluation Results (Test Set)

| Model      | Accuracy |
|------------|----------|
| **CNN**        | **93.46%**   |
| ANN        | 90.10%   |
| ViT        | 86.23%   |
| VGGNet16   | 82.91%   |
| ResNet50   | 72.75%   |

> The CNN model demonstrated the best overall performance and is the preferred candidate for deployment.

---

## 🚀 Proposed Deployment Plan

- **Platform**: TensorFlow Serving (exposed via a cloud-based API)  
- **Interface**: A web application where clinicians can upload MRI scans and receive real-time predictions  
- **Security**: Data encryption and access control to ensure patient privacy  
- **Maintenance**: Continuous monitoring and retraining with updated data

---

## 🔮 Future Directions

- Integrate explainability tools (AI/XAI) for improved clinical interpretability  
- Explore multiclass classification for more granular staging  
- Fine-tune models with larger and more diverse datasets  
- Investigate integration with clinical systems for usability and validation

---

## 📂 Repository Contents

- `Notebook.ipynb` – Jupyter notebook with all data preprocessing, model training, and evaluation  
- `Presentation.pdf` – Slide deck summarizing the project and findings
- `Report.docx` – Full written report detailing methodology, results, and references  

---

## 📜 Project Note

This is a personal research project focused on the intersection of deep learning and medical imaging, developed with potential real-world deployment in mind.

---

© 2025 Simone Castelli – All rights reserved.
