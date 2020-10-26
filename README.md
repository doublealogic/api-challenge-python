# Python API Challenge

## Overview
This repository contains two Python scripts: `WeatherPy.ipynb` and `VacationPy.ipynb`.

### Part I - WeatherPy

This Python script visualizes the weather of 500+ cities across the world of varying distance from the equator. It utilizes citipy, a [simple Python library](https://pypi.python.org/pypi/citipy), and the [OpenWeatherMap API](https://openweathermap.org/api), to create a representative model of weather across world cities.

To start, I randomly select **at least** 500 unique (non-repeat) cities based on latitude and longitude. Then I perform a weather check on each of the cities using a series of successive API calls. At the end, I print logs of each city as it's being processed with the city number and city name.

After gathering the data, I display a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

After each plot I explain what the code is and analyze each relationship.

Next, I ran a linear regression on each relationship, only this time separating them into Northern Hemisphere cities (greater than or equal to 0 degrees latitude) and Southern Hemisphere cities (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

After each pair of plots I explain what the linear regression is modeling such as any relationships I noticed and any other analysis I saw.


For all of the scatter plots above, I save a CSV of all retrieved data and a PNG image for each scatter plot.