# Signature-Fraud-Detection-Using-Deep-Learning
This applies a ResNet50-based CNN to detect genuine vs forged signatures. The system uses preprocessing, feature extraction, and supervised training to build a reliable fraud detection model for applications in banking, legal, and administrative domains.


## 🔍 Problem Statement
Manual signature verification is slow and error-prone. This project automates verification to reduce fraud in domains like banking, legal, and administrative processes.

---

## 🚀 What I did
- Built a **ResNet50-based classifier** for offline signature verification.
- Created a preprocessing pipeline: grayscale/RGB handling, resizing, normalization, and augmentation.
- Trained and evaluated the model using standard metrics (accuracy, precision, recall, F1-score).
- Saved trained model weights for deployment and inference (`models/resnet50_model.h5`).

---

## 📂 Dataset
- The repository contains a **small sample** in `dataset_sample/` (genuine/ and forged/ folders).
- **Original dataset is restricted and cannot be shared** due to confidentiality/privacy.
- Preprocessing steps: resizing, denoising, normalization, and augmentation (rotation, scaling, translation).

---

## 🏗 Architecture 
- **Base model:** ResNet50 (pretrained backbone, fine-tuned on signature images).  
- **Head:** Dense layers + Dropout → binary sigmoid output (genuine vs forged).  
- **Loss:** Binary cross-entropy.  
- **Metrics:** Accuracy, Precision, Recall, F1-score, ROC-AUC.

---

## ⚙ Requirements
Install dependencies:
```bash
pip install -r requirements.txt
