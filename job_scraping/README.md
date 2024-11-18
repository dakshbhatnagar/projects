## Naukri Job Scraper

Welcome to the **Naukri Job Scraper**! This user-friendly Python script is designed to help you effortlessly scrape job listings for **Data Analyst** positions in the Delhi/NCR region from Naukri.com.

![image](https://cdn.prod.website-files.com/65d48bc2b64ae3248b634894/664456d40e4d86aa223b002b_663cc350a3c22ab469f8bac7_JobScrapingMethodsInsightsandAlternatives_1.svg)

The scraped data is organized in a Pandas DataFrame and can be easily exported to both Google Sheets and CSV files for your convenience.

---

## How the Script Works:

1. **Import Libraries:** The script utilizes essential libraries such as Pandas for data manipulation, Selenium for web scraping, and Google API for seamless interaction with Google Sheets.
2. **Set Up WebDriver:** It configures a Chrome WebDriver to access the Naukri.com website efficiently.
3. **Scrape Data:** The script navigates through multiple pages of job listings, extracting key information like job title, company name, required experience, job link, location, and salary.
4. **Store Data:** All scraped data is neatly stored in a Pandas DataFrame for easy access.
5. **Clean Data:** The script automatically removes duplicate entries to ensure data accuracy.
6. **Export Data:** Finally, the DataFrame can be exported to a Google Sheet and a CSV file for your analysis.

This is how the final scraped data would look like:

![image](/job_scraping/image.png)

---

## Installation Instructions

To run this project locally, follow these simple steps:

1. **Clone the Repository:**
   ```python
   git clone https://github.com/dakshbhatnagar/projects/job_scraping.git
   ```

2. **Switch to the Directory:**
   ```python
   cd job_scraping
   ```
Now you're ready to explore the files and data on your local machine!

---

## Using the Script:

1. **Install Requirements:** Run the following command to install the necessary libraries:
   ```bash
   pip3 install -r requirements.txt
   ```
   
2. **Set Up Google API Credentials:** Create a project in Google Cloud, enable billing, obtain a Google API key, and store it in a file named `keys.json`.

3. **Modify Spreadsheet ID:** Replace `'your_sheet_id'` with your actual Google Sheet ID.

4. **Run the Script:** Execute the script to start scraping and exporting the data.

---

## Benefits of Using This Script:

* **Track Job Openings:** Stay updated on the latest Data Analyst job postings in Delhi/NCR.
* **Analyze Job Market Trends:** Gain valuable insights into salary ranges, company hiring patterns, and more.
* **Automate Your Job Search:** Use the scraped data to identify potential job opportunities effortlessly.

**Note:** *This script is intended for educational purposes only. Please respect the terms of service of [Naukri.com](https://www.naukri.com) and other websites you scrape.*
