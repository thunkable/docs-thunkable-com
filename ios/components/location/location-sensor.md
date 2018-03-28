#### **Thunkable for iOS **

# Location Sensor

---

The Location Sensor component uses a phone's GPS, Wi-Fi and cellular network sensors to approximate a user's location. With permission of the user, this component also can track a user's location history, both when the app is open and when it is in the background.

* [Get user's current location](#get-users-current-location-and-other-related-information)
* [Track user's location](#track-users-location)

---

#### Get user's current location \(and other related information\)

![](/assets/location-sensor-✕-fig-2.png)The Location Sensor returns a location `object`, which is a list of different location properties including latitude and longitude. To retrieve the property you are looking for, you'll have to use the `object blocks` like shown below

![](/assets/location-sensor-✕-fig-1.png)

| Event | Description |
| :--- | :--- |
| Get Current Location \(location `object`, error\) | Returns a location, which is an `object` with the following properties: i\) `latitude` and `longitude` in degrees, i\) estimated location `accuracy` in meters,  iii\) location `provider` from gps, network, passive or fused, iv\) name of `locationProvider`, v\) `speed` in meters/second, vi\) `altitude` in meters, vii\) `bearing` in degrees and viii\) `time` in milliseconds since January 1, 1970. |

---

#### Track user's location

| Event | Description |
| :--- | :--- |
| Start Tracking \(error\) | Starts tracking a user's location in the foreground and/or background depending on user's permission; Locations are stored locally on a user's phone by default |
| Stop Tracking \(error\) | Stops tracking a user's location in the foreground and/or background depending on user's permission |
| Get Stored Locations \(location `object`, error\) | Gets user's stored locations in a location `object` |
| Delete Stored Locations \(error\) | Deletes a user's locally stored locations; recommended each time you start tracking a user's location |



