#### **Thunkable Cross-Platform **✕

# Map ![](/assets/iOSviewIconGoogleMap.png)![](/assets/iOSviewIconMap.png) powered by Google and Apple Maps

---

Maps are one of the most popular services today and with the Map component, you can choose to add a Google or Apple Map \(iOS only\) to your apps

* Choose your provider
* Zoom and center your map
* Style your map \(Google Maps only\)
* Editing size
* Add markers
* Add polylines
* Add polygons

![](/assets/map-✕-fig-1.png)

---

### Choose your provider

For iOS, you have the option to choose between Apple Maps or Google Maps. On Android, only Google Maps is available. Google Maps provides more custom style options from different map types to coloring and exposing or hiding map features.

| Property | Description |
| :--- | :--- |
| Provider | Default \(`google`\); To select Apple Maps for iOS, leave the property `blank` |

---

### Zoom and center your map

To auto-center your map, you can pair the Map component with a Location Sensor. `There is currently a bug with the blocks below working on Android`

![](/assets/map-✕-fig-2.png)



| Property | Description |
| :--- | :--- |
| Latitude | Default \(`37.78`\); In degrees above the equator from `-90` to `90` where locations north of the equator are positive and those south are negative |
| Longitude | Default \(`-122.4`\); In degrees east or west from the equator from `-90` to `90` where locations west of the equator are negative and those east are positive |
| Zoom | Default \(`0`\); Range is -15 to 10 where -15 is most zoomed out |
| Shows User Location | Default \(`true`\); If `true`, shows user location as a blinking blue dot |
| Shows My Location Button \(Google Maps only\) | Default \(`true`\); In `true`, shows my location button that auto-centers map on user's location  |

---

### Style your map \(Google Maps only\)



---

### Size your map

| Property | Description |
| :--- | :--- |
| Height | Default \(`Fill container`\); Four options: 1\) `Fit contents` which auto-sizes to the content size or 2\) `Fill container` which auto-sizes to the container 3\) `Relative size` in percent of Screen, 4\) `Absolute size` in pixels |
| Width | Default \(`Fit container`\); Four options: 1\) `Fit contents` which auto-sizes to the content size or 2\) `Fill container` which auto-sizes to the container 3\) `Relative size` in percent of Screen, 4\) `Absolute size` in pixels |



