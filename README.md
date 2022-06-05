# Kickstarter_Challenge


##**Kickstarter Analysis**##

##**Overview**##
The purpose of this analysis is to evaluate how different campaigns did in relation to their launch dates and their funding goals. 

##**Analysis and Challenges**

######**Analysis of Outcomes Based on Launch Dates**
I created a pivot table to visualize and graph the campaign outcomes based on their launch date. In order to get the months, I had to group the Date Created Conversion. Then I filtered the “Parent Category” to show data for “theater” and sorted the “Campaign Labels” in descending order to make “successful” the first campaign outcome. Finally, I created a line chart to visualize the relationship between outcomes and the launch month. 


######**Analysis of Outcomes Based on Launch Dates**
For the outcomes based on launch dates, I created a new sheet where I made 8 new columns to represent “Goal”, “Number Successful”, etc. I used COUNTIFS to meet the multiple criteria of the assignment. 

I selected column D in the Kickstarter sheet to input the range of each row, then I selected column F to ensure the  correct outcome was selected, and finally column R  to set the subcategory to“plays”. 

=COUNTIFS(Kickstarter!D:D,"<1000", Kickstarter!F:F, "successful", Kickstarter!R:R, "plays")

From this formula I added the range of each row to each column, making sure to change the outcome to its respective column (“successful”,“failled”, or “canceled”)

=COUNTIFS(Kickstarter!D:D,">=1000", Kickstarter!D:D, "<=4999", Kickstarter!F:F, "successful", Kickstarter!R:R, "plays")

In the column “Total Projects”, I used SUM to add each row of successful, failed and canceled. Finally, to get the percentage of successful, failed and canceled, I took the number of outcomes and divided it by the total projects:

=B2/E2 = (141/186) = 76%
