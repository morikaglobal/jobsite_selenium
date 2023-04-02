#  jobsite web scraper - Python with selenium

## About this notebook

Automation of web job search and scraping searched job details on jobsite with Python and selenium on Google colaboratory

![About this notebook](images/jobsite.png)
    
In this <a href="https://github.com/morikaglobal/jobsite_selenium/blob/master/Jobsite%20Selenium.ipynb" target="_blank">notebook</a>, I will automate job search query and scrape the data of search results on jobsite using Python and selenium, and store the scraped then processed data in a csv file.

jobsite link: https://www.jobsite.co.uk

For each listed job, following fields are scraped:
- job title
- company
- location
- salary
- job description

In my code, I will automate and scrape job search with following set of entries as an example, however the code works with other sets of search entries as well:

- job title to search - 'Software Engineer'
- location - 'Manchester'
- radius - 'within 30 miles' (select from dropdown selection)

![About this notebook](images/search.png)

On the website, at the time of web scraping in April 2023, the searched results looked something like this: <a href="https://github.com/morikaglobal/jobsite_selenium/blob/master/images/JobsitePageLong.png" target="_blank">Search results page on jobsite</a> 

![About this notebook](images/jobs_no.png)

552 jobs found as the result of my search, however there is a message:

<b>"We have extended your search with 652 more results from outside the region"</b>

I only want to scrape the data of first 552 jobs but if I scrape all results I will end up with additional data of 652 jobs that I do not need, meaning I will scrape up to the very last page of 49, when all I need to scrape is up to page 23.

![About this notebook](images/pages.png)

Therefore, in my code I find out how many pages I need to scrape according to the number of jobs found by the search query made and divide the number by 25 (the number of jobs listed per page) so that I will only scrape the pages I need for speed and efficiency.

## Final output

![About this notebook](images/csv_view.png)

Using my scraping code, data is scraped, necessary data processing done and the data gets stored in CSV file like this: <a href="https://github.com/morikaglobal/jobsite_selenium/blob/master/Jobsite.csv" target="_blank">jobsite search result (CSV file)</a>

