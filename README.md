# Microsoft-Excel---Data-Analysis-with-Excel-Pivot-Tables
This portfolio contains my homework assignments for the Udemy course on Pivot Tables in Microsoft Excel by Chris, the Founder of Maven Analytics. I have completed these assignments entirely by myself without the assistance of others and without looking at any solutions available online. I have also written the explanations of steps below entirely by myself, based on the assignment instructions, to demonstrate my comprehension of what I am doing. The parts were completed in order, so the steps in each part assume we are beginning at the view resulting from the previous part. Each homework below is associated with a folder in Github, and each part within each homework below is associated with an excel file within the corresponding folder in Github. To see what I have done in any part, read the part in the ReadMe to see the actions I took on the IMDb Movie Database, and then check the corresponding Excel file to see the pivot table view that resulted after those actions were taken. To see the original IMDb Movie Database at any time, click into the second sheet in any of the Excel files.

# Homework 1: Excel Pivot Table 101
Part 1: I used the rows and values fields of the Pivot Table to find budget by title, used the filters to narrow my table to English films in Japan, and added a Grand Total for the rows in the design tab to find the aggregate budget for films meeting the specified criteria. I also formatted the table values as dollar amounts with no decimal places using number format. Using Cell B13 in the resulting pivot table, I can see that the aggregate budget for English films in Japan in the IMDb database is $154,000,000.

Part 2: I cleared the language filter and switched the country of interest from Japan to Denmark. I added a sum of gross revenue value to my values field and reformatted it as a currency with no decimal places. I also changed its column label from 'Sum of Gross Revenue' to 'Gross Revenue ', using a space at the end of the column in order to be able to reuse the label already entered in the pivot table. Using Cell C15 of this view, I can determine that the gross revenue for the Danish film 'The Celebration' is $1,647,780.

Part 3: I used the "Clear All" command in the PivotTable Analyze options to remove all fields from the table. Then, I placed 'Country' in the rows field, 'Genre' in the columns field, and 'Gross Revenue' in the values field, to show the aggregate gross revenue in each country for each genre of film. In this view, Cell F21 shows that $611,709 worth of revenue was generated by comedy films in Finland.

Part 4: I removed the 'Country' field, made 'Genre' the primary row label, and added 'Rating' as a secondary row label. Cell C84 shows that $445,361,439 in revenue was generated by PG-rated Family films. By double clicking on this cell, we can see that the film 'E.T. the Extra-Terrestrial' drove most of this revenue.

Part 5: I added a row to the end of the IMDb Database for a movie titled 'Cool New Movie'. Then, I used the 'Change Data Source' option to update the pivot by changing the ending row in the data location to be one higher. After doing this, filtering on 'Title' is 'Cool New Movie' with the value of 'Count of Title' gives the result 1 in Cell A8, showing that there is indeed now a movie with my created name in the data source for the active pivot table.

# Homework 2
Part 1: I added 'Budget' and 'Gross Revenue' to the values field, with 'Budget' first. I added 'Title' to the rows field. I reformatted the columns as dollar currencies with zero decimal places using the 'Number Format' option. In this view, Cell B109 shows that the budget for the film 'A Passage to India' was $16,000,000.

Part 2: I made a new table with 'Genre' in the rows field, 'Rating' in the columns field, and 'Sum of Gross Revenue' in the values field. In this view, I can see that the empty cells are already populated with '$0'. However, if they were not, I would right click on any cell and go to 'Pivot Table Options', where I would change 'Empty cells as: ' to edit this property.

Part 3: I switched 'Rating' to be a secondary row label under 'Genre'. Then, I switched the table to 'Outline' mode by going to the 'Design' tab and selecting the corresponding option under 'Report Layout'. Finally, I renamed 'Rating' to 'Film Rating' and 'Sum of Gross Revenue' to 'Gross Revenue ' by double clicking the corresponding title cells. Notice the trailing space in 'Gross Revenue ', which I used to differentiate it from 'Gross Revenue', the existing PivotTable field name.

Part 4: I removed 'Film Rating' from the view by dragging it from the fields list. I turned 'Grand Totals' off in the 'Design' tab, and then added a 'Color Scale' on the 'Gross Revenue ' values within the 'Conditional Formatting' options in the 'Home' tab. The color scale allowed me to easily and visually see that the highest value for 'Gross Revenue ' was $67,540,890,818 in Cell B8, and that this revenue is associated with the 'Action' genre.

Part 5: I added another Gross Revenue column using two trailing spaces to differentiate it from both existing labels. For this column, I added data bars using the Conditional Formatting option in the Home tab once again. I also used a custom number format with three semicolons to make the text invisible for this third column so that the data bars would be easier to read. The data bars visually show me that the second highest grossing genre is Comedy, as can be seen by the data bar in Cell C12.

HOMEWORK: Sorting, Filtering & Grouping Data with Excel Pivot Tables
