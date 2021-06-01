# Maps by Google and Apple

![](.gitbook/assets/map-fig-1.png)

## Choose Your Provider

For iOS, you have the option to choose between Apple Maps or Google Maps. On Android, only Google Maps is available. Google Maps provides more custom style options from different map types to coloring and exposing or hiding map features.

| Property | Description |
| :--- | :--- |
| Provider `Advanced` | Default \(`google`\); To select Apple Maps for iOS, leave the property `blank` |

### Google Maps: Add API Key

It is possible to add your own Google Maps API Key to your Thunkable app project.

Simply click on your project name to open the [Project Settings](projects/settings.md) menu, and scroll down to the **Google Map Settings** section. You will see the option to enter a Google Maps API Key for Android and iOS.

![](.gitbook/assets/mapapikeys.png)

You can get your own Google Maps API Key [here](https://developers.google.com/maps/documentation/javascript/get-api-key).

## Zoom and Center the Map

To auto-center your map, you can pair the Map component with a [Location Sensor](location-sensor.md)

![](.gitbook/assets/screen-shot-2021-04-08-at-4.04.15-pm.png)

| Property | Description |
| :--- | :--- |
| Latitude | Default \(`37.78`\); Degrees north or south of the equator, from `-90` to `90.`Locations north of the equator are positive and those to the south are negative. Latitude at the equator is 0°. |
| Longitude | Default \(`-122.4`\); Degrees east or west of the prime meridian, from `-180` to `180`. Locations west of the prime meridian are negative and those to the east are positive. Longitude at the prime meridian is 0°. |
| Zoom | Default \(`0`\); Range is `-15` to `10` where -15 is most zoomed out |
| Shows User Location | Default \(`true`\); If `true`, shows user location as a blinking blue dot |
| Shows My Location Button \(Google Maps only\) | Default \(`true`\); In `true`, shows my location button that auto-centers map on user's location |

## Style the Map

![](.gitbook/assets/map-fig-3.png)

To style the Map like the picture above, set Provider to `Google`, Shows Traffic to `true`, Map Type to `standard` and Custom Map Style String to:

```javascript
[ { "elementType": "geometry", "stylers": [ { "color": "#f5f5f5" } ] }, { "elementType": "geometry.fill", "stylers": [ { "color": "#ffffff" } ] }, { "elementType": "labels.icon", "stylers": [ { "visibility": "off" } ] }, { "elementType": "labels.text.fill", "stylers": [ { "color": "#000000" } ] }, { "featureType": "administrative.land_parcel", "elementType": "labels.text.fill", "stylers": [ { "color": "#bdbdbd" } ] }, { "featureType": "poi", "elementType": "geometry", "stylers": [ { "color": "#eeeeee" } ] }, { "featureType": "poi", "elementType": "labels.text.fill", "stylers": [ { "color": "#757575" } ] }, { "featureType": "poi.park", "elementType": "geometry", "stylers": [ { "color": "#e5e5e5" } ] }, { "featureType": "poi.park", "elementType": "labels.text.fill", "stylers": [ { "color": "#9e9e9e" } ] }, { "featureType": "road", "elementType": "geometry", "stylers": [ { "color": "#ffffff" } ] }, { "featureType": "road", "elementType": "geometry.fill", "stylers": [ { "color": "#d8d8d8" } ] }, { "featureType": "road.arterial", "elementType": "labels.text.fill", "stylers": [ { "color": "#757575" } ] }, { "featureType": "road.highway", "elementType": "geometry", "stylers": [ { "color": "#dadada" } ] }, { "featureType": "road.highway", "elementType": "labels.text.fill", "stylers": [ { "color": "#616161" } ] }, { "featureType": "road.local", "elementType": "labels.text.fill", "stylers": [ { "color": "#9e9e9e" } ] }, { "featureType": "transit.line", "elementType": "geometry", "stylers": [ { "color": "#e5e5e5" } ] }, { "featureType": "transit.station", "elementType": "geometry", "stylers": [ { "color": "#eeeeee" } ] }, { "featureType": "water", "elementType": "geometry", "stylers": [ { "color": "#e4e4e4" } ] }, { "featureType": "water", "elementType": "geometry.fill", "stylers": [ { "color": "#f3f3f3" } ] }, { "featureType": "water", "elementType": "labels.text.fill", "stylers": [ { "color": "#9e9e9e" } ] } ]
```

There are a number of `Advanced` properties available to help you add custom styling to your map. Below are the most popular.

| Property | Description |
| :--- | :--- |
| Map Type `Advanced` | Default \(`standard`\); `standard` is the classic map style; `satellite` displays only satellite imagery; `hybrid` shows roads and features layered over satellite imagery; `terrain` shows physical terrain overlay on top of a classic map \(Google Maps only\) |
| Custom Map Style String \(Google Maps Only\) `Advanced` | Accepts a JSON string imported from the [Google Maps API styling wizard](https://mapstyle.withgoogle.com/). Map Type must be set to `standard` and provider must be set to `google`. |
| Shows Traffic `Advanced` | Default \(`false`\); if `true`, shows real-time traffic overlay on the map |

### Edit Map size

For more information on sizing in your app, please see our [introduction here​](https://docs.thunkable.com/~/edit/primary/thunkable-cross-platform/2-create/intro-to-sizing)

| Property | Description |
| :--- | :--- |
| Height | Default \(`Fill container`\); Four options: 1\) `Fit contents` which auto-sizes to the content size or 2\) `Fill container` which auto-sizes to the container 3\) `Relative size` in percent of Screen, 4\) `Absolute size` in pixels |
| Width | Default \(`Fit container`\); Four options: 1\) `Fit contents` which auto-sizes to the content size or 2\) `Fill container` which auto-sizes to the container 3\) `Relative size` in percent of Screen, 4\) `Absolute size` in pixels |

