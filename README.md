# Microsoft-Excel---Data-Analysis-with-Excel-Pivot-Tables
This portfolio contains my homework assignments for the Udemy course on Pivot Tables in Microsoft Excel by Chris, the Founder of Maven Analytics. I have completed these assignments entirely by myself without the assistance of others and without looking at any solutions available online. I have also written the explanations of steps below entirely by myself, based on the assignment instructions, to demonstrate my comprehension of what I am doing. The parts were completed in order, so the steps in each part assume we are beginning at the view resulting from the previous part. Each homework below is associated with a folder in Github, and each part within each homework below is associated with an excel file within the corresponding folder in Github. To see what I have done in any part, read the part in the ReadMe to see the actions I took on the IMDb Movie Database, and then check the corresponding Excel file to see the pivot table view that resulted after those actions were taken. To see the original IMDb Movie Database at any time, click into the second sheet in any of the Excel files.

# Homework 1: Excel Pivot Table 101
Part 1: I used the rows and values fields of the Pivot Table to find budget by title, used the filters to narrow my table to English films in Japan, and added a Grand Total for the rows in the design tab to find the aggregate budget for films meeting the specified criteria. I also formatted the table values as dollar amounts with no decimal places using number format. Using Cell B13 in the resulting pivot table, I can see that the aggregate budget for English films in Japan in the IMDb database is $154,000,000.

Part 2: I cleared the language filter and switched the country of interest from Japan to Denmark. I added a sum of gross revenue value to my values field and reformatted it as a currency with no decimal places. I also changed its column label from 'Sum of Gross Revenue' to 'Gross Revenue ', using a space at the end of the column in order to be able to reuse the label already entered in the pivot table. Using Cell C15 of this view, I can determine that the gross revenue for the Danish film 'The Celebration' is $1,647,780.

Part 3: I used the "Clear All" command in the PivotTable Analyze options to remove all fields from the table. Then, I placed 'Country' in the rows field, 'Genre' in the columns field, and 'Gross Revenue' in the values field, to show the aggregate gross revenue in each country for each genre of film. In this view, Cell F21 shows that $611,709 worth of revenue was generated by comedy films in Finland.

Part 4: I removed the 'Country' field, made 'Genre' the primary row label, and added 'Rating' as a secondary row label. Cell C84 shows that $445,361,439 in revenue was generated by PG-rated Family films. By double clicking on this cell, we can see that the film 'E.T. the Extra-Terrestrial' drove most of this revenue.

Part 5: I added a row to the end of the IMDb Database for a movie titled 'Cool New Movie'. Then, I used the 'Change Data Source' option to update the pivot by changing the ending row in the data location to be one higher. After doing this, filtering on 'Title' is 'Cool New Movie' with the value of 'Count of Title' gives the result 1 in Cell A8, showing that there is indeed now a movie with my created name in the data source for the active pivot table.

# Homework 2: Excel Pivot Table Formatting
Part 1: I added 'Budget' and 'Gross Revenue' to the values field, with 'Budget' first. I added 'Title' to the rows field. I reformatted the columns as dollar currencies with zero decimal places using the 'Number Format' option. In this view, Cell B109 shows that the budget for the film 'A Passage to India' was $16,000,000.

Part 2: I made a new table with 'Genre' in the rows field, 'Rating' in the columns field, and 'Sum of Gross Revenue' in the values field. In this view, I can see that the empty cells are already populated with '$0'. However, if they were not, I would right click on any cell and go to 'Pivot Table Options', where I would change 'Empty cells as: ' to edit this property.

Part 3: I switched 'Rating' to be a secondary row label under 'Genre'. Then, I switched the table to 'Outline' mode by going to the 'Design' tab and selecting the corresponding option under 'Report Layout'. Finally, I renamed 'Rating' to 'Film Rating' and 'Sum of Gross Revenue' to 'Gross Revenue ' by double clicking the corresponding title cells. Notice the trailing space in 'Gross Revenue ', which I used to differentiate it from 'Gross Revenue', the existing PivotTable field name.

Part 4: I removed 'Film Rating' from the view by dragging it from the fields list. I turned 'Grand Totals' off in the 'Design' tab, and then added a 'Color Scale' on the 'Gross Revenue ' values within the 'Conditional Formatting' options in the 'Home' tab. The color scale allowed me to easily and visually see that the highest value for 'Gross Revenue ' was $67,540,890,818 in Cell B8, and that this revenue is associated with the 'Action' genre.

Part 5: I added another Gross Revenue column using two trailing spaces to differentiate it from both existing labels. For this column, I added data bars using the Conditional Formatting option in the Home tab once again. I also used a custom number format with three semicolons to make the text invisible for this third column so that the data bars would be easier to read. The data bars visually show me that the second highest grossing genre is Comedy, as can be seen by the data bar in Cell C12.

# Homework 3: Sorting, Filtering & Grouping Data with Excel Pivot Tables
Question 1: I put Title in the Rows and Gross Revenue in the values. Then, I put Release Date in the rows. To get a Years label, I selected the Release Data category, and chose the Group Selection option in the Group Selection drop down. Here, I used command click to select Days, Months, Quarters, and Years simultaneously. Then, I dragged Release Data, Months, and Quarters out of the rows, and dragged Years to the filters. There, I unselected all and then selected 2005, 2006, 2007, and 2008. Then, I selected the first value for Gross Revenue, in Cell B8. Then, I selected Custom Sort in Sort & Filter in the Home tab, chose Descending, and pressed Ok. This allowed me to see in Cell B8 that the highest grossing film out of the films released in the years 2005, 2006, 2007, and 2008 was 'The Dark Knight'.

