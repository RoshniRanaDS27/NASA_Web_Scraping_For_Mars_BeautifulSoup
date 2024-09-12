# NASA on Mars 
(News Articles And Weather data)  
#
![A fun GIF demonstrating an aspect of my project](https://media.giphy.com/media/113mtXIRqf3jfW/giphy.gif)  
#
# Planet : Mars 
![A fun GIF illustrating my project](https://media2.giphy.com/media/uU8ZXJAjwCy8mGSWsw/giphy.gif)  
#
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
#Jupyter Notebook file "part_1_mars_news_Roshni.ipynb"  
have work on this code as followed the steps below to scrape the #Mars News website.  
#

1.Used automated browsing to visit to an external data site link.     
Note that the URL is "https://static.bc-edx.com/data/web/mars_news/index.html"      
Inspected the page to identify which elements to scrape by using chrome DevTools. 
#
![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/4b3de537-bd1c-45d5-a63f-f70d7f3aad79)


  
2.Created a Beautiful Soup object and used it to extract text elements from the website. 
#
![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/b8b60f72-7d6a-46b0-923d-e94a704f5af6)


3.Extracted the titles and previewed text of the news articles that have scraped.  
  Stored the scraping results in Python data structures as follows:


  
4.Stored each title-and-previewed pair in a Python dictionary and, gave each dictionary two keys: title and preview.  
 
 An example is the following:
" {'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm",
 'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously, the result of solar storms that began on Aug. 27."}"
#
 ![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/760b96ee-b8ec-4102-ac02-3f3a3de0b69c)
   
5.Stored all the dictionaries in a Python list. 

6.Printed the list in notebook.   
7.stored the scraped data in a file (to ease sharing the data with others).  
8.exported the scraped data to a JSON file. ("mars_news_data_Roshni.json")

# Part 2: Scrape and Analyze Mars Weather Data
#Jupyter Notebook file "part_2_mars_weather_Roshni.ipynb"  
worked in this code as to follow the steps below to scrape and analyze Mars weather data.
#
1.Used automated browsing to visit the Mars Temperature Data SiteLinks to an external site.    
Inspected the page to identify which elements to scrape.     
Note that the URL is "https://static.bc-edx.com/data/web/mars_facts/temperature.html"
![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/8b9bd926-97f1-4502-9dab-1d53407dc21b)

2.Created a Beautiful Soup object and used it to scrape the data in the HTML table.    
this can also be achieved by using the Pandas "read_html" function.   
However, used Beautiful Soup here to continue sharpening web scraping skills.

3.Assembled the scraped data into a Pandas DataFrame.  
The columns have the same headings as the table on the website.  

Here’s an explanation of the column headings:
#
>id:> 'the identification number of a single transmission from the Curiosity rover'    
>terrestrial_date:> 'the date on Earth'    
>sol:> 'the number of elapsed sols (Martian days) since Curiosity landed on Mars'    
>ls:> 'the solar longitude'    
>month:> 'the Martian month'      
>min_temp:> 'the minimum temperature, in Celsius, of a single Martian day (sol)'    
>pressure:> 'The atmospheric pressure at Curiosity's location'    
#
![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/108e3ca7-1504-489d-8d6f-c3852cff8c61)
#
![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/32cf2be3-0973-40b3-8669-1e402b2db5de)

4.Examined the data types that were currently associated with each column.   
Necessarily, casted (or converted) the data to the appropriate datetime, int, or float data types.  
![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/d39ba97b-7bb2-4a3a-b1ca-24d1f3861a1f)
#
![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/19451adb-1877-4a98-bbfe-a54c64924958)


5.Analyzed dataset by using Pandas functions to answer the following questions:
#
a.How many months exist on Mars?  
![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/79616c18-7502-43dd-86f8-c026819507ba)

b.How many Martian (and not Earth) days worth of data exist in the scraped dataset?    
![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/1a65ad52-44c5-4d2b-a9aa-5fa4a8f9f44c)

c.The coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:  
![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/b799660a-15aa-4ae7-8fb0-6227ddfd70ab)

d.The average minimum daily temperature for all of the months.  
![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/9da34ce1-69ee-4efe-bfc1-e65010495c80)



e.Ploted the results as a bar chart.  

![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/c60af978-0c2f-465c-87bb-f3e1e44bf0c8)

f.Which months have the lowest and the highest atmospheric pressure on Mars?  
To answer this question:  
![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/1c64f449-f802-488b-bdef-d37aba7f72e9)

    1.Found the average daily atmospheric pressure of all the months.    
    2.Ploted the results as a bar chart.  
![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/f6eeab2a-a6ef-4140-a529-d15f102dfe5d)
![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/3ef48d72-2939-4c6a-bbe8-1d0c79e83613)


g.How many terrestrial (Earth) days exist in a Martian year?  
![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/87782790-0e4e-49e5-ba99-6e86205a0ab9)

To answer this question:  
    1.Considered how many days elapse on Earth in the time that Mars circles the Sun once.  
![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/4dc44f50-9488-4053-9215-fef5d5a30807)

    2.Visually estimated the result by plotting the daily minimum temperature.  
![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/40274552-c57b-4c60-9d0d-1c7ea54be99f)
![image](https://github.com/RoshniRanaDS/NASA_Web_Scraping_For_Mars_BeautifulSoup/assets/161755928/1f277df2-a523-4fd9-b3ae-abf34995b670)

    
h.Exported the DataFrame to a CSV file. "mars_weather_data_Roshni.csv"
