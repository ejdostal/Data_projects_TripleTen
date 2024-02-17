# TripleTen Sprint 3 Project - Superstore Profits & Losses

This is the 3rd project I worked on in the TripleTen Business Intelligence Analyst program. It was my first experience completing an analysis in Tableau and it was a great opportunity to explore the software's unique data visualization features, including Calculations, Filters and Parameters.  

### E-Commerce Cohort Analysis

The goal of this project is to review the business operations and identify ways the Superstore might increase profitability to avoid bankruptcy. The question of whether advertising might be worth it was also posed.

#### The Data

The data was spread across 2 files:

`Orders` : Each row corresponds to a unique order placed at the Superstore.
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

`Returns` : Each row corresponds to unique order that was returned to the Superstore.
- `Returned` 
- `Order ID` 

The data is provided by TripleTen, who got it from Tableau.

#### The Process

First, I joined the data in Tableau on unique Order ID. Then I wrote calculations to prepare data for aggregation and measurement. Then I assessed the Regions and Sub-Categories dimensions based on average profit and determined which states in which months had highest average profits to determine advertising recommendations. (Ad spending recommendations were calculated based on a return on ad spend ratio of 1/5 of profits.) Finally, return rates were calculated by Customer Segment and Sub-Category. Annotations and visualizations with parameters and filters were created to summarize and clarify key results from the analysis.

### Results 
Visualizations and annotations were developed describing the 2 the two biggest profit centers and 2 biggest loss makers for the Superstore by both Sub-Category and Region. Recommendations were provided as to which Sub-Categories to discontinue and which would be worth focusing more on. Recommendations were also provided as to when and where advertising could be beneficial and what the SuperStore might be willing to pay in advertising for those states in those months. Customer Segments and Sub-Categories with highest return rates were identified and final recommendations given.

Please have a look at the Google Sheets Workbook [linked here ](https://public.tableau.com/views/SuperstoreProfitsandLosses/Top2Sub-CategoriesTotalProfitRegion?:language=en-US&:display_count=n&:origin=viz_share_link)for a full description of results.
