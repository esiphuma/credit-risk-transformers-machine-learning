# Enhancing Credit Risk Assessment through Transformer-Based Machine Learning Models

This repository accompanies the research paper:

> **Elekanyani Siphuma (2025)**  
> *Enhancing Credit Risk Assessment through Transformer-Based Machine Learning Models*  
> 📄 [Link to publication](https://link.springer.com/chapter/10.1007/978-3-031-78255-8_8)  


---

## 📊 Project Overview

This project investigates how Transformer-based deep learning architectures can improve credit default prediction performance on structured (tabular) datasets. The study systematically compares transformer models against several traditional and deep learning baselines, using real-world financial datasets.

---

## 📚 Datasets Used

The study evaluates model performance on three publicly available datasets:

- **Taiwan Credit Card Default Dataset** ([UCI Repository](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients))
- **German Credit Data** ([UCI Repository](https://archive.ics.uci.edu/ml/datasets/statlog+(german+credit+data)))
- **Australian Credit Approval Dataset** ([UCI Repository](https://archive.ics.uci.edu/ml/datasets/statlog+(australian+credit+approval)))

These datasets represent varying levels of class imbalance and feature complexity, enabling robust model evaluation.

---

## 🧠 Models Compared

The following models were implemented and evaluated:

- ✅ **GRU-Transformer**: GRU-based sequential encoder with Transformer decoder  
- ✅ **CNN-SFTransformer**: Convolutional layers feeding into Transformer blocks  
- ✅ **LSTM** (State-of-the-art model for time-series forecasting)
- 🔁 **Traditional Machine Learning Models**:
  - Support Vector Machine (SVM)
  - Logistic Regression
  - Random Forest
  - XGBoost

All models were trained and validated using consistent preprocessing and evaluation metrics.

---

## 🏗️ Model Architecture Summary

- 6 Transformer blocks with:
  - Multi-Head Attention
  - Residual connections and LayerNormalization
- Dense layers with ReLU activation and dropout
- Sigmoid activation for binary classification

---

## 📈 Evaluation Metrics

Each model was evaluated using:

- Accuracy  
- Precision, Recall, F1-Score  
- ROC AUC  
- PR AUC (Average Precision Score)  
- Geometric Mean (G-Mean)  
- Kolmogorov-Smirnov (KS) Statistic

These metrics were chosen to address **class imbalance** in credit default prediction.


## 🛠️ Setup Instructions

To clone this repository and run the project locally:

```bash
# Step 1: Clone the repo
git clone https://github.com/esiphuma/credit-risk-transformers-machine-learning.git
cd credit-risk-transformers-machine-learning

# Step 2: Create and activate virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Step 3: Install required packages
pip install -r requirements.txt
