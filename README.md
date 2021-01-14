# World Weather Analysis
An Analysis of World Weather for Travel Planning

## Overview
In this project, we analyze and visualize weather data across the world for a hypothetical travel planning app.

### Pre-Project Research
Leading up to the project, we pulled in a variety of data from OpenWeatherMap, then analyzed and charted it. 

The chart here shows city latitude vs max temperature:

![City Latitude vs Max Temperature (12.29.20)](https://github.com/flowersmichael/World_Weather_Analysis/blob/main/City%20Latitude%20vs%20Max%20Temperature--122920.png)

We also ran linear regression on latitude data versus various weather elements, including humidity (Northern Hemisphere) here:

![Linear Regression Latitude vs Humidity (NH 12.29.20)](https://github.com/flowersmichael/World_Weather_Analysis/blob/main/Linear%20Regression%20on%20Northern%20Hemisphere%20for%20%25%20Humidity.png)

For the map below we joined humidity data from OpenWeatherMap data with Google Maps:

![Heatmap of Humidity (12.29.20)](https://github.com/flowersmichael/World_Weather_Analysis/blob/main/Heatmap%20of%20Humidity--122920.png)


## Final Project
For our final project, we put together a travel destinations map and itinerary. Our major steps involved:

1. Retrieving weather data
2. Creating a travel destinations map for the customer
3. Creating an itinerary map

### Retrieve Weather Data
1. Generate a set of 2,000 random latitudes and longitudes 
(including the ocean which covers ~70% of the planet, we can expect roughly 1/3 of the coordinates to be near a city)
2. Retrieve the nearest city using the citipy module
3. Perform an API call with the OpenWeatherMap
4. Retrieve weather data for the cities from the API call
5. Add the data to a Pandas DataFrame
6. Export the DataFrame as a CSV

We ended up with 703 cities. Here's a sample of our data in the DataFrame:

![DataFrame](https://github.com/flowersmichael/World_Weather_Analysis/blob/main/Dataframe.png)

### Create a Customer Travel Destinations Map
1. Write input statements that prompt the user to enter minimum and maximum temperatures for their destinations
2. Retrieve the latitude and longitude of each city to find the nearest hotel
3. Create a marker layer map that will have pop-up markers for each city on the map, with the pop-ups including:
    * Hotel Name
    * City
    * Country
    * Current Weather

![Travel Destinations Map](https://github.com/flowersmichael/World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.png)

### Create a Travel Itinerary Map
1. Enable the Directions API in Google
2. Create a marker layer map of vacation search results
3. Choose four cities a customer may want to visit, all in the same country and close together
4. Use gmaps to create a directions layer map

We decided on a trip to Madagascar!

![Travel Itinerary Map](https://github.com/flowersmichael/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map.png)

![Travel Itinerary Map Markers](https://github.com/flowersmichael/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map_markers.png)



