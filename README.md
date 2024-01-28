<b><p>Classification of Weather Data using scikit-learn
We will use scikit-learn to perform a decision tree based classification of weather data.
</p></b>

Daily Weather Data Description
The file daily_weather.csv is a comma-separated file that contains weather data. This data comes from a
weather station. The weather station is equipped with sensors that capture weather-related measurements
such as air temperature, air pressure, and relative humidity. Data was collected for a period of three years,
from September 2011 to September 2014, to ensure that sufficient data for different seasons and weather
conditions is captured.
Let us now check all the columns in the data.
<ul>
<li>Each row in daily_weather.csv captures weather data for a separate day.</li>
<li>Sensor measurements from the weather station were captured at one-minute intervals.</li>
These measurements were then processed to generate values to describe daily weather. Since this dataset
was created to classify low-humidity days vs. non-low-humidity days (that is, days with normal or
high humidity), the variables included are weather measurements in the morning, with one
measurement, namely relatively humidity, in the afternoon. The idea is to use the morning weather 
