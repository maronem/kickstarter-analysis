# kickstarter-analysis
Performing analysis on Kickstarter data to uncover trends
# Kickstarting with Excel

## Overview of Project

### Purpose
    The purpose of this project was to assess the outcome of Kickstarter campaigns based on their launch date and fundraising goals using the Kickstarter dataset. 
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
        Analysis of specifically theater related Kickstarter outcomes was first performed by creating a pivot table from the complete dataset (Fig. 1). To generate the table, the Date Created was used as rows with each cell formatted to show as a month and Kickstarter outcome was used as the columns and as the values listed in the table. The data was then filtered by Parent Category to visualize outcomes specifically for theater Kickstarters. One challenge I faced during this part of the analysis was learning how to 

        ![*Fig. 1*](https://github.com/maronem/kickstarter-analysis/blob/main/launchdate_pivot.PNG)

### Analysis of Outcomes Based on Goals
        Analysis was conducted to visualize the percentage of successful, failed, and canceled Kickstaters that were plays based on fundraiser goals. A table was generated with the rows split into categories of fundraiser goal amounts starting under $1000, then $5000 intervals up to $50000, and lastly goals greater than $50000. To assign values to each specific condition COUNTIFS statements were used to pull the number of play Kickstarter campaigns that fit each condition (Fig. 2)

        ![*Fig. 2*](https://github.com/maronem/kickstarter-analysis/blob/main/goals_countif_example.PNG)

        To calculate the percentage of successful, canceled, and failed play Kickstarters the number of successful, canceled, and failed Kickstarters within each donation goal range were divided by the number of total projects. Each cell calculated for a percentage was formatted as a percentage (Fig. 3). 

        ![*Fig. 3*] (https://github.com/maronem/kickstarter-analysis/blob/main/percentage_fnc_example.PNG)

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
        One conclusion based on the plot of Kickstarter outcomes by launch date month is that while there is no trend over time for failed and cancelled Kickstarters, there is a downward trend for successful Kickstarters over time from January to December as seen with the negative slope of the trendline. This data suggests that Kickstarters are more likely to have a successful outcome the earlier in the year that they are launched. Another conclusion based on the outcome of Kickstarters by launch date is that Kickstarters are most likely to be successful if launched in the month of May. This finding holds when assessing outcomes of all Kickstarters as well as the outcome of Kickstarters specifically in the theater category.

- What can you conclude about the Outcomes based on Goals?
        Based on the data gathered on Kickstarter outcomes based on goals, it can be concluded that there is a negative correlated between between donation goal and percentage of successful plays and a positive correlation between donation goal and failed plays. These data suggest that a play is more likely to be successful if the donation goal is less than $5000 with a 76% success rate with a donation goal of less than $1000 and a 73% success rate with a donation goal between $1000-$4999. 

- What are some limitations of this dataset?
        One limitation of this dataset is that it is not filtered for donation pledge outliers. Cleaning the dataset to eliminate outliers could elminate potential biases that are skewing the outcome of the data or causing and eliminating trends. Another limitation of this data is the is unequal distribution of Kickstarter categories. There is a large difference between the largest category, theater, with 1066 Kickstarters and the second largest, rock, with 260. With the large number of plays, play category data could be skewing the results and washing out any influence from other Kickstarter categories in the analysis. 

- What are some other possible tables and/or graphs that we could create?
        One possible table that could be created would be to assess the outcome of Kickstarer campaigns by category and subcategory and filter by the year started. This could be used to understand potential shifts in success and failures of certain fundraiser categories over time. A possible graph that could be created is to generate a stacked bar graph showing successful, failed, and cancelled Kickstarters by country. This could be used to assess which countries are the most successful to launch a Kickstarter campaign in. This data and graph could subsequently be filtered by category to determine which campaign type would be most successful or risky in your country. 
