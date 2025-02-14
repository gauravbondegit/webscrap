# webscrap
# Web Scraping Loan Service Providers using BeautifulSoup

This project is a web scraping script that extracts details of loan service providers from the Indian Yellow Pages website using Python, the requests library, and BeautifulSoup for parsing HTML. The extracted data is then stored in an Excel file using the pandas library.

*Input :-*

The script prompts the user to enter the name of a city.
It dynamically constructs the URL to scrape loan service provider data from the Indian Yellow Pages website for the specified city.
*Output :-*

If the request is successful(HTTP Status Code= 200), the script extracts the following details for each listed loan service provider:
Title (Company Name), Link (Company Profile URL), Address, Rating.

The extracted data is saved in an Excel file named loan_service_providers_.xlsx

If the request fails, an error message with the HTTP status code is displayed.(e.g. 403)

*Target Website :-* https://www.indianyellowpages.com/

How to Run the Script

Install the required Python libraries:

pip install requests beautifulsoup4 pandas

Run the script:

python script.py

Enter the desired city name when prompted.

The extracted data will be saved in an Excel file in the same directory as the script.
Enter the city name: Mumbai
Data saved to loan_service_providers_Mumbai.xlsx
