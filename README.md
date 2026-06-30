# Crowd Density Classification using CNN and MobileNetV2

## Overview

This project presents a deep learning approach for crowd density classification using Convolutional Neural Networks (CNNs) and Transfer Learning. The objective is to classify crowd images into different density levels to support applications such as public safety monitoring, smart surveillance, event management, and urban planning.

The implementation was developed as part of the Machine Learning course project.

---

## Project Objectives

- Develop a custom Convolutional Neural Network (CNN) for crowd density classification.
- Compare the CNN with a Transfer Learning model (MobileNetV2).
- Evaluate both models using multiple performance metrics.
- Generate visualizations including confusion matrices, accuracy curves, loss curves, and prediction examples.
- Save all generated outputs for reproducibility.

---

## Dataset

Dataset:
Mall Crowd Counting Dataset

The dataset contains:

- 2,000 RGB images
- Image size: 480 × 640 pixels
- Crowd count annotations
- Images captured from a fixed surveillance camera inside a shopping mall

For this project, continuous crowd counts were converted into five crowd density classes:

- Very Low
- Low
- Medium
- High
- Very High

The original Mall Dataset has been widely used for crowd counting and crowd analysis research.  [oai_citation:0‡GitHub](https://github.com/Yustira/crowd-counting?utm_source=chatgpt.com)

---

## Methodology

The project follows the complete deep learning workflow:

1. Dataset loading
2. Data preprocessing
3. Image resizing
4. Image normalization
5. Data augmentation
6. Density class generation
7. Train / Validation / Test split
8. Custom CNN development
9. MobileNetV2 transfer learning
10. Model training
11. Model evaluation
12. Confusion matrix generation
13. Classification report generation
14. Error analysis
15. Saving all outputs

---

## Deep Learning Models

### Model 1

Custom CNN

Architecture includes:

- Conv2D
- MaxPooling
- Dropout
- Dense Layers
- Softmax Classification

---

### Model 2

MobileNetV2 Transfer Learning

- ImageNet pretrained weights
- Frozen feature extractor
- Global Average Pooling
- Dense classifier

---

## Dataset Split

- Training: 64%
- Validation: 16%
- Testing: 20%

---

## Evaluation Metrics

The following evaluation metrics were used:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Classification Report
- Validation Accuracy
- Test Accuracy

---

## Results

| Model | Validation Accuracy | Test Accuracy |
|-------|--------------------:|--------------:|
| Custom CNN | 41.25% | 40.00% |
| MobileNetV2 | 39.69% | 42.00% |

The Custom CNN achieved the highest validation accuracy, while MobileNetV2 demonstrated slightly better generalization on the independent test set.

---

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Kaggle Notebook

---

## Output Files

The notebook automatically generates:

- Accuracy Curves
- Loss Curves
- Confusion Matrices
- Model Comparison
- Prediction Examples
- Final Model Summary
- Saved Trained Models
- CSV Reports

---

## Repository Structure

```
.
├── notebook.ipynb
├── README.md
└── outputs/
    ├── Accuracy Curves
    ├── Loss Curves
    ├── Confusion Matrices
    ├── Model Comparison
    ├── Prediction Examples
    └── Saved Models
```

---

## Dataset Source

Mall Crowd Counting Dataset

The dataset contains 2,000 RGB images captured from a fixed surveillance camera in a shopping mall and is commonly used for crowd counting and crowd analysis research.  [oai_citation:1‡GitHub](https://github.com/Yustira/crowd-counting?utm_source=chatgpt.com)

---

## Future Improvements

- Fine-tuning the MobileNetV2 backbone
- Testing additional transfer learning architectures
- Implementing advanced Explainable AI techniques
- Exploring crowd counting regression models
- Training on larger crowd analysis datasets

---

## Author

**Amal Siby**

Matriculation Number: **95023082**

University of Europe for Applied Sciences

MSc Data Science

---

## License

This repository is intended for educational and research purposes.
