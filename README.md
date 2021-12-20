# An Analysis of Kickstarter Campaigns

## Overview of Project
Analysis of the success or failure of Kickstarter campaigns. 

### Purpose
This analysis focuses on theatre-related campaigns and factors that contribute to their outcome in order to provide recommendations on how to formulate a successful campaign.

### Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
This analysis was performed by extracting the year from campaign launch dates, then pivoting the campaign outcomes over their start dates. This data was limited to campaigns for plays and then charted using a line graph to show trends over time.

While this analysis is focused on theatre campaigns, the source spreadsheet contains a lot of data about unrelated campaigns. Ensuring that all data was correctly filtered and sorted was therefore the primary challenge in ensuring that these results were accurately presented.

### Analysis of Outcomes Based on Goals
This analysis was performed by categorizing the monetary goals of campaigns for plays in increments of 5000, plus a "less than 1000" baseline for campaigns with very low goals. Completed play campaigns (that is, campaigns with an outcome other than "live") were then categorized based on their outcome and goal, and within each goal increment, the percentage of campaigns that were successful, failed, or canceled was calculated. These percentages were graphed over the goal increments, using a line chart to better show trends.

My primary challenge in creating this output was in properly concatenating multiple Excel functions together in order to minimize the manual input needed. I also noted that the goal categories created in this analysis do not distinguish or convert between the currencies in which they were created, which means that campaigns should be further categorized by country in order to accurately assess the benchmarks at which a campaign is more or less likely to be successful.

## Results

### Overall
The majority of theatre kickstarters are successful, including 65% of plays. 
![theatre_campaign_outcomes](https://github.com/kmburkezoo/kickstarter-analysis/blob/main/Resources/theater_campaign_outcomes.png)

## Outcomes Based on Launch Date
May had the most successfully launched campaigns of any month, followed by June, July, August, and February. Early summer therefore appears to be the best time to launch a campaign. The worst time to launch a campaign for a play is December; less than half the campaigns launched in December in this dataset were successful.
![outcomes_by_launch_date](https://github.com/kmburkezoo/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)
However, more failed campaigns were also launched over the summer than during other months, so better conclusions can be drawn from an anlysis of the percentage of succesful campaigns than a count:
![theatre campaign outcome percentage](https://github.com/kmburkezoo/kickstarter-analysis/blob/main/Resources/Theater_Outcome_Percentage_vs_Launch.png)
From this chart, we can more easily see that campaigns launched between April and July have the highest success rates, but the difference in success rates from month to month is not as great as it appears when looking at the count of campaigns.

## Outcomes Based on Goals
76% of plays with a goal of less than $1000 are successful, decreasing to 50% of plays with a goal between $15000 and $19999. A campaign with a goal under $20,000 appears most likely to succeed.
![outcomes_vs_goals](https://github.com/kmburkezoo/kickstarter-analysis/blob/main/Resources/outcomes_vs_goals.png)

While there are several goal ranges aove $20,000 in which more than half the campaigns were successful, there were far fewer campaigns in these ranges--a total of 62 campaigns had goals over $20,000, compared to 72 in the 10,000-14,999 range. Additional statistics should therefore be considered when analyzing these upper ranges, as they will be more heavily influenced by the success of a handful of campaigns.

## Limitations
As previously noted, the ability to compare goals for campaigns by different countries is limited due to the use of different currencies. Converting between them would give a clearer picture of the amount of money most campaigns can successfully raise.

The data distribution within this dataset could also benefit from additonal analysis, as campaign goals range from as low as $1 to as high as $30,000,000, and campaigns at both ends of the spectrum have the potential to skew the resulting analysis.

The dataset also does not include some potentially meaningful values, such as:
- Amounts pledged by individual backers, which would allow us to discern which plays were truly crowd-funded and which had a few wealthy patrons
- A breakdown of the amount pledged during each month of a campaign's duration, which would give us more insight into how quickly most campaigns meet, or fail to meet, their goals

## Opportunities for Additional Analysis 
This dataset contains several additional factors that have not yet been taken into account, including:
- Campaign length, likely best analyzed using a line chart
- Bar or pie charts to show the distribution of outcomes for campaigns marked as a "Staff Pick" or "Spotlight"
- The average amount pledged by a campaign's backers, which could shed light on how support from a handful of wealthy backers can make or break a campaign 
