#  Exploratory Data Analysis (EDA)

##  Objective

To deeply understand the dataset by analyzing its structure, patterns, and relationships.

---

##  Step 1: Import Libraries

```python
import pandas as pd
import matplotlib.pyplot as plt
```

---

##  Step 2: Load Dataset

```python
df = pd.read_csv("data.csv")
```

---

##  Step 3: Initial Exploration

```python
print(df.head())        # First 5 rows
print(df.tail())        # Last 5 rows
print(df.shape)         # Rows & columns
print(df.columns)       # Column names
```

---

##  Step 4: Dataset Information

```python
print(df.info())
```

 Helps to check:

* Data types
* Missing values

---

##  Step 5: Missing Values

```python
print(df.isnull().sum())
```

Handling:

```python
df['Age'] = df['Age'].fillna(df['Age'].mean())
```

---

##  Step 6: Summary Statistics

```python
print(df.describe())
```

 Gives:

* Mean
* Min, Max
* Standard deviation

---

##  Step 7: Check Duplicates

```python
print(df.duplicated().sum())

df = df.drop_duplicates()
```

---

##  Step 8: Distribution Analysis

```python
df['Age'].hist()
plt.title("Age Distribution")
plt.show()
```

---

##  Step 9: Correlation Analysis

```python
print(df.corr())
```

 Helps find relationships between variables

---

##  Step 10: Outlier Detection

```python
df = df[df['Age'] < 100]
```

---

##  Step 11: Grouping Data

```python
print(df.groupby('Name')['Salary'].mean())
```

---

##  Key Points

* Always start with understanding data
* Check missing values and duplicates
* Use visualization to identify patterns
* Correlation helps in feature selection
