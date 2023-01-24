# Web Scraping - Scraping Car Data

This script is used to scrape car data from a website and save the data to a CSV file. The script uses the Python library requests to send GET requests to the website, BeautifulSoup to parse the HTML content, and csv to write the data to a file.

## Required Libraries

* requests
* beautifulsoup4
* csv
* random

## How it works

1. The script starts by initializing empty lists to store the scraped data.
2. A for loop is used to iterate through a range of item codes, where each item code represents a specific car.
3. For each item code, the script generates a random item code within a specific range and creates the URL for each item.
4. The script then sends a GET request to the URL and parses the HTML content using BeautifulSoup.
5. The script uses the find() and find_all() methods to search for specific elements in the HTML content and extract the relevant data.
6. The scraped data is then appended to the appropriate lists.
7. The script then extracts the year, brand, and transmission from the data and saves it to new lists.
8. Finally, the script writes the scraped data to a CSV file using the csv library.

## Notes

The script uses a random number to generate a random item code within a specific range, so the data scraped will be different every time the script is run. Also, the script is configured to scrape data from a specific site, so you need to adjust the script according to the site you want to scrape.
