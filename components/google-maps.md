#### **Thunkable for Android **❤

# Google Maps

---

Google Maps is one of the most popular and powerful components on Thunkable.  It enables users to locate themselves, share that location with others in real-time \(in combination with Firebase\) or map geo-located assets \(in combination with Spreadsheets powered by Cloudstitch\).

The map itself can be styled in a million different ways and the markers you add to the map can be customized in a number of ways.

---

### Styling the map

| Property | Description |
| :--- | :--- |
| Height | Height in pixels, percent, 'Automatic' or 'Fill' |
| Width | Width in pixels, percent, 'Automatic' or 'Fill' |
| Zoom Level | 1 to 20 where 1 is most zoomed out.  We recommend zoom levels between 13 and 16 |
| Angle \(degrees\) | Tilt of the map from 0 to 90 degrees. We recommend tilts of 45 to 75 degrees and a Zoom Level of 16 for more immersive apps |
| Rotation \(degrees\) | Orientation of the map from 0 to 360 degrees. A rotation of 90 degrees rotates the map 90 degrees counterclockwise. We recommend keeping rotation at 0 except for specific circumstances |
| MapType\* | 'normal', 'terrain', 'satellite' or 'hybrid'. 'Normal' maps can be further customized with the Themes and Style \(json\) options below |
| Theme | 'standard' \(default\), 'silver', 'retro', 'dark', 'night' & 'aubergine'. MapType must be set to 'normal' \(default\) for themes to be enabled |
| Style \(json\)\* | Map style can be customized using a [Styling Wizard](https://mapstyle.withgoogle.com/) and importing the style JSON \(see example below\) |

\*Only available to be set in Blocks

#### **MapType**

Sets up map with a 'normal' MapType

![](/assets/maps-normal-blocks.png)

| 'normal' | 'terrain' | 'satellite' | 'hybrid' |
| :--- | :--- | :--- | :--- |
| ![](https://thunkable.com/reference/components/images/visualization/u3341.png) | ![](/assets/maps-terrain.png) | ![](/assets/maps-satellie.jpg) | ![](/assets/maps-hybrid.jpg) |

#### **Themes**

| 'standard' | 'silver' | 'retro' | 'dark' | 'night' | 'aubergine' |
| :--- | :--- | :--- | :--- | :--- | :--- |
| ![](/assets/maps-standard.png) | ![](/assets/maps-silver.png) | ![](/assets/maps-retro.png) | ![](/assets/maps-dark.png) | ![](/assets/maps-night.png) | ![](/assets/maps-aubergine.png) |

#### **Style \(json\)**

Google Maps lets users customize a map down to the color of the roads and the lakes.  You can use a [Styling Wizard](https://mapstyle.withgoogle.com/) to create a custom style JSON file that you can import to your map.![](/assets/maps-styling1.png)![](/assets/maps-styling2.png)

Sets up map with a custom 'white' and 'gray' style![](/assets/maps-styling-blocks.png)

`[ { "elementType": "geometry", "stylers": [ { "color": "#f5f5f5" } ] }, { "elementType": "geometry.fill", "stylers": [ { "color": "#ffffff" } ] }, { "elementType": "labels.icon", "stylers": [ { "visibility": "off" } ] }, { "elementType": "labels.text.fill", "stylers": [ { "color": "#000000" } ] }, { "featureType": "administrative.land_parcel", "elementType": "labels.text.fill", "stylers": [ { "color": "#bdbdbd" } ] }, { "featureType": "poi", "elementType": "geometry", "stylers": [ { "color": "#eeeeee" } ] }, { "featureType": "poi", "elementType": "labels.text.fill", "stylers": [ { "color": "#757575" } ] }, { "featureType": "poi.park", "elementType": "geometry", "stylers": [ { "color": "#e5e5e5" } ] }, { "featureType": "poi.park", "elementType": "labels.text.fill", "stylers": [ { "color": "#9e9e9e" } ] }, { "featureType": "road", "elementType": "geometry", "stylers": [ { "color": "#ffffff" } ] }, { "featureType": "road", "elementType": "geometry.fill", "stylers": [ { "color": "#d8d8d8" } ] }, { "featureType": "road.arterial", "elementType": "labels.text.fill", "stylers": [ { "color": "#757575" } ] }, { "featureType": "road.highway", "elementType": "geometry", "stylers": [ { "color": "#dadada" } ] }, { "featureType": "road.highway", "elementType": "labels.text.fill", "stylers": [ { "color": "#616161" } ] }, { "featureType": "road.local", "elementType": "labels.text.fill", "stylers": [ { "color": "#9e9e9e" } ] }, { "featureType": "transit.line", "elementType": "geometry", "stylers": [ { "color": "#e5e5e5" } ] }, { "featureType": "transit.station", "elementType": "geometry", "stylers": [ { "color": "#eeeeee" } ] }, { "featureType": "water", "elementType": "geometry", "stylers": [ { "color": "#e4e4e4" } ] }, { "featureType": "water", "elementType": "geometry.fill", "stylers": [ { "color": "#f3f3f3" } ] }, { "featureType": "water", "elementType": "labels.text.fill", "stylers": [ { "color": "#9e9e9e" } ] } ]`

---

### Adding standard markers, custom markers, circles & polylines to your map

| Event | Description |
| :--- | :--- |
| Height | Height in pixels, percent, 'Automatic' or 'Fill' |
| Width | Width in pixels, percent, 'Automatic' or 'Fill' |
| Zoom Level | 1 to 20 where 1 is most zoomed out.  We recommend zoom levels between 13 and 16 |
| Angle \(degrees\) | Tilt of the map from 0 to 90 degrees. We recommend tilts of 45 to 75 degrees and a Zoom Level of 16 for more immersive apps |
|  |  |

 

 

---

### Auto-centering map on user location

![](https://thunkable.com/reference/components/images/visualization/u3443.gif)

---





