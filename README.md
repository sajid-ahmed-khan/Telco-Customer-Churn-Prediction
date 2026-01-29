# 📊 Telco Customer Churn Prediction

A Machine Learning project to predict whether a customer will leave (churn) or stay, using **Support Vector Machine (SVM)**. This project analyzes customer demographics, services, and account details to classify churn status.

> **Course:** Programming in Python (Fall 2025-2026)  
> **Institution:** American International University-Bangladesh (AIUB)  
> **Section:** B | **Group:** 01

---

## 👥 Team Members & Contributions

| Name | ID | Role | Contribution |
|------|----|------|--------------|
| Sajid Ahmed Khan (Me) | 22-47631-2 | Lead Programmer | Data Cleaning, Feature Scaling & Encoding, SVM Model Implementation, Code Integration. |
| Sayed Nafisur Rahman Alif | 20-43489-1 | Data Analyst | Dataset Selection, Loading Data, Visualization. |
| Jannatul Ferdaus Eva | 21-45204-2 | Evaluator & Writer | Confusion Matrix, Accuracy Calculation, Report Drafting. |
| Md. Gazi Saffat | 22-47396-2 | Researcher & Validator | Train-Test Split, Cross-Validation, Formatting. |

---

## 📂 Dataset Details
* **Source:** Kaggle (IBM Business Analytics)
* **Volume:** 7,043 Rows, 21 Columns
* **Target:** `Churn` (Yes/No)
* [cite_start]**Key Features:** Gender, SeniorCitizen, Partner, Dependents, PhoneService, MultipleLines, InternetService, Contract, MonthlyCharges, TotalCharges [cite: 551-556].

---

## 🛠️ Project Workflow

### 1. Data Loading & Cleaning
* Loaded dataset using `pandas`.
* Converted `TotalCharges` to numeric (handled blank strings).
* Filled missing values with the median.
* [cite_start]Removed duplicates and the unneeded `customerID` column [cite: 588-590].

### 2. Visualization
* [cite_start]Analyzed feature distributions (Gender, Contract, etc.) using `matplotlib` bar charts[cite: 652].

### 3. Preprocessing
* **Label Encoding:** Converted categorical text data into numbers.
* [cite_start]**Feature Scaling:** Applied `StandardScaler` to normalize features for better SVM performance [cite: 736-737].

### 4. Model Implementation
* **Algorithm:** Support Vector Machine (SVM) Classifier.
* **Kernel:** Linear.
* [cite_start]**Split:** 80% Training, 20% Testing (`random_state=3327`)[cite: 761, 773].

---

## 📈 Results & Performance

The model was evaluated using Accuracy Score, Confusion Matrix, and 10-Fold Cross-Validation.

| Metric | Score |
|--------|-------|
| **Training Accuracy** | **79.73%** |
| **Testing Accuracy** | **80.98%** |
| **Cross-Validation Score** | **79.57%** |

* **Confusion Matrix:**
    * True Negatives: 937
    * False Positives: 105
    * False Negatives: 163
    * [cite_start]True Positives: 204 [cite: 803]

---

## 💻 Technologies Used
* **Python**
* **Pandas** (Data Manipulation)
* **NumPy** (Numerical Operations)
* **Matplotlib** (Visualization)
* **Scikit-Learn** (Machine Learning: SVM, Preprocessing, Metrics)

---

## 🚀 How to Run
1.  Clone the repository:
    ```bash
    git clone [https://github.com/sajid-ahmed-khan/Telco-Customer-Churn-Prediction.git](https://github.com/sajid-ahmed-khan/Telco-Customer-Churn-Prediction.git)
    ```
2.  Install dependencies:
    ```bash
    pip install pandas numpy matplotlib scikit-learn
    ```
3.  Run the notebook or script.
