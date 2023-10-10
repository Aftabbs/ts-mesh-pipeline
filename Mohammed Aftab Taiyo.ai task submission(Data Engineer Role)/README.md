# Taiyo.ai Data Engineer Web Scraper Task

This project is a solution to a technical assessment task provided by Taiyo.ai for a Data Engineer web scraper role. The task involved creating a web scraper to gather data from specific websites, producing the output in CSV format. The assessment criteria include the quality of the data output and the code's optimization for handling large amounts of data.

## Websites Scraped

- [NASA Earth Data](https://www.earthdata.nasa.gov/engage/open-data-services-and-software/api)

## Libraries Used

The following Python libraries were used in this project and their purposes:

- `requests`: Used for making HTTP requests to fetch data from web APIs.
- `json`: Used for parsing JSON data obtained from the News API.
- `pandas`: Used for data manipulation and creating a structured DataFrame.
- `time`: Used for introducing delays during web scraping.
- `selenium`: Used for web scraping and interaction with web pages.
- `beautifulsoup4`: Used for parsing HTML content from web pages.

## Techniques Used

### 1. Weather API Class

A Weather API class was created to access the News API and retrieve news articles based on a keyword. This class is responsible for making API calls, parsing the JSON response, and creating a DataFrame of news articles. It uses the News API key for authentication.

### 2. Web Scraper Class

A web scraper class was implemented to extract data from the NASA Earth Data website. The class utilizes the Selenium WebDriver to automate interactions with the website. Key steps include:

- Navigating to the website.
- Scrolling down to load content.
- Extracting data by parsing the HTML content with BeautifulSoup.
- Segregating the data into fields such as source, author, title, description, etc.
- Creating a DataFrame from the extracted data.
- Saving the DataFrame to a CSV file.
- 
### Snippets 
![image](https://github.com/Aftabbs/WebScraper-APIIntegration/assets/112916888/2bae5ba1-2183-443c-83f7-4d9d004b219d)

![image](https://github.com/Aftabbs/WebScraper-APIIntegration/assets/112916888/d74b7865-e24d-4945-9b8a-cbeecef00cc8)


## Usage

1. **Weather API Class**: This class can be used to fetch news articles based on a keyword. Simply create an instance of the `Weather_API` class, provide the keyword, and call the `news_api()` method.
2. **Web Scraper Class**: The Web_Scraping class is used to scrape data from specific websites. To use it, create an instance of the class, provide the desired location, and call the selenium_webdriver() method

You can further customize this README.md file by adding any additional details or sections specific to your project.
