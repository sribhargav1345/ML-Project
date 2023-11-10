# ML Project - Handwriting to Digital Text Conversion (H2DTC)

## Overview
This repository contains the code and documentation for the Handwriting to Digital Text Conversion (H2DTC) project, developed as part of CS550, Project Phase 1 at IIT Bhilai.

### Team Members
- JV Aditya (12140840)
- C Nikhil (12140530)
- B Sri Bhargav Ram (12140460)

## Project Description
### 1. Data Pre-processing
We utilized the MNIST and EMNIST datasets, comprising over 400,000 handwritten words for character recognition. The data was divided into training (331,059), testing (41,382), and validation sets (41,382). The preprocessing involved flattening images into a 1D array and using Principal Component Analysis (PCA) for dimensionality reduction (64 components).
a sample train , test folder have uploded, these contain very few images just for an example https://github.com/VaibhavKhamgaonkar/OCR.

### 2. Training with Basic Models
We employed Support Vector Machines (SVM) and K-Means clustering for training. The SVM model achieved 79% accuracy, while the K-Means clustering model achieved 15%. The completed data pipeline includes collecting and preprocessing data, PCA transformation, and model training/validation.

### 3. Future Objectives and Challenges
For the final submission, we aim to enhance model accuracy using Convolutional Neural Networks (CNN) and Recurrent Neural Networks (RNN). Challenges include improving segmentation accuracy, which we plan to address through alternative models and techniques.

### 4. Individual Contributions
- **Data Collection:** All group members contributed.
- **Data Preprocessing, Feature Extraction, Testing:** Nikhil and Aditya.
- **SVM, Grapheme Segmentation, K-Means:** Aditya and Bhargav.

## Final Deliverables
Our final deliverables will include improved machine learning models, a detailed report on methodology, findings, and techniques to overcome segmentation challenges.

## Code Example
Check out the Jupyter Notebook (`ml_proj.ipynb`) for an example of using Nearest Neighbors with K-means clustering to assess accuracy.

```python
# Code snippet from ml_proj.ipynb
from sklearn.neighbors import NearestNeighbors

# ... (previous code)

print(f"Accuracy using Nearest Neighbors with K-means: {accuracy*100:.2f}%")
