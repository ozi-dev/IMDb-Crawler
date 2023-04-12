# Web Scraping IMDb Movie Comments

This Python code scrapes movie reviews and ratings from the IMDb website using Scrapy and Selenium libraries. The scraped data is stored in a SQLite database.

## Installation

Clone or download the repository to your local machine.

Install the required dependencies using the following command in your terminal:
    
    !pip install -r requirements.txt


**Note:** chromium-chromedriver package should be installed using your system's package manager. If you're using Ubuntu, you can install it using the following command:

    sudo apt install chromium-chromedriver

Create a SQLite database by providing a path and name for the database file. In the code provided, the database is named SQLITE DB. Make sure to modify the name and path of the database to suit your needs.

Create a table in the database to store the scraped data. In the code provided, the table is named yourTableName and has two columns: rating (integer) and review (text). You can modify the table name and columns to suit your needs.

Set the url variable to the IMDb movie comments page URL you want to scrape.

Run the code using the following command in your terminal:

    python imdb_scraper.py

## Usage

When you run the code, it will perform the following steps:

    Start a headless Chrome browser and navigate to the provided URL.

    Scroll down the page and click on the "Load More" button until all the reviews are displayed.

    Scrape the ratings and reviews of each comment and insert them into the SQLite database.

    Print out the scraped data from the database.

If there are any errors while scraping the comments, the URL and error message will be added to two separate lists (error_url_list and error_msg_list) and the program will continue to scrape the remaining comments.
Dependencies

This code requires the following dependencies to be installed:

- sqlite3
- scrapy
- selenium
- numpy
- tqdm

Make sure to install these dependencies before running the code.

### Contributing

Contributions are welcome! If you find any bugs or want to suggest new features, please create an issue or a pull request.

If you have any questions or suggestions, please contact the author Oğuzhan Öztürk at oguzhanozturk0@outlook.com.
