# python-api-challenge

## Background

Whether financial, political, or social&mdash;data's true power rests in its ability to answer questions definitively. So, let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"

Now, we know what you may be thinking: _"Duh. It gets hotter ..."_

But, if pressed, how would you **prove** it?

# Instructions
## Part 1: WeatherPy

In this section, you'll create a Python script to visualize the weather of 500+ cities of varying distance from the equator. To do so, you'll use a [simple Python library](https://pypi.python.org/pypi/citipy), the [OpenWeatherMap API](https://openweathermap.org/api), and your problem-solving skills to create a representative model of weather across cities.

The first requirement is to create a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

After each plot, add a sentence or two explaining what the code is analyzing.

The second requirement is to compute the linear regression for each relationship. This time, separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

After each pair of plots, explain what the linear regression is modeling. For example, describe any relationships that you notice and any other findings you may have.

## Part 2: VacationPy

Now, let's use your skills working with weather data to plan future vacations. Use Jupyter-gmaps and the Google Places API for this part of the assignment.

To complete this part of the assignment, you will need to do the following:

* Create a heat map that displays the humidity for every city from Part 1

* Narrow down the DataFrame to find your ideal weather condition. My ideal weather conditions were:

  * A max temperature between 16C and 23C

  * Humidity between 30% and 50%

  * Cloudiness percentage between 0% and 40%

  * Drop any rows that don't satisfy all three conditions. You want to be sure the weather is ideal.

* Use Google Places API to find the first hotel for each city located within 5,000 meters of your coordinates.

* Plot the hotels on top of the humidity heatmap, with each pin containing the **Hotel Name**, **City**, and **Country**.