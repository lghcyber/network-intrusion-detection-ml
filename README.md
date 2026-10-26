# Network Intrusion Detection Using Machine Learning

A machine learning project that uses a Support Vector Machine (SVM) classifier to detect malicious network traffic using the NSL-KDD intrusion detection dataset.

## 🔍 Project Overview

The goal of this project is to perform binary classification on network traffic and determine whether a network connection is normal or malicious.

The project uses the NSL-KDD dataset, which contains network traffic features commonly used for evaluating network intrusion detection systems.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Support Vector Machine (SVM)
- StandardScaler
- One-Hot Encoding
- Matplotlib
- Jupyter Notebook

## ⚙️ Methodology

### 1. Data Preprocessing

The dataset was prepared for machine learning by:

- Splitting the data into 80% training and 20% testing sets
- One-hot encoding categorical network features such as:
  - `protocol_type`
  - `service`
  - `flag`
- Standardizing numerical features using `StandardScaler`
- Preserving class balance during the train/test split

### 2. Model

A Support Vector Machine classifier was used with the following configuration:

- **Kernel:** RBF
- **Probability Estimates:** Enabled
- **Random State:** 42

### 3. Evaluation

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- AUROC
- AUPRC
- Confusion Matrix
- ROC Curve
- Precision-Recall Curve

## 📊 Results

| Metric | Score |
|---|---:|
| Accuracy | 98.95% |
| Precision | 98.69% |
| Recall | 99.06% |
| F1-Score | 98.87% |
| AUROC | 99.81% |
| AUPRC | 99.78% |

The results demonstrate strong performance on the test split, with high precision and recall for binary network intrusion detection.

## 📈 Model Evaluation

The project includes several visualizations for evaluating model performance:

- Confusion Matrix
- Receiver Operating Characteristic (ROC) Curve
- Precision-Recall Curve

These visualizations provide additional insight into the classifier's ability to distinguish between normal and malicious network traffic.

## 📁 Repository Structure

```text
network-intrusion-detection-ml/
│
├── network_intrusion_detection_svm.ipynb
└── README.md
