# 🛡️ Malicious URL Detection using Machine Learning

This project uses machine learning to detect malicious URLs based on extracted features from the URLs. It is designed for data security analysis, with a focus on **feature engineering** and **XGBoost** classification.

---

## 🚀 Features

- Preprocessing and cleaning of URL dataset
- Rich feature extraction from URLs (e.g., number of dots, length, presence of `@`, `https`, `=`, etc.)
- Training an **XGBoost classifier** for high accuracy
- Evaluation using classification report and confusion matrix
- Visualization of training loss over boosting rounds

---

## 📊 Dataset

The dataset was originally a CSV containing URLs labeled with their type. The labels were encoded for classification. Optionally, we demonstrate how to use a HuggingFace-hosted dataset as well.

---

## 🧠 Feature Engineering Examples

Some of the engineered features:

- Number of `.` characters
- URL length
- Use of `http` or `https`
- Count of `@`, `=`, `-`, `/`
- Abnormal hostname detection using `urlparse`
- Presence of IP address

These features help identify suspicious patterns common in phishing or malicious links.

---

## ⚙️ Model

The model used is **XGBoostClassifier**:

- Lightweight, fast, and accurate
- Handles multiclass classification
- Visualization of log-loss over training epochs

---

## 📈 Results

- High classification accuracy
- Confusion matrix plotted with Seaborn
- Log-loss progression plotted for training and test sets

---

## 📦 Dependencies

Install required packages with:

```bash
pip install torch numpy transformers evaluate python-whois seaborn scikit-learn xgboost datasets
```
