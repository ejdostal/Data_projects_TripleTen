# Project 5 - NYC Parking Tickets Analysis
This is a project I worked on with a team of other analysts as part of a Dec 2023 - Jan 2024 Data Hackathon hosted by TripleTen. During this hackathon, each team was given a dataset to analysis and asked solve specific business problems. This experience was a great one for a lot of reasons, not the least of which because it gave us an opportunity to collaborate with other analysts, practice with new datasets, and observe how others approached business problems differently. 

<img width="1204" alt="Screenshot 2024-02-14 at 2 57 11 PM" src="https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/f8dee051-9168-4704-9054-38afe356af7e">

### NYC Parking Tickets
My team was asked to provide a report for a private parking providing company about their possible growth in NYC using a dataset on parking violations from the NYC Department of Finance. We were asked to analyze the data for relevant insights, including the most popular parking areas and vehicle types, tickets info, and seasonality.


#### The Data  
The data was spread across 4 files and covered information collected by the NYC Department of Finance on parking violations from August 2013 to June 2017.

`Parking_Violations_Issued_-_Fiscal_Year_2014__August_2013___June_2014` 

- `Summons Number`: Nu  
- `Plate ID`: Plain Text  
- `Registration State`: Plain Text  
- `Plate Type`: Plain Text  
- `Issue Date`: Date & Time  
- `Violation Code`: Number  
- `Vehicle Body Type`: Plain Text  
- `Vehicle Make`: Plain Text  
- `Issuing Agency`: Plain Text  
- `Street Code1`: Number  
- `Street Code2`: Number  
- `Street Code3`: Number  
- `Vehicle Expiration Date`: Number  
- `Violation Location`: Plain Text   
- `Violation Precinct`: Number   
- `Issuer Precinct`: Number   
- `Issuer Code`: Number  
- `Issuer Command`: Plain Text   
- `Issuer Squad`: Plain Text  
- `Violation Time`: Plain Text  
- `Time First Observed`: Plain Text   
- `Violation County`: Plain Text  
- `Violation In Front Of Or Opposite`: Plain Text  
- `House Number`: Plain Text  
- `Street Name`: Plain Text  
- `Intersecting Street`: Plain Text   
- `Date First Observed`: Number  
- `Law Section`: Number  
- `Sub Division`: Plain Text  
- `Violation Legal Code`: Plain Text  
- `Days Parking In Effect`: Plain Text  
- `From Hours In Effect`: Plain Text  
- `To Hours In Effect`: Plain Text  
- `Vehicle Color`: Plain Text  
- `Unregistered Vehicle?`: Plain Text  
- `Vehicle Year`: Number   
- `Meter Number`: Plain Text  
- `Feet From Curb`: Number   
- `Violation Post Code`: Plain Text  
- `Violation Description`: Plain Text  
- `No Standing or Stopping Violation`: Plain Text  
- `Hydrant Violation`: Plain Text   
- `Double Parking Violation`: Plain Text   

     
`Parking_Violations_Issued_-_Fiscal_Year_2015`   

- `Summons Number`: Number  
- `Plate ID`: Plain Text  
- `Registration State`: Plain Text  
- `Plate Type`: Plain Text   
- `Issue Date`: Date & Time   
- `Violation Code`: Number  
- `Vehicle Body Type`: Plain Text  
- `Vehicle Make`: Plain Text  
- `Issuing Agency`: Plain Text  
- `Street Code1`: Number  
- `Street Code2`: Number  
- `Street Code3`: Number  
- `Vehicle Expiration Date`: Number  
- `Violation Location`: Plain Text  
- `Violation Precinct`: Number  
- `Issuer Precinct`: Number  
- `Issuer Code`: Number  
- `Issuer Command`: Plain Text  
- `Issuer Squad`: Plain Text  
- `Violation Time`: Plain Text  
- `Time First Observed`: Plain Text  
- `Violation County`: Plain Text  
- `Violation In Front Of Or Opposite`: Plain Text   
- `House Number`: Plain Text   
- `Street Name`: Plain Text  
- `Intersecting Street`: Plain Text  
- `Date First Observed`: Number  
- `Law Section`: Number  
- `Sub Division`: Plain Text  
- `Violation Legal Code`: Plain Text  
- `Days Parking In Effect`: Plain Text  
- `From Hours In Effect`: Plain Text  
- `To Hours In Effect`: Plain Text  
- `Vehicle Color`: Plain Text   
- `Unregistered Vehicle?`: Plain Text     
- `Vehicle Year`: Number  
- `Meter Number`: Plain Text  
- `Feet From Curb`: Number  
- `Violation Post Code`: Plain Text  
- `Violation Description`: Plain Text  
- `No Standing or Stopping Violation`: Plain Text  
- `Hydrant Violation`: Plain Text  
- `Double Parking Violation`: Plain Text  
- `Latitude`: Number  
- `Longitude`: Number  
- `Community Board`: Number  
- `Community Council`: Number  
- `Census Tract`: Number  
- `BIN`: Number  
- `BBL`: Number  
- `NTA`: Plain Text

`Parking_Violations_Issued_-_Fiscal_Year_2016`  

