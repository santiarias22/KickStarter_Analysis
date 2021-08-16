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
One conclusion is made about the Outcomes based on Goals 
There is a summary of the limitations of the dataset, and there is a recommendation for additional tables or graphs
