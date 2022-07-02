# kickstarter-analysis

## Overview of the Project

### Background
Louise wanted to start a campaign to help crowdfund $10,000 for her theatre play. As this is her first campaign, she has come to us to perform data analysis on several thousand crowdfunding projects to guide her in her endeavour. Thanks to our initial findings, Louise's fundraising campaign came close to its goal in a short amount of time and we have now been tasked with analyzing how different campaigns fared in relation to their lauch date and funding goals.

### Purpose
In this assignment we will be looking specifically at campaign outcomes based on their launch dates and their funding goals, using the same dataset from Kickstarter.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
<img src="https://github.com/jdutronc/kickstarter-analysis/blob/main/Resources/2_Goal_Columns.png" width="300">
I initially tried to split the goal range column into 2 columns (with a lower threshold and a higher threshold) to be able to easily drag/copy the formula for  the lower rows and then for the "Successful" column to the "Failed" and "Canceled" columns but I wasn't happy with the results. The syntax of the COUNTIFS function looked right but all rows returned a zero value.

### Analysis of Outcomes Based on Funding Goals




- 525 theater campaigns were successful in the US
- average campaign goal of $5,049
- median campaign goal of $3,000
- 50 backers on average each donating $89
- the month that launched the most successful campaigns was May
![Outcomes_Based_On_Launch_Date](C:/Desktop/BootCamp/Module_1/Crowdfunding_Analysis/Outcomes_Based_On_Launch_Date.png)
- Louise's goal is not only twice as high as the average goal for a successful campaign, it's even outside the range for outliers for amounts pledged, which indicates that Lousie has a very low chance of reaching her goal
![Goals_And_Pledges_for_Successful_GB_Campaigns](C:/Desktop/BootCamp/Module_1/Crowdfunding_Analysis/Goals_And_Pledges_for_Successful_GB_Campaigns.png)
