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
values to predict whether the day will be low-humidity or not based on the afternoon measurement
of relative humidity.
<li>Each row, or sample, consists of the following variables:</li></ul>
<ul><li> number: unique number for each row </li>
<li></li>air_pressure_9am: air pressure averaged over a period from 8:55am to 9:04am (Unit:
hectopascals)</li>
<li></li>air_temp_9am: air temperature averaged over a period from 8:55am to 9:04am (Unit:
degrees Fahrenheit)</li>
o air_wind_direction_9am: wind direction averaged over a period from 8:55am to 9:04am
(Unit: degrees, with 0 means coming from the North, and increasing clockwise)
o air_wind_speed_9am: wind speed averaged over a period from 8:55am to 9:04am (Unit:
miles per hour)
o max_wind_direction_9am:** wind gust direction averaged over a period from 8:55am to
9:10am (Unit: degrees, with 0 being North and increasing clockwise*)
o max_wind_speed_9am: wind gust speed averaged over a period from 8:55am to 9:04am
(Unit: miles per hour)
<li> rain_accumulation_9am: amount of rain accumulated in the 24 hours prior to 9am (Unit:
millimeters)</li>
<li>rain_duration_9am: amount of time rain was recorded in the 24 hours prior to 9am (Unit:
seconds)</li>
<li>relative_humidity_9am: relative humidity averaged over a period from 8:55am to 9:04am
(Unit: percent)</li>
<li>relative_humidity_3pm: relative humidity averaged over a period from 2:55pm to 3:04pm
(*Unit: percent *)</li></ul>

