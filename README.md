# TRPV6-ML-Clustering-in-Breast-Cancer


# **Machine Learning–Based Clustering of Tumor Cells to Identify TRPV6 Overexpression Patterns in Breast Cancer**

### **📌 Project Overview**

This project applies **unsupervised machine learning (K-means, PCA)** to cluster tumor cell expression profiles and identify **TRPV6 overexpression patterns** in breast cancer. TRPV6 is a calcium-selective ion channel associated with **tumor progression, chemoresistance, and poor prognosis** in Triple-Negative Breast Cancer (TNBC).
The goal is to computationally separate tumor subpopulations and detect TRPV6-linked aggressive phenotypes.

---

## **🎯 Objectives**

* Identify expression-based clusters of tumor cells using ML techniques.
* Detect subgroups with **high TRPV6 expression**.
* Visualize clustering patterns through PCA and heatmaps.
* Provide insight into TRPV6-related tumor heterogeneity.

---

## **🧬 Biological Significance**

TRPV6 overexpression is strongly associated with:

* Tumor proliferation
* Metastatic potential
* Calcium dysregulation
* Chemoresistance mechanisms

Understanding TRPV6-positive clusters can help in:

* Developing **ion-channel–targeted therapies**
* Patient stratification
* Identifying potential biomarkers

---

## **🧠 Methods Used**

### **1. Data Preprocessing**

* Normalization
* Filtering
* Handling variability

### **2. Machine Learning**

* **K-Means Clustering**
* Elbow Method for K selection
* Principal Component Analysis (PCA)

### **3. Visualization**

* PCA scatterplots
* TRPV6 expression plots
* Cluster-level TRPV6 distribution

.

🧪 Full Workflow
PHASE 1 — Data Collection

Download & extract all GSM files

Prepare matrix, barcodes, and features

PHASE 2 — Create & Merge .h5ad Files
PHASE 3 — Preprocessing & QC

Filter low-quality cells

Normalize, log-transform

Select HVGs

Regress confounders

Scale data

PHASE 4 — Dimensionality Reduction

PCA

Nearest-neighbors graph

UMAP

PHASE 5 — Clustering

Leiden clustering at multiple resolutions

PHASE 6 — Cell-Type Annotation

Using canonical markers:

EPCAM, KRT8/18 (tumor epithelial)

CD3D (T cells)

CD14 (myeloid)

COL1A1 (fibroblasts)

PHASE 7 — TRPV6 Analysis

UMAP visualization

Violin and dot plots

Identification of TRPV6-high tumor clusters

PHASE 8 — Machine Learning

Models used:

Random Forest

XGBoost

Logistic Regression

Purpose:

Predict TRPV6-high cells

Identify gene signatures driving TRPV6 expression

PHASE 9 — Biological Interpretation

TRPV6-high vs TRPV6-low DEGs

GO/KEGG pathway enrichment

Drug target inference (Curcumin, CIS-22A, calcium-channel modulators)

PHASE 10 — Export

Save processed .h5ad

Save all figures
---

## **📊 Results Summary**

* Tumor cells form distinct clusters.
* One or more clusters show **significantly higher TRPV6 expression**, indicating an aggressive phenotype.
* PCA confirms separability between TRPV6-high and TRPV6-low groups.
* Supports hypothesis: **TRPV6 is a key molecular marker in breast cancer heterogeneity.**

---

## **🧪 Tools & Technologies**

* Python
* Google Colab
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn

---

## **📁 File Structure**

```
📂 TRPV6-ML-Clustering
│── data/                 # raw or preprocessed datasets (if shareable)
│── results/              # plots and output
│── notebook.ipynb        # Google Colab notebook
│── README.md             # project description
```

---

## **👩‍🔬 Author**

**Fakhia Mubashir**
B.Sc. Zoology | Computational Biology Enthusiast
Research Focus: Ion Channels, Breast Cancer, and Machine Learning

---

