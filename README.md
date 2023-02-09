# Airbnb Berlin Exploratory Data Analysis 🏘️

![Berlin](https://www.br.de/unternehmen/inhalt/organisation/korrespondenten/berlin-deutschland-studio-100~_v-img__16__9__xl_-d31c35f8186ebeb80b0cd843a7c267a0e0c81647.jpg)

# Summary 

Airbnb is an online marketplace that connects people who want to rent out their homes with people who are looking for accommodations in that locale. It currently covers more than 100,000 cities and 220 countries worldwide.

Berlin has faced several challenges with the growth of Airbnb and other short-term rental platforms in recent years. The city has implemented strict regulations on short-term rentals, which has resulted in some neighborhoods being off-limits for such rentals. This has raised concerns about the impact of Airbnb on the availability of affordable housing for long-term residents and on the city's housing market as a whole. The high demand for short-term rentals has also put pressure on the city's infrastructure, such as public transportation, leading to concerns about the sustainability of the industry. The issue of Airbnb in Berlin is complex and multifaceted, and it continues to be a subject of ongoing debate and discussion.

# Dataset 

For this project we are analyzing Berlin’s Airbnb data from 2010 to 2021. 

The dataset is publicly available at http://insideairbnb.com/get-the-data.html


<p align="left">
  <img alt="data_model" src="./img/airbnb_data_model.png">
</p>

| Field  | Description |
| ------------- | ------------- |
| id  | Airbnb's unique identifier for the listing |
| host_id  | Airbnb's unique identifier for the host/user |
| room_type  | All homes are grouped into the following three room types: Entire place, Private room and Shared room |
| neighbourhood_group_cleansed  | The neighbourhood group as geocoded using the latitude and longitude against neighborhoods as defined by open or public digital shapefiles |
| price  | Daily price |
| accommodates  | The maximum capacity of the listing |
| latitude  | Uses the World Geodetic System (WGS84) projection for latitude and longitude |
| longitude  | Uses the World Geodetic System (WGS84) projection for latitude and longitude |

| Field  | Description |
| ------------- | ------------- |
| listing_id  | Airbnb's unique identifier for the listing |
| id  | Airbnb's unique identifier for the review |
| date  | Date the review was submitted |
| reviewer_id  | Airbnb's unique identifier for the reviewer |
| reviewer_name  | Reviewer name |
| comments  | Review content |


# Tools

- [Python](https://www.python.org/)
- [Jupyter Notebook](https://jupyter.org/)
- [pandas](https://pandas.pydata.org/)
- [GeoPandas](https://geopandas.org/en/stable/)
- [Matplotlib](https://matplotlib.org/)
- [Seaborn](https://seaborn.pydata.org/)

# Analysis 

We will uncover insights on:

+ Listings types: Airbnb original idea was to offer a room or a shared room within one's home. Is it still so?
+ Listings density: Are listings evenly spread across neighborhoods or are there hotspots?
+ Ownership: are properties owned by individual users or are there users with multiple rental properties (i.e. potentially for speculation)?
+ Price fairness: Are prices inflated for tourists? That is, is there a significative difference in prices between listings in English (i.e. for tourists) and German (i.e. "locals", or at least German-speaking tourists)? If there is, is this difference more pronounced in certain districts?
+ Trends and Seasonality: Since we do not have historic data about stays but only about reviews, we could use reviews as estimators of stays. Has the number of reviews increased over time? If it has, can we say that the increase is due to an increased number of visitors or it must be simply abscribed to an increment in the popularity of the platform? Is the flow of tourists seasonal, that is does it follow a seasonal trend? Can we explain the pattern?

