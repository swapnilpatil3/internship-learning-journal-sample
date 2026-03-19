#  Data Transformation

##  Objective

Convert raw data into a format suitable for machine learning.

---

##  1. Encoding Categorical Data

### Label Encoding

```python
from sklearn.preprocessing import LabelEncoder

le = LabelEncoder()
df['Name'] = le.fit_transform(df['Name'])
```

---

### One-Hot Encoding

```python
df = pd.get_dummies(df, columns=['Name'])
```

---

##  2. Normalization (Min-Max Scaling)

```python
from sklearn.preprocessing import MinMaxScaler

scaler = MinMaxScaler()
df[['Age', 'Salary']] = scaler.fit_transform(df[['Age', 'Salary']])
```

---

##  3. Standardization (Z-score)

```python
from sklearn.preprocessing import StandardScaler

scaler = StandardScaler()
df[['Age', 'Salary']] = scaler.fit_transform(df[['Age', 'Salary']])
```

---

##  4. Feature Engineering

```python
# Create new feature
df['Age_Group'] = df['Age'] // 10
```

---

##  5. Feature Selection

```python
# Select specific columns
df = df[['Age', 'Salary']]
```

---

##  6. Splitting Data

```python
from sklearn.model_selection import train_test_split

X = df.drop('Salary', axis=1)
y = df['Salary']

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)
```

---

##  Final Output

Transformed dataset ready for machine learning.

---

## 🚀 Key Points

* Encoding is required for categorical data
* Scaling improves model performance
* Feature selection reduces complexity
