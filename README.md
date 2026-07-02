\# Breast Cancer Subtype Classification Using Machine Learning



\## Project Overview



This project develops a machine learning model to classify breast cancer into four molecular subtypes using gene expression microarray data from the Gene Expression Omnibus (GEO).



The project covers the complete bioinformatics workflow, including data preprocessing, feature extraction, feature selection, machine learning model development, evaluation, and visualization.



\---



\## Objectives



\- Classify breast cancer molecular subtypes

\- Process raw GEO gene expression data

\- Build a Random Forest classifier

\- Identify important genes for classification

\- Evaluate model performance using multiple metrics



\---



\## Dataset



\*\*Dataset:\*\* GSE45827



\*\*Source:\*\* NCBI Gene Expression Omnibus (GEO)



\*\*Platform:\*\* Affymetrix Human Genome U133 Plus 2.0 Array



\*\*Samples Used\*\*



\- Basal

\- HER2

\- Luminal A

\- Luminal B



Total tumor samples used: \*\*130\*\*



\---



\## Machine Learning Workflow



1\. Download GEO dataset

2\. Load Series Matrix file

3\. Extract tumor subtype labels

4\. Clean and preprocess the dataset

5\. Create feature matrix (X) and target labels (y)

6\. Train Random Forest classifier

7\. Evaluate model performance

8\. Perform feature importance analysis

9\. Perform 5-fold cross-validation

10\. Apply feature selection (Top 500 genes)

11\. Save trained model



\---



\## Results



| Metric | Value |

|--------|------:|

| Algorithm | Random Forest |

| Test Accuracy | \*\*96.15%\*\* |

| 5-Fold Cross Validation Accuracy | \*\*93.85%\*\* |

| Original Features | 29,873 genes |

| Selected Features | 500 genes |

| Cancer Classes | 4 |



\---



\## Visualizations



\- Confusion Matrix

\- Feature Importance Plot



\---



\## Technologies Used



\- Python

\- Pandas

\- NumPy

\- Scikit-learn

\- Matplotlib

\- Jupyter Notebook



\---



\## Project Structure



```text

Cancer\_Subtype\_Project

│

├── Data

│     └── GSE45827\_series\_matrix.txt

│

├── Figures

│     ├── confusion\_matrix.png

│     └── top15\_genes.png

│

├── Models

│     └── random\_forest\_model.pkl

│

├── Results

│     ├── feature\_importance.csv

│     └── top500\_selected\_genes.csv

│

├── Notebooks

│

└── Cancer\_Subtype\_Classification.ipynb

```



\---



\## Future Improvements



\- Convert Affymetrix probe IDs to gene symbols

\- Compare multiple machine learning algorithms

\- Apply deep learning models

\- Validate the model using external datasets



\---



\## Author



\*\*Sneha Galimotu\*\*





