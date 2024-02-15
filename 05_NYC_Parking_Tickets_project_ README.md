# TripleTen Hackathon Project - NYC Parking Tickets

This is a project I worked on with a team of other professionals during the Dec 2023 Hackathon hosted by TripleTen. It was a great opportunity to work with other students and graduates of the program and gain exposure to some different ways of looking at and approached data problems. I really enjoyed the experience of meeting other professionals and getting to work with people all over the world.

### NYC Parking Tickets

The goal of this project is to provide a report to a private parking providing company about their potential growth in NYC. In particular, the tickets were analyzed to identify specific times and places that parking might be more in demand. Information about the types of cars ticketed were also of interest to identify potential target markets.

#### The Data

4 datasets were used for this analysis, each correlating to a fiscal year between 2014 and 2017. For all datasets, each row corresponded to a unique summons number associated with a ticket.


`Parking_Violations_Issued_-_Fiscal_Year_2014__August_2013___June_2014` 

`Summons Number`: Nu 
`Plate ID`: Plain Text
`Registration State`: Plain Text
`Plate Type`: Plain Text
`Issue Date`: Date & Time
`Violation Code`: Number
`Vehicle Body Type`: Plain Text
`Vehicle Make`: Plain Text
`Issuing Agency`: Plain Text
`Street Code1`: Number
`Street Code2`: Number
`Street Code3`: Number
`Vehicle Expiration Date`: Number
`Violation Location`: Plain Text
`Violation Precinct`: Number
`Issuer Precinct`: Number
`Issuer Code`: Number
`Issuer Command`: Plain Text
`Issuer Squad`: Plain Text
`Violation Time`: Plain Text
`Time First Observed`: Plain Text
`Violation County`: Plain Text
`Violation In Front Of Or Opposite`: Plain Text
`House Number`: Plain Text
`Street Name`: Plain Text
`Intersecting Street`: Plain Text
`Date First Observed`: Number
`Law Section`: Number
`Sub Division`: Plain Text
`Violation Legal Code`: Plain Text
`Days Parking In Effect`: Plain Text
`From Hours In Effect`: Plain Text
`To Hours In Effect`: Plain Text
`Vehicle Color`: Plain Text
`Unregistered Vehicle?`: Plain Text
`Vehicle Year`: Number
`Meter Number`: Plain Text
`Feet From Curb`: Number
`Violation Post Code`: Plain Text
`Violation Description`: Plain Text
`No Standing or Stopping Violation`: Plain Text
`Hydrant Violation`: Plain Text
`Double Parking Violation`: Plain Text


`Parking_Violations_Issued_-_Fiscal_Year_2015`

`Summons Number`: Number
`Plate ID`: Plain Text
`Registration State`: Plain Text
`Plate Type`: Plain Text
`Issue Date`: Date & Time
`Violation Code`: Number
`Vehicle Body Type`: Plain Text
`Vehicle Make`: Plain Text
`Issuing Agency`: Plain Text
`Street Code1`: Number
`Street Code2`: Number
`Street Code3`: Number
`Vehicle Expiration Date`: Number
`Violation Location`: Plain Text
`Violation Precinct`: Number
`Issuer Precinct`: Number
`Issuer Code`: Number
`Issuer Command`: Plain Text
`Issuer Squad`: Plain Text
`Violation Time`: Plain Text
`Time First Observed`: Plain Text
`Violation County`: Plain Text
`Violation In Front Of Or Opposite`: Plain Text
`House Number`: Plain Text
`Street Name`: Plain Text
`Intersecting Street`: Plain Text
`Date First Observed`: Number
`Law Section`: Number
`Sub Division`: Plain Text
`Violation Legal Code`: Plain Text
`Days Parking In Effect`: Plain Text
`From Hours In Effect`: Plain Text
`To Hours In Effect`: Plain Text
`Vehicle Color`: Plain Text
`Unregistered Vehicle?`: Plain Text
`Vehicle Year`: Number
`Meter Number`: Plain Text
`Feet From Curb`: Number
`Violation Post Code`: Plain Text
`Violation Description`: Plain Text
`No Standing or Stopping Violation`: Plain Text
`Hydrant Violation`: Plain Text
`Double Parking Violation`: Plain Text
`Latitude`: Number
`Longitude`: Number
`Community Board`: Number
`Community Council`: Number
`Census Tract`: Number
`BIN`: Number
`BBL`: Number
`NTA`: Plain Text


`Parking_Violations_Issued_-_Fiscal_Year_2016`

