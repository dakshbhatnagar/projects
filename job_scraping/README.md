## Naukri Job Scraper

This Python script scrapes job listings from the Naukri.com website for Data Analyst positions in Delhi/NCR. It then stores the scraped data in a Pandas DataFrame and exports it to a Google Sheet and a CSV file.

![image](https://cdn.prod.website-files.com/65d48bc2b64ae3248b634894/664456d40e4d86aa223b002b_663cc350a3c22ab469f8bac7_JobScrapingMethodsInsightsandAlternatives_1.svg)

---

**Here's how it works:**

1. **Import Libraries:** The script imports necessary libraries like Pandas for data manipulation, Selenium for web scraping, and Google API for interacting with Google Sheets.
2. **Set Up WebDriver:** It configures a Chrome WebDriver to access the Naukri.com website.
3. **Scrape Data:** The script iterates through multiple pages of job listings, extracting information like job title, company name, experience required, job link, location, and salary.
4. **Store Data:** The scraped data is stored in a Pandas DataFrame.
5. **Clean Data:** Duplicate entries are removed from the DataFrame.
6. **Export Data:** The DataFrame is exported to a Google Sheet and a CSV file.

This is how the final scraped data would look like:-

![image](/job_scraping/image.png)

---

**Installation**

To run the project locally, open up the code editor of your choice and move to the terminal. Then follow the instructions below:-

Clone the repository:

```python
git clone https://github.com/dakshbhatnagar/projects/job_scraping.git
```

Switch to the directory:

```python
cd job_scraping
```

You can now start browsing files and exploring data locally on your machine.

**To use this script:**

1. **Install Requirements:** Run `pip3 install -r requirements.txt` command to install the necessary libraries.
2. **Set Up Google API Credentials:** Obtain a Google API key and store it in a file named `keys.json`.
3. **Modify Spreadsheet ID:** Replace `'your_sheet_id'` with your Google Sheet ID.
4. **Run the Script:** Execute the script to scrape and export the data.

---

**Benefits of Script:**

* **Track job openings:** Monitor the latest Data Analyst job postings in Delhi/NCR.
* **Analyze job market trends:** Gain insights into salary ranges, company hiring patterns, and other relevant data.
* **Automate job search:** Use the scraped data to identify potential job opportunities.

**Note:** *This script is for educational purposes only. Please respect the terms of service of Naukri.com and other websites you scrape.*
