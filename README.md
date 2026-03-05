# ❤️ Heart Disease Data Analysis (EDA)

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-purple)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Plotting-green)

---

# 📌 Project Overview

Cardiovascular diseases (CVDs) are the **leading cause of death globally**, responsible for an estimated **17.9 million deaths each year**, which accounts for **31% of all deaths worldwide**.

Early detection of heart disease is crucial. This project performs **Exploratory Data Analysis (EDA)** on a heart disease dataset to understand patterns, relationships, and potential risk factors contributing to cardiovascular disease.

The goal of this analysis is to **identify insights from the data that can later help build machine learning models for heart disease prediction**.

---

# 📊 Dataset Information

The dataset contains **918 patient records** and **11 clinical features** related to heart disease.

The dataset was created by combining **five different heart disease datasets**:

| Dataset | Observations |
|--------|--------------|
| Cleveland | 303 |
| Hungarian | 294 |
| Switzerland | 123 |
| Long Beach VA | 200 |
| Stalog (Heart) | 270 |

Total records before cleaning: **1190**  
Duplicate records removed: **272**  
Final dataset: **918 observations**

---

# Feature Description

| Feature | Description |
|--------|-------------|
| Age | Age of the patient |
| Sex | Gender (M: Male, F: Female) |
| ChestPainType | Type of chest pain |
| RestingBP | Resting blood pressure |
| Cholesterol | Serum cholesterol |
| FastingBS | Fasting blood sugar |
| RestingECG | Resting electrocardiogram result |
| MaxHR | Maximum heart rate achieved |
| ExerciseAngina | Exercise induced angina |
| Oldpeak | ST depression value |
| ST_Slope | Slope of peak exercise ST segment |
| HeartDisease | Target variable (1 = Disease, 0 = Normal) |

---

# Exploratory Data Analysis

The analysis was performed using **Python, Pandas, Seaborn, and Matplotlib**.

## Data Inspection

Initial exploration of the dataset was done using:

- `df.head()`
- `df.info()`

to understand the structure of the dataset and data types.

---

# Numerical Feature Distribution

Histograms with KDE were used to analyze numerical feature distributions.

Features analyzed:

- Age
- RestingBP
- Cholesterol
- FastingBS
- MaxHR
- Oldpeak

### Observations

- Most patients fall between **40–70 years of age**
- **Resting Blood Pressure** mostly lies between **100–150 mm Hg**
- Many patients have **cholesterol levels between 150–300**
- **Maximum heart rate** values are mostly between **110–170**

---

# Categorical Feature Analysis

Pie charts were used to analyze categorical variables.

### Sex Distribution
- **79% Male**
- **21% Female**

### Chest Pain Type
Types include:
- TA – Typical Angina  
- ATA – Atypical Angina  
- NAP – Non-Anginal Pain  
- ASY – Asymptomatic  

Observation:
- **Asymptomatic chest pain has the highest occurrence**

### Resting ECG
- About **60% of ECG results are normal**

### Exercise Angina
- Nearly **40% of patients experience exercise-induced angina**

### ST Slope
- About **50% of patients have a flat ST slope**

---

# Violin Plot Analysis

Violin plots were used to analyze relationships between numerical variables and the target variable **HeartDisease**.

### Age vs HeartDisease
- Heart disease is more common between **ages 50–65**

### RestingBP vs HeartDisease
- No strong relationship observed

### Cholesterol vs HeartDisease
- Weak relationship observed

---

# Correlation Analysis

A **correlation heatmap** was used to identify relationships between numerical variables.

Important correlations observed:

- **Age and MaxHR → Negative correlation**
- **HeartDisease and MaxHR → Negative correlation**

This suggests that **as age increases, maximum heart rate tends to decrease**, and patients with heart disease often have **lower MaxHR values**.

---

# Joint Plot Analysis

Joint plots were used to visualize relationships between variables.

### Age vs MaxHR
- Hexagonal density plot shows **negative correlation**

### MaxHR vs Age
- Regression plot confirms **negative relationship**

### HeartDisease vs MaxHR
- Regression line indicates that **lower MaxHR may be associated with heart disease**

---

# Pair Plot

A **pairplot** was generated to visualize relationships between all numerical features simultaneously.

This helps identify **patterns, correlations, and distributions** across multiple variables.

---

# 🛠️ Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  

---

# ▶️ How to Run This Project

Follow these steps to run the project on your local machine:

### 1️⃣ Clone the repository

```bash
git clone https://github.com/Darsh-Paliwal/Heart_Failure_Prediction_EDA.git
```

### 2️⃣ Install required libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3️⃣ Run the notebook

Open Jupyter Notebook:

```bash
jupyter notebook
```

Then open:

```
Heart_Failure_Predection_EDA.ipynb
```

Run all cells to reproduce the analysis.

---

# 📁 Project Structure

```
Heart-Disease-EDA
│
├── Heart_Failure_Predection_EDA.ipynb
├── heart.csv
├── README.md
```

---

# Future Work

Possible improvements for this project:

- Build machine learning models for heart disease prediction
- Apply algorithms like:
  - Logistic Regression
  - Random Forest
  - Support Vector Machine
  - XGBoost
- Perform feature engineering
- Evaluate models using accuracy, precision, recall, and ROC-AUC

---

# 👤 Author

**Darsh Paliwal**
