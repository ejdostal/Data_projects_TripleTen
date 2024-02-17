# TripleTen Sprint 5 Project - Zomato

This is the final project I worked on in the TripleTen Business Intelligence Analyst program. It was a great opportunity to practice and review many of the new skills I learned throughout the curriculum. For this project, I given the choice between three major areas of analysis: customer analysis, resturaunt analysis, and sales analysis. For these datasets, I chose to focus on Zomato customers. 

### Zomato

Zomato is a multinational restaurant aggregator and food delivery service company. The goal of this project is to analyze the business performance of restaurants and customers registered to the Zomato service. In particular, I chose to focus on Zomato customers, their characteristics, and their purchasing behaviors.


#### The Data  
The data was spread across 5 files:

`users`: each row corresponds to a unique user id.   
- `user_id`  
- `name`  
- `email`  
- `password`  
- `Age`  
- `Gender`  
- `Marital Status`  
- `Occupation`  
- `Monthly Income`  
- `Educational Qualifications`  
- `Family size`   

`orders`:  each row corresponds to a unique order date.  
- `order_date`  
- `sales_qty`  
- `sales_amount`  
- `currency`  
- `user_id`  
- `r_id`  
   

`resturant`: each row corresponds to a unique resturant id.  
- `id`  
- `name`  
- `city`  
- `rating`  
- `rating_count`  
- `cost`  
- `cuisine`  
- `lic_no`   
- `link`  
- `address`  
- `menu`  

`menu`: each row corresponds to a unique menu id.  
- `menu_id`  
- `r_id`  
- `f_id`  
- `cuisine`  
- `price`  

`food`: each row corresponds to a unique food id.  
- `f_d`  
- `item`  
- `veg_or_non_veg`  
  
  
The data was provided by TripleTen.  


#### The Process

After reviewing the datasets and choosing an area of focus, I wrote and submitted a decomposition for approval. Upon recieving approval, I began my analysis in Tableau. I joined the datasets together, cleaned and preprocessed essential columns, converted currencies as necessary, and peformed aggregations. A number of visualizations and tables were created to help identify patterns, trends, and correlations of significance. Customers were segmented by their months of first purchase, and active user retention rates and revenue were calculated by cohort month by month. Finally, a report was prepared summarizing the key findings of the analysis as well as a dashboard for further customer analysis.

### Results 

The results of this analysis included a decomposition, a final report summarizing key analysis findings, and a dashboard for further analysis of Zomato customers. 


Please have a look at the Zomato customer analysis dashboard [linked here ](https://public.tableau.com/views/ZomatoCustomerAnalysisDashboard/CustomerCohortDashboard?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link)for a full description of results.
