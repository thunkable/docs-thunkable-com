#### **Thunkable Cross-Platform **✕

# Location Sensor ![](/assets/iOSviewIconLocationSensor.png)

---

The Location Sensor component uses a phone's GPS, Wi-Fi and cellular network sensors to approximate a user's location

* [Get user's current location](#get-users-current-location-and-other-related-information)



---

#### Get user's current location \(and other related information\)



The Location Sensor returns a location `object`, which is a list of different location properties including latitude and longitude. To retrieve the property you are looking for, you'll have to use the `object blocks` like shown below

![](/assets/location-sensor-✕-fig-1.png)

| Event | Description |
| :--- | :--- |
| Get Current Location | If there is no error, returns a location `object` with the following properties: i\) `latitude` and `longitude` in degrees, i\) estimated location `accuracy` in meters,  iii\) location `provider` from gps, network, passive or fused, iv\) name of `locationProvider`, v\) `speed` in meters/second, vi\) `altitude` in meters, vii\) `bearing` in degrees and viii\) `time` in milliseconds since January 1, 1970. |

#### 



