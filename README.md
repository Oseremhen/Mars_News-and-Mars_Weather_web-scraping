# Mars News and Mars Weather
Scrape titles and preview text from Mars news articles. Scrape and analyze Mars weather data, which exists in a table.

![header](https://user-images.githubusercontent.com/106120403/213423822-6079197f-8f26-4e4b-ad72-8d8ec6bad526.jpg)

- Deliverable 1: Scrape titles and preview text from Mars news articles.
- Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.

Inspected https://static.bc-edx.com/data/web/mars_news/index.html to identify which elements to scrape.
I created a Beautiful Soup object and used it to extract text elements from the website.
Extracted the titles and preview text of the news articles that I scraped. Stored the scraping results in Python data structures.


Used automated browsing to visit the (https://static.bc-edx.com/data/web/mars_facts/temperature.html) and inspected the page to identify which elements to scrape
I created a Beautiful Soup object and used it to scrape the data in the HTML table. I assembled the scraped data into a Pandas DataFrame.
I examined the data types that are currently associated with each column and converted the data to the appropriate datetime, int, or float data types.

Analysis - 

I analyzed my dataset by using Pandas functions to answer the following questions:
1. How many months exist on Mars?
2. How many Martian (and not Earth) days worth of data exist in the scraped dataset?
3. What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
I found the average minimum daily temperature for all of the months and created a plot for the results as a bar chart.

![avg_min_temp](https://user-images.githubusercontent.com/106120403/213426274-45495af8-5c2a-4a34-b06b-ca137860a89e.png)

4. Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
I found the average daily atmospheric pressure of all the months and created a plot for the results as a bar chart.

![avg_pressure](https://user-images.githubusercontent.com/106120403/213426378-39adc7dd-9156-445d-b5ac-6f58d4506a34.png)

5. About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
I considered how many days elapse on Earth in the time that Mars circles the Sun once and used a plot to visually estimate the result by plotting the daily minimum temperature.

![daily_mim_temp](https://user-images.githubusercontent.com/106120403/213426568-b68f5bd8-6a08-413c-b3d5-b006936d2f7a.png)

I exported the DataFrame to a CSV file that can be found in the starter_code folder.
