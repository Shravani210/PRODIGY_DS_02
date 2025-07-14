<h1 align="center"> 🧼 Data Cleaning & 📊 EDA on Titanic Dataset </h1>


This project focuses on analyzing the Titanic dataset from [Kaggle](https://www.kaggle.com/competitions/titanic) to uncover patterns and insights related to passenger survival. The goal is to perform data cleaning and exploratory data analysis (EDA) using Python.


## 📌 Objectives

- Handle missing and inconsistent data
- Transform categorical variables into numeric format
- Visualize survival trends across different features
- Understand how factors like sex, class, age, and fare affected survival


## 🔍 Dataset Used

We used the **`train.csv`** file from the Titanic dataset available on Kaggle.

- This file contains information about **891 passengers**, including whether they survived (`Survived` column).
- It includes features like:
  - `Pclass` (Ticket class)
  - `Sex`
  - `Age`
  - `SibSp` (Number of siblings/spouses aboard)
  - `Parch` (Number of parents/children aboard)
  - `Fare` (Ticket fare)
  - `Embarked` (Port of embarkation)
  - and more...

⚠️ The `train.csv` file is the **only file used** for this EDA project.  
We did **not use** `test.csv` or `gender_submission.csv`, as they do not contain the `Survived` column required for analysis.


## 🧹 Data Cleaning Steps

- Filled missing `Age` values with the median age
- Filled missing `Embarked` values with the most frequent category (mode)
- Converted `Sex` into binary format (male → 0, female → 1)
- One-hot encoded `Embarked` using `get_dummies()`
- Dropped columns not relevant for EDA (`Cabin`, `PassengerId`, etc.)


## 📊 Visualizations

- **Survival Count**: Bar plot showing number of survivors and non-survivors
- **Survival by Sex**: Survival comparison between males and females
- **Survival by Class**: Distribution of survival across passenger classes (Pclass)
- **Age Distribution**: Overall distribution of passenger ages
- **Age vs Survival**: Age distribution split by survival status
- **Fare vs Survival**: Boxplot comparing fare ranges between survived and not survived
- **Correlation Heatmap**: Showed relationships between numerical features


## 🛠 Tools Used

- Python 🐍
- Pandas
- Seaborn
- Matplotlib
- Jupyter Notebook


## 📈 Output Insight (Example)

- Females had a higher survival rate than males
- First-class passengers were more likely to survive
- Younger passengers had slightly better survival odds
