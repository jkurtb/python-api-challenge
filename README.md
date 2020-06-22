# python-api-challenge

### Real-time Weather Report Analysis and Geolocation Mapping

Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like? 

<div align="center">
  
![weather pic](https://user-images.githubusercontent.com/65078870/85257447-e1a15580-b433-11ea-834d-f57f0e19da50.png)

</div>
source: Co.Design

## WeatherPy

### Tools
Created a script to report and analyze the weather of 500+ cities across the world of varying distance from the equator, with the tools essentially required as follows: 
* CityPy Python Library
* OpenWeatherMap API
* and a little common sense to create a model representation of weather across world cities

### Figures and Analysis
Subsequently, the output entails a series of scatter plots that showcase the following relationships: 

* Temperature (F) vs. Latitude
![Fig1_LatitudeVsTemperature](https://user-images.githubusercontent.com/65078870/85260447-b2411780-b438-11ea-8c7f-29f6ed97fb29.png)
 
 Figure 1 illustrates that the city's locations are situated somewhere between the latitude range of -60° at the South Pole and +80° at the North Pole of the Equator.

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

### Linear Regression Analysis
Furthermore, the output also depicts the regression on each relationship as the data is clustered into the Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude) locations:


  ![Fig5_linear](https://user-images.githubusercontent.com/65078870/85263613-6a70bf00-b43d-11ea-9303-020b3535b34d.png)
  * Northern Hemisphere - Max Temp vs. Latitude Linear Regression
 "Max Temperature vs. Latitude Linear Regression" in the Northern Hemisphere showed a moderately negative correlation.

* Southern Hemisphere - Max Temp vs. Latitude Linear Regression
  ![Fig6_linear](https://user-images.githubusercontent.com/65078870/85263761-a60b8900-b43d-11ea-8050-0d94790eda5e.png)

  On the other hand, "Max Temperature vs. Latitude Linear Regression" in the Southern Hemisphere showed a nearly strong postive correlation.
  
  
  
 * Northern Hemisphere - Humidity (%) vs. Latitude Linear Regression
![Fig7_linear](https://user-images.githubusercontent.com/65078870/85263880-d6ebbe00-b43d-11ea-9c56-3c0d25d810fb.png)

  "Humidity vs. Latitude" in the Northern Hemisphere showed no linear relationship, as the r-squared value is almost equal to zero.
  
 * Southern Hemisphere - Humidity (%) vs. Latitude Linear Regression
![Fig8_linear](https://user-images.githubusercontent.com/65078870/85264065-1dd9b380-b43e-11ea-874a-3aa564315dc9.png)
 
  Likewise, "Humidity vs. Latitude" in the Southern Hemisphere also showed no linear relationship.
  
  
  
 * Northern Hemisphere - Cloudiness (%) vs. Latitude Linear Regression





