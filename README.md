# World_Weather_Analysis
Project 6 of the Data Analysis BootCamp. Analysis weather data using APIs and statistics to create visualizations and recommendations for a travel company.
## Overview
This project aimed to collect and analyze weather data across cities worldwide and use the data to recommend ideal hotels based on weather preferences.
The analysis was divided into three parts.
1. Retrieval of the Weather Data
2. Creation of a Travel Destinations Map
3. Creation of a Travel Itinerary Map
## Retrieval of the Weather Data
The NumPy module was used to generate more than 2,000 random latitudes and longitudes, and the citipy module was used to list the nearest city to the latitudes and longitudes.Then the OpenWeatherMap API was used to request the current weather data from each unique city in the list. The results were saved into a Pandas DataFrame and then a .csv file.The [cities.csv](https://github.com/RuthLD/World_Weather_Analysis/blob/main/weather_data/cities.csv), the [WeatherPy_Database.csv](https://github.com/RuthLD/World_Weather_Analysis/blob/main/Weather_Database/WeatherPy_Database.csv), and the [WeatherPy_vacation.csv](https://github.com/RuthLD/World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation.csv) are the resulting files used for the analysis.
## Creation of a Travel Destination Map
To create a map with markers the [WeatherPy_Database.csv](https://github.com/RuthLD/World_Weather_Analysis/blob/main/Weather_Database/WeatherPy_Database.csv) was filtered as a Pandas DataFrame based on user inputs for a minimum and maximum temperature. Then hotels from the cities' coordinates were collected using Google's Maps and Places API, and Search Nearby feature. The ![WeatherPy_vacation_map.png](https://github.com/RuthLD/World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.png) was the result.
## Creation of a Travel Itinerary Map
The Google Directions API was used to create a travel itinerary that shows the route between four cities chosen from the possible travel destinations base on weather preferences. ![WeatherPy_travel_map.png](https://github.com/RuthLD/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map.png) shows the suggested route. ![WeatherPy_travel_map_markers.png](https://github.com/RuthLD/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map_markers.png) shows the hotel and city information for the destinations with map markers.
