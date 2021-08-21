[KickStarter_Challenge.xlsx](https://github.com/santiarias22/KickStarter_Analysis/files/6989739/KickStarter_Challenge.xlsx)
<img width="617" alt="Outcomes_vs_Goals" src="https://user-images.githubusercontent.com/88511476/129510847-0eafc772-9fa3-49dc-93e1-cc5e330f47af.png">
<img width="329" alt="Theather_Outcomes_vs_Launch" src="https://user-images.githubusercontent.com/88511476/129510848-ced0e597-aa49-46b9-b4a2-ee72425d2573.png">

# KickStarter_Analysis

## Challenge_Module_1

### Overview of the Project
Two analyses are performed to practice Excel skills for Module 1: outcomes based on goals and outcomes based on launch date using the following dat set as shown below:
![KickStarter_Challenge](path/to/KickStater_Challenge.xlxs)
### Analysis & Challenges
Using the Kickstarter dataset, the main purose was to visualize campaign outcomes based on their launch dates and their funding goals. 

#### Deliverable 1: Outcomes based on goals:
This challenge was perfomed by creating pivot tables and graphing in Excel were used to visualize campaign outcomes ("successful," "failed," and "canceled") based on launch date. So I created a new column labeled "Years." Then in the "Years" column, I use the YEAR() function to extract the year from the “Date Created Conversion” column. 
After creating a new pivot table in a new sheet from the KickStarter worksheet, I filtered the pivot table based on "Parent Category" and "Years," placed the appropriate pivot table fields in the columns, rows, and values to finally filtered the column labels to show only "successful," "failed," and "canceled." The final result can be seen below:
![image_Theather_Outcomes_vs_Launch](path/to/image_Theather_Outcomes_vs_Launch.png)

As can be seen, it is important to filter the "Parent Category" to show only the data for "theater" on the pivot table, and , then, sort the campaign outcomes in descending order so "successful" is first.
The challenge in this exercise for me was basically to understand clearly what is going to be visualized and how columns, rows, and filter work to show what was required.

#### Deliverable 2: Outcomes based on Goals

The second challenge consisted of visualizing the percentage of successful, failed, and canceled plays based on the funding goal amount. So, in the KickStarter Data, I created a new worksheet with a series of columns for goal, number of succesful, failed, and canceled plays, the total number and the percentage for each category, and using the COUNTIFS function I populate each cell (=COUNTIFS(Kickstarter!$D:$D,">=1000",Kickstarter!$F:$F,"successful",Kickstarter!$D:$D,"<=4999",Kickstarter!$R:$R,"plays").
In the “Goal” column, I created the following dollar-amount ranges (from <1000 to >= 50,000 USD) so projects can be grouped based on their goal amount.

It was very challenging to figure out that "$" fixates the column you want the COUNTIFS function to consider as stable, and also to realize that you need to set the criteria before and after filtering using that function. Finally, I Used the "SUM" function to create toatals for each subcategory and dollar amount ranges to calculate the percentages, and I created a graph that shows the outcomes and goals palying together based on dollar-amount range, as it follows:
![image_Outcomes_vs_Goals](path/to/image_Outcomes_vs_Goals.png)

#### Results (two Conclusions)
One conclusion that can be made about the Outcomes based on Goals sheet is that the higher the goal gets the more difficult it gets to achieve it. If we compare the number of projects below 10,000 USD with the ones higher than 10,000 USD, we can see that the percentage of succesful projects decreases conforming the goal amount increases. Thus, the main recommendation here is to increase the number of fundraising projects under 5,000 USD and decreases the number of the higher ones, specially during the montsh of April, May, June, July, and August as the Theater Outcomes by launch date sheet indicated. 

One main limitation for the dataset is that it would important to see what are the topics or themes that made the succesful projects as such and why during the months of April, May, June, July, and August, the chance to get a succesful project is the highest compared to rest of the year. Additionally, it would be interesting to create a new table to analyze the relationship between the succesfulness likelihood of projects based on deadlines to see whether or not the more time the plays have to prepare the higher succesfulness chance it gets. Overall, another table and graph about how true this analysis become across countries to learn from other countries in which projects gets succesful in other months other than April, May, June, July, And August to see if it is a seasonal influence or not.
