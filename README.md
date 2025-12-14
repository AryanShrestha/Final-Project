# MSCS-634 Final Project (Deliverable 4)

This repository consolidates Deliverables **1–4** for *Advanced Data Mining for Data-Driven Insights and Predictive Modeling*.

## Dataset
**Breast Cancer Wisconsin (Diagnostic)** (scikit-learn / UCI)  
- 569 samples, 30 numeric features, binary diagnosis (malignant vs benign).

## Included Files
- `Deliverable4_Final_Project_Notebook.ipynb` — consolidated analysis and visuals
- `requirements.txt` — dependencies

## Key Findings
- **EDA:** clear class separation in multiple features; strong multicollinearity among size-related features.
- **Regression:** best model = **Poly2+Ridge** (predicting `mean area`).
- **Classification:** tuned SVM best params = {'svc__C': 10, 'svc__gamma': 0.01}; Test Accuracy=0.982, F1=0.986, AUC=0.997.
- **Clustering:** K-Means (k=2) yields clusters that align reasonably with diagnosis labels.
- **Pattern mining:** high/low feature combinations generate interpretable association rules linked to diagnosis.

## Ethics
- Dataset is anonymized and public (no PII).
- Potential sampling/representation bias; external validation and fairness checks recommended.
- Models intended for decision support, not automated diagnosis.
