# Weather-Data-Analysis

## Intoduction & Purpose
The purpose of this project was to further master skills in `API Calls` and transforming the data into analyzable and insightful format. For this project, 500 random cities were generated and their weather data was collected using `openweathermapy`. This project also used `citipy` module to find the nearest cities based on the random combination of latitude and longitude generated.

## Objective
This project's objective as to find relation between `Latitude` and different weather data variables such as `Temprature, Cloudiness, Wind Speed & Humidity`. By latitude, the data had the equator line as the point of reference. Overall, trying to measure the effect of equator on factos such as `Temprature, Cloudiness, Wind Speed`.

## Approach
```
1. Generate longitude and latitude
    - using numpy generate random numbers in range of long and lat. 
    - zip them together so they can be sent as coordinates.
```

```
2. Generate Cities 
    - using citipy library, find the nearest city for the given coordinate.
    - make a list of all the cities (500).
```

```
3. Get Weather Data for cities 
    - use the openweathermapy library to get information on each city.
    - create a log to see which url failed to fetch.  
```

```
3. Draw Conclusions 
    - visualize the variables to find the correlation.
    - making conclusions.
```

## Analysis & Visualization 
**Scatter Plot: City Latitude vs. Max Temperature** The point of this chart was to see relationship between the closeness of city to the equator, `Latitude` against the `Maximum Temprature`. This graph will indicate if there is any strong relationship between the two variables. 

`Provides answer to the question: Are cities near the equator hotter?`

<img src="images/2.png" width="600" height="400" />

**Scatter Plot: City Latitude vs. Cloudiness** The point of this chart was to see relationship between the closeness of city to the equator, `Latitude` against the `Cloudiness`. This graph will indicate if there is any strong relationship between the two variables. 

`Provides answer to the question: Are cities near the equator cloudier?`

<img src="images/3.png" width="600" height="400" />

**Scatter Plot: City Latitude vs. Humidity** The point of this chart was to see relationship between the closeness of city to the equator, `Latitude` against the `Cloudiness`. This graph will indicate if there is any strong relationship between the two variables. 

`Provides answer to the question: Are cities near the equator more humid?`

<img src="images/4.png" width="600" height="400" />

**Scatter Plot: City Latitude vs. Windspeed** The point of this chart was to see relationship between the closeness of city to the equator, `Latitude` against the `Cloudiness`. This graph will indicate if there is any strong relationship between the two variables. 

`Provides answer to the question: Are cities near the equator windier?`

<img src="images/5.png" width="600" height="400" />

## Conclusions
* As expected, the weather becomes significantly warmer as one approaches the equator (0 Deg. Latitude). More interestingly, however, is the fact that the southern hemisphere tends to be warmer this time of year than the northern hemisphere. This may be due to the tilt of the earth.
* There is no strong relationship between latitude and cloudiness, however, it is interesting to see that a strong band of cities sits at 0, 80, and 100% cloudiness.
* There is no strong relationship between latitude and wind speed, however in northern hemispheres there is a flurry of cities with over 20 mph of wind.

## Advantages and Insights
* The assumption that the cities near the equator are hotter is proved and if anyone disagress then this report will suffice. 
* Direct correlations could have been calculated using the `statistics` library but for this project visualizing the chart was a priority. 
* Also the relations between other variables(`Cloudiness, Wind Speed & Humidity`) and latiude were clarified thus knowing that the equator line has no effect on it. 