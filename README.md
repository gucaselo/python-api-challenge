# Python API
### Using two API, analyzed Weather data and generated Vacation destinations.


## WeatherPy
#### Created a `python` script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this we used the [citypy library](https://pypi.python.org/pypi/citipy) and the [OpenWeatherMap API](https://openweathermap.org/api). Generated a csv file with the data obtained.

***Please add your API if you intend to use this script.***

The following scatter plots were generated with the data obtained:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude


After separating the plots into Northern and Southern Hemisphere, I ran linear regression on the following relationships:

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

## VacationPy
#### In an effor to find the ideal locations for vacation, I filtered the data from the csv file generated by WeatherPy to my personal ideal weather conditions. To accomplish this we used `jupyter-gmaps` and the [Google API](https://console.developers.google.com/), specifically Google Places API, Geocoding API and Maps JavaScript API.

***Please add your API if you intend to use this script.***

The following maps were generated with the dataset available:

* Generated a Heat Map  that displayed the humidity for every city.
* Used Google Places API to find the first hotel for 10 cities located within 5000 meters of each coordinates.
* Plotted the hotels on top of the humidity heatmap and added a pin containing the Hotel Name, City and Country.
