## Project Overview
 This project is designed to scrape real estate data from Realtor.com for properties listed in San Francisco, CA. Using Python, the project gathers data on property type, prices, number of beds and baths, and addresses. It then processes and cleans this data to prepare it for further analysis or visualization. The project leverages several web scraping techniques and libraries to collect and process the data efficiently.

## Key Steps and Techniques Used
1. Setting Up Environment and Making Requests:

- Libraries Used: requests, BeautifulSoup, pandas, and numpy.
- Headers: Custom headers are set to mimic a browser request.
- URL Construction: A list of URLs for the first 10 pages of property listings in San Francisco is created.

2. Sending Requests and Parsing HTML:

- Sessions: Using a requests session to handle multiple HTTP requests.
- BeautifulSoup: Parsing the HTML content of each page to extract relevant information.
- Status Code Check: Ensuring requests are successful by checking the status codes.

3. Data Extraction and Structuring:

- DataFrames: Creating pandas DataFrames to hold the extracted data.
- HTML Element Extraction: Using BeautifulSoup to find specific HTML elements containing property details.
- Combining Data: Concatenating data from multiple pages into a single DataFrame.

4. Data Cleaning:

- HTML Tag Removal: Cleaning HTML tags from the extracted text.
- String Manipulation: Formatting address fields and other text data.
- Function for HTML Tag Removal: A custom function to strip HTML tags and format text properly.

## Web Scraping in the Project
Web scraping involves extracting data from websites and converting it into a structured format that can be used for analysis or other purposes. In this project:

- HTTP Requests: The requests library is used to send HTTP requests to the Realtor.com website. Custom headers are included to mimic a real browser and avoid being blocked by the website.
- HTML Parsing: The BeautifulSoup library parses the HTML content of the web pages. It identifies and extracts specific elements such as property type, prices, number of beds and baths, and addresses.
- Pagination: The project handles pagination by constructing URLs for multiple pages of property listings and sending requests for each page.
- Data Extraction: HTML elements containing the required data are identified using tags and attributes. The text content is extracted and cleaned to remove any unwanted HTML tags and formatting.
- Data Structuring: Extracted data is organized into pandas DataFrames, which facilitate further data manipulation, cleaning, and analysis.


## Conclusion
The project efficiently scrapes and processes real estate data from multiple pages on Realtor.com, standardizing and cleaning the extracted data for analysis. It demonstrates the use of various Python libraries for web scraping, data manipulation, and cleaning, making it a useful tool for real estate data analysis. The use of web scraping techniques ensures that the data is collected in an automated and efficient manner, saving time and effort compared to manual data collection.



## Realtor Listings Scraper

A web scraper that extracts real estate listings from realtor.com. Users can filter the results based on location, price range, property type, and other parameters to find their ideal property.

![realtor com](https://github.com/shikhasingh96/realtor_listings_scraper/assets/136284820/e16665e9-18c6-4b97-a7e4-0e88bb6e4eda)
