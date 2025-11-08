# Web Scraping Project – Extracting Car Details from Cars24

## **Project Overview**

This project focuses on building an automated web scraping system to extract used car details from the **Cars24** website. The goal is to collect structured information such as car model, year, kilometers driven, fuel type, transmission, and price, and store it in a clean CSV file.

The project provides a complete pipeline: scraping → cleaning → exporting → documenting the analysis. It is suitable for beginners learning Python, Selenium/BeautifulSoup, data processing, and end-to-end mini-project workflow.

---

## ✅ **Objective**

To scrape structured car information from Cars24, clean the extracted data, and present it in a usable CSV format, along with a documented Jupyter notebook, project report, and presentation.

---

## ✅ **Technologies Used**

* **Python 3.x**
* **Selenium** (Dynamic website scraping)
* **BeautifulSoup4** (Optional HTML parsing)
* **Pandas** (Cleaning & exporting CSV)
* **Jupyter Notebook** (Documentation)
* **ChromeDriver / WebDriver Manager**
* **Matplotlib / Seaborn** (Optional visualizations)

---

## ✅ **Project Workflow**

1. **Check robots.txt legality**
2. **Inspect website structure**
3. **Automate browser using Selenium**
4. **Extract required car attributes**
5. **Clean and preprocess extracted data**
6. **Export to CSV**
7. **Create Jupyter documentation**
8. **Create PDF report & presentation**

---

## ✅ **Folder Structure**

```
Cars24_WebScraping_Project/
│
├── notebooks/
│   └── cars24_scraping_documentation.ipynb
│
├── src/
│   ├── scraper.py
│   ├── parser.py
│   └── utils.py
│
├── output/
│   ├── cars24_data.csv
│   └── clean_data.csv
│
├── reports/
│   ├── presentation.pdf
│   └── project_report.pdf
│
├── requirements.txt
└── README.md
```

---

# ✅ **Step-by-Step Breakdown**

## **Step 1: Checking robots.txt**

Before scraping, check Cars24’s robots.txt page to ensure compliance with scraping policies.

You must verify:

* Allowed/disallowed paths
* Rate limiting

---

## **Step 2: Understanding the Website Structure**

Inspect each car listing using browser Developer Tools.

Extract fields like:

* Car name/model
* Year of manufacture
* Kilometers driven
* Fuel type
* Transmission
* Price

---

## **Step 3: Building the Scraper (Selenium)**

Selenium automates browser actions.

Process:

* Launch the URL
* Scroll/load dynamic content
* Locate elements using XPaths/CSS selectors
* Extract text fields

---

## **Step 4: Parsing and Cleaning Data**

After extraction, clean the data using Pandas:

* Remove extra characters ("km", ",", etc.)
* Convert text to numeric
* Handle missing values
* Ensure data consistency

---

## **Step 5: Exporting Data to CSV**

Save the final structured dataset:

```
output/cars24_data.csv
```

---

## ✅ **Sample Output Columns**

| Model            | Year | KM Driven | Fuel Type | Transmission | Price     |
| ---------------- | ---- | --------- | --------- | ------------ | --------- |
| Maruti Swift VXI | 2019 | 42,000    | Petrol    | Manual       | ₹5,20,000 |

---

## **Step 6: Notebook Documentation**

The Jupyter Notebook includes:

* Code walkthrough
* Explanations
* Visualizations (optional)
* Dataset summary
* Challenges & solutions

---

## **Step 7: Creating Project Report & Presentation**

Include:

* Objective
* Tools used
* Workflow diagram
* Sample output
* Key insights
* Future improvements

---

# ✅ **Key Challenges & Solutions**

### **1. Dynamic Content Loading**

Cars24 uses infinite scroll → **Use Selenium scroll() method** to load all listings.

### **2. Changing HTML structure**

Selectors break often → Use **robust CSS/XPath**.

### **3. Delayed loading**

Use:

```
WebDriverWait(driver, timeout).until(...)
```

### **4. Legal constraints**

Always follow **robots.txt** and fair use.

---

# ✅ **Future Improvements**

* Add more cities and filters
* Add a dashboard (Streamlit/Power BI)
* Add price prediction using ML
* Automate scheduling with CRON/Airflow

---

# ✅ **Conclusion**

This project demonstrates how to:

* Use Selenium to scrape dynamic websites
* Clean and structure real-world data
* Export CSV datasets
* Document and present a complete scraping workflow

The project is an ideal beginner-to-intermediate mini-project showing practical data extraction, cleaning, and reporting skills.

---

# ✅ **Contributors**

* Harsha (Developer)
* Evoastra Ventures (Mentorship)

---

# ✅ **License**

Open-source under MIT License.
