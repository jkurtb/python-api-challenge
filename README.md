# python-api-challenge

### Real-time Weather Report Analysis and Geolocation Mapping

Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like? 

<div align="center">
  
![weather pic](https://user-images.githubusercontent.com/65078870/85257447-e1a15580-b433-11ea-834d-f57f0e19da50.png)

</div>
source: Co.Design

## WeatherPy

Created a script to report and analyze the weather of 500+ cities across the world of varying distance from the equator, with the tools essentially required as follows: 
* CityPy Python Library
* OpenWeatherMap API
* and a little common sense to create a model representation of weather across world cities

Subsequently, the output entails a series of scatter plots to showcase the following relationships: 

* ### Temperature (F) vs. Latitude
![Fig1_LatitudeVsTemperature](https://user-images.githubusercontent.com/65078870/85260447-b2411780-b438-11ea-8c7f-29f6ed97fb29.png)

  Figure 1 illustrates that the city's locations are situated somewhere between the latitude range of -60° at the South Pole and +80° at the North Pole of the Equator.

  According to the National Geographic channel, there's a relationship between temperature and latitude around the world, as temperatures are typically warmer approaching the Equator. There are variations, though, as other factors such as elevation, ocean currents, and precipitation will still affect climate patterns.

  The graphical plots depict a curve form rather than a straight line. It supports the variations brought about by other factors affecting climate patterns. One variable does not increase at a constant rate and may even start decreasing at a certain point.

* Humidity (%) vs. Latitude
![Fig2_LatitudeVsHumidity](https://user-images.githubusercontent.com/65078870/85260475-bec57000-b438-11ea-9993-222b67166ee5.png)

* Cloudiness (%) vs. Latitude
![Fig3_LatitudeVsCloudiness](https://user-images.githubusercontent.com/65078870/85260510-cc7af580-b438-11ea-884f-496f8f24e25f.png)

* Wind Speed (mph) vs. Latitude
![Fig4_LatitudeVsWindspeed](https://user-images.githubusercontent.com/65078870/85260605-f207ff00-b438-11ea-95d3-1e935782807d.png)

