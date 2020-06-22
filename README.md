# python-api-challenge

### Real-time Weather Report, Analysis and Geolocation Mapping

Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like? 

<div align="center">
  
![weather-3688572_1920](https://user-images.githubusercontent.com/65078870/85277188-fb9d6100-b450-11ea-8427-f224958a0f61.jpg)

</div>
Image by mohamed Hassan from Pixabay

## Part I - WeatherPy

### Background
Created a script to report and analyze the weather of 500+ cities across the world with varying distance from the equator. These tools have been very useful: 
* CityPy Python Library
* OpenWeatherMap API
* and a little common sense to create a model representation of weather across world cities

### Figures and Analysis
Subsequently, the output entails a series of scatter plots that showcase the following relationships: 

* Temperature (F) vs. Latitude
![Fig1_LatitudeVsTemperature](https://user-images.githubusercontent.com/65078870/85260447-b2411780-b438-11ea-8c7f-29f6ed97fb29.png)
 
 Figure 1 illustrates that the location of cities are situated somewhere between the latitude range of -60° to +80° at the South Pole and North Pole of the Equator respectively.

  According to the National Geographic channel, there's a relationship between temperature and latitude around the world, as temperatures are typically warmer approaching the Equator. There are variations, though, as other factors such as elevation, ocean currents, and precipitation will still affect climate patterns.

  The graphical plots depict a curve form rather than a straight line. It supports the variations brought about by other factors affecting climate patterns. One variable does not increase at a constant rate and may even start decreasing at a certain point.

* Humidity (%) vs. Latitude
![Fig2_LatitudeVsHumidity](https://user-images.githubusercontent.com/65078870/85260475-bec57000-b438-11ea-9993-222b67166ee5.png)

Figure 2 illustrates that humidity does not correlate strongly with latitude. The plots are scattered mostly between 60% to around 90% humidity readings.

It is believed that when relative humidity reaches 100%, the air is totally saturated with water vapor and more likely to rain.

* Cloudiness (%) vs. Latitude
![Fig3_LatitudeVsCloudiness](https://user-images.githubusercontent.com/65078870/85260510-cc7af580-b438-11ea-884f-496f8f24e25f.png)

Figure 3 illustrates that cloudiness rate does not have any correlation with latitude. But it appears to have colletion points along 0%, 75% and 100% readings.

* Wind Speed (mph) vs. Latitude
![Fig4_LatitudeVsWindspeed](https://user-images.githubusercontent.com/65078870/85260605-f207ff00-b438-11ea-95d3-1e935782807d.png)

Figure 4 illustrates that wind speed does not have any correlation with latitude.

It shows that the speed of wind has been going at 0-5 meters/sec rate regardless of the city's latitude at the time the information was collected.

---

<div align="center">

#### Now, if someone ask a question: "What's the weather like as we approach the equator?"

#### The answer will not just be: "Duh. It gets hotter..."

#### But, "I can find out real-time and show you what the world looks like with the current weather". 

---

### Linear Regression Analysis
Furthermore, the output also showcases the regression on each relationship as the data is clustered into the Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude) locations.
  
--- 

![Fig5_linear](https://user-images.githubusercontent.com/65078870/85263613-6a70bf00-b43d-11ea-9303-020b3535b34d.png)![Fig6_linear](https://user-images.githubusercontent.com/65078870/85263761-a60b8900-b43d-11ea-8050-0d94790eda5e.png)
* "Max Temperature vs. Latitude Linear Regression" in the Northern Hemisphere showed a moderately negative correlation. On the other hand, the Southern Hemisphere showed a nearly strong postive correlation.
 
 ---
 
![Fig7_linear](https://user-images.githubusercontent.com/65078870/85263880-d6ebbe00-b43d-11ea-9c56-3c0d25d810fb.png)![Fig8_linear](https://user-images.githubusercontent.com/65078870/85264065-1dd9b380-b43e-11ea-874a-3aa564315dc9.png)

* "Humidity vs. Latitude" in the Northern Hemisphere showed no linear relationship, as the r-squared value is almost equal to zero. Likewise, no correlation was observed in the Southern Hemisphere.
  
---

![Fig9_linear](https://user-images.githubusercontent.com/65078870/85266212-8bd3aa00-b441-11ea-9471-f477791f887d.png) ![Fig10_linear](https://user-images.githubusercontent.com/65078870/85266223-8f673100-b441-11ea-985a-653ecdc4ac8a.png)

* "Cloudiness vs. Latitude" in the Northern Hemisphere had no significant relationship based on the r-squared value. The plots appear no visible trend nor sensible shape. The same manner was observed in the Southern Hemisphere where it had no significant correlation.

---

![Fig11_linear](https://user-images.githubusercontent.com/65078870/85266637-2207d000-b442-11ea-8561-085fdb4866bf.png) ![Fig12_linear](https://user-images.githubusercontent.com/65078870/85266644-246a2a00-b442-11ea-9f95-bbbd14e22781.png)

* "Wind Speed vs. Latitude Linear Regression" in both Northern and Southern Hemispheres showed no correlations. 

---

##### I know what you may be thinking: "The last charts or figures seem a little boring..."

##### Okay, let's move on and dip into the world of Heatmaps and Geolocations. It's going to be more interesting, for sure. 

## Part II - VacationPy
<div align="center">
  
![wood-591618_1280](https://user-images.githubusercontent.com/65078870/85289784-f39bec00-b465-11ea-998d-9caf4e43f2f2.jpg)

</div>
Image by Michael Schwarzenberger from Pixabay

### Background
Designed a script to consider weather data in real-time to plan for future vacations. Jupyter-gmaps displayed the intensity of humidity levels accross the globe. Google Places API performed an online data search for hotels following a set parameters. And the final output generated an interactive heat map showcasing heat maps and Geolocation markers. 

### Maps and Figures

![image](https://user-images.githubusercontent.com/65078870/85272252-ebce4e80-b449-11ea-8615-e24ac53a1ea9.png)


#### My Vacation Dreamboard
<div align="center">
<img width="488" alt="My_VacationSpots_Hotels" src="https://user-images.githubusercontent.com/65078870/85272387-1b7d5680-b44a-11ea-8863-c9a02fd9e851.PNG">
</div>

#### Geolocations 
<div align="center">
<img width="474" alt="Hotel_markers_hybrid" src="https://user-images.githubusercontent.com/65078870/85272662-78790c80-b44a-11ea-9ea6-18f824010ebb.PNG">
</div>

#### Geolocation and Label Info
<div align="center">
<img width="532" alt="Hotel_markerInfo" src="https://user-images.githubusercontent.com/65078870/85272755-95154480-b44a-11ea-8911-ffda666f9fbb.PNG">
</div>

#### Geolocation with Heatmap and Pinned Markers
<div align="center">
<img width="478" alt="Hotel_heatmap" src="https://user-images.githubusercontent.com/65078870/85272851-baa24e00-b44a-11ea-9dfd-66b048227e75.PNG">
</div>

---





