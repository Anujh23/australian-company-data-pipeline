#Australian Company Data Pipeline

This project builds a simple data pipeline to combine business information from **Common Crawl** and **ABR (Australian Business Register)** using **Python, PySpark, and PostgreSQL**.

---

##What This Project Does

- Gets 200,000+ Australian company websites from **Common Crawl**
- Extracts official company info from **ABR XML files**
- Cleans, joins, and stores both datasets in a **PostgreSQL** database
- Uses **Apache Spark** to process big data
- Checks data quality with basic tests

---

##Data Sources

1. **Common Crawl**  
   - URL, company name, and industry (if available)  
   - Data from March 2025 index

2. **ABR (https://data.gov.au/)**  
   - ABN, entity name/type/status  
   - Address, postcode, state, and start date  

---

##Tools Used

- Python 🐍
- Apache Spark ⚡
- PostgreSQL 🐘
- Jupyter Notebooks 📓
- BeautifulSoup & Requests (for scraping)

---



