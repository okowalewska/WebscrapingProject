### Webscraping  - comparison of BeautifulSoup, Selenium and Scrapy
This repository contains three scrapers that get the information about the Top 100 rankings for the last 12 months from the website [Lubimy Czytać]( https://lubimyczytac.pl/top100?page=1&listId=listTop100&month=4&year=2021&paginatorType=Standard)

* To run the BS scraper you need to download the code and run it with python3 from the command line. BS file contains also a simple analysis done on a scraped data.

* To run Selenium scraper you need to download the code and run it with python3 from the command line.

* To run scrapy scraper you need enter a command line and create a scrapy project with the following command:

scrapy startproject myproject [project_dir]

in a directory of your choice. 

Then go to the specified directory with a command:

cd project_dir

Please download the project_scrapy.py file and place it in the folder "spiders" inside the directory from the previous step. There is only a single spider to extract all the information about top 100 books for all the available monhts from the lubimyczytac.pl site. Spiders name is "scrapy_books"

Run the spider with a command 

scrapy crawl scrapy_books

If you want to store the results in a .csv file you can add -o file_name.csv:

scrapy crawl scrapy_books
