# README: AirBnB Lab 5 Model

## Data

Today’s data is about Airbnb listings in Santa Cruz, CA. The data can be obtained from <http://insideairbnb.com/> ; it was originally scraped from airbnb.com.

You can see a visualization of some of the data used in today’s lab at <http://insideairbnb.com/santa-cruz-county/>

- price: Cost per night (in U.S. dollars)
- neighbourhood: Santa Cruz county City (Santa Cruz, Capitola, Scotts Valley, etc.)
- room_type:
	- Entire home/apt (guests have entire place to themselves)
	- Private room (Guests have private room to sleep, all other rooms shared)
	- Shared room (Guests sleep in room shared with others)
- number_of_reviews: Total number of reviews for the listing
- reviews_per_month: The number of reviews per month the listing has over the lifetime of the listing.
- minimum_nights: Number of nights required to book rental

## Lab

The lab wants us to create multi linear regression model uses the inputs modified neighbourhood, number_of_reviews, and reviews_per_month from the dataset to predict the average price for a three night stay at an AirBnB in Santa Cruz County which is calculated based
on the price(per night) x 3 + cleaning fee (2% of price/night). The dataset was filtered so it only includes those who had minimum_nights >= 3 where the neighbourhoods were reduced to four categories (The top 3 + others were joined).