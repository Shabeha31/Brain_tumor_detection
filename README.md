Brain Tumor Detection Using CNN and Transfer Learning Models

Project Overview
This project explores the application of deep learning models for detecting brain tumors from MRI images. The study leverages Convolutional Neural Networks (CNN) and various pre-trained transfer learning models such as VGG-16, InceptionV3, and MobileNet. The models are trained and tested on MRI images with data augmentation techniques to improve generalization, mitigate overfitting, and enhance detection accuracy. Among the evaluated models, MobileNet achieved the highest accuracy, demonstrating its suitability for clinical applications.

Objectives
The primary goals of this project are:
1.	To implement CNN and transfer learning architectures (VGG-16, InceptionV3, MobileNet) for brain tumor detection.
2.	To apply data augmentation to overcome data scarcity and reduce model overfitting.
3.	To evaluate and compare model performance using metrics such as accuracy, precision, recall, and F1 score.
4.	To identify the best model based on detection accuracy, computation time, and model generalization capabilities.

Dataset
The dataset, sourced from Kaggle, includes 253 MRI images categorized into tumor and non-tumor classes. Given the limited size of the dataset, data augmentation techniques (such as flipping, scaling, and brightness adjustment) were applied to expand the training set and improve model robustness. After augmentation, the training set expanded significantly, enhancing the model's learning ability.

Methodology
1.	Data Preprocessing: The MRI images were normalized, resized, and cropped to focus on the brain region. This step ensures consistency in image dimensions and reduces computational complexity.
2.	Data Augmentation: Augmentation was used to artificially increase the dataset's size, helping reduce overfitting and improve model generalization.
3.	Model Architecture:
o	CNN Architecture: Custom CNN with convolutional, pooling, and dense layers to extract and classify MRI image features.
o	Transfer Learning Models: Pre-trained models (VGG-16, InceptionV3, MobileNet) fine-tuned on the MRI dataset. These models were adapted to the binary classification task (tumor vs. no-tumor).
4.	Evaluation Metrics: The models were evaluated based on accuracy, precision, recall, and F1 score. Confusion matrices and accuracy/loss curves were also analyzed.

Results

Model	Training Accuracy	Validation Accuracy	Test Accuracy	Training Time
  CNN (Real)	58%	73%	63%	3:56
  CNN (Augmented)	100%	89%	93%	29:50
  VGG-16	98%	94%	95%	1:59:58
  InceptionV3	100%	97%	98%	26:42
  MobileNet	100%	99%	99%	9:46

Best Model: MobileNet achieved the highest test accuracy (99%) and was the most time-efficient, completing training in just under 10 minutes. This model’s efficiency and accuracy make it ideal for real-time clinical use.

Key Findings

•	Data Augmentation: Significantly improved model performance by expanding the dataset and reducing overfitting.

•	Model Comparison: MobileNet outperformed other models, combining high accuracy with low computational demands, making it well-suited for clinical applications.
•	Transfer Learning Advantage: Pre-trained models provided higher accuracy and generalization compared to the custom CNN model, especially on the augmented dataset.

Conclusion
This study demonstrates the effectiveness of transfer learning models, especially MobileNet, in accurately detecting brain tumors from MRI images. By leveraging data augmentation and pre-trained models, this project offers a reliable, fast, and accurate approach that could support radiologists in diagnosing brain tumors.

