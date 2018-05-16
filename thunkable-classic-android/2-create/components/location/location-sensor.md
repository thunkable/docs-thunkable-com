---
description: >-
  The Location Sensor triangulates between GPS satellites and mobile data
  networks to estimate a device's location in latitude and longitude
---

# Location Sensor

###  ![](../../../../.gitbook/assets/location-sensor-icon.png)

If available, the Location Sensor also measures altitude but you likely have to be outside for it to work properly. From the latitude and longitude readings, the location sensor can also provide an estimated street address and the speed at which a device may be moving

![](../../../../.gitbook/assets/location-sensor-fig-1%20%281%29.png)

### Estimating Location, Altitude and Speed

| Event / Property | Description |
| :--- | :--- |
| Time Interval \(milliseconds\) | Determines the minimum time interval, in milliseconds, that the sensor will try to use for sending out location updates. Location updates will only be received when the location of the phone actually changes, and use of the specified time interval is not guaranteed. For example, if 1000 is used as the time interval, location updates will never be fired sooner than 1000ms, but they may be fired anytime after |
| Distance Interval \(meters\) | Determines the minimum distance interval, in meters, that the sensor will try to use for sending out location updates. For example, if this is set to 5, then the sensor will fire a LocationChanged event only after 5 meters have been traversed. However, the sensor does not guarantee that an update will be received at exactly the distance interval. It may take more than 5 meters to fire an event, for instance |
| Location Changed \(latitude, longitude, altitude, speed \(meters / second\) | Indicates that a new location has been detected |
| Latitude | In degrees from -90 to 90 |
| Longitude | In degrees from -180 to 180 |
| Altitude \(meters\) | In meters above sea level |
| Speed \(meters / second\) | Speed \(in meters / second\) as calculated by the distance between the most recent locations divided by the distance interval |
| Current Address | Estimated street address based on the sensed latitude and longitude coordinates that are geocoded or matches to a list of known addresses |
| Enabled | If 'true', location sensor will be enabled |

### Location Troubleshooting

While location accuracy has significantly improved in recent years, there are times when location is not easy to detect such as indoors.

| Property / Event | Description |
| :--- | :--- |
| Has Accuracy | Indicates if location sensor is able to connect to its service providers |
| Accuracy \(meters\) | Location confidence interval in meters |
| Has LongitudeLatitude | 'true' if location sensor is returning a longitude and latitude |
| Has Altitude | 'true' if location sensor is returning an altitude |
| Status Changed \(provider, status\) | Indicates that the status of the location provider service has changed, such as when a provider is lost or a new provider starts being used |
| Available Providers | List of available location providers including 'gps' |
| Provider Name | 'gps' or other network |
| Provider Locked | If "true", locked to current location provider |

### Estimating Latitude and Longitude from an Address

The Location Sensor can also estimate latitude and longitude from a street address

| Event | Description |
| :--- | :--- |
| Latitude From Address \(locationName\) | Derives latitude of given address |
| Longitude From Address \(locationName\) | Derives longitude of given address |

