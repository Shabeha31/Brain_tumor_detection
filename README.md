# 🧠 Brain Tumor Detection Using CNN & Transfer Learning

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Models Evaluated](#models-evaluated)
- [Installation & Setup](#installation--setup)
- [Usage](#usage)
- [Results](#results)
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
2. Install dependencies:
   pip install -r requirements.txt
3. Ensure you have Jupyter Notebook or a Python IDE installed.

---

## Usage
1. Open the Jupyter Notebook:
   jupyter notebook Brain_Tumor_Detection.ipynb
2. Follow the notebook cells to:
   . Load and preprocess the dataset
   . Train and evaluate models
   . Visualize results
3. Optionally, adjust hyperparameters (epochs, batch size, learning rate) to experiment.

---

## Results

Model	Training Accuracy	Validation Accuracy	Test Accuracy	Training Time
CNN (Real)	58%	73%	63%	3:56
CNN (Augmented)	100%	89%	93%	29:50
VGG-16	98%	94%	95%	1:59:58
InceptionV3	100%	97%	98%	26:42
MobileNet	100%	99%	99%	9:46

Best Model: MobileNet – highest test accuracy with efficient training time.

---

