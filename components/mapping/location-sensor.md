#### **Thunkable for Android **❤

# Location Sensor ![](/assets/location-sensor-icon.png)

---

The Location Sensor triangulates between GPS satellites and mobile data networks to estimate a device's location in latitude, longitude. If available, GPS also measures altitude but you likely have to be outside for it to work properly. From the latitude and longitude readings, the location sensor can also provide an estimated street address and the speed at which a device may be moving.![](/assets/location-sensor-fig-1.png)

---

#### Measuring Location, Altitude and Speed

| Event / Property | Description |
| :--- | :--- |
| Available | Indicates whether the proximity sensor is present on the device |
| Maximum Range \(cm\) | Reports the maximum range of the device's proximity sensor |
| Proximity Changed \(distance \(cm\)\) | Called when distance \(in cm\) of the object to the device changes |
| Distance \(cm\) | Returns the distance from the object to the device \(in cm\) |
| Keep Running When on Pause | If  'true', will keep sensing for proximity changes even when the app is not visible |
| Enabled | If 'true', the proximity sensor is enabled |