`Summons Number`: Number
`Plate ID`: Plain Text
`Registration State`: Plain Text
`Plate Type`: Plain Text
`Issue Date`: Date & Time
`Violation Code`: Number
`Vehicle Body Type`: Plain Text
`Vehicle Make`: Plain Text
`Issuing Agency`: Plain Text
`Street Code1`: Number
`Street Code2`: Number
`Street Code3`: Number
`Vehicle Expiration Date`: Number
`Violation Location`: Plain Text
`Violation Precinct`: Number
`Issuer Precinct`: Number
`Issuer Code`: Number
`Issuer Command`: Plain Text
`Issuer Squad`: Plain Text
`Violation Time`: Plain Text
`Time First Observed`: Plain Text
`Violation County`: Plain Text
`Violation In Front Of Or Opposite`: Plain Text
`House Number`: Plain Text
`Street Name`: Plain Text
`Intersecting Street`: Plain Text
`Date First Observed`: Number
`Law Section`: Number
`Sub Division`: Plain Text
`Violation Legal Code`: Plain Text
`Days Parking In Effect`: Plain Text
`From Hours In Effect`: Plain Text
`To Hours In Effect`: Plain Text
`Vehicle Color`: Plain Text
`Unregistered Vehicle?`: Plain Text
`Vehicle Year`: Number
`Meter Number`: Plain Text
`Feet From Curb`: Number
`Violation Post Code`: Plain Text
`Violation Description`: Plain Text
`No Standing or Stopping Violation`: Plain Text
`Hydrant Violation`: Plain Text
`Double Parking Violation`: Plain Text
`Latitude`: Number
`Longitude`: Number
`Community Board`: Number
`Community Council`: Number
`Census Tract`: Number
`BIN`: Number
`BBL`: Number
`NTA`: Plain Text

`Parking_Violations_Issued_-_Fiscal_Year_2017`
`Summons Number`: Number
`Plate ID`: Plain Text
`Registration State`: Plain Text
`Plate Type`: Plain Text
`Issue Date`: Date & Time
`Violation Code`: Number
`Vehicle Body Type`: Plain Text
`Vehicle Make`: Plain Text
`Issuing Agency`: Plain Text
`Street Code1`: Number
`Street Code2`: Number
`Street Code3`: Number
`Vehicle Expiration Date`: Number
`Violation Location`: Plain Text
`Violation Precinct`: Number
`Issuer Precinct`: Number
`Issuer Code`: Number
`Issuer Command`: Plain Text
`Issuer Squad`: Plain Text
`Violation Time`: Plain Text
`Time First Observed`: Plain Text
`Violation County`: Plain Text
`Violation In Front Of Or Opposite`: Plain Text
`House Number`: Plain Text
`Street Name`: Plain Text
`Intersecting Street`: Plain Text
`Date First Observed`: Number
`Law Section`: Number
`Sub Division`: Plain Text
`Violation Legal Code`: Plain Text
`Days Parking In Effect`: Plain Text
`From Hours In Effect`: Plain Text
`To Hours In Effect`: Plain Text
`Vehicle Color`: Plain Text
`Unregistered Vehicle?`: Plain Text
`Vehicle Year`: Number
`Meter Number`: Plain Text
`Feet From Curb`: Number
`Violation Post Code`: Plain Text
`Violation Description`: Plain Text
`No Standing or Stopping Violation`: Plain Text
`Hydrant Violation`: Plain Text
`Double Parking Violation`: Plain Text

The data was provided by TripleTen, who got it from [Kaggle](https://www.kaggle.com/datasets/new-york-city/nyc-parking-tickets), who got it from the NYC Department of Finance.


#### The Process

Once we were assigned teams, we got together via Zoom to go over our roles and and assess the data avaliable to us. We decided to split the workload up into 3 major sub-groups for efficiency: cleaning, analysis and conclusions. After one pair of analysts finished cleaning and joining the dataset to prepare it analysis, the next pair recieved it to analyze for relevant questions and develop visualizations. Finally, then the last pair recieved it to condense and summarize key conclusions in a presentation for the client. My primary role was on the conclusions team. It was my job to develop a presentation that adequately summarized the steps my teammates took, clarified any assumptions that were made during in analysis process, and offered some practical recommendations for next steps for the business.

### Results 

The results of this analysis included a Tableau Story presentation in which key analysis findings and recommendations were presented to the judges.

Please have a look at the [ NYC Parking Tickets analysis ](https://public.tableau.com/views/NYCParkingTickets_17079577730140/NYCParkingTickets?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link) presentation linked here for a full description of results.
