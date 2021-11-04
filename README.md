# Kickstarting with Excel

## Overview of Project
Louise created a Kickstarter campaign for her play *Fever* that almost achieved its fundraising goal in a short amount of time. She wants to know how the outcomes of different campaigns fared in relation to their launch dates and funding goals.

### Purpose
Using a dataset from Kickstarter, we will create visualizations for the campaign outcomes based launch date under the Parent Category "Theater" and ratio of outcomes based on funding goals under the Subcategory "plays".

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
This visualization displays the outcomes "Theater" Kickstarter campaigns by the month of the year that they were launched.
![Outcomes Based on Launch Date.png](https://github.com/rptseng/kickstarter-analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
This visualization displays the outcomes of "Plays" Kickstarter campaigns by their funding goals, grouped by intervals of $5000.

![Outcomes vs goals](https://github.com/rptseng/kickstarter-analysis/blob/main/resources/Outcomes_vs_goals.png)

### Challenges and Difficulties Encountered
We may encounter difficulty generating a recommendation for a launch date and goal if we do not analyze the success rates on the intersection of these two variables. The "Analysis of Outcomes Based on Launch Date" only counts successes by month irrespective of goal amount, while "Analysis of Outcomes Based on Goals" does not consider the launch date or the number of samples in each goal interval.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

The months with the highest number of successfully funded "Theater" campaigns are May, June, and July respectively. Additionally, these three months also feature the highest percentage of successfully funded campaigns against the total campaigns launched (May 67%, June 65%, July 63%). Based on this slice, we may recommend "Theater" campaigns to feature a launch date from May-July because they correlate with successful outcomes.

- What can you conclude about the Outcomes based on Goals?

The highest ratio of successes to failures occurs in the "Less than $1000" goal bin at 75.8% successes, followed by the "$1000 too $4999" bucket at 72.7% successes. The results may suggest that the lower the goal, the higher the likelihood of getting successfully funded. 

- What are some limitations of this dataset?

There is an inconsistency where "Analysis of Outcomes Based on Launch Date" includes 1369 outcomes from the Parent Category "theater" while "Analysis of Outcomes Based on Goals" only includes 1047 outcomes from its Subcategory "plays". There is an opportunity to put both analyses at the same level of granularity so the findings of each analysis are more applicable to each other.

A limitation on "Analysis of Outcomes Based on Goals" is the small number of samples at the higher goal buckets. There are 961/1047 total campaigns in the first four intervals, and only 86/1047 spread over the last eight intervals. It would be important to consider that the rate of goals funded above $15,000 is only being represented on a small sample size.

- What are some other possible tables and/or graphs that we could create?

We could make a box plot showing the distribution of Goals($) with Successful Outcomes by Launch Month in "plays" campaigns. 

Using this graphic we can observe the range of goals that are likely to be successful when launched in a given month. This might help Louise set a goal that is more likely to be funded depending on when she needs to launch the campaign, or help her choose a launch date if she's determined how much money she needs to raise for her campaign.

![Successful Outcomes by Month boxplot](https://github.com/rptseng/kickstarter-analysis/blob/main/resources/Successful_Campaign_Goals_by_Month_boxplot.png)
