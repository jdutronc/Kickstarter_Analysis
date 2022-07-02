# kickstarter-analysis

## Overview of the Project

### Background
Louise wanted to start a campaign to help crowdfund $10,000 for her theatre play. As this is her first campaign, she has come to us to perform data analysis on several thousand crowdfunding projects to guide her in her endeavour. Thanks to our initial findings, Louise's fundraising campaign came close to its goal in a short amount of time and we have now been tasked with analyzing how different campaigns fared in relation to their launch date and funding goals.

### Purpose
In this assignment we will be looking specifically at campaign outcomes based on their launch dates and their funding goals, using the same dataset from Kickstarter.

<br>

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
<img align="right" src="https://github.com/jdutronc/kickstarter-analysis/blob/main/Resources/Theatre_Outcomes_Based_on_Launched_Date.png" width="300">
The chart on the right shows the crowdfunding campaign outcomes for theater plays based on launch date by calendar month. We created a pivot chart based on the Kickstater dataset to extract the years and months of campaign launch dates and we have highlighted the successful campaigns in green, the failed campaigns in red and the canceled campaigns in yellow.

<br> Click the image to enlarge.

<br>

### Analysis of Outcomes Based on Funding Goals
<img align="left" src="https://github.com/jdutronc/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png" width="400">
The chart on the left shows the crowdfunding campaign outcomes for theater plays based on their initial funding goals. We sorted successful, failed and canceled campaigns in ranges of initial crowdfunding goal and displayed the results into a line chart, with successful campaigns highlighted in green, failed campaigns in red and canceled campaigns in yellow.

<br> Click the image to enlarge.

<br>

### Challenges Encountered
<img align="right" src="https://github.com/jdutronc/kickstarter-analysis/blob/main/Resources/2_Goal_Columns.png" width="400">
I initially tried to split the goal range column into 2 columns (with a lower threshold and a higher threshold) to be able to easily drag/copy the formula in O2 down to O13 then to the other "Failed" and "Canceled" columns but I wasn't happy with the results. The syntax of the COUNTIFS function looked right but all rows returned a zero value (see picture attached right here) and the cell references in the criteria ">=" and "<=" would remain unchanged when dragging.

<br/> So I proceeded with just one "goal" column as described in the assignment and with absolute numbers in my ">=" and "<=" criteria instead of cell references, and it worked beautifully.

<br>

## Results

Campaign success seems to seasonal, with campaigns launching in May-Jun having a higher chance of success than average (about twice as many campaigns launched in May succeed vs. rest of the year).

Campaign failure on the other hand seems to not be impacted by seasonality, with a fairly consistent monthly number of failed campaigns all year round, so there must be other key factors deciding the failure of the campaigns beside seasonality.

About 70% of campaigns with a goal of $10,000 or less are successful, but as the goal amounts increase, so does the unpredictability of success (about 50:50 chance between $10k and $50k). And campaigns with a goal of $50k or higher have an 88% chance of failure.

 
