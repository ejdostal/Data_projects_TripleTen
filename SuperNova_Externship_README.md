# SuperNova Externship - Health Inspection Records Analysis

This is a project I worked on during a two month long externship with SuperNova MGU. It was a great opportunity for me to gain some real world experience and to continue growing as a professional. Collaborating with two other data analysts and the team lead, we completed a big data project together from start to finish: from web scraping, to cleaning and pre-processing, to conducting analyses and creating data visualizations, to presentating final esults and recommendations to stakeholders. 


## SuperNova MGU

As mentioned above, this data project was coducted for the company, SuperNova MGU. SuperNova's mission is to redefine insurance excellence and it brings together a team of seasoned industry leaders dedicated to innovation and efficiency with a broker-centric approach. You can [read more SuperNova MGU here at their website. ](https://supernovamgu.com/)

<img width="1106" alt="Screenshot 2024-06-03 at 2 24 18 PM" src="https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/086c4cea-3d61-44b4-9bff-df5916323d6d">


## Health Inspection Records

The goal for this project was to analyze data avaliable online from a variety of different health inspection records for linkage with claims. Major milestones of the process included the scraping and collection of this data into a single, organized spreadsheet, the cleaning/normalizing of data columns sourced from different regions, the forming and communication of unique analyses and insights with collaborators, and the combining and consolidation of all major insights into a concise, informative presentation for stakeholders.


## The Data

The data we used to accomplish this came from 10 unique regions and was made up of a total of 112,811 unique inspection records. Our team lead, Mike Lee, was primarily responsible for web scraping of data, which was accomplished using Python Selenium and Jupyter Notebook. My fellow analysts and I participated closely in the scraping process through via observations of Mike's process, ongoing learning of basic Python structures and applications through a concurrent learning sprint, and ongoing workshops and office hours where we had opportunities to ask questions and attempt to replicate Mike's process. 

All data scraped was eventually aggregated into single spreadsheet for further analysis. Each row in the table represented a unique inspection record. A one-to-many relationship also existed between entities (business) and inspections:

- `url_inspection_full`: represents unique ID for each inspection report created
- `inspection_results`
- `actions_taken`
- `url_entity_full`: represents unique ID for each business
- `Facility Name`
- `Site Address`
- `Community`
- `Facility Type`
- `url_entry_partial`
- `category`: represents each category of health inspection within the website. (ie. Food premises, Enforcement, Water Quality etc.)
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


## The Process

Upon recieving the aggregated data, my fellow analysts and I each began our own unique explorations of the content. 

The first step I took in my analysis was to explore the data avaliable and make sure I understood the purpose and meaning of relevant columns. I clarified data column purposes and definitions by inspecting associated urls and consulting with the team lead as needed. 

Next, upon better understanding of data column similarities and differences, I worked to standardize and merge relevant columns for futher aggregation and analysis. As the content was scraped 10 different web sources, their were irregularities in human recording in many of the columns that required pre-processing before further analysis could be done. A combination of frequency analysis based on keywords, as well as functions and formulas, data slicing and some manual evaluation, was used to merge similar columns and aggregate values based on inspection result and inspection category. This process took up the most time. You can see greater detail about [the specifics of this process here in the find_and_change_log page. ](https://docs.google.com/spreadsheets/d/1ZwUbskAimnJ_r7CBGr2PWSiFIXGusyGLmnMqu_lA-Uk/edit?usp=sharing)

Then, I began aggregating and slicing data further based on some big picture questions I had regarding the data scraped, using a combination of both the original and newly normalized columns to orientate myself (and the client). In particular, my analysis focused on determining average pass/fail rate compositions by region and inspection category and their relations to one another.

Finally, I developed multiple data visualizations and charts with descriptive headers to represent my key findings in order make data comparison, understanding, and communication of major results easier to digest for stakeholders during final presentation. 

![Recreational Water and Food categories showed the highest rates of violation, total with inspections failing about 48% and 37% of the time, respectively]


## Results 

We met up again with the team lead to share and combine our findings. We each established unique stories to present based on our analyses and combined and consolidated them into a single, cohesive presentation to present to stakeholders.

As first speaker, I attempted to orientate the client by providing a bigger picture view of the data scraped and provide context for the significance of some of the key facts and figures. In particular, my portion of the presentation focused on conveying overall data makeup across region, inspection category and pass/fail rate and how these figures compared with one another. 

You can have a look at the [Google Sheets Workbook linked here ](https://docs.google.com/spreadsheets/d/1ZwUbskAimnJ_r7CBGr2PWSiFIXGusyGLmnMqu_lA-Uk/edit?usp=sharing) for a more detailed view of major analysis results as well as my portion of the [final presentation to SuperNova stakeholders here. ](https://docs.google.com/presentation/d/10mfSnhwbdKAL2EqM8qvk7jkkBh-F2K-GsZtmS3M1sqg/edit?usp=sharing) 

![Supernova_MGU_Externships_Erica](https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/d612c1bc-9857-478d-af42-f6038e99b9e8)

