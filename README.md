#  Audible web scraper - Python with selenium

## About this notebook

![About this notebook](images/Audiblebooks.png)
    
Scraping Best Sellers (Top 100) on Audible.com with Python and Selenium on Google colaboratory

In this notebook, I will scrape Best Sellers section on Audible.com using Python and selenium where Top 100 audio books are listed, and store the data in a csv file.

the link to scrape:
https://www.audible.com/adblbestsellers

robots.txt has been checked and the above link is allowed.

For each audio book, following fields are scraped:
- Book title
- Authors
- Narrators
- Length
- Release date
- Language
- Ratings

On the website, Best Sellers section looks like this: <a href="https://covid19-tableau-299208.an.r.appspot.com/tracker" target="_blank">Best Sellers (Top 100) on Audible.com</a>

![About this notebook](images/csv_view.png)

Using my scraping code, data is scraped, necessary data processing done and top 100 Audible audio books are stored in CSV file like this: <a href="https://covid19-tableau-299208.an.r.appspot.com/tracker" target="_blank">Top 100 Audible audio books (CSV file)</a>

For more details on how the application was built, 
please take a look at the notes on the <a href="https://covid19-tableau-299208.an.r.appspot.com/tracker" target="_blank">application website</a>
