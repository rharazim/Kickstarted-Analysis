# An Analysis of Kickstarter Campaigns
Module 1 Excel Kickstarter Analysis

## Overview
Our friend Louise used the website Kickstarter.com to crowdfund her play Fever. It came close to its goal, so she asked us to conduct an analysis using historical Kickstarter data in Microsoft Excel. We were asked to analyze campaign success based on their launch dates and their funding goals. We specifically narrowed our criteria to include theatrical campaigns to have better data to show Louise. After conducting our analyses, we visualized the results using appropriate graphs so the data may be interpreted easier. 

## Analysis & Challenges

### Theatrical Outcomes by Launch Date
We first analyzed theatrical Kickstarter outcomes by their launch date. To do this, we had import the relevant data into a pivot table. The relevant data are the launch date and the outcomes (successful, failed, canceled). A challenge here is that the pivot table will initially want to list every launch date individually. This makes for way too many data points and is not readable. What we want is to organize the data by their launch month regardless of day or year. So, we have to filter by the year, format the data by month. We also wanted to organize the outcomes in the order of successful, failed, and then canceled. After the data is organized to our liking, we graphed it with months being on the X-axis and the number of each outcome on the Y-axis. The graph should show clearly the number of each outcome in any given month from January to December. This is the final result that we will show to Louise.

### Outcomes Base on Goals
Secondly, we analyzed the outcome of Kickstarter plays by their initial fundraising goals. We organized this analysis in a new worksheet. We want the number of successful, failed and cancelled Kickstarter plays of each predetermined dollar range. We used a COUNTIFS formula to filter multiple columns of data and give us a count of each specific range and outcome. For example, the formula for the number of successful plays with fundraising goals between $5000 to $9999 looks like this:
 =COUNTIFS('Raw Data'!$D:$D,">=1000",'Raw Data'!$D:$D,"<=4999",'Raw Data'!$P:$P,"plays",'Raw Data'!$F:$F,"successful"). 
Then we used the SUM function to add every outcome for each range to get a total of that range. We did this so we could find the percentage of frequency of each outcome. For example, to get the percentage of failed projects with goals less than $1000, we would divide the number of failed outcomes (45) by the total count for that goal range (186) to get 0.24 or 24%. Once we have all the data, we can visualize it with a graph. A line graph is the best choice for this set of data because each data point is between 0% and 100%. The X-axis should be each fundraising goal range, and the Y-axis should be the percentage of outcome. After we title the graph “Outcome Based on Goal,” we are ready to show it to Louise.

## Results
### Theatrical Outcomes by Launch Date
Looking at our graph for the outcomes by launch date analysis, we see immediately that the most successful month to launch a Kickstarter campaign has been May. In May, a campaign was twice as likely to meet its goal than to fail or be canceled. While there were no months where there were more failures than successes, December has been the worst month to launch a campaign. A possible explanation for this is that during this month, people may be spending their disposable income on gifts or traveling due to the holidays rather than contributing to Kickstarter campaigns. Louise should shoot for one of May, June or July to launch a campaign if she is considering giving it another shot. One thing to be careful for is that May is also the most popular month to launch a theatrical Kickstarter. This means she would also be facing the most competition for her own funding. 

### Outcomes Based on Goals
The Outcomes Based on Goals graph shows that, based on percentage, the most successful Kickstarters for plays have goals between $0-$15000 and $35000-$45000. The least successful campaigns had goals between $20000-$35000, and greater than $45000. We can assert from the graph that Kickstarter success becomes more inconsistent with goals greater than $15,000. A failure of this graph is that it doesn’t show the weight of each goal range. For example, there was only one campaign in the range of $45000 to $49999, so the graphical result will be at either extreme, 0% or 100%, which does not accurately reflect the actual odds of success given a larger sample size.

### Limitations
This dataset is limited somewhat by the presence of outliers. This is due to the nature of Kickstarters where the goal can be set to any amount no matter how outrageous or unrealistic. Another limitation is that the dollar amount pledged is in different currencies due to the different countries. This may alter our expectations about results of certain analyses. 

### Other Possible Analyses
I would recommend further analysis by cross-referencing the two graphs we made to find the most successful Kickstarters in May-July with goals ranging from $0-$15000. These were the two categories that we found to be most successful through our two analyses. Another analysis we could do would be the outcome by the total time between launch and end date. This would help us see if successful kickstarters are typically shorter or longer. We could also graph the outcome versus the average donation to see if backers were donating small or large amounts to successful campaigns.  
