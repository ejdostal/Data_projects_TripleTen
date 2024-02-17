# TripleTen Sprint 1 Project - NYC Airbnb Properties

This is the 1st project I worked on in the TripleTen Business Intelligence Analyst program. It was a great opportunity for me to practice and combine many of the skills I learned about working with data in Google Sheets in a realistic, real-world project. Functions and formulas were used to clean, combine, split, and perform calculations on the data provided. Pivot tables were created to analyze and slice the data to explore the relevant questions. Best practices were maintained to protect, organize and navigate the project including versioning control, a linked Table of Contents, an Executive Summary and an Assumptions & Change Log.

### NYC Airbnb Properties

The goal of this project is to determine useful insights from current Airbnb listings for a client interested in investing in the vacation rental market in the Manhattan borough of New York City. The client needed help prioritizing where to focus their research and wanted some guidance on what types of properties to consider for investment.

#### The Data

The data was spread across 2 files:

`listings`: each row corresponds to a unique Airbnb listing
- `id`: Airbnb's unique identifier for the listing  
- `listing_url`  
- `scrape_id`: Inside Airbnb "Scrape" this was part of  
- `last_scraped`: UTC. The date and time this listing was "scraped"  
- `source`: One of "neighbourhood search" or "previous scrape". "neighbourhood search" means that the    listing was found by searching the city, while "previous scrape" means that the listing was seen in another scrape performed in the last 65 days, and the listing was confirmed to be still available on the Airbnb site.  
- `name`: Name of the listing  
- `description`: Detailed description of the listing  
- `neighborhood_overview`: Host's description of the neighbourhood  
- `picture_url`: URL to the Airbnb hosted regular sized image for the listing 
- `host_id`: Airbnb's unique identifier for the host/user  
- `host_name`: Name of the host. Usually just the first name(s).   
- `host_since`: The date the host/user was created. For hosts that are Airbnb guests this could be the date they registered as a guest.  
- `host_location`: The host's self reported location  
- `host_about`: Description about the host  
- `host_response_time`
- `host_response_rate`  
- `host_acceptance_rate`: That rate at which a host accepts booking requests.  
- `host_is_superhost`: name of the aisle  
- `host_thumbnail_url`  
- `host_picture_url`  
- `host_neighborhood`  
- `host_listings_count`: The number of listings the host has (per Airbnb calculations)  
- `host_verifications`  
- `host_has_profile_pic`  
- `host_identity_verified`  
- `neighborhood`: The neighbourhood as geocoded using the latitude and longitude against neighborhoods as defined by open or public digital shapefiles.  
- `neighborhood_group`: The neighbourhood group as geocoded using the latitude and longitude against neighborhoods as defined by open or public digital shapefiles.  
- `latitude`: Uses the World Geodetic System (WGS84) projection for latitude and longitude.  
- `longitude`: Uses the World Geodetic System (WGS84) projection for latitude and longitude.  
- `property_type`: Self selected property type. Hotels and Bed and Breakfasts are described as such by their hosts in this field  
- `room_type`: All homes are grouped into the following three room types:  
Entire places are best if you're seeking a home away from home. With an entire place, you'll have the whole space to yourself. This usually includes a bedroom, a bathroom, a kitchen, and a separate, dedicated entrance. Hosts should note in the description if they'll be on the property or not (ex: "Host occupies first floor of the home"), and provide further details on the listing.
Private rooms are great for when you prefer a little privacy, and still value a local connection. When you book a private room, you'll have your own private room for sleeping and may share some spaces with others. You might need to walk through indoor spaces that another host or guest may occupy to get to your room.
Shared rooms are for when you don't mind sharing a space with others. When you book a shared room, you'll be sleeping in a space that is shared with others and share the entire space with other people. Shared rooms are popular among flexible travelers looking for new friends and budget-friendly stays.
  
