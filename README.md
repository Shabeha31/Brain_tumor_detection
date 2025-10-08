# 🧠 Brain Tumor Detection Using CNN & Transfer Learning

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Models Evaluated](#models-evaluated)
- [Installation & Setup](#installation--setup)
- [Usage](#usage)
- [Results](#results)
- [License](#license)
- [Author](#author)

---

## Project Overview
This project applies deep learning models for detecting brain tumors from MRI images.  
It uses CNNs and pre-trained transfer learning models (VGG-16, InceptionV3, MobileNet) with data augmentation to improve generalization and accuracy. MobileNet achieved the highest test accuracy of 99%, demonstrating suitability for clinical applications.

---

## Dataset
- 253 MRI images from Kaggle, labeled as **Tumor** or **No Tumor**.  
- Data augmentation (flipping, scaling, brightness adjustment) increased training set size for better model performance.

---

## Models Evaluated
- **CNN (Custom)**: Convolutional layers with pooling and dense layers.  
- **VGG-16**: Pre-trained, fine-tuned on MRI dataset.  
- **InceptionV3**: Pre-trained, fine-tuned.  
- **MobileNet**: Lightweight pre-trained model, achieved highest accuracy.

---

## Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/Shabeha31/Brain_tumor_detection.git
   cd Brain_tumor_detection
