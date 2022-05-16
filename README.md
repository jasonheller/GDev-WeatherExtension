# OWM GDev 5 Extension

# Example
![Here you can see how i use the extension](https://imgur.com/a/HmhKMHI)


You need to create 2 scene variables to use this extension, you will also need an API Key from open weather map (https://openweathermap.org/). 
- response -> for catching results
- response2 -> for converting the result

# Usage
Get an Latitude and Longtitude value of an Location, e.g. Berlin: 52.520008, 13.404954
To change a Text value to let's say the temperature. You will need to type VariableString(response2.main.temp)

# Commands
1. Temperature                   | response2.main.temp
2. Feeled temperature            | response2.main.feels_like
3. Minimum temperature           | response2.main.temp_min
4. Maximum temperature           | response2.main.temp_max
5. Pressure                      | response2.main.pressure
6. Humidity                      | response2.main.humidity
7. Country                       | response2.sys.country
8. City                          | response2.name
9. Weather Title                 | response2.weather.value.main
10. Weather Description          | response2.weather.value.description
11. Wind Angle                   | response2.wind.deg
12. Wind Speed                   | response2.wind.speed

** If you need more commands you can find them using the debugger and looking into the response2 variable.**
** If you want to set the Language for example for the Weather Descriptions go into the Extension, into GetWeather and add [+"&lang=de"] at the end of the URL. (Replace "de" with your language, e.g. de, en, fr, it etc.."**

# Important
If you are using the Free plan of openweathermap you should only update your weather data 15 times a minute.
This would be 604.800 calls a month. You "only" got 1.000.000 calls a month. So keep that in mind..

# Credits
Weather API from https://openweathermap.org/api 
