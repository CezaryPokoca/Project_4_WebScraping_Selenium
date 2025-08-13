# 🏛 YouGov UK Charity Organization - WebScraping Project

## 📄 Project Overview

This project is performed in **Jupyter Notebook** for portfolio purposes. 
The goal was to extract detailed information on UK charity organizations from YouGov, including their popularity, fame, and public sentiment.
The objective was to automate the collection of structured data from the YouGov website and store it in a JSON format for further analysis or visualization.

---

## 📂 Code Structure

* **`get_browser_firefox()`** – Initializes a Firefox browser instance with GeckoDriver.
* **`get_organization_data(org)`** – Extracts the names and links of the top 20 charity organizations from a ranking page.
* **`get_organization_detailed_data(org)`** – Extracts statistical data for a single charity organization, including fame, popularity, dislike, and neutral metrics.
* **`get_data(org)`** – Iterates over all organizations to scrape both their URLs and detailed statistics.
* **`charity_organizations.json`** – Output JSON file containing the scraped data.

---

## 🛠 Data Collection and Preparation

The following steps were performed to collect and prepare the data:

| Step | Action                          | Description                                                                              |
| ---- | ------------------------------- | ---------------------------------------------------------------------------------------- |
| 1    | **Browser Setup**               | Installed and initialized Firefox browser via Selenium and GeckoDriver Manager.          |
| 2    | **Cookie Handling**             | Automated acceptance of cookie banners on YouGov pages.                                  |
| 3    | **Top Organization Extraction** | Scraped top 20 organizations’ names and profile URLs from ranking pages.                 |
| 4    | **Single Org Data Extraction**  | Extracted detailed metrics (`Fame`, `Popularity`, `Disliked by`, `Neutral`) for one org. |
| 5    | **Full Dataset Extraction**     | Iterated over all organizations to collect both URLs and statistics programmatically.    |
| 6    | **Data Storage**                | Saved the final dataset as `charity_organizations.json` for future analysis.             |
| 7    | **Data Validation**             | Reopened the JSON file to verify completeness and correctness of the stored data.        |

---

## 📊 Analysis & Findings

* Collected a comprehensive dataset of UK charity organizations from YouGov.
* Extracted key metrics for each organization to facilitate comparisons and ranking analysis.
* Enabled future analysis such as trend tracking, sentiment evaluation, and organizational benchmarking.

### 🔍 Additional Insights

#### Top 20 Charities

**Summary:**
The scraping captured the top 20 charity organizations with links to their profile pages, enabling targeted extraction of detailed metrics.

* Key fields: Name, Profile URL, Fame, Popularity, Disliked by, Neutral
* Metrics are normalized as text values; can be converted to numeric for analysis.

**Conclusions:**

* Automated extraction allows for periodic updates of rankings.
* Detailed statistics provide insight into public perception and engagement with charities.

#### Full Dataset

**Summary:**
The complete dataset contains all listed UK charities from YouGov along with their respective metrics.

* The JSON structure is hierarchical, pairing organization names with performance metrics.
* Dataset can be imported into Python, Excel, or Tableau for visualization and deeper insights.

**Conclusions:**

* Dataset is ready for quantitative analysis or dashboard creation.
* Enables trend monitoring, popularity benchmarking, and comparative research.

---

## ✅ Summary & Conclusions

* **Automated Data Collection** – Selenium scripts efficiently gathered large-scale public opinion data.
* **Structured Data Output** – JSON format provides flexibility for further analysis.
* **Actionable Insights Enabled** – Dataset supports charity benchmarking and public sentiment evaluation.
* **Reusable Methodology** – Modular Python functions allow scraping of new categories or updated rankings.

---

## 📎 Files in Repository

* `Project_4_WebScraping_Selenium.ipynb` – Python script with all functions to extract charity organization data.
* `charity_organizations.json` – Final dataset containing all scraped information.
* `README.md` – Project description, methodology, and conclusions (this file).

---

## 💡 Tools Used

* **Python** – Data extraction and processing
* **Selenium** – Browser automation and web scraping
* **Firefox + GeckoDriver** – Browser driver for automated navigation
* **JSON** – Storage format for structured output

---

