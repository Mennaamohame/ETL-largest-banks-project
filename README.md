# World's Largest Banks ETL Pipeline

An end-to-end Data Engineering project that automates the extraction, transformation, and loading (ETL) of global bank market capitalization data.

## Project Overview
This Python-based pipeline extracts financial data of the largest banks worldwide from a web source, applies currency conversion based on exchange rates, saves the transformed dataset to a CSV file, and loads it into a local SQLite database for query execution.

## Tech Stack
* **Language:** Python 3.x
* **Data Processing:** Pandas, NumPy
* **Web Scraping:** BeautifulSoup4, Requests
* **Database:** SQLite3
* **Logging & Tracking:** Custom Python logging mechanism

## ETL Process Workflow
1. **Extraction:** Scrapes bank names and market capitalization data (in USD billions) from the web source.
2. **Transformation:** Converts market cap values from USD to GBP, EUR, and INR using current exchange rate rates and rounds output values.
3. **Loading:** 
   * Saves the final dataset to `Largest_banks_data.csv`.
   * Loads data into an SQLite table named `Largest_banks` in `World_Economies.db`.
4. **Automated Logging:** Logs every step with timestamps into `code_log.txt`.

## How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/Mennaamohame/etl-largest-banks-project.git](https://github.com/Mennaamohame/etl-largest-banks-project.git)
