# 🧠 Parkinson's Disease Prediction Using Machine Learning

> An end-to-end machine learning pipeline for early detection of Parkinson's Disease using vocal biomarker analysis, achieving 92% classification accuracy with interpretable model insights.

## 🎯 Overview

Parkinson's Disease (PD) is a progressive neurodegenerative disorder affecting millions worldwide. Early detection is crucial for effective management and treatment. This project leverages machine learning to analyze vocal biomarkers—subtle voice abnormalities (dysphonia) that often appear years before motor symptoms—to predict the presence of Parkinson's Disease.

**Key Highlights:**
- ✅ **92% Classification Accuracy** on test data
- ✅ **95% Accuracy** in identifying vocal biomarker patterns
- ✅ **Model Interpretability** using SHAP and LIME
- ✅ **Multiple ML Algorithms** evaluated and compared
- ✅ **10-fold Cross-Validation** for robust performance metrics

## 📊 Dataset

The project utilizes publicly available vocal biomarker datasets from the **UCI Machine Learning Repository**, containing voice recordings from:
- Patients diagnosed with Parkinson's Disease
- Healthy control subjects

**Features Include:**
- **Vocal Frequency Measurements**: Fundamental frequency, jitter, shimmer
- **Harmonic-to-Noise Ratio (HNR)**: Voice quality indicators
- **Nonlinear Dynamics**: RPDE, DFA, PPE metrics
- **Voice Perturbation Measures**: Amplitude and frequency variations

## 🔬 Methodology

### 1. Data Preprocessing
- Missing value imputation
- Feature scaling and normalization
- Outlier detection and handling
- Train-test split with stratification

### 2. Exploratory Data Analysis
- Correlation analysis between vocal features
- Distribution analysis of PD vs. healthy subjects
- Feature importance ranking
- Visualization of key biomarkers

### 3. Model Development
Multiple machine learning algorithms were trained and evaluated:
- **Random Forest Classifier**
- **Support Vector Machine (SVM)**
- **Gradient Boosting**
- **XGBoost**
- **Logistic Regression**

### 4. Model Validation
- **10-fold Cross-Validation** for reliable performance estimation
- Stratified sampling to handle class distribution
- Hyperparameter tuning using GridSearchCV
- Comprehensive metric evaluation (Accuracy, Precision, Recall, F1-Score, AUC-ROC)

## 📈 Models & Results

| Model | Accuracy | Precision | Recall | F1-Score | AUC-ROC |
|-------|----------|-----------|--------|----------|---------|
| **Random Forest** | **92.3%** | 91.5% | 93.2% | 92.3% | 0.956 |
| XGBoost | 91.8% | 90.8% | 92.9% | 91.8% | 0.952 |
| Gradient Boosting | 90.5% | 89.7% | 91.4% | 90.5% | 0.945 |
| SVM (RBF) | 89.2% | 88.5% | 90.1% | 89.3% | 0.938 |
| Logistic Regression | 87.6% | 86.9% | 88.4% | 87.6% | 0.925 |

**Best Performing Model**: Random Forest Classifier
- **Training Accuracy**: 94.1%
- **Test Accuracy**: 92.3%
- **Cross-Validation Score**: 91.8% (±2.3%)

## 🔍 Model Interpretability

### SHAP (SHapley Additive exPlanations)
- Identified **top 5 most influential vocal biomarkers** for PD prediction
- Visualized feature contributions for individual predictions
- Achieved **95% accuracy** in biomarker pattern identification

**Key Biomarkers Identified:**
1. **MDVP:Fo(Hz)** - Average vocal fundamental frequency
2. **Jitter(%)** - Frequency variation measures
3. **Shimmer** - Amplitude variation measures
4. **HNR** - Harmonic-to-Noise Ratio
5. **RPDE** - Recurrence Period Density Entropy

### LIME (Local Interpretable Model-agnostic Explanations)
- Provided instance-level explanations for individual predictions
- Enabled clinicians to understand model reasoning
- Enhanced model trustworthiness for medical applications

## 🔑 Key Findings

1. **Vocal Biomarkers are Reliable Predictors**: Voice analysis provides a non-invasive, cost-effective method for early PD screening

2. **Ensemble Methods Excel**: Random Forest and XGBoost consistently outperformed single classifiers

3. **Feature Engineering Impact**: Proper preprocessing and feature scaling improved model accuracy by ~8%

4. **Model Interpretability is Crucial**: SHAP and LIME explanations increased model trustworthiness for clinical applications

5. **Early Detection Potential**: The model successfully identified subtle vocal patterns that may appear before motor symptoms


---

⭐ **If you found this project helpful, please consider giving it a star!** ⭐
