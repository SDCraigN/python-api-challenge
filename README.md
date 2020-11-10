# python-api-challenge - What's the Weather Like?
 

### Background of the challenge
Whether financial, political, or social -- data's true power lies in its ability to answer questions definitively. So let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"

### Observations & Analysis
1. It gets warmer closer to the equator, but it doesn't mean it is hottest along the equator** :sun_with_face::sun_with_face::sun_with_face::thermometer:

We know that the weather gets warmer as we approach the equator. We can observe this relationship by looking at the scatter plot between Latitude and Maximum Temperature of a city.

![Latitude vs Temperature Scatter Plot](/WeatherPy/output_data/Fig1.png)

The chart above clearly illustrates the *linear relationship where temperatures are higher nearer to the equator* (at 0 degree latitude) and vice versa.

Interestingly though, the tempteratures are highest at approximately 20 degree latitude rather than the equator. This is likely due to the tilt of the Earth's axis at this time of the year, causing the Sun to be nearer to cities along the Tropic of Cancer (approximately 23.5 degree latitude).

2. While there isn't a strong correlation between latitude and humidity, we can observe that tropical cities surrounding the equator tend to be more humid. The lowest percentage humidity for cities along the equator is just above 40%. In contrast, there are 2 clusters of cities with humidity under 40% at around 20 to 40 degree latitude within both the northern and southern hemispheres. This suggests that the air is are drier along the Tropic of Cancer and Tropic of Capricon.

![Latitude vs Temperature Scatter Plot](/WeatherPy/output_data/Fig2.png)

3. We can observe a wide spread of cloudiness across the range of latitudes. We can confirm the variability using the standard deviation for cloudiness at 37.9%. From the plot, we can also determine that there isn't a strong relationship between latitude and cloudiness.

![Latitude vs Temperature Scatter Plot](/WeatherPy/output_data/Fig3.png)

However, we can observe 3 clusters worth mentioning. First cluster has 100% cloudiness for cities between 0 and 20 degree latitude. The second and third clusters are the 0% cloudiness at around 20 to 40 degree latitudes at both sides of the hemisphere. 

This could potentially infer that *tropical cities closer to the equator tend to be cloudier while there are clearer skies along the Tropic of Cancer and Tropic of Capricon.*

### Files:

**1. WeatherPy**
* Jupyter Notebook (filename: WeatherPy.ipynb)
* Output Data:
   * Cities data retrieved from OpenWeatherMap API (filename: cities.csv)
   * Scatter plot of Latitude vs Temperature (filename: Fig1.png)
   * Scatter plot of Latitude vs Humidity (filename: Fig2.png)
   * Scatter plot of Latitude vs Cloudiness (filename: Fig3.png)
   * Scatter plot of Latitude vs Wind Speed (filename: Fig4.png)
   
**2. VacationPy**
* Jupyter Notebook (filename: VacationPy.ipynb)
