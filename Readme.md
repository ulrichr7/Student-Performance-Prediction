# **Student Academic Performance Prediction**

## **Overview**

This project compares traditional machine learning and deep learning approaches for predicting student academic performance using the UCI Student Performance dataset.

The objective is to classify students as one of the following:

* Pass (G3 ≥ 10\)  
* At Risk (G3 \< 10\)

The study evaluates multiple machine learning and neural network models using a common evaluation framework.

---

## **Dataset**

Source: UCI Student Performance Dataset

* Records: 395 students  
* Features: 33 attributes  
* Domain: Educational Data Mining  
* Target: Pass/Fail classification derived from final grade (G3)

---

## **Technologies Used**

* Python  
* Pandas  
* NumPy  
* Scikit-learn  
* TensorFlow / Keras  
* Matplotlib  
* Seaborn

---

## **Data Preprocessing**

The following preprocessing steps were applied:

1. Missing value inspection  
2. Binary target engineering  
3. One-hot encoding of categorical variables  
4. Standardization of numerical features  
5. Train-test split (80/20)

---

## **Experiments**

### **Traditional Machine Learning**

1. Logistic Regression Baseline  
2. Logistic Regression (C \= 0.5)  
3. Random Forest  
4. Tuned Random Forest

### **Deep Learning**

5. Sequential Neural Network  
6. Deep Sequential Neural Network  
7. Sequential Neural Network with Dropout  
8. Functional API Neural Network

---

## **Results**

| Model | Accuracy | Precision | Recall | F1 | ROC-AUC |
| ----- | ----- | ----- | ----- | ----- | ----- |
| Logistic Regression Baseline | 87.34% | 95.74% | 84.91% | 0.900 | 0.948 |
| Logistic Regression, C=0.5 | 86.08% | 94.34% | 84.91% | 0.889 | 0.944 |
| Random Forest Default | 86.08% | 92.73% | 86.44% | 0.891 | 0.929 |
| Random Forest Tuned | 87.34% | 92.86% | 87.93% | 0.902 | 0.922 |
| Sequential Deep | 84.81% | 92.59% | 84.75% | 0.882 | 0.927 |
| Sequential Dropout | 83.54% | 91.07% | 83.05% | 0.871 | 0.934 |
| Functional API | 82.28% | 89.29% | 83.05% | 0.860 | 0.924 |

---

## **Key Findings**

* Traditional machine learning outperformed deep learning.  
* Logistic regression achieved the highest ROC-AUC (0.948).  
* Tuned Random Forest achieved the highest F1-score (0.902).  
* Deep learning models showed mild overfitting.  
* Dataset size limited neural network performance.

---

## **How to Run**

1. Install dependencies

pip install \-r requirements.txt

2. Open the notebook

jupyter notebook

3. Run all cells sequentially.

---

