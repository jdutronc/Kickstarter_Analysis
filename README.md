# kickstarter-analysis

## Overview of the Project

### Background
Louise wanted to start a campaign to help crowdfund $10,000 for her theatre play. As this is her first campaign, she has come to us to perform data analysis on several thousand crowdfunding projects to guide her in her endeavour. Thanks to our initial findings, Louise's fundraising campaign came close to its goal in a short amount of time and we have now been tasked with analyzing how different campaigns fared in relation to their launch date and funding goals.

### Purpose
In this assignment we will be looking specifically at campaign outcomes based on their launch dates and their funding goals, using the same dataset from Kickstarter.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
<img align="right" src="https://github.com/jdutronc/kickstarter-analysis/blob/main/Resources/Theatre_Outcomes_Based_on_Launched_Date.png" width="300">
The chart on the right shows the crowdfunding campaign outcomes for theater plays based on launch date by calendar month. We created a pivot chart based on the Kickstater dataset to extract relevant data and we have highlighted the successful campaigns in green, the failed campaigns in red and the canceled campaigns in yellow.

<br> Click the image to enlarge.
<br>
<br>

### Analysis of Outcomes Based on Funding Goals
<img align="left" src="https://github.com/jdutronc/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png" width="400">
The chart on the right shows the crowdfunding campaign outcomes for theater plays based on their initial funding goals.

### Challenges Encountered
<img align="right" src="https://github.com/jdutronc/kickstarter-analysis/blob/main/Resources/2_Goal_Columns.png" width="400">
I initially tried to split the goal range column into 2 columns (with a lower threshold and a higher threshold) to be able to easily drag/copy the formula in O2 down to O13 then to the other "Failed" and "Canceled" columns but I wasn't happy with the results. The syntax of the COUNTIFS function looked right but all rows returned a zero value (see picture attached right here) and the cell references in the criteria ">=" and "<=" would remain unchanged when dragging.

<br/> So I proceeded with just one "goal" column as described in the assignment and with absolute numbers in my ">=" and "<=" criteria instead of cell references, and it worked beautifully.



- 525 theater campaigns were successful in the US
- average campaign goal of $5,049
- median campaign goal of $3,000
- 50 backers on average each donating $89
- the month that launched the most successful campaigns was May
![Outcomes_Based_On_Launch_Date](C:/Desktop/BootCamp/Module_1/Crowdfunding_Analysis/Outcomes_Based_On_Launch_Date.png)
- Louise's goal is not only twice as high as the average goal for a successful campaign, it's even outside the range for outliers for amounts pledged, which indicates that Lousie has a very low chance of reaching her goal
![Goals_And_Pledges_for_Successful_GB_Campaigns](C:/Desktop/BootCamp/Module_1/Crowdfunding_Analysis/Goals_And_Pledges_for_Successful_GB_Campaigns.png)