Question 2: I clicked on the drop down menu next to the Title category in the pivot table and selected a filter for 'Ends with' and chose the value '2' for my ends with criteria. Doing this gave a view with seven titles. Since these titles are still ordered by descending gross revenue and the filter on years is still applied, I can see that the highest grossing film ending with 2 in the years 2005, 2006, 2007, and 2008 was 'Cheaper by the Dozen 2' in Cell A8.

Question 3: I chose the same drop down menu and selected Clear Filter to get rid of my label filter. Then, I added a value filter for gross revenue between 1000000 and 3000000. Cells A8 to A58 show me that there were 51 films released in these four years with gross revenues between $1,000,000 and $3,000,000.

Question 4: In the PivotTable options, Layout field, I checked "Allow multiple filters per field" in order to be able to use a label and a value filter simultaneously. Then, I used the drop down to add a label filter for movies starting with 'm'. This returned a view with five movies, as can be seen from cells A8 to A12.

Question 5: I changed the Begins With value for label filter to 'm*s' to find titles that begin with 'm' and contain 's'. The titles returned, as can be seen in Cells A8 and A9, were 'Miss Potter' and 'Me and Orson Welles'.

# HOMEWORK 4: Enriching Data with Pivot Table Calculated Values & Fields
Question 1: I created a view with IMDb score by Title. From this view, we can see that the IMDb score does indeed range from 1 to 10 for individual titles. However, when I replace Title with Genre, the IMDb scores no longer fall within this range. To fix this, I right clicked the Sum of IMDb Score (1-10) column, and chose Average within the Summarize Values By column.

Question 2: I added Year as a secondary row label. Then, I added a second instance of IMDb score (1-10) and set the summarization mode to average again. Then, I right-clicked the column again and set the Show Values As option to Rank from Largest to Smallest. This view allows me to quickly see that with a rank of 1, the year 2013 saw the highest-rated Biography films on average, while with a rank of 4, the year 2011 saw the lowest-rated Biography films on average.

Question 3: I added another column for Sum of Gross Revenue by checking Gross Revenue in the field list. Then, I used the show values as option for % difference from, chose previous as the base item, and chose year as the base field, so that the value in each field is the change from year to year given as a percent for that genre. From this view, I can see in Cell E13 that gross revenue for action movies in 2014 was 57.1% greater than in 2013.

Question 4: I replaced genre and year in the rows with title. Then, I selected one of the existing column labels and chose insert and insert calculated field from the toolbar at the top. I named it Profit and set the formula to be Gross Revenue minus Budget by double clicking fields from the list and typing in the operations. Then, I used the same process to add a field called Profit Margin for Profit divided by gross revenue. Then, I added these two new fields to the values by checking them, and I removed all the values besides these two calculated fields. I right clicked the sum of profit margin column label, chose sort and sorted by largest to smallest to quickly show that the Title with the strongest Profit Margin in the entire sample accross all years was 'Paranormal Activity'.

Question 5: I inserted a calculated field, called it 'Cast + Director Likes', and used the formula 'Cast FB Likes + Director FB Likes'. Then, I inserted another calculated field, called it 'Cast + Director Likes per Title', and used the formula 'Cast + Director Likes / Number of Titles'. Since 'Number of Titles' is a count of the number of titles in a group, when I put 'Genre' in Rows, it divides by the number of titles of that genre to give me an average per title. Then, I removed both fields using the right click drop downs, inserted the 'Cast FB Likes' and 'Director FB Likes' fields by dragging them to values, changed the summarization type for those to average in the right click drop down, and finally readded 'Cast + Director Likes per Title' by dragging it to Values, which showed that indeed, the fields are working correctly because the 'Cast + Director Likes per Title' for each category is equal to the average number of cast likes plus the average number of director likes within that category.

# Homework 5: Visualizing Data with Excel Pivot Charts

1. Create a view to show # of Titles by Country, excluding the USA, for the entire sample. Name the PivotTable "Titles by Country", then use a PivotChart to visualize this view as a Clustered Column Chart.

2. Hide the Field Buttons from the PivotChart, then apply a value filter to only show the top 10 countries by # of Titles (hint: you may need to enable multiple filters). Which country is #2?

3. Change the chart type to a Clustered Bar, and change the PivotTable sorting to ascending by # of Titles.

4. Pull in IMDb Score as a second series, and summarize values by Average. Change your PivotChart type to Combo, with # of Titles as a Clustered Column and IMDb Score as a Line with Markers, on the Secondary Axis. Which of the 10 countries generated the lowest average IMDb Scores? (Bonus: Format the IMDb series in the chart to only show the markers, with no line)

5. Copy the existing pivot and create a second view below the combo chart to show Budget by Genre, with a Top 5 filter applied. Name the table "Budget by Genre", then visualize this view with a Pie chart, with hidden field buttons.

6. Insert a Slicer for Genre, enable multi-select, then connect it to both PivotTables. Create a simple dashboard by hiding the columns of your raw PivotTable views, disabling gridlines, and aligning/formatting the PivotCharts and Slicer as you see fit. Practice adjusting slicer selections to see how the dashboard updates!

# HOMEWORK: Analyzing U.S. Voter Demographics

1. How many states had a Voter Population % below 55%? Which states?

2. How many confirmed voters in California were over 65 years old in 2012? What percentage does that represent out of the total confirmed voters in California? What percentage out of the confirmed voters in the entire country?

3. Show both Citizen Population and Confirmed Voters by Age, as % of Column Total. What percentage of the citizen population do 45 to 64 year olds represent? What percentage of the confirmed voter population?

4. Create a new calculated field named "Voter Turnout" (Confirmed Voters/Registered Voters), formatted as a percentage with 2 decimal points. Which state had the highest voter turnout rate? What about among 18-24 year old voters specifically?

5. As a politician seeking to improve voter turnout rates among young adults (18-24), which particular states would you target first?
