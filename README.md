# Relational Dataset Classification Project

This repository contains the implementation of a supervised learning project for classifying nodes in relational datasets (`Cora`, `CiteSeer`, and `Pubmed`). The project applies and compares various machine learning algorithms on these datasets, focusing on feature matrices and performance evaluation.

---

## 📂 Datasets
The datasets include:
1. **Cora:** 2,708 nodes, 5,429 links, 1,433 features, and 7 classes.
2. **CiteSeer:** 3,312 nodes, 4,732 links, 3,703 features, and 6 classes.
3. **Pubmed:** 19,717 nodes, 44,338 links, 500 features, and 3 classes.

Datasets are stored as `.mat` files, containing:
- **Feature matrix (\(X\)):** Encodes node attributes.
- **Adjacency matrix (\(W\)):** Represents relationships or edges between nodes.
- **Labels (\(gnd\)):** Ground truth for supervised learning.

---

## 📊 Models Implemented
The following classifiers were implemented and evaluated:
- **Random Forest**
- **XGBoost**
- **Support Vector Machine (SVM)**
- **Neural Network**
- **Logistic Regression**
- **Naive Bayes**
- **K-Nearest Neighbors (KNN)**

---

## 🛠️ Methodology
1. **Preprocessing:**
   - Standardized or normalized features.
   - Adjusted class labels for compatibility with scikit-learn.

2. **Training and Evaluation:**
   - Applied **Stratified K-Fold Cross-Validation**.
   - Evaluated models using:
     - **Accuracy**
     - **F1-score (weighted)**
     - **Normalized Mutual Information (NMI)**
   - Visualized results with heatmaps and confusion matrices.

---

## 🔑 Results
- **Best Performers:** Random Forest and XGBoost achieved the highest scores across metrics.
- **Neural Network and SVM:** Competitive but slightly underperformed on smaller datasets.
- **Weaker Models:** Naive Bayes and KNN faced challenges with high-dimensional data and feature dependencies.

---

## 🚀 Future Work
- Integrate adjacency matrix (\(W\)) using graph-based methods like **Graph Neural Networks (GNN)** or **Graph Convolutional Networks (GCN)**.
- Address class imbalance with techniques like SMOTE or class-weight adjustments.
- Perform hyperparameter tuning for top-performing models.

---

## 📁 Repository Structure
- `data/`: Contains the datasets in `.mat` format.
- `notebooks/`: Includes the main Jupyter Notebook.
---

## 💡 How to Run

```bash
pip install numpy pandas scikit-learn matplotlib seaborn xgboost notebook
