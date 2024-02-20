# WeatherPy and VacationPy

## Overview
In this project, we aim to visualize weather data from over 500 cities around the world and use this data to plan future vacations. The project consists of two main parts: WeatherPy and VacationPy.

### Part 1: WeatherPy

In WeatherPy, we create a Python script to visualize the weather of over 500 cities of varying distances from the equator. We utilize the citipy Python library, the OpenWeatherMap API, and our problem-solving skills to create a representative model of weather across cities.

#### Steps:

1. **Create Plots to Showcase the Relationship Between Weather Variables and Latitude:**
    - We use the OpenWeatherMap API to retrieve weather data from the cities list generated.
    - Scatter plots are created to showcase the relationships between latitude and weather variables such as temperature, humidity, cloudiness, and wind speed.

2. **Compute Linear Regression for Each Relationship:**
    - Linear regression is computed for each relationship.
    - Plots are separated into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude).
    - A series of scatter plots is created, including the linear regression line, the model's formula, and the r values.

#### Findings:
After each pair of plots, we describe what the linear regression is modeling and any relationships or findings uncovered.

### Part 2: VacationPy

In VacationPy, we use the weather data skills developed in Part 1 to plan future vacations. We utilize Jupyter notebooks, the geoViews Python library, and the Geoapify API to create map visualizations.

#### Steps:

1. **Create a Map with City Points:**
    - We display a point for every city in the city_data_df DataFrame, with the size of the point representing the humidity in each city.

2. **Narrow Down the DataFrame to Find Ideal Weather Conditions:**
    - We filter the city data to find cities with ideal weather conditions based on criteria such as temperature, wind speed, and cloudiness.

3. **Find Nearest Hotels:**
    - Using the Geoapify API, we find the first hotel located within 10,000 meters of each city's coordinates.
    - We create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity, along with the nearest hotel name.

4. **Display Information on Map:**
    - We add the hotel name and country as additional information in the hover message for each city on the map.

## Conclusion

Through WeatherPy and VacationPy, we have not only visualized weather data but also utilized it to plan future vacations, making informed decisions based on ideal weather conditions and proximity to amenities such as hotels.
