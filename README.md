<p align="center">
<img src="https://github.com/theidari/python-api-challenge/blob/main/Design/ocean%20gif.gif" width="800">
</p>

---

<p align="center">
<img src="https://github.com/theidari/python-api-challenge/blob/main/Design/blue.png" width="12"><a href="https://github.com/theidari/python-api-challenge/blob/main/README.md#-overview-of-project-"> Overview of Project </a><img src="https://github.com/theidari/python-api-challenge/blob/main/Design/blue.png" width="12"><a href="https://github.com/theidari/python-api-challenge/blob/main/README.md#how-to-use"> How to Use </a><img src="https://github.com/theidari/python-api-challenge/blob/main/Design/blue.png" width="12"><a href="https://github.com/theidari/python-api-challenge/blob/main/README.md#results"> Results </a><img src="https://github.com/theidari/python-api-challenge/blob/main/Design/blue.png" width="12"><a href="https://github.com/theidari/python-api-challenge/blob/main/README.md#references"> References </a><img src="https://github.com/theidari/python-api-challenge/blob/main/Design/blue.png" width="12">
</p>

---


<h3 align=left> Overview of Project </h3>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This activity is broken down into two deliverables, WeatherPy and VacationPy.


#### Objective
- <i>WeatherPy:</i>
   - Use the [OpenWeatherMap API](https://openweathermap.org/) to retrieve weather data from the cities list generated with citipy Python library.
   - Create a series of scatter plots to showcase the relationships between `Latitude` and:</br> 
<img src="https://github.com/theidari/python-api-challenge/blob/main/Design/1.png" width="30"> `Temperature` <img src="https://github.com/theidari/python-api-challenge/blob/main/Design/2.png" width="30"> `Humidity` <img src="https://github.com/theidari/python-api-challenge/blob/main/Design/3.png" width="30"> `Cloudiness` <img src="https://github.com/theidari/python-api-challenge/blob/main/Design/4.png" width="30"> `Wind Speed`
   - Linear regression scatter plot for <ins>Northern Hemisphere</ins> and <ins>Southern Hemisphere</ins> to showcase above relationships.
   
- <i>VacationPy:</i>
   - Create a map that displays a point for every city in the <i>WeatherPy</i> section DataFrame.
   - Narrow down the DataFrame to find your ideal weather condition and make hotel DataFrame.
      - ideal weather condition: <img src="https://github.com/theidari/python-api-challenge/blob/main/Design/1.png" width="30"> `21°C < temperature < 27°C` <img src="https://github.com/theidari/python-api-challenge/blob/main/Design/2.png" width="30"> `Wind speed less than 4.5 m/s` <img src="https://github.com/theidari/python-api-challenge/blob/main/Design/3.png" width="30"> `Zero cloudiness`
   - Use the [Geoapify API](https://www.geoapify.com/) to find the first hotel located within 10,000 metres of every city coordinates
   - Add the hotel name and the country as additional information for each city in the map.
   

#### Methods, Software and Attribution

- The analyses were performed using the [OpenWeatherMap Weather](https://api.openweathermap.org/data/2.5/weather?) API in metric units and [Geoapify Place](https://api.geoapify.com/v2/places) API by `accommodation.hotel` category, and correlation checked by Linear Reression method.

- Following programming languages, software, and libraries were used in this project:

<img src="https://github.com/theidari/python-api-challenge/blob/main/Design/redcube.png" width="10"> `python v.3.9.13`</br>
<img src="https://github.com/theidari/python-api-challenge/blob/main/Design/bluecube.png" width="10"> `jupyter notebook v.6.4.12`
`Visual Studio v.1.73.1`
`PowerPoint v.16.0.14026.20298`</br>
<img src="https://github.com/theidari/python-api-challenge/blob/main/Design/yellowcube.png" width="10"> `pandas v.1.4.4`
`SciPy v.1.9.3`
`Matplotlib v.3.6.0`
`citipy v.0.0.5`
`NumPy v.1.23.4`
`GeoViews v.1.9.5` 
`bokeh v.3.0.2`
`hvplot v.0.8.2`</br>

- The project header GIF has been designed by powerpoint and `photopea.com` using assets from `Freepik.com` (include: <a href="https://www.freepik.com/free-vector/green-grass-pattern-set_9175193.htm#query=grass&position=6&from_view=keyword">grass</a>, <a href="https://www.freepik.com/free-vector/young-man-woman-couple-tourists-with-poles-backpacks-travelling-climbing-trekking-hiking-walking-camping-adventures-nature_27399687.htm#query=man%20and%20woman%20tourist&position=21&from_view=search&track=sph">tourists</a> and <a href="https://www.freepik.com/free-vector/set-plant-tree-with-its-silhouette_9306595.htm#query=tree&position=4&from_view=search&track=sph">tree</a>).

---

<h3 align=left>How to Use</h3>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Before running <a href="https://github.com/theidari/python-api-challenge/blob/main/WeatherPy/WeatherPy.ipynb">WeatherPy</a> and <a href="https://github.com/theidari/python-api-challenge/blob/main/VacationPy/VacationPy.ipynb">VacationPy</a>, you will need API keys. Create an <b>api_keys.py</b> file in the same directory containing:

```python
# OpenWeatherMap API Key
weather_api_key = "YOUR KEY HERE"

# Geoapify API Key
geoapify_key = "YOUR KEY HERE"
```


<p align="right">
<a href="https://github.com/theidari/pymaceuticals#overview-of-project-"><sup>TOP PAGE</sup></a>
</P>

---

<h3 align=left>Results</h3>

<img src="https://github.com/theidari/python-api-challenge/blob/main/Design/WeatherPy.png" width="120">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Corrolation Between latitute of <ins>553 cities</ins> and their maximum temprature, humidity, cloudiness, and wind speed are shown in the following figures.

<h6 align="center">Fig [1]: Corrolation Between latitute and maximum temprature, humidity, cloudiness, and wind speed.</h6>
<table>
<tr>
<td><img src="https://github.com/theidari/python-api-challenge/blob/main/OutputData/Max%20Temp.png" width="400"></td>
<td><img src="https://github.com/theidari/python-api-challenge/blob/main/OutputData/Humidity.png" width="400"></td>
</tr>
<tr>
<td><img src="https://github.com/theidari/python-api-challenge/blob/main/OutputData/Cloudiness.png" width="400"></td>
<td><img src="https://github.com/theidari/python-api-challenge/blob/main/OutputData/Wind%20Speed.png" width="400"></td>
</tr>
</table>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<b>Figures [2]</b> to <b>Figures [5]</b> illustrate the relation of latitude for <ins>553 cities</ins> and their maximum temperature, humidity, cloudiness, and wind speed with linear regression in the `Northern Hemisphere` and `Southern Hemisphere`.

<h6 align="center">Fig [2]: latitute vs. maximum temprature</h6>
<table>
<tr>
<td><img src="https://github.com/theidari/python-api-challenge/blob/main/OutputData/Max%20Temp%20LR%20Northern%20Hemisphere.png" width="400"></td>
<td><img src="https://github.com/theidari/python-api-challenge/blob/main/OutputData/Max%20Temp%20LR%20Southern%20Hemisphere.png" width="400"></td>
</tr>
</table>

The above figure shows a  <ins>strong correlation</ins> with r<sup>2</sup>=0.84 for Northern Hemisphere and a <ins>moderate correlation</ins> with r<sup>2</sup>=0.57 for Southern Hemisphere. this means by moving away from the equator the temperature decreases.

<h6 align="center">Fig [3]: latitute vs. humidity</h6>
<table>
<tr>
<td><img src="https://github.com/theidari/python-api-challenge/blob/main/OutputData/Humidity%20LR%20Northern%20Hemisphere.png" width="400"></td>
<td><img src="https://github.com/theidari/python-api-challenge/blob/main/OutputData/Humidity%20LR%20Southern%20Hemisphere.png" width="400"></td>
</tr>
</table>

<h6 align="center">Fig [4]: latitute vs. cloudiness</h6>
<table>
<tr>
<td><img src="https://github.com/theidari/python-api-challenge/blob/main/OutputData/Cloudiness%20LR%20Northern%20Hemisphere.png" width="400"></td>
<td><img src="https://github.com/theidari/python-api-challenge/blob/main/OutputData/Cloudiness%20LR%20Southern%20Hemisphere.png" width="400"></td>
</tr>
</table>

<h6 align="center">Fig [5]: latitute vs. wind speed</h6>
<table>
<tr>
<td><img src="https://github.com/theidari/python-api-challenge/blob/main/OutputData/Wind%20Speed%20LR%20Northern%20Hemisphere.png" width="400"></td>
<td><img src="https://github.com/theidari/python-api-challenge/blob/main/OutputData/Wind%20Speed%20LR%20Southern%20Hemisphere.png" width="400"></td>
</tr>
</table>

Figure [3] to Figure [5] visualize a <ins>weak</ins> correlation between `humidity`, `cloudiness`, and `wind speed` with latitude for both Northern Hemisphere and Southern Hemisphere. Therefore, we cannot hypothesize that by increasing latitude these properties vary too significantly.



<p align="right">
<a href="https://github.com/theidari/pymaceuticals#overview-of-project-"><sup>TOP PAGE</sup></a>
</P>
 
 <img src="https://github.com/theidari/python-api-challenge/blob/main/Design/VacationPy.png" width="120">




 
<img src="https://github.com/theidari/python-api-challenge/blob/main/OutputData/Cities%20Location.png" width="800">

<img src="https://github.com/theidari/python-api-challenge/blob/main/OutputData/Hotel%20Location.png" width="800">
<img src="https://github.com/theidari/python-api-challenge/blob/main/OutputData/Clean%20Hotel%20Location.png" width="800">

---
<h3 align=left>References</h3>
<sup>[1]</sup> Trilogy Education Services, a <a href="https://2u.com/">2U, Inc.</a> brand.


<p align="right">
<a href="https://github.com/theidari/pymaceuticals#overview-of-project-"><sup>TOP PAGE</sup></a>
</P>








