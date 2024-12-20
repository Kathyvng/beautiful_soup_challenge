# Beautiful Soup Challenge

## Background

In this project, you will conduct a full web-scraping and data analysis project. The challenge will strengthen your skills in identifying HTML elements, using their attributes to extract information, and utilizing Beautiful Soup and Splinter for automated browsing and HTML parsing. You'll scrape and analyze data, then visually communicate your insights.

## Deliverables

This project consists of two main technical deliverables:

1. **Deliverable 1**: Scrape titles and preview text from Mars news articles.  
   - File: `part_1_mars_news.ipynb`

2. **Deliverable 2**: Scrape and analyze Mars weather data from a table.  
   - File: `part_2_mars_weather.ipynb`

---

## Files

Download the starter files to begin the challenge:

- [Module 11 Challenge files](https://bootcampspot.instructure.com/courses/6252/external_tools/313)

---

## Instructions

### Part 1: Scrape Titles and Preview Text from Mars News

1. Open the Jupyter Notebook: `part_1_mars_news.ipynb`.
2. Use automated browsing to visit the [Mars News site](https://redplanetscience.com).
3. Inspect the page to identify which elements to scrape.
   - **Hint**: Create a Beautiful Soup object and extract text elements from the site.
4. Extract the titles and preview text of the news articles:
   - Store the results in a Python dictionary with two keys: `title` and `preview`. Example:
     ```python
     {
         'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm",
         'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously, the result of solar storms that began on Aug. 27."
     }
     ```
   - Append each dictionary to a list.
5. Print the list in your notebook.
6. (Optional) Export the scraped data to a JSON file for sharing.

---

### Part 2: Scrape and Analyze Mars Weather Data

1. Open the Jupyter Notebook: `part_2_mars_weather.ipynb`.
2. Use automated browsing to visit the [Mars Temperature Data Site](https://static.bc-edx.com/data/web/mars_facts/temperature.html).
3. Inspect the page to identify which elements to scrape.
   - **Hint**: Use Beautiful Soup to scrape the HTML table. Avoid using `Pandas.read_html` to practice web scraping.
4. Assemble the data into a Pandas DataFrame with the following columns:
   - `id`: Identification number of a transmission.
   - `terrestrial_date`: Earth date.
   - `sol`: Number of elapsed sols (Martian days) since Curiosity landed.
   - `ls`: Solar longitude.
   - `month`: Martian month.
   - `min_temp`: Minimum temperature (Celsius) on a Martian day.
   - `pressure`: Atmospheric pressure at Curiosity's location.
5. Examine and, if necessary, cast the data types to appropriate formats (e.g., `datetime`, `int`, or `float`).

---

### Data Analysis

Use Pandas to analyze the dataset and answer the following:

1. **How many months exist on Mars?**
2. **How many Martian days (sols) of data are in the dataset?**
3. **What are the coldest and warmest months on Mars?**  
   - Calculate the average minimum daily temperature for each month.  
   - Plot the results in a bar chart.
4. **Which months have the lowest and highest atmospheric pressure on Mars?**  
   - Calculate the average daily atmospheric pressure for each month.  
   - Plot the results in a bar chart.
5. **How many terrestrial days exist in a Martian year?**  
   - Estimate this by visualizing the daily minimum temperature across all observations.

---

### Export Results

Export the final DataFrame to a CSV file for future use: `mars_data.csv`

---

## Notes

- This project involves data scraping, organizing, and analysis using tools such as Beautiful Soup, Splinter, and Pandas.


