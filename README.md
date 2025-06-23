# Titanic-Data-Preprocessing

# 🚢 Titanic Data Preprocessing & Cleaning Project

This project is a comprehensive demonstration of data cleaning and preprocessing techniques on the **Titanic dataset** — a classic dataset used in machine learning and data science. The goal is to prepare the raw data for downstream ML modeling by cleaning, transforming, and visualizing it.

---

## 📁 Project Contents

This bundle contains:

| File Name                            | Description |
|-------------------------------------|-------------|
| `Titanic-Dataset.csv`               | Original Titanic dataset used for preprocessing |
| `Cleaned_Titanic_Dataset.csv`       | Cleaned version of the dataset (missing values handled, features encoded, outliers removed) |
| `titanic_data_cleaning.py`          | Python script that automates the preprocessing pipeline |
| `Titanic_Preprocessing_Notebook.ipynb` | Jupyter Notebook version with step-by-step explanations and code cells |
| `outlier_boxplots.png`              | Boxplot visualizations of numerical columns showing outliers |
| `preview_boxplots.png`              | Clean preview image of visualized outliers |
| `README.md`                         | This documentation file |

---

## 🎯 Objective

To demonstrate the **entire data cleaning and preprocessing workflow**, which includes:
- Handling missing values
- Encoding categorical features
- Normalizing numerical data
- Detecting and removing outliers
- Saving cleaned data for further analysis or model training

---

## 🧰 Tools & Technologies Used

- **Python 3.x**
- **Pandas** – for data manipulation
- **NumPy** – for numerical operations
- **Matplotlib** & **Seaborn** – for data visualization
- **Scikit-learn** – for feature scaling
- **Jupyter Notebook** – for interactive analysis
- **Termcolor** – for colorful script output (in Python script)

---

## 🗃 Dataset Overview

The Titanic dataset includes information about passengers aboard the RMS Titanic. Each record contains details such as:

- Passenger class (`Pclass`)
- Sex (`Sex`)
- Age (`Age`)
- Number of siblings/spouses aboard (`SibSp`)
- Number of parents/children aboard (`Parch`)
- Ticket fare (`Fare`)
- Port of Embarkation (`Embarked`)
- Survival status (`Survived`)

---

## 🔧 Preprocessing Steps

### 1. 📥 Load & Inspect Data
- Loaded the CSV using `pandas.read_csv`
- Explored missing values and data types

### 2. 🚨 Handle Missing Values
- `Age`: Filled using **median**
- `Embarked`: Filled using **mode**
- `Cabin`: Dropped due to excessive missingness

### 3. 🔢 Encode Categorical Variables
- Converted `Sex` to binary: `0` (male), `1` (female)
- Applied **one-hot encoding** on `Embarked`, dropping one column to avoid multicollinearity

### 4. 📏 Normalize Numerical Features
Used `StandardScaler` from `scikit-learn` to scale:
- `Age`
- `Fare`
- `SibSp`
- `Parch`

### 5. 📦 Outlier Detection & Removal
- Visualized outliers with **boxplots**
- Removed outliers using the **Interquartile Range (IQR)** method

### 6. 💾 Save Outputs
- Cleaned dataset exported to `Cleaned_Titanic_Dataset.csv`
- All visuals and scripts saved into a portable bundle

---

## 🖼 Visualizations

### Outlier Boxplots
The included image `outlier_boxplots.png` visualizes the distribution and outliers of key numeric fields:
- Age
- Fare
- SibSp
- Parch

These plots help in understanding data skewness and support the outlier removal process.

---

## PREVIEW 

![Image](https://github.com/user-attachments/assets/387bfffe-ede3-413e-a88c-2be892ba8fc7)

![Image](https://github.com/user-attachments/assets/74325845-fa91-4f6a-833c-b02e873aba5d)

---

💡 Open the Notebook
Open Titanic_Preprocessing_Notebook.ipynb in JupyterLab or Jupyter Notebook to interactively explore the steps and visualize the process.

---

🔄 Future Enhancements
Add exploratory data analysis (EDA)

Train predictive models (logistic regression, random forest, etc.)

Deploy model using Flask or Streamlit

Perform hyperparameter tuning and model evaluation

---

evaluation

📬 Contact
If you have any questions, feel free to connect:

Developer: Rangesh Pandian PT
Email: [rangeshpandian@gmail.com]

---

