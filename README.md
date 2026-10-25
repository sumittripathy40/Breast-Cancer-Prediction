# Breast Cancer Prediction using K-Nearest Neighbors

A machine-learning notebook that explores the Wisconsin breast cancer dataset and uses a **K-Nearest Neighbors (KNN)** classifier to classify tumors as benign or malignant based on measured cell-nuclei features.

> **Important:** This repository is an educational machine-learning project, not a medical diagnostic tool. Its predictions must not be used to make healthcare decisions.

## 📌 Project Overview

The notebook loads and explores a breast cancer dataset, scales numeric features, trains a KNN classifier, evaluates its performance, and experiments with feature selection and different values of *k*.

## ✨ What’s Included

- Exploratory analysis of diagnosis labels and feature distributions
- Z-score standardization of numeric features for distance-based classification
- Train/test split for model evaluation
- KNN classification with distance-based weighting
- Confusion-matrix evaluation
- Experiments with removing a correlated feature
- 10-fold cross-validation to compare neighbor counts and estimate an optimal *k*
- A plot of misclassification error against the number of neighbors

## 🧰 Tech Stack

- **Python**
- **Jupyter Notebook**
- **NumPy** and **Pandas** for data handling
- **scikit-learn** for KNN, train/test splitting, cross-validation, and metrics
- **SciPy** for Z-score standardization
- **Matplotlib** and **Seaborn** for visualization

## 📁 Repository Contents

| File | Description |
| --- | --- |
| `KNN+Breast+Cancer+Modeling.ipynb` | Notebook containing data exploration, preprocessing, model training, and evaluation |
| `data set.csv` | Dataset file present in the repository |

**Dataset note:** The notebook currently references a file named `wisc_bc_data.csv`. Make sure the dataset filename in the notebook matches the CSV filename you use before running all cells.

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/sumittripathy40/Breast-Cancer-Prediction.git
cd Breast-Cancer-Prediction
```

### 2. Install dependencies

Use Python 3 with Jupyter Notebook and the libraries used in the notebook:

```bash
python -m pip install numpy pandas scikit-learn scipy seaborn matplotlib notebook
```

### 3. Open the notebook

```bash
jupyter notebook
```

Open `KNN+Breast+Cancer+Modeling.ipynb` from the Jupyter interface and run the cells in order. Confirm the dataset path and filename before executing the data-loading cell.

## 🔬 Model Details

The notebook first trains a KNN classifier with **5 neighbors** and distance-based weighting. It then explores a reduced feature set and uses 10-fold cross-validation to compare values of *k*.

An accuracy value of approximately **96.49%** is recorded in the notebook for the initial 70/30 train/test split. A later experiment records approximately **95.91%** after removing one feature and changing the neighbor count. These are results from the notebook's existing run, not a guarantee of future performance.

## 👨‍💻 Author

**Sumit Tripathy**

- GitHub: [@sumittripathy40](https://github.com/sumittripathy40)
- Repository: [Breast-Cancer-Prediction](https://github.com/sumittripathy40/Breast-Cancer-Prediction)

## 📄 Disclaimer

This project is intended for learning and demonstration only. It is not clinically validated, and it does not provide medical advice or a diagnosis. Always consult qualified healthcare professionals for medical concerns.
