# 📄 README
## Metaheuristic-Driven Feature Selection in Deep Neural Networks for Automated Brain Tumor Detection

---

## Project Overview
This project presents an end-to-end deep learning–based medical image analysis system for automated brain tumor classification using MRI scans.
The work combines pre-trained convolutional neural networks (CNNs) with bio-inspired and metaheuristic optimization algorithms to enhance feature selection and comparative analysis.

The project is submitted as part of the **Final Group Project** for the *Machine Learning and Data Visualization* course and focuses on performance comparison, visual analytics, and decision-oriented insights.

---

## Dataset Description

### Domain
Healthcare — Medical Image Analysis (Brain MRI)

### Dataset Structure
```
Dataset/
 ├── Training/
 │    ├── glioma/
 │    ├── meningioma/
 │    ├── notumor/
 │    └── pituitary/
 └── Testing/
      ├── glioma/
      ├── meningioma/
      ├── notumor/
      └── pituitary/
```

### Classes
- Glioma
- Meningioma
- Pituitary Tumor
- No Tumor

The dataset contains labelled MRI brain scans organized into training and testing sets.

---

## Raw vs Processed Data Explanation

- **Raw Data**: Original MRI images stored in class-based directories.
- **Processed Data**: Images were preprocessed dynamically during model training using Keras `ImageDataGenerator`.

### Preprocessing Steps
- Image resizing to **224 × 224**
- Pixel normalisation (rescale = 1/255)
- Batch loading using generators

No separate processed image files were saved, as preprocessing was applied **on-the-fly**, which is standard practice in deep learning workflows.

---

## Models Implemented
Deep Learning Models

Custom CNN (from scratch)

VGG16 (Pre-trained)

ResNet50 (Pre-trained)

DenseNet121 (Pre-trained)

Classical Model

Basic Artificial Neural Network (ANN)

---

## Feature Selection

1. Grey Wolf Optimiser (GWO)

Applied to DenseNet121 deep features

Performs feature selection before SVM classification

Includes convergence analysis and feature reduction evaluation

2. Morphogenetic Algorithm (Morphogenesis-Inspired Optimisation)

Inspired by biological morphogenesis and cellular differentiation

Implements adaptive feature evolution and interaction

Included as a research-oriented bio-inspired optimisation method

Results and limitations are discussed in the final report


 Morphogenesis is included for experimental comparison and academic exploration.

---

## Evaluation Metrics
- Classification Accuracy
- Precision, Recall, F1-Score
- Confusion Matrix
- Loss values
- Computational cost comparison

---

## Visualizations Included
- Model accuracy comparison (bar chart)
- Loss comparison across pre-trained models
- Confusion matrix heatmap
- GWO convergence plot
- Accuracy vs computational cost scatter plot
- Training and validation performance curves

All visualizations are provided as **static images** and embedded in the report and presentation.

---

## Code
- Full implementation is provided as a **PDF export from Google Colab**
- Includes:
  - Data preprocessing
  - Model training
  - Feature extraction
  - GWO optimization
  - Evaluation and visualization

---

## Dashboard Note
An interactive dashboard was not implemented due to the **image-based nature** of the dataset.
Instead, insights are communicated through well-designed analytical visualizations, which are more suitable for medical image classification tasks.

---

## Submission Contents
├── Final_Report.pdf
├── Presentation.pptx
├── Code.pdf
├── Dataset/
│   ├── Training/
│   └── Testing/
├── Images/
│   ├── accuracy_plots.png
│   ├── loss_comparison.png
│   ├── confusion_matrices.png
│   ├── gwo_convergence.png
│   └── feature_visualizations.png
└── README.md
---

## Authors
Group Final Project Submission  
(All group members’ names are listed on the report cover page)

---

## Final Notes
The code link for colab https://colab.research.google.com/drive/1hdOHLF4ip_Ua-HOv3TR78uMqOH0YIXCE?usp=sharing
