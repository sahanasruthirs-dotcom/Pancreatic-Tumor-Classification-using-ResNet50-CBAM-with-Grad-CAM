# Pancreatic Tumor Classification using ResNet50-CBAM with Grad-CAM

## 📌 Overview

This project explores deep-learning-based pancreatic tumor classification using **ResNet50 enhanced with the Convolutional Block Attention Module (CBAM)** and **Grad-CAM for visual explainability**.

The system aims to classify pancreatic images into two categories: **Normal** and **Pancreatic Tumour**. ResNet50 serves as the feature extraction backbone, CBAM enhances feature representation through channel and spatial attention, and Grad-CAM generates heatmaps to visualize image regions influencing model predictions.

The project also explores integrating the trained model into a web application for single-image analysis.

## 🎯 Objectives

- Develop a ResNet50-CBAM model for pancreatic tumor classification.
- Explore attention mechanisms for improved feature representation.
- Visualize model predictions using Grad-CAM heatmaps.
- Evaluate classification performance using appropriate metrics.
- Provide a user interface for image-based inference.

## 🧠 Methodology

1. **Data Preparation:** Organize and preprocess pancreatic images into training and testing subsets.
2. **Feature Extraction:** Use ResNet50 to extract deep image features.
3. **Attention Mechanism:** Apply CBAM to refine channel-wise and spatial feature representations.
4. **Classification:** Predict one of two classes: Normal or Pancreatic Tumour.
5. **Explainability:** Generate Grad-CAM heatmaps to visualize regions influencing predictions.
6. **Evaluation:** Assess model performance using accuracy, precision, recall, specificity, F1-score, ROC-AUC, and a confusion matrix, where supported by the evaluation pipeline.

## 🛠️ Technologies

- Python
- PyTorch
- Torchvision
- ResNet50
- Convolutional Block Attention Module (CBAM)
- Grad-CAM
- FastAPI
- React

## 🗂️ Dataset Classes

| Label | Class |
|---|---|
| 0 | Normal |
| 1 | Pancreatic Tumour |

The dataset is organized into training and testing subsets. The testing subset should remain separate from training and model selection to reduce the risk of data leakage.

## 📁 Repository Structure

```text
Pancreatic-Malignancy-Detection/
├── app/
├── src/
├── results/
├── notebooks/
├── README.md
└── requirements.txt
```

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd Pancreatic-Malignancy-Detection
```

### 2. Create and activate a virtual environment

```bash
python -m venv .venv
```

On Windows:

```powershell
.venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Prepare the dataset

Place the dataset in the directory structure expected by the project code. Verify class mappings, preprocessing, and model checkpoint paths before running experiments.

### 5. Run the application

Follow the backend and frontend startup instructions defined in the project files. The exact commands depend on the application's entry points and configuration.

## 📊 Evaluation

Model performance should be reported using verified experimental results. Relevant metrics include:

- Accuracy
- Precision
- Sensitivity (Recall)
- Specificity
- F1-score
- ROC-AUC
- Confusion matrix

No performance values are stated here because results must be taken from the actual completed experiments.

## 🔍 Explainable AI with Grad-CAM

Grad-CAM produces class-specific heatmaps that highlight image regions contributing to a model's prediction. These visualizations help inspect model behavior but do not independently establish the presence of a tumor or demonstrate clinical reliability.

## 🔮 Future Work

- Validate performance on independent datasets.
- Investigate robustness across different imaging conditions.
- Perform model comparisons and ablation studies.
- Improve interpretability and error analysis.
- Explore deployment optimization and further validation.

## ⚠️ Disclaimer

This project is intended for academic research and educational purposes. It is not a clinically validated diagnostic system and must not replace professional medical evaluation.

## 👩‍💻 Author

**Sahana Sruthi R. S.**

B.Tech — Computer Science and Engineering  
Artificial Intelligence and Data Analytics
