# 📊 Australian Company Data Pipeline

This project builds a simple data pipeline to combine business information from **Common Crawl** and **ABR (Australian Business Register)** using **Python, PySpark, and PostgreSQL**.

---

## 🚀 What This Project Does

- Gets 200,000+ Australian company websites from **Common Crawl**
- Extracts official company info from **ABR XML files**
- Cleans, joins, and stores both datasets in a **PostgreSQL** database
- Uses **Apache Spark** to process big data
- Checks data quality with basic tests

---
##  Architecture

![Firmable-architecture](https://github.com/user-attachments/assets/6d293dd6-6708-4ed0-8bb6-aa422e0f3f76)


## 🧾 Data Sources

1. **Common Crawl**  
   - URL, company name, and industry (if available)  
   - Data from March 2025 index

2. **ABR (https://data.gov.au/)**  
   - ABN, entity name/type/status  
   - Address, postcode, state, and start date  

---

## 🛠️ Tools Used

- Python 🐍
- Apache Spark ⚡
- PostgreSQL 🐘
- Jupyter Notebooks 📓
- dbt (optional for data modeling)
- BeautifulSoup & Requests (for scraping)

---


## 🧱 Project Structure 
- **Extraction**:  
  Microservices or Fabric notebooks for extracting data from websites.

- **Transformation**:
  - **Bronze Layer**: Unzipping ABR XML zip files and storing as CSV.
  - **Gold Layer**: Normalizing and deduplicating data, then joining Common Crawl and ABR datasets.

- **Loading**:
  Final clean data is loaded into the PostgreSQL database.

- **data/**:
  - australian_companies.csv: Sample output of processed data.
  - abr.csv: (Not included due to file size limits)

- **test/**:
  - Scripts and notebooks to validate schema and data integrity.
