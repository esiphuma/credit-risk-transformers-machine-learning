# credit-risk-transformers-machine-learning
Code for the paper: Enhancing Credit Risk Assessment through Transformer-based Machine Learning Models

# Enhancing Credit Risk Assessment through Transformer-Based Machine Learning Models

This repository contains the official codebase accompanying the research paper:

> **Elekanyani Siphuma (2025)**  
> *Enhancing Credit Risk Assessment through Transformer-Based Machine Learning Models*  
> 📄 [Link to the publication](https://link.springer.com/chapter/10.1007/978-3-031-78255-8_8) (Insert DOI or journal link here)


## 📊 Project Overview

Credit risk assessment is a critical task for financial institutions. This study explores the application of Transformer-based neural network models to improve credit default classification on tabular data. The approach incorporates:

- Multi-head self-attention to learn feature interactions
- Robust evaluation metrics suitable for imbalanced datasets
- Comparative analysis with traditional methods (included in the paper)

## 🧠 Model Summary

- Architecture: Custom Transformer blocks for tabular data
- Layers:
  - MultiHeadAttention with residual connections
  - Feed-forward networks with LayerNormalization
  - Final dense layers with sigmoid output
- Training:
  - Binary cross-entropy loss
  - Early stopping based on validation loss
- Evaluation:
  - Accuracy, Precision, Recall, F1-score
  - ROC AUC, PR AUC, KS statistic, Geometric Mean

## 🛠️ Installation

Clone this repository and install the required packages:

```bash
git clone https://github.com/YOUR_USERNAME/credit-risk-transformers.git
cd credit-risk-transformers
pip install -r requirements.txt
