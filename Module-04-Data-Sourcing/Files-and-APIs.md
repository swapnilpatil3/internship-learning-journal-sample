#  Files and APIs in Data Sourcing

##  Overview

Data sourcing involves collecting data from different sources such as files and APIs.

---

##  1. Files as Data Source

Files are one of the simplest ways to store and access data.

###  Types of Files

* CSV (Comma Separated Values)
* Excel (.xlsx)
* JSON
* XML

###  Example (CSV File)

```python
import pandas as pd

# Read CSV file
df = pd.read_csv("data.csv")

print(df.head())
```

###  Advantages

* Easy to use
* No internet required
* Good for small datasets

---

##  2. APIs as Data Source

API (Application Programming Interface) allows applications to communicate and exchange data. ([Amazon Web Services, Inc.][1])

👉 It acts like a bridge between two systems.

### 🌐 Example:

* Weather apps getting data from weather servers
* Payment apps connecting to banks

---

##  Example (API Call)

```python
import requests

url = "https://api.example.com/data"
response = requests.get(url)

data = response.json()
print(data)
```

---

##  3. Difference Between Files and APIs

| Feature     | Files          | APIs                |
| ----------- | -------------- | ------------------- |
| Data Source | Stored locally | Remote server       |
| Speed       | Fast           | Depends on internet |
| Updates     | Static         | Real-time           |
| Usage       | Simple         | Dynamic data        |

---

##  4. When to Use What?

* Use **files** → when data is small and static
* Use **APIs** → when data is live and dynamic

---

##  Key Takeaways

* Files are simple and offline
* APIs provide real-time data
* Both are important in data sourcing

[1]: https://aws.amazon.com/what-is/api/?utm_source=chatgpt.com "What is an API? - Application Programming Interfaces ..."
