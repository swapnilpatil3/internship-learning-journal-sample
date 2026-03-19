#  Web Sources in Data Sourcing

##  Overview

Web sources refer to collecting data from websites using techniques like web scraping or public datasets available online.

---

##  1. What are Web Sources?

Web sources are websites that provide data such as:

* News websites
* E-commerce websites
* Government data portals
* Blogs and articles

---

##  2. Web Scraping

Web scraping is the process of extracting data from websites.

 It helps collect large amounts of data automatically.

---

##  Example: Web Scraping using Python

```python id="tsd1np"
import requests
from bs4 import BeautifulSoup

url = "https://example.com"

response = requests.get(url)
soup = BeautifulSoup(response.text, "html.parser")

# Extract all headings
for heading in soup.find_all("h1"):
    print(heading.text)
```

---

##  3. Popular Libraries

* requests → To fetch web pages
* BeautifulSoup → To parse HTML
* Selenium → For dynamic websites

---

##  4. Public Data Sources

Some websites provide free datasets:

* Kaggle
* Government portals
* Open data websites

---

##  5. Advantages

* Access to large datasets
* Real-time information
* Useful for research and analysis

---

##  6. Challenges

* Legal restrictions
* Website blocking (rate limits)
* Data inconsistency

---

##  7. Best Practices

* Always check website terms
* Avoid too many requests
* Use APIs if available instead of scraping

---

##  Key Takeaways

* Web scraping helps collect online data
* Use libraries like requests and BeautifulSoup
* Always follow ethical practices
