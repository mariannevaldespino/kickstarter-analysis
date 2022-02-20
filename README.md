# Kickstarting with Excel

## Overview of Project

### Purpose: The purpose of this analysis was to determine if the chance of a theater Kickstarter campaign being successful was correlated to the launch date and/or the goal amount.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date: 

I performed this analysis by firstly creating a new column labeled "Years" and using the YEAR() function with the column "Date Created Conversion".

![Screen Shot 2022-02-20 at 12 07 34 PM](https://user-images.githubusercontent.com/96892095/154854796-0dca176d-021f-4c31-b986-d232c00e68b1.png)

Then I created a pivot table showing the number of successful, failed, and canceled theater Kickstarter campaigns in each month of the year. Finally, I created a line chart from the pivot table in order to visualize this data.

![Screen Shot 2022-02-20 at 12 08 23 PM](https://user-images.githubusercontent.com/96892095/154854829-aed34a1c-9e2a-4277-89ed-9f22cffcd53f.png)

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/96892095/154854835-254c5a7e-0611-4899-afea-3481b02fd985.png)


### Analysis of Outcomes Based on Goals: 

I performed this analysis by firstly creating a new sheet and creating dollar-amount ranges so the number of successful, failed, and canceled Kickstarter campaigns could be grouped based on their goal amount. Then, I calculated the amount of each outcome by using the COUNTIFS() function and filtering by goal amount, outcome, and subcategory, choosing "plays" as the criteria. 

![Screen Shot 2022-02-20 at 12 09 33 PM](https://user-images.githubusercontent.com/96892095/154854874-93515b2c-3503-49f9-b8bc-f99a0176cf5d.png)

Finally, I calculated the percentage of successful, failed, and canceled campaigns for each dollar range and created a line chart to visualize this data.

![Screen Shot 2022-02-20 at 12 10 08 PM](https://user-images.githubusercontent.com/96892095/154854913-00833e61-75de-4f04-afa9-1001ee1489ef.png)

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/96892095/154854923-7210bfc3-d238-4e5a-a23f-08cc3d27a948.png)


### Challenges and Difficulties Encountered: 

A challenge I encountered was displaying the campaign outcomes by month on the pivot table for Theater Outcomes Based on Launch Date. I overcame this by grouping the dates the campaigns were created and filtering by month.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date? Two conclusions I can draw are that the best times to launch a campaign would be during the months of May and June, and that the worst time to launch a campaign would be during December.

- What can you conclude about the Outcomes based on Goals? I can conclude that the campaigns that are most successful are those with goals less than $4999.

- What are some limitations of this dataset? A limitation of this dataset is that we are only provided with the country, instead of a more specific location like state or city.  

- What are some other possible tables and/or graphs that we could create? Another possible table or graph we could create is outcomes based on the amount of time people had to donate, which would be calculated by finding the difference in days between when the campaign was launched and when it ended.
