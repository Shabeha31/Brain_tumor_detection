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
This project explores the application of deep learning models for detecting brain tumors from MRI images. The study leverages Convolutional Neural Networks (CNN) and various pre-trained transfer learning models such as VGG-16, InceptionV3, and MobileNet. The models are trained and tested on MRI images with data augmentation techniques to improve generalization, mitigate overfitting, and enhance detection accuracy. Among the evaluated models, MobileNet achieved the highest accuracy, demonstrating its suitability for clinical applications..

Key objectives:
- Apply deep learning techniques for image classification.
- Compare performance of CNN and transfer learning models.
- Use data augmentation to improve model accuracy and generalization.

---

## Dataset
The dataset consists of labeled MRI images divided into two categories:
- **Yes**: MRI scans showing brain tumors.
- **No**: MRI scans of healthy brains.

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

| Model            | Training Accuracy | Validation Accuracy | Test Accuracy | Training Time |
|-----------------|-----------------|-------------------|---------------|---------------|
| CNN (Real)      | 58%             | 73%               | 63%           | 3:56          |
| CNN (Augmented) | 100%            | 89%               | 93%           | 29:50         |
| VGG-16          | 98%             | 94%               | 95%           | 1:59:58       |
| InceptionV3     | 100%            | 97%               | 98%           | 26:42         |
| MobileNet       | 100%            | 99%               | 99%           | 9:46          |

**Best Model:** MobileNet achieved the highest test accuracy (**99%**) and was the most time-efficient, completing training in just under 10 minutes.  
This model’s efficiency and accuracy make it ideal for real-time clinical use.


