# NASA on Mars 
(News Articles And Weather data)

# Web-Scraping and Data Analysis

This data analysis work consists of two technical products. 

Deliverable 1: Scrape titles and preview text from Mars news articles.  
Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.

# Background
have learned to identify HTML elements on a page, 
identified their id and class attributes, and used this knowledge to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup.  
Also have learned to scrape various types of information. These include HTML tables and recurring elements, like multiple news articles on a webpage.

As have worked on this, has strengthened the same core skills that i have been developing until now:   
collecting data, organizing and storing data, analyzing data, and then visually communicating insights.

# Instructions
# Part 1: Scrape Titles and Preview Text from Mars News
Jupyter Notebook file "part_1_mars_news.ipynb" 
have work on this code as followed the steps below to scrape the # Mars News website.

Use automated browsing to visit the Mars news siteLinks to an external site.. Inspect the page to identify which elements to scrape.

HINT
Create a Beautiful Soup object and use it to extract text elements from the website.

Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:

Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview. An example is the following:

{'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm",
 'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously, the result of solar storms that began on Aug. 27."}
Store all the dictionaries in a Python list.

Print the list in your notebook.

Optionally, store the scraped data in a file (to ease sharing the data with others). To do so, export the scraped data to a JSON file. (Note: there will be no extra points for completing this.)
