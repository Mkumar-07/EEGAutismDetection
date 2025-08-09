# EEG-Based Autism Detection

This repository contains code for detecting autism spectrum disorder (ASD) from EEG signals using a combination of signal processing, feature extraction, and machine learning/deep learning techniques.

## 📌 Overview
Autism Spectrum Disorder affects neural activity patterns, which can be detected using EEG (electroencephalography).
This project preprocesses EEG data, extracts meaningful features, and classifies signals into ASD or control groups.

## 🧠 Key Features
- **EEG Preprocessing:** Filtering, resampling, artifact handling.
- **Feature Extraction:**
  - Sample Entropy
  - Higuchi & Petrosian Fractal Dimensions
  - Skewness & Kurtosis
  - Power Spectral Density (PSD)
- **Dimensionality Reduction:** PCA
- **Classification Models:**
  - Logistic Regression
  - Random Forest
  - Support Vector Machine
  - Deep Learning (CNN)

## 📂 Dataset
- EEG recordings in `.vhdr`, `.eeg`, and `.vmrk` formats.
- The dataset path should be set in the notebook.
- Data is expected to be organized in per-subject folders.

## ⚙️ Installation
Clone this repository:
```bash
git clone https://github.com/yourusername/eeg-autism-detection.git
cd eeg-autism-detection
```

Install dependencies:
```bash
pip install -r requirements.txt
```

## 🚀 Usage
Run the Jupyter Notebook:
```bash
jupyter notebook EEG_Autism.ipynb
```

Steps performed:
1. **Load & Fix Data Files** – Adjust header references in `.vhdr` files.
2. **Preprocess Signals** – Filter, resample, segment EEG data.
3. **Extract Features** – Compute entropy, fractal dimensions, spectral features.
4. **Train Models** – Fit ML/DL classifiers and evaluate performance.
5. **Evaluate** – View accuracy, confusion matrix, ROC curves.

## 🔮 Future Work
- Expand dataset size for better generalization.
- Experiment with transformer-based EEG models.
- Perform subject-independent validation.
