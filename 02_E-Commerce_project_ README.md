## TripleTen Sprint 2 Project - E-Commerce Cohort Analysis

This is the 2nd project I worked on in the TripleTen Business Intelligence Analyst program. It was a great opportunity to work with transaction logs and use them to analyze website performance.

### E-Commerce Cohort Analysis

The goal of this project is to help an e-commerce team understand how well their website is converting product page views into purchases. 

#### The Data

The data included one raw_user_activity transaction log:

- `'user_id:'` unique customer IDs
- `'event_type:'` the type of activity by the user
- `'category_code:'` category of the product being viewed or purchased
- `'brand:'` company that makes the product
- `'price:'` price of the product, in USD
- `'event_date:'` date of the user activity, in YYYY-MM-DD format

The data is provided by TripleTen.

#### The Process

First I built a conversion funnel outlining each stage of the funnel and customer retention by step. Then I prepared the raw transactional data for cohort analysis by filtering purchases and performing key calculations. Cohorts were then aggregated and further analyzed individually and cumulatively month by month.

### Results 
Total customer conversion rates and conversion rates from step to step in the funnel were calculated to determine how often customers who visited the website went on to make a purchase. Total customer retention rate and retention rates by cohorts month by month were also determined to analyze how frequently customers who made an initial purchase came back to make additional purchases with the compnay. A summary of analysis findings can be found in the Executive Summary as well as practical recommendations the e-commerce comany might consider moving forward. 


Please have a look at the [Google Sheets Workbook linked here ](https://docs.google.com/spreadsheets/d/1Zt4jZ3kDbDwjamdXg27JpeNK1POlpxEzIytspTWkBwc/edit?usp=sharing)for a full description of results.
