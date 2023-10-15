# python-api-challenge
## Module 6 Challenge
<br />

### WeatherPy

This section explore the possible correlations between the weather and the latitude measured at cities in the vicinity of 1,500 randomely generated coordinates.
Out of these 1,500 random locations, a query to the module citipy has returned 600 distinct cities out of which 576 of them had existing weather data available on openweathermap.org when queried on 10/11/2023.
From this data, the maximum temperature, the humidity, the cloudiness, and the wind speed for these cities were used to explore if they could be explained by a linear regression model using the latitude as input parameter.
<br />
The cities and scatter plots are available in the output_data folder.
https://github.com/xoffvsg/python-api-challenge/tree/main/WeatherPy/output_data. The plots with the linear regressions are shown in the Jupyter Notebook.

<br />

The humidity, the cloudiness, and the wind speed were found to be poorly correlated to the latitude, but the maximum temperatures in our dataset could be reasonably explained by the latitude of the cities.



<br />
<br />

### VacationPy

The map of the 576 cities identified previously was generated with the pandas module hvplot.

They were then filtered to only retain the ones with a temberature between 21C and 27C (included), a humidity less that 80%, and no cloud coverage. For the 12 cities meeting this criteria on 10/11/2023, we used the Geoapify API to identify the closest hotel within 10km. Eight cities have at least one hotel within the distance specified.
The maps and the list of hotels are shown in the Jupyter Notebook. The code in the cells must be run for the maps (HoloViews objects) to be displayed.






