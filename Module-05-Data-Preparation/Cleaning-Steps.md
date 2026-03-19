#  Data Cleaning Steps

##  Objective

To clean raw data and make it ready for analysis.

---

##  Step 1: Load Dataset

```python
import pandas as pd

df = pd.read_csv("sample.csv")
print(df.head())
```

---

##  Step 2: Check Basic Info

```python
print(df.info())
print(df.describe())
```

---

##  Step 3: Handle Missing Values

```python
# Check missing values
print(df.isnull().sum())

# Fill missing values with mean
df['Age'] = df['Age'].fillna(df['Age'].mean())
```

---

##  Step 4: Remove Duplicates

```python
df = df.drop_duplicates()
```

---

##  Step 5: Handle Outliers (Basic)

```python
# Example: Removing values greater than threshold
df = df[df['Age'] < 100]
```

---

##  Step 6: Fix Data Types

```python
df['Age'] = df['Age'].astype(int)
```

---

##  Step 7: Rename Columns (Optional)

```python
df.columns = ['Name', 'Age', 'Salary']
```

---

##  Step 8: Save Cleaned Data

```python
df.to_csv("cleaned_data.csv", index=False)
```

---

##  Final Output

Clean dataset ready for analysis or ML.

---

##  Key Points

* Always check missing values
* Remove duplicates carefully
* Validate data before saving
