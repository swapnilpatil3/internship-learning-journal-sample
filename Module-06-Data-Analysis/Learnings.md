#  Data Analysis - Learnings

##  Overview

Data analysis is the process of inspecting, cleaning, transforming, and modeling data to discover useful information, draw conclusions, and support decision-making.

---

##  What is Exploratory Data Analysis (EDA)?

Exploratory Data Analysis (EDA) is the initial step in data analysis where we explore the dataset to understand its structure, patterns, relationships, and anomalies.

 Purpose of EDA:

* Understand dataset structure
* Identify missing values
* Detect outliers
* Find patterns and trends
* Check relationships between variables

---

##  Types of Data Analysis

1. **Descriptive Analysis** → What happened?
2. **Diagnostic Analysis** → Why it happened?
3. **Predictive Analysis** → What will happen?
4. **Prescriptive Analysis** → What should we do?

---

##  Steps in Data Analysis

### 1. Problem Understanding

* Define objective clearly
* Identify required data

---

### 2. Data Collection

* Files (CSV, Excel)
* APIs
* Databases

---

### 3. Data Cleaning

* Handle missing values
* Remove duplicates
* Fix inconsistent data

---

### 4. Exploratory Data Analysis (EDA)

* Summary statistics
* Data distribution
* Relationship analysis

---

### 5. Data Transformation

* Feature engineering
* Encoding
* Scaling

---

### 6. Data Visualization

* Bar charts
* Line charts
* Histograms
* Scatter plots

---

### 7. Insights & Reporting

* Identify patterns
* Draw conclusions
* Make decisions

---

##  Example Code (Basic Analysis)

```python
import pandas as pd

# Load dataset
df = pd.read_csv("data.csv")

# Basic understanding
print(df.head())
print(df.shape)
print(df.columns)

# Info
print(df.info())

# Summary
print(df.describe())

# Missing values
print(df.isnull().sum())
```

---

## Visualization Example

```python
import matplotlib.pyplot as plt

# Histogram
df['Age'].hist()
plt.title("Age Distribution")
plt.xlabel("Age")
plt.ylabel("Frequency")
plt.show()
```

---

## 🔹 Important Concepts

### 1. Mean, Median, Mode

* Mean → Average
* Median → Middle value
* Mode → Most frequent value

---

### 2. Standard Deviation

* Measures spread of data

---

### 3. Correlation

* Shows relationship between variables
* Value ranges from -1 to 1

---

##  Importance of Data Analysis

* Helps in business decisions
* Identifies trends
* Improves performance
* Supports machine learning

---

##  Key Takeaways

* Always understand data before modeling
* EDA is the most critical step
* Visualization simplifies complex data
* Clean data leads to better insights
