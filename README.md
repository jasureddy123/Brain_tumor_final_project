# Brain_tumor_final_project
Automated Brain Tumor Classification using Deep Learning & Explainable AI
Project Overview

This project focuses on building an automated multi-class brain tumor classification system using Deep Learning and Explainable AI (XAI) techniques.

The system analyzes MRI brain images and classifies them into four categories:

Glioma
Meningioma
Pituitary Tumor
No Tumor

In addition to classification, the model provides visual explanations using Grad-CAM to highlight tumor regions, improving trust and interpretability in medical applications.

Objectives
Compare multiple pre-trained CNN models (VGG16, DenseNet121, InceptionV3)
Improve performance using data augmentation & fine-tuning
Evaluate models using:
Accuracy
Precision
Recall
F1-score
Implement Explainable AI (Grad-CAM) for visualization
Build a reliable multi-class classification system for medical use
Dataset
Type: MRI Brain Images
Classes: 4 (Glioma, Meningioma, Pituitary, No Tumor)
Source: Public dataset (Mendeley / Kaggle)
Format: Labeled image folders
Preprocessing
Image resizing: 128 × 128
Normalization: Pixel values scaled (0–1)
One-hot encoding for labels
Data augmentation applied to reduce overfitting
Models Used

The project uses transfer learning with the following architectures:

VGG16
DenseNet121
InceptionV3
Training Setup
Optimizer: Adam
Learning Rate: 0.0001
Batch Size: 32
Epochs: 10
Loss Function: Categorical Crossentropy
Fine-tuning applied after initial training
Results
Before Fine-Tuning
Model	Accuracy	F1 Score
DenseNet121	84.67%	0.8348
InceptionV3	84.36%	0.8322
VGG16	78.72%	0.7687
After Fine-Tuning
Model	Accuracy	F1 Score
InceptionV3	85.13%	0.8415
DenseNet121	84.82%	0.8354
VGG16	79.10%	0.7736

Best Model: InceptionV3

Explainable AI (Grad-CAM)
Highlights important regions in MRI images
Shows where the model is focusing
Improves interpretability and clinical trust

Confirms that predictions are based on tumor regions, not random features

Key Insights
Transfer learning works effectively for medical imaging
Fine-tuning significantly improves performance
Data augmentation helps handle class imbalance
Explainable AI is essential for real-world healthcare use
Limitations
Limited dataset size compared to real-world data
Uses 2D images instead of 3D MRI scans
Lower resolution (128x128) may miss fine details
Training epochs were limited
Future Work
Use larger and more diverse datasets
Implement 3D CNN models
Increase image resolution
Improve real-time deployment
Enhance explainability techniques
Technologies Used
Python
TensorFlow / Keras
NumPy, Matplotlib
Google Colab
References
Iqbal et al. (2024) – EfficientNet for IoMT
Disci et al. (2025) – CNN comparison
Wong et al. (2025) – Data augmentation impact
Nimmagadda & Devi (2025) – YOLOv7 detection
Zarenia et al. (2025) – Attention-based models
Author

Jashwanth Gandavarapu
MSc Data Science – Final Project
