# Amazon Web Scraper

This project is a Python script that scrapes product information from the Amazon website and saves it to a CSV file. It also includes functionality to send an email notification when the price of a specific product drops below a certain level.

## Overview

The goal of this project is to scrape product details from the Amazon website, including the title and price of a specific product. The script uses the BeautifulSoup library to parse the HTML content of the webpage and extract the required information. The extracted data is then stored in a CSV file for further analysis.

## Dependencies

The following Python libraries are used in this project:

- `datetime`: Used to get the current date for timestamping the data.
- `csv`: Used for reading and writing CSV files.
- `time`: Used for setting a time delay between scraping requests.
- `smtplib`: Used for sending email notifications.
- `BeautifulSoup`: Used for parsing HTML content and extracting data.
- `requests`: Used for making HTTP requests to the Amazon website.
- `pandas`: Used for reading the CSV file into a DataFrame for analysis.

## Usage

To use this scraper, follow these steps:

1. Set the `URL` variable to the URL of the product page on Amazon that you want to scrape.
2. Modify the `HEADERS` dictionary with appropriate user agent and connection settings.
3. Set the `FILENAME` variable to the desired name of the CSV file where the data will be stored.
4. Run the script. It will continuously scrape the product information from the Amazon page and append it to the CSV file every 24 hours.
5. To stop the script, you can manually interrupt the execution.

Note: The script includes a placeholder email notification function (`send_mail()`) that can be customized to send an email when the price drops below a certain level. You need to provide your own SMTP server details and authentication credentials to enable email notifications.

## Dataset Information

The dataset saved in the CSV file contains the following fields:

- `Title`: The title of the product.
- `Price`: The price of the product.
- `Date`: The date when the data was collected.

Please ensure that you have the necessary permissions to scrape data from the Amazon website and comply with their terms of service.

Feel free to customize and enhance the script according to your specific needs.

