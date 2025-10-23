# Machine Learning for Medical Predictions  
Master’s Project — University of Essex  

This repository contains my MSc in Artificial Intelligence coursework for the **CE802 – Machine Learning** module.  
The project applies supervised learning algorithms to real-world healthcare data for **disease classification** and **drug dosage prediction** tasks using Python and scikit-learn.

---

## 📘 Overview

This project demonstrates how machine learning models can be used for **medical diagnosis** and **treatment prediction** through two main experiments:

1. **Classification Task (P2):** Predict whether a patient is diabetic.  
2. **Regression Task (P3):** Predict the appropriate drug dosage for a patient.

Both tasks involve data preprocessing, feature encoding, model training, evaluation, and result interpretation.

---

## 📂 Repository Structure

| File | Description |
|------|--------------|
| `CE802_P2_Notebook.ipynb` | Jupyter Notebook implementing classification models (Decision Tree, Random Forest, Gradient Boosting). |
| `CE802_P2_Test.csv` | Test dataset for classification task. |
| `CE802_P3_Notebook.ipynb` | Jupyter Notebook implementing regression models (Linear, Decision Tree, Lasso). |
| `CE802_P3_Test.csv` | Test dataset for regression task. |
| `CE802_Report.pdf` | Full project report including methodology, implementation, and results. |
| `CE802_pilot.pdf` | Pilot study outlining project scope, feasibility, and objectives. |

---

## ⚙️ Methodology

### Data Preparation
- Loaded and cleaned datasets using `pandas`.  
- Removed null values (750 missing in column `F15`).  
- Encoded categorical variables using `LabelEncoder`.  
- Split data into 75% training and 25% testing sets.

### Models Implemented

#### **Classification**
- Decision Tree Classifier  
- Random Forest Classifier  
- Gradient Boosting Classifier  

**Accuracy:**
| Model | Accuracy |
|--------|-----------|
| Decision Tree | 0.776 |
| Random Forest | 0.776 |
| Gradient Boosting | **0.848** |

#### **Regression**
- Linear Regression  
- Decision Tree Regressor  
- Lasso Regression  

**R² Score:**
| Model | R² Score |
|--------|-----------|
| Linear Regression | 0.551 |
| Decision Tree Regressor | 0.186 |
| Lasso Regression | 0.551 |

---

## 📈 Results & Insights

- **Gradient Boosting Classifier** achieved the highest accuracy (~84%).  
- Regression models showed moderate predictive strength, with Linear and Lasso outperforming Decision Tree Regressor.  
- Model performance was constrained by dataset size and weak feature–target correlation.  
- Expanding the dataset could significantly improve predictive performance.

---

## 🧰 Dependencies

```bash
pandas
numpy
scikit-learn
matplotlib
seaborn
