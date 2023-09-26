# 4th_wave_cantek #Web Sraping Project

**Topic of the Project:** Analysing the largest revenue generators in the United States. 

**Project Overview:** This project is about web scraping a webpage ('https://en.wikipedia.org/wiki/List_of_largest_companies_in_the_United_States_by_revenue') to analyse the different revenue generators in the United States.  

# Steps involved are:
For the analysis, first, we import the required files: pandas, matplotlib.pyplot, BeautifulSoup, requests.
A particular table is extracted from the webpage and then its contents in rows/columns using the function 'find_all()' and 'for' loop. Since the webpage has more than one table so the position of the table to be scraped is also reuired to be mentioned. The headrers in the table are also displayed verifying the table we need. 
Using pandas, a DataFrame has been created with the data extracted from the table in terms of rows and columns. The heading of the columns in the DataFrame would be the same as the titles of the extacted table. This Dataframe contains 100 rows and 7 columns. So, extracting top 15 rows using 'head()' function for the analysis and visualizing the revenue(USD millions) of different companies of United States using 'matplotlib.pyplot' file. 
Another kind of visualisation form is used to display the revenue growth of top 20 companies by converting datatype of Column 'Renevue growth' from string to float.
Another Dataframe is craeted with the sorted 'Employees' column. For that firstly, we will convert the datatype of 'Employees' column from string to integer in the previous DataFrame and, then sorting is applied on the 'Employees' column. The final result which is DataFrame with sorted 'Employess' column is assigned to a new DataFrame. Further, the index of the new DataFrame is reset.
Now, we will find the average revenue industriwise. For this, DataFrame.groupby() function is used to group the identical industry and their average revenue is computed in the next column using mean() function. Also, the datatype of the column 'Revenue (USD millions)'is changed to float to compute the average. And the results are displayed through bar plot for top 15 companies.

**Conclusion**
Visualizations help you identify patterns, correlations, and relationships in your data that might not be immediately apparent when looking at raw numbers. Here, the revenue in terms of milloin USD and its percentage growth by different largest companies in the United States is analysed and visualised using Pandas, BeautifulSoup. We also scraped the data about which company provide more employments. 
