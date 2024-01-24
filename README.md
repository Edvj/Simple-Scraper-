*** Simple web scraper for e-commerce stores ***

=============================================
#About
This script can get required info from webshops such as Product titles, prices, delivery options and so on..
The script works with only HTML webpages, webpages developed Javascript requires more complex tools.
The script is written in Python and uses the requests library to fetch web pages and BeautifulSoup from bs4 for parsing HTML content. 
=============================================
#Requirements 
Please check Requirements.txt if you use Pycharm IDE please add this file to the script files directory to start automatic install of needed packages and libraries.
=============================================
#Instructions
Clone or download this repository to your local machine.
Install the required Python packages:
"--pip install requests beautifulsoup4--"
Ensure you have the config.ini file in the same directory as the script with appropriate configurations set.
=============================================
Please Edit the config.ini file to set the parameters for web scraping:

[scraping]
url: <-- "url address of scraping page"
"change those of your scraping page content (right click - press inscpect - copy selector)"

product_item_selector: div.product-item <-- insert here
title_selector: a.product-title <-- insert here
price_selector: div.product-price <-- insert here
wait_time: 0 <-- default (0); "change for your needs"
max_pages: 15 <-- "change for your needs"

[output]
log_to_console: yes <-- "on or off"
output_file: scraped_data.json <-- default
[logging]
log_file: scraping_log.log <-- default
=============================================
Start run the script and check log file for info if script works you will get message:
"Successfully retrieved the webpage" if not please check for the errors in log file.
Most cases do not work css selectors. Please check those.
=============================================
** Developed by Edvj CodeAcademy project 2024 **
