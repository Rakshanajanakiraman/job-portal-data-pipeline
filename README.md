# Job Portal Data Pipeline

An end-to-end **Python data pipeline project** that scrapes job listings from a live website, integrates them with a Kaggle dataset, cleans and merges the data, and uploads the final result to **Google Sheets**.

This project demonstrates real-world skills in **web scraping, data cleaning, logging, API integration, and automation**.

---

##  Project Overview

The pipeline performs the following steps:

1. Scrapes Python job listings from `pythonjobs.github.io`
2. Loads a Kaggle job dataset from CSV
3. Cleans and standardizes column names
4. Safely merges both datasets
5. Exports cleaned data to CSV files
6. Uploads the merged dataset to Google Sheets
7. Logs each step for traceability and debugging

---

##  Technologies Used

- Python 3
- Requests
- BeautifulSoup
- Pandas
- Logging
- Google Sheets API
- gspread
- OAuth2 Service Account

---

##  Project Structure

```text
job-portal-data-pipeline/
│
├── scraper.py
├── README.md
├── requirements.txt
├── .gitignore
│
├── data/
│   ├── Scraped_Jobs.csv
│   ├── Kaggle_Cleaned.csv
│   └── Merged_Job_Data.csv
│
├── logs/
│   └── scraper.log
│
└── credentials/
    └── service_account.json   # ignored by git
