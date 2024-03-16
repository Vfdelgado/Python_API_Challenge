# Python API Challenge

## WeatherPy

The goal of this part is to create visualizations showcasing the relationship between various weather variables and latitude across over 500 cities worldwide. This involves retrieving weather data using the OpenWeatherMap API, plotting scatter plots to visualize the relationships, and performing linear regression analysis to understand the trends.

Weather Data Retrieval:

The OpenWeatherMap API is utilized to retrieve weather data for the cities generated in the starter code.
The weather data includes temperature, humidity, cloudiness, and wind speed.

Scatter Plots:

Scatter plots are created to display the relationships between latitude and each weather variable: temperature, humidity, cloudiness, and wind speed.
The scatter plots provide insights into how these weather variables change with latitude.

Linear Regression:

Linear regression analysis is performed separately for the Northern Hemisphere (latitude >= 0) and the Southern Hemisphere (latitude < 0) for each weather variable.

Scatter plots with linear regression lines are generated for temperature, humidity, cloudiness, and wind speed to visualize the trends in both hemispheres.

The linear regression lines help identify any significant relationships between latitude and the weather variables.

Findings:

Temperature: In the Northern Hemisphere, there is a negative correlation between latitude and temperature, indicating that temperature decreases as we move away from the equator. Conversely, in the Southern Hemisphere, there is a positive correlation, with temperature increasing closer to the equator.

Humidity: There doesn't appear to be a strong correlation between latitude and humidity in either hemisphere, as indicated by the relatively flat regression lines.

Cloudiness: Cloudiness does not show a clear correlation with latitude in either hemisphere, as observed by the scattered distribution of data points around the regression lines.

Wind Speed: Similar to humidity and cloudiness, wind speed does not exhibit a consistent trend with latitude, with scattered data points across both hemispheres.

## VacationPy

In this part, the goal is to utilize the weather data obtained in WeatherPy to plan future vacations. This involves creating maps using the geoViews Python library and the Geoapify API to visualize city locations, humidity levels, and nearby hotels meeting specified criteria.

City Visualization:

A map displaying a point for every city in the city_data_df DataFrame is created. The size of the points represents the humidity level in each city.
This visualization provides an overview of city locations and humidity levels worldwide.

Ideal Weather Conditions:

The city_data_df DataFrame is narrowed down to find cities with ideal weather conditions based on specified criteria, such as temperature range, wind speed, and cloudiness.
The ideal weather conditions help identify potential vacation destinations with comfortable weather conditions.

Hotel Search:

For each city in the hotel_df DataFrame, the Geoapify API is used to find the first hotel located within 10,000 meters of the city's coordinates.
The hotel name and country are added as additional information in the hover message for each city on the map, providing insights into available accommodation options.

Findings:

The city map allows users to visualize cities with suitable weather conditions for vacation planning.
By incorporating hotel information into the map, users can identify potential accommodation options in their desired destinations, enhancing the vacation planning experience.

Conclusion:
WeatherPy and VacationPy provide valuable tools for analyzing weather data and planning future vacations. The analysis conducted in WeatherPy helps understand the relationship between weather variables and latitude, while VacationPy leverages this information to identify ideal vacation destinations and nearby hotels. Together, these tools enable users to make informed decisions when planning their next trip.

Resources: 
Past class activities, online resources, tutoring.
