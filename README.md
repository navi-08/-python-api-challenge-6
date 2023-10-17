# -python-api-challenge-6
assignment 6


Your analysis and linear regression plots for Temperature vs. Latitude in both the Northern and Southern Hemispheres are well presented. Here's a summary of the findings for each hemisphere:

Northern Hemisphere:

The linear regression analysis indicates a strong negative correlation between temperature and latitude in the northern hemisphere.
The high r-value (0.766) suggests a robust linear relationship between temperature and latitude, with temperatures dropping as cities in the northern hemisphere move closer to the north pole and farther from the equator.
The scatterplot and regression line clearly illustrate this negative correlation.
Southern Hemisphere:

The linear regression analysis indicates a slight positive correlation between temperature and latitude in the southern hemisphere.
The r-value (0.529) suggests a relatively weaker linear relationship compared to the northern hemisphere, but it still supports a positive correlation.
The scatterplot and regression line demonstrate that temperatures tend to rise as some cities in the southern hemisphere move closer to the equator.
Your analysis provides a clear and accurate interpretation of the linear relationships between temperature and latitude in both hemispheres. The high r-value in the northern hemisphere indicates a strong correlation, while the positive r-value in the southern hemisphere suggests a milder, yet still significant, positive correlation between temperature and latitude. This is consistent with our understanding of how temperature varies with latitude and proximity to the equator.



summary

Northern Hemisphere:

The linear regression analysis indicates a very weak positive correlation between wind speed and latitude in the northern hemisphere.
The r-value is close to zero (0.090), which suggests that there is little to no significant linear relationship between wind speed and latitude in the northern hemisphere.
The scatterplot and regression line show that wind speed tends to be relatively consistent across different latitudes in the northern hemisphere.
Southern Hemisphere:

The linear regression analysis indicates a very weak negative correlation between wind speed and latitude in the southern hemisphere.
The r-value is also close to zero (0.0218), indicating a very weak linear relationship.
The scatterplot and regression line suggest that wind speed is relatively consistent across different latitudes in the southern hemisphere, with a slight decrease as you move closer to the equator.
In both hemispheres, the r-values are very low, indicating that latitude is not a significant predictor of wind speed. Other factors, such as local geography and weather patterns, likely play a more substantial role in determining wind speeds in different regions.

Your analysis provides a clear and accurate interpretation of the linear relationships and the limited impact of latitude on wind speed in both hemispheres.





**Background
Weather is constantly changing, but it can be helpful to analyze weather patterns across the globe and uncover trends about why places have the weather they do, such as their distance from the equator. Utilizing Python requests, APIs, and JSON traversals, I uncovered some interesting trends about different cities and the weather they had at the specific time and day of my API request: January 05, 2021.

3 Observations
1. **Temperature Decreases with Distance from the Equator:** As cities move farther away from the equator, their maximum temperatures decrease gradually. This corresponds with what most people expect since the equator is typically assumed to have warmer and more stable temperatures year-round due to the fact that sunlight hits the Earth's surface from almost directly above.

2. **Wind Speed Doesn't Strongly Correlate with Latitude:** Though there was no strong correlation suggested in the scatter plot for wind speed vs. latitude, it is important to note that the vast majority of cities have wind speeds from 0 to low-20s, with very few cities lying above the 25mph mark.

3. **Cloudiness Varies, But No Strong Correlation with Latitude:** Cloudiness does not appear to have much correlation with latitude. However, there are several cities which show 100% cloudiness and 0% cloudiness. It would be interesting to dive deeper to see which cities reported 0% cloudiness and others which had 100% cloudiness, and see if common regions can be pinpointed to note whether certain regions are generally more cloudy than others.

WeatherPy
In this example, I created a Python script to visualize the weather of over 500 cities across the world with varying distances from the equator. I utilized a simple Python library and an API Key from OpenWeatherMap to construct representative models of the weather across world cities on January 05, 2021.

For the first part of my analysis, I created a series of scatter plots to showcase the following relationships:

1. Temperature (F) vs. Latitude
2. Humidity (%) vs. Latitude
3. Cloudiness (%) vs. Latitude
4. Wind Speed (mph) vs. Latitude

I then added a simple observation for each scatter plot describing what each plot suggests.

For the second part of my analysis, I ran a linear regression on each relationship listed above after separating the plots by the Northern and Southern Hemispheres.

After each pair of plots, I showed the r-squared value and a description of any relationships I noticed.

The script is in the WeatherPy directory titled "WeatherPy.ipynb", and .pngs of each plot are included in the output_data folder of the WeatherPy directory, along with the city_weather.csv file I conducted my analysis with after cleaning the data I received from the API request.

VacationPy
For this part of the analysis, I started by creating a heat map that displays the humidity for every city from Part I.

I then narrowed down my DataFrame to find my ideal weather condition and dropped the cities which didn't meet the conditions. My ideal weather conditions are:

1. A maximum temperature equal to or lower than 85 degrees but higher than 72 degrees.
2. Wind speed being less than 5 mph.
3. Cloudiness less than or equal to 30%, since blue skies with nice clouds are hard to beat!