### Add Spacing

For more information on adding spacing in your app, please see our [introduction here](intro-to-spacing.md)

To find the spacing properties, you'll have to select the `Advanced` tab

| Property | Description |
| :--- | :--- |
| Margin `Advanced` | Default \(`none`\); Margin is the space outside of the border of a component; You can set space on the `top`, `bottom`, `right` or `left` of the component in both pixels or percent of Screen |
| Padding `Advanced` | Default \(`none`\); Padding is the space between the contents and the border of a component; You can set space on the `top`, `bottom`, `right` or `left` of the component in both pixels or percent of Screen |

### Add Marker

{% hint style="info" %}
There are limited styling options for markers at the moment. We are working to add the ability to change colors as well as add custom icons
{% endhint %}

![The default map marker is red on both Google and Apple Maps](.gitbook/assets/thunkable-documentation-exhibits-75%20%281%29.png)

You can add a standard default marker to your map with the blocks below. The Map component does not yet supply its own latitude and longitude so we currently recommend using the Location Sensor component

![](.gitbook/assets/screen-shot-2021-04-08-at-4.05.29-pm.png)

### Add Polyline

![This is the satellite map available on Google Maps on Android and iOS](.gitbook/assets/thunkable-documentation-exhibits-77.png)

To add a polyline, you can use the blocks below where `coordinates` need to be in a list of latitude and longitude objects, `stroke Width` is an integer and `stroke Color` is in hex format

![](.gitbook/assets/screen-shot-2021-04-08-at-4.07.39-pm.png)

### Add Polygon

![This is the satellite map available on Apple Maps, available for iOS](.gitbook/assets/thunkable-documentation-exhibits-76%20%281%29.png)

To add a polygon, you can use the blocks below where `coordinates` need to be in a list of latitude and longitude objects, `stroke Width` is an integer, `stroke Color` is in hex format, and `fill Color` is in hex format



![](.gitbook/assets/screen-shot-2021-04-08-at-4.09.05-pm.png)

### Delete Markers, Polylines and Polygons

You can use the **deleteAllMarkers** block to delete all [markers](map.md#add-marker) from your app.

![](.gitbook/assets/screen-shot-2021-04-08-at-4.09.33-pm.png)

You can use the **deleteAllPolylines** block to delete all [polylines](map.md#add-polyline) from your app.

![](.gitbook/assets/screen-shot-2021-04-08-at-4.10.01-pm.png)

You can use the **deleteAllPolygons** block to delete all [polygons](map.md#add-polygon) from your app.

![](.gitbook/assets/screen-shot-2021-04-08-at-4.09.45-pm.png)

## Map Events

The map has several events. You can trigger actions to happen when these events occur.

### On Map Ready

This event happens when the Map has loaded in your app. This is a good time to add any markers, polylines or polygons to your app that you want the user to see as soon as your app opens.

![](.gitbook/assets/screen-shot-2021-04-08-at-4.10.55-pm.png)

### On User Location Change

This event happens when the location of the user changes. It returns the **coordinate** object.  
You can use [object blocks](objects.md) to get the properties of the coordinate object.

The **coordinate** object has the following properties:

**target:** Numeric ID for your app  
**coordinate:{  
      latitude:** latitude of point selected  
      **longitude:** longitude of point selected   
**}  
position:{  
      x:** x-position of selected point on the Map component  
      **y:** x-position of selected point on the Map component  
**}**

![](.gitbook/assets/screen-shot-2021-04-08-at-4.12.54-pm.png)

### On Press

This event happens when the user taps on the Map.

![](.gitbook/assets/maponpressnew%20%281%29.png)

| Output name | Output value |
| :--- | :--- |
| Latitude | Latitude of selected position |
| Longitude | Longitude of selected position |
| position X | X Co-ordinate of selected position on map component |
| position Y | Y Co-ordinate of selected position on map component |

### On Long Press

This event happens when the user presses on the map for a longer period of time.

![](.gitbook/assets/maponlongpressnew.png)

| Output name | Output value |
| :--- | :--- |
| Latitude | Latitude of selected position |
| Longitude | Longitude of selected position |
| position X | X Co-ordinate of selected position on map component |
| position Y | Y Co-ordinate of selected position on map component |

### On Marker Press

This event happens when the user clicks on a Marker that is on the Map.

The **On Marker Press** block returns an **event** object. This is an object which can be used with [object blocks.](objects.md) The **event** block has the following properties:

**latitude:** returns the latitude of the selected Marker  
**longitude**: returns the longitude of the selected Marker

![](.gitbook/assets/screen-shot-2021-04-08-at-4.13.46-pm.png)

