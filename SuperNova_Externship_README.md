# SuperNova Externship - Health Inspection Records Analysis

This is a project I worked on as part of a two month long externship with SuperNova MGU. It was a valuable opportunity for me to gain some real world experience and to continue growth as a professional. Collaborating with two other data professionals under the team lead, we completeda big data project was completed from start to finish: from the scraping of data, to cleaning and pre-processing process, to conducting unique analyses and estabishing informative data visualizations, to the presentation of major results and data recommendations to stakeholders. 

# SuperNova MGU

As mentioned above, this externship was hosted by SuperNova MGU. SuperNova seeks to redefine insurance excellence  company brings together a team of seasoned industry leaders dedicated to innovation and efficiency with a broker-centric approach. You can [read more SuperNova MGU here at their website.] (https://supernovamgu.com/) 

### Health Inspection Records

The goal for this externship was to analyze data avaliable online from a variety of unique health inspection records and violations for insights and linkage with claims. Major milestones of this process included the scraping and collection of the data in a spreadsheet, the cleaning/standardizing of collected data with irregularities, the forming and sharing of unique analyses and insights, and the combining of all major analysis results into a single, cohesive presentation to stakeholders.

#### The Data

The data we used to accomplish this came from 10 unique health units and was composed of a total of 112,811 unique inspection records. Our team lead, Mike Lee, was primarily responsible for the scraping of data, which was accomplished using Python Selenium and Jupyter Notebook. My fellow analysts and I participated closely in this web scraping process through live observations of Mike's process, ongoing learning of basic Python a through a concurrent learning sprint course, and ongoing workshops and office hours where we had opportunities to ask questions and try to replicate Mike's process. 

All web data scraped was combined into single spreadsheet for further analysis. Each row represented in the table represented a unique inspection record and a one-to-many relationship between entities (business) and inspections:

- `url_inspection_full`: represents unique ID for each inspection report created
- `inspection_results`
- `actions_taken`
- `url_entity_full`: represents unique ID for each business
- `Facility Name`
`Site Address`
`Community`
`Facility Type`
`url_entry_partial`
`category`: represents each category of health inspection within the website. (ie. Food premises, Enforcement, Water Quality etc.)
- `Enforcement`
- `Action Taken`
- `Status`
- `Date of Issuance`
- `Details`
- `Status Data`
- `source`: which health unit or region the info came from
- `Last Inspection Date`
- `Services Inspected`
- `Type`
- `Offense`
- `Outcome`
- `Offense Date`
- `Comment`
- `Resolved Date`
- `Colour Posting`
- `Legislation`
- `Offence Date`
- `Description`
- `Status Updated`
- `Name`
- `Address`
- `Inspection Result`
- `Risk Rating`
- `Date Issued`
- `Date of Conviction`
- `Program Area`
- `Reason`
- `Reopen Date`


#### The Process

Upon recieving the aggregated data, we each began our unique explorations of the content. 

The very first step I took was to explore the data avaliable and make sure I understood the purpose and meaning of relevant columns. I clarified data column purposes and definitions where necessary through the inspection of associated urls as well as through consultations with the team lead. 

Next, upon clearer understanding of column similarities and differences, I worked to standardize relevant columns for futher aggregation and analysis through pre-processing. As the content came scraped 10 different web sources, their were irregularities in human recording in many of the columns. Frequency analysis based on common keywords was required to merge similar columns and aggregate findings based on their pass/fail rates and associated inspection categories. This was done through a combination of functions and formulas, data slicing, and manual evaluation. This data cleaning process took up a majority of the time. You can see much greater detail about my approach here in the find_and_change_log page.

After, I began aggregating and slicing data based on some big picture questions I had regarding the data. I used a combination of original and newly normalized columns to orientate myself (and the client) to get a better understanding of the scraped data and it's significance. I went on to determining average pass/fail rates by region and inspection categories, as well overall composition of the data to determine result significance.

As a final step, I developed multiple data visualizations and charts with descriptive headers to represent key findings in make data comparison, understanding, and communication of major results easier to digest for stakeholders. 

### Results 

My fellow analysts and I met up again with the team lead to share and aggregate our findings. We worked together to establish unique stories based our on our own unique analyses and then combined them into a single final presentation to stakeholders, providing a wealth of unique insights for the stakeholder to pull from.

For my own unique data story, I tried orientate the client by providing a bigger picture view of the data scraped. As the first presenter, my goal was to convey the major results of the web scrape and provide context for the significance of some of the key facts and figures. In particular, my presentation focused on conveying data makeup across region, inspection category and pass/fail rate and how these figures compared with one another. 

You can have a look at the [Google Sheets Workbook linked here ](https://docs.google.com/spreadsheets/d/1RJXpP5sq4VEvNBJWPpVhWK2vMkSgRY1oYPffN4hywLo/edit?usp=sharing)for a more detailed view of major analysis results as well as [my final presentation to stakeholder here].(https://docs.google.com/presentation/d/10mfSnhwbdKAL2EqM8qvk7jkkBh-F2K-GsZtmS3M1sqg/edit?usp=sharing) 
