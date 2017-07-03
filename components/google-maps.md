#### **Thunkable for Android **❤

# Google Maps

---

Google Maps is one of the most popular and powerful components on Thunkable.  It enables users to locate themselves, share that location with others in real-time \(in combination with Firebase\) or map geo-located assets \(in combination with Spreadsheets powered by Cloudstitch\).

The map itself can be styled in a million different ways as can the markers that you add to the map.

---

### 

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

\*Only available in Blocks

**MapType**

Sets up map with a 'normal' MapType

![](/assets/maps-normal-blocks.png)

| 'normal' | 'terrain' |
| :--- | :--- |
| ![](https://thunkable.com/reference/components/images/visualization/u3341.png) | ![](/assets/maps-terrain.png) |
| 'satellite' | 'hybrid' |
| ![](/assets/maps-satellie.jpg) | ![](/assets/maps-hybrid.jpg) |

**Themes**

| 'standard' | 'silver' |
| :--- | :--- |
| ![](/assets/maps-standard.png) | ![](/assets/maps-silver.png) |
| 'retro' | 'dark' |
| ![](/assets/maps-retro.png) | ![](/assets/maps-dark.png) |
| 'night' | 'aubergine' |
| ![](/assets/maps-night.png) | ![](/assets/maps-aubergine.png) |

Style

\[   {     "elementType": "geometry",     "stylers": \[       {         "color": "\#f5f5f5"       }     \]   },   {     "elementType": "geometry.fill",     "stylers": \[       {         "color": "\#e3e3e3"       }     \]   },   {     "elementType": "labels.icon",     "stylers": \[       {         "visibility": "off"       }     \]   },   {     "elementType": "labels.text.fill",     "stylers": \[       {         "color": "\#616161"       }     \]   },   {     "elementType": "labels.text.stroke",     "stylers": \[       {         "color": "\#f5f5f5"       }     \]   },   {     "featureType": "administrative.land\_parcel",     "elementType": "labels.text.fill",     "stylers": \[       {         "color": "\#bdbdbd"       }     \]   },   {     "featureType": "poi",     "elementType": "geometry",     "stylers": \[       {         "color": "\#eeeeee"       }     \]   },   {     "featureType": "poi",     "elementType": "labels.text.fill",     "stylers": \[       {         "color": "\#757575"       }     \]   },   {     "featureType": "poi.park",     "elementType": "geometry",     "stylers": \[       {         "color": "\#e5e5e5"       }     \]   },   {     "featureType": "poi.park",     "elementType": "labels.text.fill",     "stylers": \[       {         "color": "\#9e9e9e"       }     \]   },   {     "featureType": "road",     "elementType": "geometry",     "stylers": \[       {         "color": "\#ffffff"       }     \]   },   {     "featureType": "road.arterial",     "elementType": "labels.text.fill",     "stylers": \[       {         "color": "\#757575"       }     \]   },   {     "featureType": "road.highway",     "elementType": "geometry",     "stylers": \[       {         "color": "\#dadada"       }     \]   },   {     "featureType": "road.highway",     "elementType": "labels.text.fill",     "stylers": \[       {         "color": "\#616161"       }     \]   },   {     "featureType": "road.local",     "elementType": "labels.text.fill",     "stylers": \[       {         "color": "\#9e9e9e"       }     \]   },   {     "featureType": "transit.line",     "elementType": "geometry",     "stylers": \[       {         "color": "\#e5e5e5"       }     \]   },   {     "featureType": "transit.station",     "elementType": "geometry",     "stylers": \[       {         "color": "\#eeeeee"       }     \]   },   {     "featureType": "transit.station.bus",     "stylers": \[       {         "weight": 6.5       }     \]   },   {     "featureType": "transit.station.bus",     "elementType": "labels.icon",     "stylers": \[       {         "color": "\#5aff97"       }     \]   },   {     "featureType": "transit.station.bus",     "elementType": "labels.text",     "stylers": \[       {         "color": "\#5aff97"       }     \]   },   {     "featureType": "water",     "elementType": "geometry",     "stylers": \[       {         "color": "\#c9c9c9"       }     \]   },   {     "featureType": "water",     "elementType": "geometry.fill",     "stylers": \[       {         "color": "\#c8f4ff"       }     \]   },   {     "featureType": "water",     "elementType": "geometry.stroke",     "stylers": \[       {         "weight": 3       }     \]   },   {     "featureType": "water",     "elementType": "labels.text.fill",     "stylers": \[       {         "color": "\#9e9e9e"       }     \]   }

