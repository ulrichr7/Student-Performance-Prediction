**Student Academic Performance Prediction**

*Overview:*

This project compares traditional machine learning and deep learning approaches for predicting student academic performance using the UCI Student Performance dataset.
The objective is to classify students as one of the following:
Pass (G3 ≥ 10)
At Risk (G3 < 10)
*The study evaluates multiple machine learning and neural network models using a common evaluation framework.*

**Dataset**

Source: UCI Student Performance Dataset
Records: 395 students
Features: 33 attributes
Domain: Educational Data Mining
Target: Pass/Fail classification derived from final grade (G3)

**Technologies Used:**

Python
Pandas
NumPy
Scikit-learn
TensorFlow / Keras
Matplotlib
Seaborn

**Data Preprocessing:**

The following preprocessing steps were applied:
Missing value inspection
Binary target engineering
One-hot encoding of categorical variables
Standardization of numerical features
Train-test split (80/20)

**Experiments:**

Traditional Machine Learning
Logistic Regression Baseline
Logistic Regression (C = 0.5)
Random Forest
Tuned Random Forest
Deep Learning
Sequential Neural Network
Deep Sequential Neural Network
Sequential Neural Network with Dropout
Functional API Neural Network

**Results:**

Model
Accuracy
Precision
Recall
F1
ROC-AUC
Logistic Regression Baseline
87.34%
95.74%
84.91%
0.900
0.948
Logistic Regression, C=0.5
86.08%
94.34%
84.91%
0.889
0.944
Random Forest Default
86.08%
92.73%
86.44%
0.891
0.929
Random Forest Tuned
87.34%
92.86%
87.93%
0.902
0.922
Sequential Deep
84.81%
92.59%
84.75%
0.882
0.927
Sequential Dropout
83.54%
91.07%
83.05%
0.871
0.934
Functional API
82.28%
89.29%
83.05%
0.860
0.924


**Key Findings:**

Traditional machine learning outperformed deep learning.
Logistic regression achieved the highest ROC-AUC (0.948).
Tuned Random Forest achieved the highest F1-score (0.902).
Deep learning models showed mild overfitting.
The dataset size limited neural network performance.

**How to Run:**

Install dependencies
pip install -r requirements.txt

Open the notebook
jupyter notebook

Run all cells sequentially.
