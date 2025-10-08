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
This project focuses on detecting brain tumors from MRI images using deep learning. It combines custom Convolutional Neural Network (CNN) architectures and pre-trained transfer learning models to classify MRI scans as 'Tumor' or 'No Tumor'. The goal is to provide a reliable and automated method for early detection of brain tumors.

Key objectives:
- Apply deep learning techniques for image classification.
- Compare performance of CNN and transfer learning models.
- Use data augmentation to improve model accuracy and generalization.

---

## Dataset
The dataset consists of labeled MRI images divided into two categories:
- **Tumor**: MRI scans showing brain tumors.
- **No Tumor**: MRI scans of healthy brains.

Data preprocessing steps include resizing, normalization, and augmentation (rotation, flipping, zooming) to enhance model performance.

---

## Models Evaluated
- **Convolutional Neural Network (CNN)**: A custom architecture designed specifically for this dataset.
- **VGG-16**: A deep pre-trained network fine-tuned for tumor detection.
- **InceptionV3**: Pre-trained InceptionV3 model adapted to this classification task.
- **MobileNet**: Lightweight pre-trained MobileNet model fine-tuned for high accuracy and speed.

---

## Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/Shabeha31/Brain_tumor_detection.git
   cd Brain_tumor_detection
   pip install -r requirements.txt

