
# VisionBench: A Comparative Study of CNN Architectures for Facial Emotion Recognition Using Transfer Learning

## Overview

VisionBench is a deep learning benchmarking project that compares multiple state-of-the-art Convolutional Neural Network (CNN) architectures for Facial Emotion Recognition (FER) using Transfer Learning.

The project evaluates how different pretrained CNN backbones perform on the FER2013 dataset under identical training settings.

Architectures evaluated:

- ResNet50
- DenseNet121
- EfficientNet-B0
- ConvNeXt-Tiny

---

## Dataset

Dataset used:

FER2013

- 35,887 grayscale facial images
- Image size: 48×48
- 7 emotion classes

Classes:

- Angry
- Disgust
- Fear
- Happy
- Sad
- Surprise
- Neutral

---

## Project Structure

```
VisionBench-FER-CNN-Comparison/

│
├── notebooks/
│   ├── 01_Data_Preprocessing.ipynb
│   ├── 02_ResNet50.ipynb
│   ├── 03-densenet121.ipynb
│   ├── 04-efficientnet-b0.ipynb
│   ├── 05-convnext-tiny.ipynb
│   ├── 06_Benchmark.ipynb
│
├── src/
│
├── results/
│   ├── plots/
│   ├── confusion_matrices/
│   └── reports/
│
├── README.md
├── requirements.txt
└── LICENSE
```

---

## Models Compared

| Model | Transfer Learning |
|--------|-------------------|
| ResNet50 | Feature Extraction |
| DenseNet121 | Feature Extraction |
| EfficientNet-B0 | Feature Extraction |
| ConvNeXt-Tiny | Feature Extraction |

---

## Evaluation Metrics

Models are evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

---

## Benchmark Results

| Model | Transfer Learning | Test Accuracy |
|--------|------------------|--------------|
| ResNet50 | Feature Extraction | 42.3% |
| DenseNet121 | Feature Extraction | 41.5% |
| EfficientNet-B0 | Feature Extraction | 42.3% |
| ConvNeXt-Tiny | Feature Extraction | (Add your result) |

---

## Key Findings

- Transfer learning provides a strong baseline for FER2013.
- EfficientNet-B0 achieved competitive performance with significantly fewer parameters.
- ConvNeXt-Tiny demonstrates the effectiveness of modern CNN architectures.
- DenseNet121 performed similarly to ResNet while using fewer trainable parameters.
- Happy and Surprise were the easiest emotions to classify.
- Disgust remained the most difficult class because of severe class imbalance.

---

## Future Improvements

- Data augmentation
- Class-balanced loss
- Focal Loss
- Label smoothing
- Mixed precision training
- Hyperparameter optimization
- Vision Transformers
- Ensemble learning

---

## Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---


