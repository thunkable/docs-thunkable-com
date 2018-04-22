#### T**hunkable Cross-Platform **✕

# ⎍ Objects

---

Often, data that you retrieve from APIs \([Web API](/x/components/data-storage/web-api.md), [Map](/x/components/map-location/map.md) and [Location Sensor](/x/components/map-location/location-sensor.md)\) is stored as objects, which can store multiple properties for a given object.  The object blocks are extremely helpful to pull out the specific attribute of data that you want. For the [Spreadsheet](/x/components/data-storage/spreadsheet.md) component, you will also need to upload your data in object format as well

* [Retrieving a single property from a data API](#retrieving-a-single-property-from-a-data-api)
* [Uploading a row of data into a Spreadsheet](#uploading-a-row-of-data-into-a-spreadsheet)
* [Understanding what properties are contained in a Location object](#understanding-what-properties-are-contained-in-a-location-object)

---

### Retrieving a single property from a data API

![](/assets/blocks-object-✕-fig-4.png)![](/assets/blocks-object-✕-fig-2.png)

Often, when retrieving data form an API like [Weather Underground](https://www.wunderground.com/weather/api/d/docs?MR=1), you will get a large data dump in JSON format like shown below.

`{ "response": { "version": "0.1", "termsofService": "http://www.wunderground.com/weather/api/d/terms.html", "features": { "conditions": 1 } }, "current_observation": { "image": { "url": "http://icons-ak.wxug.com/graphics/wu2/logo_130x80.png", "title": "Weather Underground", "link": "http://www.wunderground.com" }, "display_location": { "full": "San Francisco, CA", "city": "San Francisco", "state": "CA", "state_name": "California", "country": "US", "country_iso3166": "US", "zip": "94101", "latitude": "37.77500916", "longitude": "-122.41825867", "elevation": "47.00000000" }, "observation_location": { "full": "SOMA - Near Van Ness, San Francisco, California", "city": "SOMA - Near Van Ness, San Francisco", "state": "California", "country": "US", "country_iso3166": "US", "latitude": "37.773285", "longitude": "-122.417725", "elevation": "49 ft" }, "estimated": {}, "station_id": "KCASANFR58", "observation_time": "Last Updated on June 27, 5:27 PM PDT", "observation_time_rfc822": "Wed, 27 Jun 2012 17:27:13 -0700", "observation_epoch": "1340843233", "local_time_rfc822": "Wed, 27 Jun 2012 17:27:14 -0700", "local_epoch": "1340843234", "local_tz_short": "PDT", "local_tz_long": "America/Los_Angeles", "local_tz_offset": "-0700", "weather": "Partly Cloudy", "temperature_string": "66.3 F (19.1 C)", "temp_f": 66.3, "temp_c": 19.1, "relative_humidity": "65%", "wind_string": "From the NNW at 22.0 MPH Gusting to 28.0 MPH", "wind_dir": "NNW", "wind_degrees": 346, "wind_mph": 22.0, "wind_gust_mph": "28.0", "wind_kph": 35.4, "wind_gust_kph": "45.1", "pressure_mb": "1013", "pressure_in": "29.93", "pressure_trend": "+", "dewpoint_string": "54 F (12 C)", "dewpoint_f": 54, "dewpoint_c": 12, "heat_index_string": "NA", "heat_index_f": "NA", "heat_index_c": "NA", "windchill_string": "NA", "windchill_f": "NA", "windchill_c": "NA", "feelslike_string": "66.3 F (19.1 C)", "feelslike_f": "66.3", "feelslike_c": "19.1", "visibility_mi": "10.0", "visibility_km": "16.1", "solarradiation": "", "UV": "5", "precip_1hr_string": "0.00 in ( 0 mm)", "precip_1hr_in": "0.00", "precip_1hr_metric": " 0", "precip_today_string": "0.00 in (0 mm)", "precip_today_in": "0.00", "precip_today_metric": "0", "icon": "partlycloudy", "icon_url": "http://icons-ak.wxug.com/i/c/k/partlycloudy.gif", "forecast_url": "http://www.wunderground.com/US/CA/San_Francisco.html", "history_url": "http://www.wunderground.com/history/airport/KCASANFR58/2012/6/27/DailyHistory.html", "ob_url": "http://www.wunderground.com/cgi-bin/findweather/getForecast?query=37.773285,-122.417725" } }`

You may just want to pull out one attribute \(like temp\_f or the temperature in Farenheit\). To do so, you'll need to use the object blocks below:

![](/assets/web-api-✕-fig-2.png)

---

### Uploading a row of data into a Spreadsheet

![](/assets/blocks-object-✕-fig-5.png)

For the Spreadsheet component, you will have to upload a row of data as an object similar to the blocks below:

![](/assets/blocks-object-✕-fig-6.png)

---

### Understanding what properties are contained in a Location object

![](/assets/blocks-object-✕-fig-3.png)

The Location Sensor components returns a latitude, longitude and location object and it's not always clear which attributes are available. One way to troubleshoot is to print out the JSON from the object like below

![](/assets/blocks-object-✕-fig-7.png)

This will output the following on your app

![](/assets/blocks-object-✕-fig-8.png)

