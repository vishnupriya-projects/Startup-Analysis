# Startup-Analysis
Identification of financial factors thriving, currently operating &amp; cease operations startups using EDA and Hypothesis testing 
## Problem Statement
Company X, a leading Indian online publisher dedicated to startup industry insights, is driven by a mission to empower its audience with actionable knowledge. In the dynamic world of startups, the company recognizes the crucial need to answer a pivotal question: What financial factors differentiate thriving, currently operating startups from those that ultimately cease operations?
## Objective
To determine What are the financial factors differentiate thriving, currently operating startups from those that ultimately cease operations.
The following are the analysis conducted based on above objective.
1. Startup Characteristics:
- Examine the distribution of startups across different categories or industries to identify the most prevalent sectors.
- Investigate the distribution of startup statuses (e.g., operating, closed) to understand the success rates and longevity of startups.
2. Geographic distribution:
- Explore patterns in startup distribution across different states, and cities.
3. Funding Analysis:
- Analyze the distribution of funding amounts and rounds across different categories and regions.
4. Hypothesis testing:
#### Hypothesis 1: Funding Amount and Startup Success
- Null Hypothesis: There is no significant difference in the mean funding amount between successful startups (operating) and failed startups (closed).
- Alternative Hypothesis: Successful startups receive a significantly higher mean funding amount compared to failed startups.
- Analysis: Conduct a t-test or ANOVA to compare the funding amounts of successful and failed startups and determine if there is a statistically significant difference.
#### Hypothesis 2: Relationship between number of funding rounds for operating Startups & closed startups
- Null Hypothesis: There is no significant difference in the no. of funding rounds between successful startups (operating) and failed startups (closed).
- Alternative Hypothesis: There is a significant difference in the no. of funding rounds between successful startups (operating) and failed startups (closed).
- Analysis: Perform a chi-square test or ANOVA to investigate if there are significant differences in the number of funding rounds between successful startups (operating) and failed startups (closed).
## Data
Startup_Data.csv- : The data set contains information of various startups around the world.
Dataset Credits --> https://www.kaggle.com/datasets/yanmaksi/big-startup-secsees-fail-dataset-from-crunchbase
Filter on country and status column to get particular country analaysis.
The following analysis was carried for indian startup-ecosystem.
## Data Cleaning and Preparation:
- we require category_list, city columns which are having missing values, funding_total_usd , status, funding_rounds have no missing values. 
- The category_list has multiple words, we need to extract common words to obtain a defined category.
- Region has duplicate names, which need to fix.
## Data Analysis & Insights:
- The average funding is 23 million dollars, max funding was 3 billion dollars, min was 569 dollars.
- In terms of funding rounds, avg funding round for all startups was '1', min funding round also '1' representing every startup has at-least '1' funding rounds & max no of funding rounds happen was '12'.
- Among all sectors, E-commerce, education, software, internet & web are the categories having the major startups.
- In total 1134 startups, Majority of startups(1085) are still in operating state & very few (49) are closed.
- Among closed startups, E-commerce based are closed majorly followed by adverstising, finance & IT.
- Majority of closed startups belong to banglore & mumbai followed by delhi, chennai regions.
- Almost All The Startups Are At Banglore, Delhi & Mumbai Follwed By Hyderabad, Chennai, Pune. Remaining All Other Places Have Very Few Startups Which Are Less Than 20. This Representing that Majority of Startups Are Growing In Major Metro Cities Than Other Regions In India.
- In terms of region wise fundings, even though Bangalore has highest number of startups (300), delhi gained overall higher funding amount(86 billion dollars) followed by mumbai(67 billion dollars), Bangalore (64 billion dollars), kolkata (12 billion dollars) & chennai (10 billion dollars).
- This represents the funding amount was given based on value/popularity of startup.
- In the number of funding rounds distribution we see that very few companies having higher funding rounds.
- considering funding rounds >=7 to find which companies having more funding amount with high success rates are flipkart, snapdeal are in top in terms of funding rounds followed by zomato, ola, manthan systems with 8 to 7 rounds of funding respectively, all these 5 companies are in top players in recent times in their categories which represents higher funding rounds.
- It represents their could be a possible relationship b/w funding amount, funding rounds with startup success. To understand it further lets run statistical analysis.
- Based on the statistical analyses conducted, it can be concluded that:
There is no statistically significant difference in the funds raised by currently operating startups and startups that have closed, as per the independent sample t-test.
There is no statistically significant association between the number of funding rounds and the status of startups, as indicated by the Chi-Square Test of Independence.

### Acknowledgement
Thanks to @aditi @dataanalystduo team for providing dataset & their guidence throughout the project.


