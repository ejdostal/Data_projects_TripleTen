# Project 3 - Superstore Operations Analysis

This is the third project I worked on in the TripleTen Business Intelligence Analyst program. It was my first experience completing an analysis in Tableau and it was a great opportunity for me to explore the software's unique data visualization features, including calculations, filters and parameters.  

### Superstore Operations

The goal of this project was to review the Superstore's overall business operations and to identify ways it might increase store profitability. The question of whether advertising might be worth it in some places and times was also posed.

![superstore logo](https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/dfb9d239-bff1-4093-8a1d-4c1aa2de2c2d)

### The Data

The data was spread across 2 files: `Orders` and `Returns`.

`Orders` : Each row corresponded to a unique order placed at the Superstore.
- `Row ID` 
- `Order ID` 
- `Order Date` 
- `Ship Mode` 
- `Customer ID`   
- `Customer Name` 
- `Segment` 
- `Country / Region` 
- `City` 
- `State` 
- `Postal Code` 
- `Region`
- `Product ID` 
- `Category` 
- `Sub-Category` 
- `Product Name` 
- `Sales` 
- `Quantity` 
- `Discount` 
- `Profit` 

`Returns` : Each row corresponded to a unique order returned to the Superstore.
- `Returned` 
- `Order ID` 

This data was provided by TripleTen, who recieved it from Tableau.

### The Process

First, I uploaded the two datasets to Tableau and joined them based on unique Order ID. Next, I created Calculations to pre-process the data and prepare it for aggregation and measurement. Then, I assessed average profit by Region and Sub-Category and determined the states and months with highest average sales. The latter information helped me to determine advertising recommendations, which were based on a Return On Ad Spend (ROA) ratio of 1/5 of profits. Return rates were then calculated by Customer Segment and Product Sub-Category. Finally, annotations and visualizations utilizing parameters and filters were created to summarize and clarify key analysis conclusions.

<img width="650" alt="Screenshot 2024-02-16 at 8 16 39 PM" src="https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/87473c2b-3fc3-478a-b629-cdd3c0ead0c8">

<img width="1035" alt="Screenshot 2024-02-16 at 8 13 30 PM" src="https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/99596c6c-7db0-4b78-b70f-7b361d8c04ca">

<img width="1192" alt="Screenshot 2024-02-16 at 8 14 05 PM" src="https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/e8775ef1-b9d9-4f50-9e91-b30cba4da184">

<img width="806" alt="Screenshot 2024-02-16 at 8 16 06 PM" src="https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/9ef67bfe-0aab-4513-b8f6-eb973469dfe9">


### Results 
Visualizations and annotations described the two biggest profit centers and loss makers for the Superstore, by both Sub-Category and Region. Customer Segments and Sub-Categories with highest return rates were identified. Final recommendations were also provided as to which product Sub-Categories to consider discontinuing and which to devote more time and resources to. Suggestions were made as to which states and time periods might be most impactful to advertise in, as well as the maximum spending amount of spending to consider.

Please have a look at the Tableau Workbook [linked here ](https://public.tableau.com/views/SuperstoreProfitsandLosses/Top2Sub-CategoriesTotalProfitRegion?:language=en-US&:display_count=n&:origin=viz_share_link)for a full description of results.
