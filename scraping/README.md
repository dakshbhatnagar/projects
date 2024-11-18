# Scraping Financial Data

## Background and Overview

This project automates the process of collecting financial data from two popular websites: [screener.in](https://www.screener.in) and [nseindia.com](https://www.nseindia.com). By leveraging web scraping techniques, it gathers essential information on various companies and stores it in easily accessible files. This tool is particularly beneficial for finance professionals, analysts, and investors who require timely and accurate data for informed decision-making.

![image](https://www.billdu.com/wp-content/uploads/2021/03/Financial-data-analytics-for-SMBs.png)

---

## Data Structure Overview

The collected data is organized into structured CSV files, which include key financial metrics such as:
- Market Capitalization
- Price-to-Earnings Ratio
- Book Value
- 52-Week Highs and Lows
- Volatility Measures

This structured format allows for easy analysis and integration into financial models or reports.

---

## Executive Summary

This project serves as a comprehensive solution for automating the collection of financial data, significantly reducing the time and effort required for manual data entry. 

By providing a reliable and efficient way to gather data, it empowers users to focus on analysis and strategic decision-making.

---

## Insights and Takeaways

- **Automated Data Collection:** The use of Selenium for automated web browsing ensures that users can gather data without manual intervention, saving valuable time.
- **Data Extraction and Cleaning:** BeautifulSoup is employed to parse HTML content, ensuring that the extracted data is relevant and accurate. The cleaning process prepares the data for structured storage, which is crucial for analysis.
- **Error Handling:** The project includes mechanisms to handle potential errors during data collection, ensuring that users receive accurate and reliable data.

---

## Recommendations

- **Customization:** Users are encouraged to modify the scraping logic to include additional websites or specific data points that are relevant to their analysis needs.
- **Integration with Analytical Tools:** The CSV files generated can be easily integrated into various analytical tools or software, enhancing the overall data analysis process.
- **Regular Updates:** To maintain the relevance of the data, it is recommended to run the scraping process regularly maybe using a YAML file in your project and use GitHub Actions to automate this, especially for dynamic financial metrics.

---

## How to Use

1. Install the required libraries: `pip install -r requirements.txt` which is also the first line in the code.
2. Run the Jupyter Notebook file [data.ipynb](data.ipynb).
3. The scraped data will be saved as CSV files in the same directory as the notebook, ready for analysis or integration into financial models.

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