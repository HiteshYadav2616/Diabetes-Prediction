# 🩺 Diabetes Prediction using Machine Learning

A Machine Learning project that predicts whether a person is diabetic or non-diabetic based on various medical attributes. This project uses a **Support Vector Machine (SVM)** classifier with data preprocessing and feature standardization to achieve reliable prediction performance.

---

## 📌 Project Overview

Diabetes is one of the most common chronic diseases worldwide. Early detection can help prevent serious health complications.

In this project, a Machine Learning model is trained on the Pima Indians Diabetes Dataset to classify patients into:

- ✅ Non-Diabetic (0)
- ✅ Diabetic (1)

The project demonstrates the complete Machine Learning workflow from data preprocessing to model deployment-ready prediction.

---

## 🚀 Features

- Data loading and preprocessing
- Exploratory Data Analysis (EDA)
- Missing value inspection
- Duplicate value checking
- Statistical summary of the dataset
- Feature scaling using StandardScaler
- Train-Test Split
- Support Vector Machine (SVM) Classification
- Model evaluation using Accuracy Score
- Predict diabetes for custom user input

---

## 📂 Project Structure

```
Diabetes-Prediction/
│
├── Diabetes_Prediction.ipynb      # Jupyter Notebook
├── diabetes.csv                   # Dataset
├── README.md                      # Project Documentation
├── .gitignore
```

---

## 📊 Dataset Information

The project uses the **Pima Indians Diabetes Dataset**, which contains medical records of female patients.

### Features

| Feature | Description |
|----------|-------------|
| Pregnancies | Number of pregnancies |
| Glucose | Plasma glucose concentration |
| BloodPressure | Diastolic blood pressure (mm Hg) |
| SkinThickness | Triceps skin fold thickness |
| Insulin | 2-Hour serum insulin |
| BMI | Body Mass Index |
| DiabetesPedigreeFunction | Diabetes pedigree function |
| Age | Age of the patient |
| Outcome | Target Variable (0 = Non-Diabetic, 1 = Diabetic) |

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook
- Google Colab

---

## 📚 Libraries Used

```python
import pandas as pd
import numpy as np

from sklearn.model_selection import train_test_split
from sklearn.preprocessing import MinMaxScaler, StandardScaler
from sklearn.svm import SVC
from sklearn.metrics import accuracy_score
```

---

## 🔄 Machine Learning Workflow

### 1. Import Libraries

Required Python libraries are imported for data manipulation, preprocessing, model building, and evaluation.

---

### 2. Load Dataset

The diabetes dataset is loaded using Pandas.

```python
df = pd.read_csv("diabetes.csv")
```

---

### 3. Data Exploration

The following checks are performed:

- Dataset information
- Statistical summary
- Missing values
- Duplicate records
- Class distribution
- Average values grouped by Outcome

---

### 4. Data Preprocessing

- Features and target variable are separated.
- Dataset is divided into training and testing sets.
- Feature scaling is performed using **StandardScaler**.

Why StandardScaler?

Since SVM is distance-based, scaling helps improve model performance by ensuring all features contribute equally.

---

### 5. Train-Test Split

```python
80% Training Data
20% Testing Data
```

Random state is fixed for reproducibility.

---

### 6. Model Training

A Support Vector Machine classifier with a linear kernel is trained.

```python
model = SVC(kernel='linear')
```

---

### 7. Model Evaluation

Prediction is performed on the test data.

Evaluation metric used:

- Accuracy Score

```python
accuracy_score(y_test, predictions)
```

---

### 8. Prediction System

The notebook includes a custom prediction system where users can input patient information.

Example:

```python
[5,116,74,0,0,25.6,0.201,30]
```

Output:

```
Non-Diabetic
```

or

```
Diabetic
```

---

## 📈 Model Used

### Support Vector Machine (SVM)

Support Vector Machine is a supervised Machine Learning algorithm mainly used for classification tasks.

### Advantages

- Performs well on small datasets
- Effective in high-dimensional spaces
- Robust against overfitting
- Works well with standardized data

---

## 🎯 Results

The model successfully classifies patients into diabetic and non-diabetic categories using medical information.

The notebook evaluates the model using **Accuracy Score**, demonstrating the effectiveness of SVM for binary classification.

---

## 💡 Future Improvements

- Hyperparameter tuning using GridSearchCV
- Compare multiple algorithms
  - Logistic Regression
  - Random Forest
  - Decision Tree
  - XGBoost
- Cross-validation
- Feature engineering
- Build a Streamlit or Flask web application
- Deploy the model on Render, Hugging Face Spaces, or Streamlit Cloud

---

## ▶️ How to Run

### Clone the repository

```bash
git clone https://github.com/HiteshYadav2616/Diabetes-Prediction.git
```

### Navigate to the project

```bash
cd Diabetes-Prediction
```

### Install dependencies

```bash
pip install pandas numpy scikit-learn jupyter
```

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```
Diabetes_Prediction.ipynb
```

---

## 📷 Project Workflow

```
Dataset
    │
    ▼
Data Cleaning
    │
    ▼
EDA
    │
    ▼
Train-Test Split
    │
    ▼
Feature Scaling
    │
    ▼
Support Vector Machine
    │
    ▼
Model Evaluation
    │
    ▼
Prediction
```

---

## 📖 Learning Outcomes

Through this project, I learned:

- Data preprocessing techniques
- Exploratory Data Analysis
- Feature scaling
- Train-test splitting
- Support Vector Machine (SVM)
- Model evaluation
- Building a prediction pipeline
- Creating a complete end-to-end Machine Learning workflow

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

If you find any issue, feel free to open an issue or submit a pull request.

---

## 📜 License

This project is created for educational and learning purposes.

---

## 👨‍💻 Author

**Hitesh**

Aspiring AI & Machine Learning Engineer

---

⭐ If you found this project useful, consider giving it a Star on GitHub!