- `Summons Number`: Number   
- `Plate ID`: Plain Text  
- `Registration State`: Plain Text  
- `Plate Type`: Plain Text  
- `Issue Date`: Date & Time  
- `Violation Code`: Number  
- `Vehicle Body Type`: Plain Text  
- `Vehicle Make`: Plain Text  
- `Issuing Agency`: Plain Text  
- `Street Code1`: Number  
- `Street Code2`: Number  
- `Street Code3`: Number  
- `Vehicle Expiration Date`: Number  
- `Violation Location`: Plain Text  
- `Violation Precinct`: Number  
- `Issuer Precinct`: Number  
- `Issuer Code`: Number  
- `Issuer Command`: Plain Text  
- `Issuer Squad`: Plain Text  
- `Violation Time`: Plain Text  
- `Time First Observed`: Plain Text  
- `Violation County`: Plain Text  
- `Violation In Front Of Or Opposite`: Plain Text  
- `House Number`: Plain Text  
- `Street Name`: Plain Text  
- `Intersecting Street`: Plain Text  
- `Date First Observed`: Number  
- `Law Section`: Number  
- `Sub Division`: Plain Text  
- `Violation Legal Code`: Plain Text  
- `Days Parking In Effect`: Plain Text  
- `From Hours In Effect`: Plain Text  
- `To Hours In Effect`: Plain Text  
- `Vehicle Color`: Plain Text  
- `Unregistered Vehicle?`: Plain Text  
- `Vehicle Year`: Number  
- `Meter Number`: Plain Text  
- `Feet From Curb`: Number  
- `Violation Post Code`: Plain Text  
- `Violation Description`: Plain Text  
- `No Standing or Stopping Violation`: Plain Text   
- `Hydrant Violation`: Plain Text  
- `Double Parking Violation`: Plain Text  
- `Latitude`: Number  
- `Longitude`: Number  
- `Community Board`: Number  
- `Community Council`: Number  
- `Census Tract`: Number  
- `BIN`: Number  
- `BBL`: Number  
- `NTA`: Plain Text  

`Parking_Violations_Issued_-_Fiscal_Year_2017`  

- `Summons Number`: Number  
- `Plate ID`: Plain Text  
- `Registration State`: Plain Text  
- `Plate Type`: Plain Text  
- `Issue Date`: Date & Time  
- `Violation Code`: Number  
- `Vehicle Body Type`: Plain Text  
- `Vehicle Make`: Plain Text  
- `Issuing Agency`: Plain Text  
- `Street Code1`: Number  
- `Street Code2`: Number  
- `Street Code3`: Number  
- `Vehicle Expiration Date`: Number  
- `Violation Location`: Plain Text  
- `Violation Precinct`: Number  
- `Issuer Precinct`: Number  
- `Issuer Code`: Number  
- `Issuer Command`: Plain Text   
-`Issuer Squad`: Plain Text   
- `Violation Time`: Plain Text  
- `Time First Observed`: Plain Text  
- `Violation County`: Plain Text  
- `Violation In Front Of Or Opposite`: Plain Text  
- `House Number`: Plain Text  
- `Street Name`: Plain Text  
- `Intersecting Street`: Plain Text  
- `Date First Observed`: Number  
- `Law Section`: Number  
- `Sub Division`: Plain Text  
- `Violation Legal Code`: Plain Text  
- `Days Parking In Effect`: Plain Text  
- `From Hours In Effect`: Plain Text  
- `To Hours In Effect`: Plain Text  
- `Vehicle Color`: Plain Text  
- `Unregistered Vehicle?`: Plain Text  
- `Vehicle Year`: Number  
- `Meter Number`: Plain Text  
- `Feet From Curb`: Number  
- `Violation Post Code`: Plain Text  
- `Violation Description`: Plain Text  
- `No Standing or Stopping Violation`: Plain Text  
- `Hydrant Violation`: Plain Text  
- `Double Parking Violation`: Plain Text  


This data was provided by TripleTen, who got it from Kaggle.  


#### The Process

First our team met via Zoom and went over the NYC Department of Finance dataset. We clarified what our analysis goals were and identified the provided data most likely to be helpful to our purpose. Then we split up team responsibilities and allocated project roles. One group was assigned responsibility for cleaning the dataset and and joining the data into a single file. A second group was responsible for conducting the analysis from the newly cleaned dataset. Finally, a third group was responsible for consolidating the findings into final conclusions and offering business recommendations in a final report for stakeholders. I was a part of the third group.

Upon recieving a cleaned dataset as well as a wealth of data findings from the analysis process, we reviewed, summarized/ consolidated analysis findings into final conclusions. We organized our report into slides explaining findings based on location, time, and vehicle type. At the beginning of the presentation we made sure to include any assumptions recorded by our teams during the cleaning and analysis processes as well as a review of the key questions this analysis intended to answer. At the end of the presentation we offered relevant business recommendations based off the conclusions drawn from the analysis.

<img width="1094" alt="Screenshot 2024-03-15 at 2 23 21 PM" src="https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/bf73b782-10d5-47b7-8fdb-9a5149d8ac55">

<img width="1094" alt="Screenshot 2024-03-15 at 2 23 29 PM" src="https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/534e90c7-4bb9-4f6e-a903-c741c1fa7b4a">


### Results 

The results of this analysis included a final, cleaned dataset, a Jupiter notebook with findings and visuals gathered from the data analysis, and a final Tableau Story presentation reporting key conclusions and business recommendations based on group analysis findings.


Please have a look at the [final presentation ](https://public.tableau.com/views/NYCParkingTickets_17079577730140/NYCParkingTickets?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link)linked here for a full description of results.

