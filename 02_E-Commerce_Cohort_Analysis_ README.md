# Project 2 - E-Commerce Cohort Analysis

This is the 2nd project I worked on in the TripleTen Business Intelligence Analyst program. It was a great opportunity to work with transaction logs and practice using them to analyze website performance.

### E-Commerce Cohort Analysis

The goal of this project was to help an e-commerce team understand how well their website was converting product page views into purchases. It was a good opportunity to practice building conversion funnels and aggregating customers into cohorts based on their months of first purchase.

![e-commerce website](https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/1b54ddaf-ad88-47f2-ba64-2ae23c5a3d13)

### The Data

The data included one website transaction log: `raw_user_activity`.  
  
`raw_user_activity`
- `user_id`: unique customer IDs
- `event_type`: the type of activity by the user
- `category_code`: category of the product being viewed or purchased
- `brand`: company that makes the product
- `price`: price of the product, in USD
- `event_date`: date of the user activity, in `YYYY-MM-DD` format

This data was provided by TripleTen.

### The Process

First, I built a conversion funnel, outlining each stage of the funnel and customer retention by step. Then I prepared the raw transactional data for cohort analysis by filtering purchases and performing necessary calculations. Cohorts were then aggregated and further analyzed individually and cumulatively month by month.

<img width="583" alt="Screenshot 2024-02-16 at 7 49 26 PM" src="https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/330ea44d-abe3-407c-9508-0682f31d08d9">

<img width="705" alt="Screenshot 2024-02-16 at 7 48 40 PM" src="https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/6221ba89-bd7a-42d5-8cb0-1d184fab7b5a">

<img width="666" alt="Screenshot 2024-02-16 at 7 48 59 PM" src="https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/65ef3b72-0c5b-48b1-ba85-5e99a1f5ab15">


### Results 
Total customer conversion rates and conversion rates from step to step in the funnel were calculated to determine how often customers who visited the website went on to make a purchase. Total customer retention rate and retention rate by cohorts month by month were also determined to analyze how frequently customers who made an initial purchase came back to make additional purchases with the company. A summary of analysis findings can be found in the Executive Summary tab within the Google Sheets Workbook linked below, as well as practical recommendations for the e-commerce company moving forward based off of those findings. 

<img width="447" alt="Screenshot 2024-02-16 at 7 47 50 PM" src="https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/a9516f2e-d934-4ce6-9edc-764e232ee126">


Please have a look at the Google Sheets Workbook [linked here ](https://docs.google.com/spreadsheets/d/1Zt4jZ3kDbDwjamdXg27JpeNK1POlpxEzIytspTWkBwc/edit?usp=sharing)for a full description of results.

### Idea for Improvement
If I were to continue working on this project, I would probably change the intensity of the colors used in the Table of Contents tab. While I know it seems minor, I think it might distract from the content and even make the workbook a bit harder to navigate. I'd probably change the colors to something a little less busy and more readable.