- `accomodates`: The maximum capacity of the listing  
- `bathrooms`: The number of bathrooms in the listing  
- `bathrooms_text`: The number of bathrooms in the listing. On the Airbnb web-site, the bathrooms field has evolved from a number to a textual description. For older scrapes, bathrooms is used.  
- `bedrooms`: The number of bedrooms  
- `beds`: The number of bed(s)  
- `amenities`  
- `price`: daily price in local currency  
- `minimum_nights`: minimum number of night stay for the listing (calendar rules may be different)  
- `maximum_nights`: maximum number of night stay for the listing (calendar rules may be different)  
- `minimum_minimum_nights`: the smallest minimum_night value from the calender (looking 365 nights in the future)  
- `maximum_minimum_nights`: the largest minimum_night value from the calender (looking 365 nights in the future)  
- `minimum_maximum_nights`: the smallest maximum_night value from the calender (looking 365 nights in the future)  
- `maximum_maximum_nights`: the largest maximum_night value from the calender (looking 365 nights in the future)  
- `minimum_nights_avg_ntm`: the average minimum_night value from the calender (looking 365 nights in the future)  
- `maximum_nights_avg_ntm`: the average maximum_night value from the calender (looking 365 nights in the future)  
- `calendar_updated`  
- `calendar_last_scraped`  
- `number_of_reviews`: The number of reviews the listing has  
- `number_of_reviews_ltm`: The number of reviews the listing has (in the last 12 months)  
- `number_of_reviews_l30d`: The number of reviews the listing has (in the last 30 days)  
- `first_review`: The date of the first/oldest review  
- `last_review`: The date of the last/newest review  
- `review_scores_rating`  
- `review_scores_accuracy`  
- `review_scores_cleanliness`  
- `review_scores_checkin`  
- `review_scores_communication`  
- `review_scores_location`  
- `review_scores_value`  
- `license`: The licence/permit/registration number  
- `The licence/permit/registration number`: [t=true; f=false]. Whether the guest can automatically book the listing without the host requiring to accept their booking request. An indicator of a commercial listing.  
- `calculated_host_listings_count`: The number of listings the host has in the current scrape, in the city/region geography.  
- `calculated_host_listings_count_entire_homes`: The number of Entire home/apt listings the host has in the current scrape, in the city/region geography  
- `calculated_host_listings_count_private_rooms`: The number of Private room listings the host has in the current scrape, in the city/region geography  
- `calculated_host_listings_count_shared_rooms`: The number of Shared room listings the host has in the current scrape, in the city/region geography  
- `reviews_per_month`: The number of reviews the listing has over the lifetime of the listing  
   
 
`calendar`: each row corresponds to a unique Airbnb listing ; The calendar file records the price, availability and other details from the listing's calendar for each day of the next 365 days from the given date.

- `listing_id`: ID number that uniquely identifies each Airbnb listing
- `date`: The date in the listing's calendar
- `avaliable`: Whether the date is available for a booking
- `price`: The price listed for the day
- `adjusted_price`: The price listed for the day, after adjustments
- `minimum_nights`: Minimum nights for a booking made on this day
- `maximum_nights`: Maximum nights for a booking made on this day

The data is provided by TripleTen.

### The Process

I first explored the dataset to better understand the data avaliable and how it would apply to the needs of the client. Then I cleaned and filtered the data, prepared essential columns, and combined essential information across tables. Finally, I analyzed the data using visualizations and pivot tables. 

<img width="608" alt="10 Most Popular Neighborhoods - P1" src="https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/f06f80c6-d782-48b1-8785-bfc0c143402e">
<img width="1460" alt="Screenshot 2024-02-16 at 5 17 54 PM" src="https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/f9bb20ce-b5b9-40e6-bb45-a6077ce74a79">
<img width="876" alt="Screenshot 2024-02-16 at 5 18 35 PM" src="https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/738312f2-e840-43cc-b1e0-4ddb8e4a005a">


### Results 
Taking the time to explain my results at each step was a key element in this process, and this was my first attempt at doing it. I outlined the key analysis results in the Executive Summary page and provided a linked Table of Contents for easier navigating of the workbook.

<img width="1614" alt="Client Recommendations   TOC_P1_NYC Airbnb" src="https://github.com/ejdostal/Data_projects_TripleTen/assets/151595335/459dd782-9fcd-4525-9be4-e3e2827c5c02">



Please have a look at the Google Sheets Workbook [linked here ](https://docs.google.com/spreadsheets/d/1RJXpP5sq4VEvNBJWPpVhWK2vMkSgRY1oYPffN4hywLo/edit?usp=sharing)for a full description of results.
