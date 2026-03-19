#  Data Preparation - Learnings

##  Overview

Data preparation is the process of cleaning, transforming, and organizing raw data into a usable format for analysis or machine learning.

---

##  What I Learned

### 1. Data Cleaning

* Removing duplicate records
* Fixing inconsistent or incorrect values
* Handling outliers in the dataset

---

### 2. Handling Missing Values

* Removing rows with missing data
* Filling missing values using:

  * Mean
  * Median
  * Mode
* Using forward fill and backward fill techniques

---

### 3. Data Transformation

* Converting categorical data into numerical format

  * Label Encoding
  * One-Hot Encoding
* Scaling data:

  * Normalization (Min-Max Scaling)
  * Standardization (Z-score)

---

### 4. Feature Engineering

* Creating new features from existing data
* Selecting important features for better model performance

---

### 5. Data Splitting

* Dividing dataset into:

  * Training Data
  * Testing Data

---

##  Steps in Data Preparation

1. Collect Data
2. Clean Data
3. Handle Missing Values
4. Transform Data
5. Feature Selection
6. Split Data

---

##  Tools Used

* Python
* Pandas
* NumPy
* Scikit-learn

---

##  Example Code

```python
import pandas as pd

# Load dataset
df = pd.read_csv("sample.csv")

# Remove duplicates
df = df.drop_duplicates()

# Fill missing values
df['Age'] = df['Age'].fillna(df['Age'].mean())

print(df.head())
```

---

##  Sample Dataset

```csv
Name,Age,Salary
John,25,50000
Alice,,60000
Bob,30,55000
John,25,50000
```

---

##  Key Takeaways

* Clean data = Better results
* Missing values must be handled properly
* Data transformation is essential for machine learning
* Feature selection improves model performance
