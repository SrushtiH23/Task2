# Titanic Data Analysis Project

## Overview

This project performs data cleaning, exploratory data analysis (EDA), and visualization on the Titanic dataset using Python. The goal is to understand patterns that influenced passenger survival, such as gender, class, fare, and age.

---

## Dataset

Source: Kaggle Titanic Dataset
Contains passenger details including class, gender, age, fare, and survival status.

---

## Technologies Used

* Python
* Pandas
* Matplotlib
* Seaborn
* Opendatasets (for Kaggle download)

---

## Steps Performed

### 1. Data Loading

Dataset downloaded from Kaggle using `opendatasets` and loaded into a Pandas DataFrame.

### 2. Data Cleaning

* Dropped irrelevant columns: `PassengerId`, `Name`, `Ticket`, `Cabin`
* Filled missing **Age** values with median
* Filled missing **Embarked** values with mode
* Verified no null values remain

### 3. Exploratory Data Analysis

Generated:

* Summary statistics
* Survival rates grouped by:

  * Gender
  * Passenger class
  * Embarkation port
* Distribution statistics for Age and Fare
* Correlation matrix for numeric variables

### 4. Visualization

Created plots showing:

* Survival rate by gender, class, and embarkation point
* Age distribution by survival
* Fare distribution by survival

---

## Key Insights

* Females had significantly higher survival rates than males.
* Passengers in 1st class survived more than those in lower classes.
* Higher fare passengers were more likely to survive.
* Age had weak correlation with survival.

---

## How to Run

```bash
pip install opendatasets pandas matplotlib seaborn
```

```python
import opendatasets as od
od.download("https://www.kaggle.com/datasets/yasserh/titanic-dataset")
```

Then run the notebook/script.

---



---

## Future Improvements

* Feature engineering (family size, title extraction)
* Machine learning model for survival prediction
* Hyperparameter tuning
* Cross-validation

