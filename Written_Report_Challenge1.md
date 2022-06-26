                          # Kickstarting with Excel

## Overview of Project
   This project will be gathering data on fundraising goals for a client. Data will be analyzed to look at different outcomes around fundraising goals.

### Purpose
Louise’s play Fever came close to its fundraising goal in a short amount of time. I will look at how her different campaigns fared in relation to their launch dates and their funding goals. Using the Kickstarter dataset, I will visualize campaign outcomes based on their launch dates and their funding goals. Seeing these results will help Louise have analysis around her fundraising goals for future projects.

## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
The first analysis I put together was theater outcomes by launch date. I ran a filter on my main "Kickstarter" sheet to filter out the plays, since this is the data, I want to look at. I then added a new column to my "Kickstarter" spreadsheet and labeled it "Years." I was able to calculate this by =Year(R2). R2 is the column that had the full date. Now that I had my year for each campaign (focused on plays), I created a pivot table (Insert-pivot table). I filtered the data by parent category and year. For values I input outcomes. I added a row for data created conversion and calculated by month of launch date. Once I had my pivot table created, I made a line graph to compare successful, failed, canceled outcomes for each month.

![Outcomes_vs_Launch](Resources/Theater_Outcomes_vs_Launch.png)

Some of the challenges I faced in this data was due to filtering by Month. It took me a couple of tries to gather the month. Since I had filtered by years the data kept presenting itself as year over year. When I adjusted the settings further, it would calculate the data by quarter. Filtering by month took a few tries until I finally figured out, I had to sort by years and then remove years and quarter when it left me with the month only. Another challenge I faced was trying to filter out the launched campaigns. I had a few campaigns that did not fall under successful, failed or cancelled and were showing up as “go live”. When I sorted the data in the pivot table it removed that information.

### Analysis of Outcomes Based on Goals

On the second analysis, outcomes based on goals, the goals were broken into brackets. Each bracket was $5K, starting less than $1K and going up to 50K or more. I again filtered by sucessful, failed and canceled campaigns in each caegory. I used the Countif formula to populate the data for each field.

=Countif (refer to the spreadsheet to review the formulas for each category).

![Outcomes_vs_Launch](Resources/Outcomes_based_on_goals)

The challenge I encountered on this data was getting the formulas correct. There were a couple of formulas were I put the quotes or > < areas in the wrong direction. One typo skews the data completely. I discovered these mistakes when I created my chart and the data looked off. I went back to my data and double checked everything to find my typos and fix them.



### Challenges and Difficulties Encountered
(See above regarding challenges in the data handling) There were difficulties in creating the charts. I could see how challenges could be created if you picked the wrong type of line chart. I played around with different types of charts and did see slight differences, until I ultimately picked the line chart I used.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
A very clear conclusion that stands out the most is the spike in successful outcomes in May and June. An assumption could be made that these are typically around spring break/summer breaks when more people would have the time to go see plays. Another conclusion that could be seen in the data is the very little to no canceled plays. Cancelling plays makes sense if the play is not a popular play or is not in demand from play goers.

- What can you conclude about the Outcomes based on Goals?
One conclusion from outcomes based on goals is that the highest number of successful outcomes is those in the $1K to $4999K range and the least being $50K or more. The lower price range is a more attainable number whereas getting $50K would be less likely because the higher dollar number would be more difficult to obtain.


- What are some limitations of this dataset?
Some limitations on the data set could be the reason why some campaigns are unsuccessful. Is it because the play or tv show is not popular, there is no demand for it or is there some other reason. If the reason was known (possibly through surveys) then we would have information to present as to why some campaigns are unsuccessful over others.

- What are some other possible tables and/or graphs that we could create?
--we could try to identify outliers amount he whole kickstarter data set and see if that skew any of our plays data.
--we could analyze other subcategories rather than plays
--we could look at all plays together and see what that data would represent. 
--It would also be interesting to see which category/subcategory had the most successful outcomes against each other (or look at the means and compare them against each other)


