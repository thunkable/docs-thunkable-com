#### **Thunkable for iOS **

# Location Sensor ![](/assets/iOSviewIconLocationSensor.png)

---

The Location Sensor component uses a phone's GPS, Wi-Fi and cellular network sensors to approximate a user's location. With permission of the user, this component also can track a user's location history, both when the app is open and when it is in the background.

The Location Sensor component is optimized to save battery \(since location tracking can be battery intensive\). In tracking mode, the Location Sensor does not track the phone when it is stationary.

* [Get user's current location](#get-users-current-location-and-other-related-information)
* [Track user's location](#track-users-location)

---

#### Get user's current location \(and other related information\)

![](/assets/location-sensor-✕-fig-2.png)The Location Sensor returns a location `object`, which is a list of different location properties including latitude and longitude. To retrieve the property you are looking for, you'll have to use the `object blocks` like shown below

![](/assets/location-sensor-✕-fig-1.png)

| Event | Description |
| :--- | :--- |
| Get Current Location | If there is no error, returns a location `object` with the following properties: i\) `latitude` and `longitude` in degrees, i\) estimated location `accuracy` in meters,  iii\) location `provider` from gps, network, passive or fused, iv\) name of `locationProvider`, v\) `speed` in meters/second, vi\) `altitude` in meters, vii\) `bearing` in degrees and viii\) `time` in milliseconds since January 1, 1970. |

---

#### Track user's location

Location tracking is both a very useful and potentially worrisome superpower that most phones are now able to do. On the positive side, location tracking can provide information that can improve the user experience e.g. when Uber knows your pick-up location when you open the app.

On the negative side, it can be a violation of user privacy so both Android and iOS have controls on the operating system level to make sure users must give permission to track their location.

The Location Sensor component by default tracks a user's location both when the app is open \(foreground\) and when it is in the background. A user on iOS can designate if she or he wants to allow location tracking only when the app is open, at all times or not at all. A user on Android must accept permission to track during installation.![](/assets/location-sensor-✕-fig-3.png)

Location Sensory history is stored locally on the phone so must be deleted when starting a new session.

| Event | Description |
| :--- | :--- |
| Start Tracking | Starts tracking a user's location in the foreground and/or background depending on user's permission; Locations are stored locally on a user's phone by default |
| Stop Tracking | Stops tracking a user's location in the foreground and/or background depending on user's permission |
| Get Stored Locations | Returns a user's stored locations in as a list of location `objects` |
| Delete Stored Locations | Deletes a user's locally stored locations; recommended each time you start tracking a user's location |



