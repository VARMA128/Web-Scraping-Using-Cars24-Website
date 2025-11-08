🚗 Web Scraping Car Details – Mini Project

📌 Project Objective:
This mini-project aims to build practical skills in web scraping, data cleaning, and structured data presentation.
Interns will scrape real-world car listing data from Cars24.com, CarDekho.com, or AckoDrive.com and extract key details such as:
Kilometers Driven

Year of Manufacture

Fuel Type

Transmission

Price

By the end of this project, interns will gain hands-on experience in extracting data from dynamic websites, processing it, and exporting it in a clean, analyzable format.

Project Requirements:
1. Scraping Target
Choose one of the following platforms:

Cars24 — https://www.cars24.com/

CarDekho — https://www.cardekho.com/

AckoDrive — https://ackodrive.com/

Scrape car listings for the assigned brand.

2. Data Fields to Collect
For each car listing, extract:

Kilometers Driven

Year of Manufacture

Fuel Type

Transmission Type

Price

Make sure the scraped values are consistent and clean.

🛠️ Steps to Follow
1. Research & Planning:
Study the structure of the website you choose.

Inspect car listing pages using browser DevTools.

Identify HTML elements containing the required fields.

Check whether data loads dynamically (AJAX) or directly.

2. Data Extraction

Write a Python script (or any assigned language) to scrape all required fields.

Use libraries like:

requests

BeautifulSoup

Selenium (if dynamic content)

pandas

Extract details only for the assigned car brand.

3. Data Cleaning:
Remove unwanted characters (e.g., “₹”, “KM”).

Convert numeric fields to proper integer/float formats.

Ensure:

No missing columns

No mixed data types

Consistent formatting

Handle duplicates if present.

4. Data Presentation:
Save the final cleaned dataset in CSV format.

Columns should follow this order:

Brand | Car Name | Year | Kilometers Driven | Fuel Type | Transmission | Price 
