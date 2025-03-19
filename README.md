# Web-Scraping
## Web Scraping with Python


### Overview

This Jupyter Notebook demonstrates how to scrape data from the Wisdom Pet Medicine website using Python. It utilizes the requests library to fetch web pages and extract useful information.

### Features

Fetches website data using requests.

Extracts and processes HTML content.

Retrieves images and displays URLs.

Parses information using BeautifulSoup (if included in the notebook).

### Requirements

Before running the notebook, install the required dependencies:
```bash
pip install requests beautifulsoup4
```
### Usage

Open Webscraping.ipynb in Jupyter Notebook.

Run each cell sequentially to scrape and process data.

Modify the target URL to scrape other websites.

### Example Code Snippet
```bash
import requests
from bs4 import BeautifulSoup
```
# Fetch the webpage
```bash
url = "https://wisdompetmed.com/"
response = requests.get(url)
```

# Parse HTML content
soup = BeautifulSoup(response.text, "html.parser")

# Print page title
```bash
print("Page Title:", soup.title.text)
```
