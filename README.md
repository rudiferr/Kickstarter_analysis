# "kickstarting_excel" Week 1 Challenge
## Overview of Project
Tools Used: Microsoft Excel
### Purpose
The purpose of this project is to answer the two questions "Which month of the year has the most successfully launched theater-related Kickstarter campaigns?" and "Which funding goal range sees the most successful Kickstarter campaigns?" Visualizing the datasets allows us quickly answer these questions, while also gathering insights into other potential follow-up questions by organzing the data in such a manner that the pivot tables and formulas used can be easily modified for future use.
## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
Using a pivot table the dataset was organized such that the counts of the different outcomes states were mapped against different months a Kickstarter project can be launched throughout the year. These numbers were then organized in a line chart to see the months throughout the year that had successfully launched the most Kickstarter campaigns.
![Graph of Outcomes Based on Launch Date (count)](https://github.com/rudiferr/kickstarter-analysis/blob/main/graphPictures/Theater%20Outcomes%20vs%20Launch%20(count).png)
### Analysis of Outcomes Based on Goals
Using the `=COUNTIF()` and `=SUM()` functions in Excel the dataset was organized such that the counts of the different outcomes states were mapped against fixed monetary ranges of funding goals were a Kickstarter project can have. These numbers were then used to find the percentage successful, failed, and cancelled outcomes compared to the total outcomes that existed for a given range. Those percentages were then organized in a line chart to visualize the trend of these percentages as the funding goal ranges increase.
![Graph of Outcomes Based on Goals](https://github.com/rudiferr/kickstarter-analysis/blob/main/graphPictures/Outcomes%20vs%20Goals.png)
### Challenges and Difficulties Encountered
The *Outcomes Based on Goals* portion of this project required a lot of functions to be potentially retyped manually, which can painstakingly increase the amount of work required to successfully parse through the sheet with all of the raw data. Though, knowing how to make absolute cell references drastically decreased the amount of time required as you didn't have to worry about Excel changing the function due to them potentially being relative cell references.
## Results
- What are two conclusions you can draw about the Outcomes based on Launch Date?
1. One primary conclusion we can draw based on the potential success of a Kickstarter campaign is that the summer months collectively seem to have the most successful projects, with the start of the summer (May and June) having the highest amount.
2. A secondary conclusion related to the potential failures of projects is that the amount of successful projects starts to rapidly decrease when started throughout the fall and winter seasons, with the smallest amount of successfully launched campaigns throughout the entirety of the year belonging to December.
- What can you conclude about the Outcomes based on Goals?

A clear conclusion that can be drawn is that Kickstarter projects that have a funding goal of less than $5,000 will see the most overall success - not only proven by having the highest percentage of successfull campaigns, but also the lowest amount of campaigns that were cancelled.
- What are some limitations of this dataset?

Potential limitations of this dataset relate to lack of data about the exposure and impressions of the projects: having metrics about clickthrough rate, overall impressions that can be mapped against the total backers provided, etc., which are all valuable pieces of data, are missing here and can provide deeper analysis about what contributes to the most successful campaigns on Kickstarter.
- What are some other possible tables and/or graphs that we could create?

Although the graphs we created are great starting points, they lack granularity to be able to explain some nuanced questions that come up; for example, "Why do the summer projects have the most success of the year?" Instead of mapping purely count, seeing the percentage of successful campaigns across the year (shown below) actually determines that the summer month are not the most successful, as proportionally they yield the same results compared to other calendar moonths. Simply putting datapoints against eachother  doesn't provide effective insight; to answer this question (and others), tables and graphs that feature a combinations of datapoints need to be considered before effective conclusions can be made, such as launch date against duration of campaign against funding goal.
![Graph of Outcomes Based On Launch Date (percentage)](https://github.com/rudiferr/kickstarter-analysis/blob/main/graphPictures/Theater%20Outcomes%20vs%20Launch%20(percentage).png)
