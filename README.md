# Twitter Scraper

This project is a Twitter scraper built using Selenium. It logs into Twitter, searches for tweets based on a specified query, and extracts tweets with their metadata. The extracted data is saved in a JSON file.

- [Setup]
 **Configure your credentials and settings:**
   - Open `config.py` and add your Twitter email, username, and password:
     ```python
     EMAIL = "your_email@gmail.com"
     USERNAME = "your_username"
     PASSWORD = "your_password"
     COOKIES_FILE = "twitter_cookies.pkl"
     JSON_FILE = "tweets_data.json"
     CHROMEDRIVER_PATH = 'chromedriver-win64/chromedriver.exe'
     ```
     
## Usage

To run, use the following command:

```sh
python main.py "your_search_query" 10 "latest"
```
Replace "your_search_query", 10, and "latest" with your desired search query, the number of posts to fetch, and the search type (latest or top).

## Files

config.py: Configuration file for storing credentials and paths.
setup.py: Contains the setup for Selenium WebDriver.
auth.py: Handles authentication and cookie management.
scraper.py: Contains the functions to search Twitter and extract tweets.
utils.py: Utility functions for loading and saving data.
main.py: Main script to run the Twitter miner.
