# Brain Tumor Classifier

A binary classifier that detects brain tumors from MRI texture features using Logistic Regression.

## Results
- **Accuracy:** 99%
- **ROC-AUC:** 0.999

## Dataset
3,762 MRI samples with GLCM texture features (Mean, Variance, Entropy, Energy, ASM, Homogeneity, etc.)  
Labels: 0 = No Tumor, 1 = Tumor

## What I did
1. **EDA** — explored feature distributions and correlation heatmap, dropped `Coarseness` (near-zero variance) and `Image` (ID column)
2. **Preprocessing** — 80/20 stratified split, StandardScaler
3. **Model** — Logistic Regression (sklearn)
4. **Evaluation** — classification report, confusion matrix, ROC-AUC



