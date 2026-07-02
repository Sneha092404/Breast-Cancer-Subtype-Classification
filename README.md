🧬 Breast Cancer Subtype Classification Using Machine Learning

## 📌 Project Overview

This project develops a machine learning model to classify breast cancer into four molecular subtypes using gene expression microarray data obtained from the NCBI Gene Expression Omnibus (GEO).

The workflow includes data preprocessing, metadata extraction, feature engineering, feature selection, machine learning model development, model evaluation, and visualization.

---

## 🎯 Objectives

- Classify breast cancer molecular subtypes using gene expression data.
- Process and clean raw GEO Series Matrix files.
- Train a Random Forest classifier.
- Identify the most informative genes for subtype prediction.
- Evaluate model performance using multiple metrics.

---

## 📂 Dataset

**Dataset:** GSE45827

**Source:** NCBI Gene Expression Omnibus (GEO)

**Platform:** Affymetrix Human Genome U133 Plus 2.0 Array

### Tumor Subtypes Included

- Basal
- HER2
- Luminal A
- Luminal B

**Total tumor samples used:** 130

---

## ⚙️ Project Workflow

1. Download GEO dataset (GSE45827)
2. Load and parse the Series Matrix file
3. Extract tumor subtype labels
4. Clean and preprocess the data
5. Construct feature matrix (X) and target labels (y)
6. Split data into training and testing sets
7. Train a Random Forest classifier
8. Evaluate model performance
9. Generate a confusion matrix
10. Analyze feature importance
11. Perform 5-fold cross-validation
12. Apply feature selection (Top 500 genes)
13. Save the trained model

---

## 🤖 Machine Learning Model

**Algorithm:** Random Forest Classifier

**Train/Test Split:** 80% / 20%

**Cross Validation:** 5-Fold

---

## 📊 Results

| Metric | Value |
|--------|------:|
| Algorithm | Random Forest |
| Test Accuracy | **96.15%** |
| 5-Fold Cross-Validation Accuracy | **93.85%** |
| Original Features | **29,873 genes** |
| Selected Features | **500 genes** |
| Number of Classes | **4** |

---

## 📈 Visualizations

The project includes:

- Confusion Matrix
- Top 15 Important Gene Features
- Feature Importance Analysis

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook

---

## 📁 Project Structure

```text
Breast-Cancer-Subtype-Classification/
│
├── Data/
│   └── GSE45827_series_matrix.txt
│
├── Figures/
│   ├── confusion_matrix.png
│   └── top15_genes.png
│
├── Models/
│   └── random_forest_model.pkl
│
├── Results/
│   ├── feature_importance.csv
│   └── top500_selected_genes.csv
│
├── Notebooks/
│
├── Cancer_Subtype_Classification.ipynb
│
└── README.md
```

---

## 🚀 Future Improvements

- Convert Affymetrix probe IDs to gene symbols.
- Compare additional machine learning models (XGBoost, SVM).
- Explore deep learning approaches for subtype classification.
- Validate the model using independent external datasets.

---

## 📚 Reference

Edgar R, Domrachev M, Lash AE. *Gene Expression Omnibus: NCBI gene expression and hybridization array data repository.* Nucleic Acids Research.

Dataset: **GSE45827**

---

## 👩‍💻 Author

**Sneha Galimotu**
