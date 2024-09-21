# Scraping Financial Data

## Overview

This Project automates the process of collecting financial data from two popular websites: [screener.in](https://www.screener.in) and [nseindia.com](https://www.nseindia.com). It uses web scraping techniques to gather information on various companies and stores it into easily accessible files.

![image](https://www.billdu.com/wp-content/uploads/2021/03/Financial-data-analytics-for-SMBs.png)

This notebook is a great starting point for anyone interested in financial data analysis or building their own web scraping applications.

---

## What it Does

- **Scrapes data from Screener.in:** Extracts financial metrics like market cap, price-to-earnings ratio, and book value for a list of companies.
- **Scrapes data from NSE India:** Collects stock data including 52-week highs and lows, volatility measures, and other relevant information.
- **Organizes data into spreadsheets:** Saves the collected data as CSV files, making it easy to analyze and use in other applications.

---

## Key Features

- **Automated web browsing:** Uses Selenium to control a web browser (like Chrome) and navigate to the target websites.
- **Data extraction:** Employs BeautifulSoup to parse the HTML content of the websites and extract the desired data.
- **Data cleaning and formatting:** Cleans the extracted data and prepares it for storage in a structured format.
- **Efficient and reliable:** Handles potential errors and ensures accurate data collection.

---

## How to Use

1. Install the required libraries: `pip install selenium pandas beautifulsoup4 numpy` which is also the first line in the code.
2. Run the Jupyter Notebook file [data.ipynb](data.ipynb).
3. The scraped data will be saved as CSV files in the same directory as the notebook.

---

## Benefits

- **Saves time and effort:** Automates the tedious process of manually collecting data from multiple websites.
- **Provides comprehensive data:** Gathers a wide range of financial metrics for analysis.
- **Easy to use:** Simple and straightforward code with clear explanations.
- **Customizable:** Can be easily modified to scrape data from other websites or extract different information.

---

## Installation

To run the project locally, open up the code editor of your choice and move to the terminal. Then follow the instructions below:-

Clone the repository:

```python
git clone https://github.com/dakshbhatnagar/projects/scraping.git
```

Switch to the directory:

```python
cd scraping
```

You can now start browsing files and exploring data locally on your machine.

--

*Thanks for stopping by and happy analysing*


