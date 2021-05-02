# Python-API

This project utilizes Openweathermap API calls to collect temperature, humidity, cloudiness, and wind speed from more than 500 randomly selected cities.  The list of cities is selected by randomly generating coordinate pairs, then using citipy to determine the closest available city for those coordinates.  The data is cleaned to remove any data if a coordinate pair does not successfully yield a city.  Once the weather information is collected, the information is divided for cities in the northern and southern hemispheres.  For each hemisphere, the four weather parameters are plotted against latitude, and linear regression is used to determine if there is a correlation between latitude and the given parameter.  Each graph is generated as an output .png file, and the complete city weather data is output as a .csv file.

The .csv file containing city weather data is then used to determine "vacation spots" based on weather parameters.  Initially, humidity for all cities in the file are displayed on the Google maps extension. Next, one's ideal temperature, humidity, cloudiness, and wind speed parameters are entered, and cities that meet the desired criteria are displayed.  A google API is run to determine the closest hotel to the city coordinates, and appends the hotel names to the data frame for their respective cities.  Finally, the hotels of choice are displayed as options on Google maps.

The locations can vary greatly, but you can be sure the weather there is exactly what you're looking for--you just have to decide where you want to go!

-Christian
