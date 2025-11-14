# Heart Disease Prediction Using Logistic Regression

# Project Overview
This project predicts the likelihood of **heart disease** using *Logistic Regression*, a supervised machine learning algorithm.  
The model is trained on a structured medical dataset containing features such as **age, cholesterol level, BMI, systolic BP, smoking habits, glucose level**, and more.

The project also includes **data cleaning**, **visualization**, and **performance evaluation**.

---

# Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn  
- Jupyter Notebook  

---

# Dataset Description
The dataset includes **3661 patient records** with the following health parameters:

- Gender  
- Age  
- Smoking Status  
- Cigarettes per Day  
- Blood Pressure Medication  
- Stroke History  
- Hypertension History  
- Diabetes  
- Total Cholesterol  
- Systolic BP  
- Diastolic BP  
- BMI  
- Heart Rate  
- Glucose  
- **Heart Disease (Target: 1 = Yes, 0 = No)**

---

#  Approach

# 1. Data Loading
Dataset loaded using Pandas and inspected for missing values, duplicate entries, and column types.

# 2. Data Preprocessing
- Dropped irrelevant columns (e.g., `education`)  
- Encoded categorical variables (`Gender`, `smokingStatus`, `diabetes`, `Heart Disease`)  
- Replaced invalid values in `smokingStatus`  
- Removed rows with missing values using `dropna()`  
- Split the dataset into **80% training** and **20% testing**

# 3. Exploratory Data Analysis (EDA)
Created visualizations including:
- Age Distribution (Histogram)  
- BMI vs Heart Disease (Bar Graph)  
- Total Cholesterol vs Heart Disease (Bar Graph)  
- Systolic BP vs Heart Disease (Bar Graph)  
- Cigarettes per Day vs Heart Disease (Pie Chart)

# 4. Model Building
Used Logistic Regression:
```
model = LogisticRegression()
model.fit(X_train, y_train)
```

# 5. Model Evaluation
```
Accuracy: 85.13%
```

---

# Results
- Model accuracy: **85%**  
- Clear relationship observed between heart disease and features like BMI, cholesterol, smoking, and blood pressure.  
- Logistic Regression serves as a strong baseline classifier.

---

# Project Structure
```
project/
│── Heart_Disease.csv
│── Heart_disease_project.ipynb
│── README.md
```



