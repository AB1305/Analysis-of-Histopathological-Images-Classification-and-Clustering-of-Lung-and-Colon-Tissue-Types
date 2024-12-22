# Comprehensive Analysis of Histopathological Images: Classification and Clustering of Lung and Colon Tissue Types

This project aims to classify and cluster histopathological images of lung and colon tissue using advanced deep learning techniques and clustering algorithms. The goal is to develop robust models to assist in cancer diagnosis and treatment planning.

## Table of Contents

- [About the Dataset](#about-the-dataset)
- [Project Overview](#project-overview)
- [Methodology](#methodology)
- [Key Findings](#key-findings)
- [Conclusion](#conclusion)
- [Usage](#usage)

## About the Dataset

- **Source**: [Kaggle Dataset](https://www.kaggle.com/datasets/andrewmvd/lung-and-colon-cancer-histopathological-images/data)
- **Description**:
  - 25,000 images (JPEG, 768x768 pixels) distributed into 5 classes:
    - Lung: benign tissue, adenocarcinoma, squamous cell carcinoma
    - Colon: benign tissue, adenocarcinoma
  - Data augmented using the Augmentor package.

## Project Overview

The project involves the classification of histopathological images to differentiate between healthy and cancerous tissues. Specific objectives include:
- Identifying lung and colon cancer types.
- Visualizing clusters to understand tissue structure.

## Methodology

### Tech Stack
- **Programming Language**: Python
- **Libraries**: PyTorch, Torchvision, Matplotlib, Seaborn, Scikit-learn

### Data Processing
- Dataset split into 80% training and 20% validation sets.
- Images resized to 224x224, normalized, and converted to tensors.

### Model Training
- **Model**: Pre-trained ResNet-18
- **Loss Function**: CrossEntropyLoss
- **Optimizer**: Adam optimizer
- Achieved a validation accuracy of **99.46%**.

### Feature Extraction
- Extracted 512 features per image using ResNet-18.
- Saved features as `.npy` files.

### Clustering Analysis
- Used KMeans clustering with 20 clusters.
- Visualized clusters with PCA and t-SNE.

## Key Findings

### Classification
- **Validation Loss**: 0.0175
- **Validation Accuracy**: 99.46%

### Clustering Metrics
- **Training Silhouette Score**: 0.381
- **Validation Silhouette Score**: 0.424

Visualizations include confusion matrices and t-SNE plots showcasing effective clustering and classification.

## Conclusion

The project demonstrates strong model performance for histopathological image classification and clustering. Future improvements could involve tuning clustering algorithms and enhancing feature extraction methods.

