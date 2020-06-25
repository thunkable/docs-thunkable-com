# Maps by Google and Apple

* [Choose your provider](map.md#choose-your-provider)
* [Zoom and center the Map](map.md#zoom-and-center-the-map)
* [Style the Map](map.md#style-the-map) 
  * [Edit Map size](map.md#edit-map-size)
  * [Add spacing](map.md#add-spacing)
  * [Add marker](map.md#add-marker)
  * [Add polyline](map.md#add-polyline)
  * [Add polygon](map.md#add-polygon)
  * [Clear map](https://docs.thunkable.com/map#clear-map)
* [Map Events](map.md#map-events)
  * [On Map Ready](map.md#on-map-ready)
  * [On User Location Change](map.md#on-user-location-change)
  * [On Press](map.md#on-press)
  * [On Long Press](map.md#on-long-press)
  * [On Marker Press](map.md#on-marker-press)

![](.gitbook/assets/map-fig-1.png)

## Choose Your Provider

For iOS, you have the option to choose between Apple Maps or Google Maps. On Android, only Google Maps is available. Google Maps provides more custom style options from different map types to coloring and exposing or hiding map features.

| Property | Description |
| :--- | :--- |
| Provider `Advanced` | Default \(`google`\); To select Apple Maps for iOS, leave the property `blank` |

## Zoom and Center the Map

To auto-center your map, you can pair the Map component with a Location Sensor

![](.gitbook/assets/map-fig-2.png)

| Property | Description |
| :--- | :--- |
| Latitude | Default \(`37.78`\); Degrees north or south of the equator, from `-90` to `90.`Locations north of the equator are positive and those to the south are negative. Latitude at the equator is 0°. |
| Longitude | Default \(`-122.4`\); Degrees east or west of the prime meridian, from `-180` to `180`. Locations west of the prime meridian are negative and those to the east are positive. Longitude at the prime meridian is 0°. |
| Zoom | Default \(`0`\); Range is `-15` to `10` where -15 is most zoomed out |
| Shows User Location | Default \(`true`\); If `true`, shows user location as a blinking blue dot |
| Shows My Location Button \(Google Maps only\) | Default \(`true`\); In `true`, shows my location button that auto-centers map on user's location |

## Style the Map

![](.gitbook/assets/map-fig-3.png)

To style the Map like the picture above, set Prover to `google`, Shows Traffic to `true`, Map Type to `standard` and Custom Map Style String to:

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

![](.gitbook/assets/screen-shot-2018-04-24-at-1.18.26-pm.png)

### Add Polyline

![This is the satellite map available on Google Maps on Android and iOS](.gitbook/assets/thunkable-documentation-exhibits-77.png)

To add a polyline, you can use the blocks below where `coordinates` need to be in a list of latitude and longitude objects, `stroke Width` is an integer and `stroke Color` is in hex format

![](.gitbook/assets/screen-shot-2018-04-24-at-4.58.42-pm.png)

### Add Polygon

![This is the satellite map available on Apple Maps, available for iOS](.gitbook/assets/thunkable-documentation-exhibits-76%20%281%29.png)

To add a polygon, you can use the blocks below where `coordinates` need to be in a list of latitude and longitude objects, `stroke Width` is an integer, `stroke Color` is in hex format, and `fill Color` is in hex format



![](.gitbook/assets/screen-shot-2018-04-24-at-5.14.08-pm.png)

### Clear Map

Sometimes it's helpful to clear all of the markers, polylines and polygons from the map, e.g. when you are trying to update your location in real-time which requires adding a marker and deleting existing markers.

The **deleteAllMarkers** block will clear all data from the map. This includes markers, polylines, and polygons.

![](.gitbook/assets/screen-shot-2019-06-18-at-2.56.36-pm.png)

## Map Events

The map has several events. You can trigger actions to happen when these events occur.

Some of these blocks return **position** and **coordinate** outputs. These are objects which can be used with [object blocks.](objects.md)

**Position** and **coordinate** will both return an object with the following properties:

**target:** Numeric ID for your app  
**coordinate:{  
      latitude:** latitude of point selected  
      **longitude:** longitude of point selected   
**}  
position:{  
      x:** x-position of selected point on the Map component  
      **y:** x-position of selected point on the Map component  
**}**  


### On Map Ready

This event happens when the Map has loaded in your app. This is a good time to add any markers, polylines or polygons to your app that you want the user to see as soon as your app opens.

![Example of using On Map Ready block](.gitbook/assets/onmapready.png)

### On User Location Change

This event happens when the location of the user changes. It returns the **coordinate** object.

![Example of using On user Location Change block](.gitbook/assets/userlocationchangedemo.png)

### On Press

This event happens when the user taps on the Map. It returns the **coordinate** and **position** objects.

![Example of using On Press block](.gitbook/assets/pressdemo.png)

### On Long Press

This event happens when the user presses on the map for a longer period of time. It returns the **coordinate** and **position** objects.

![Example of using On Long Press block](.gitbook/assets/maplongpressdemo.png)

### On Marker Press

This event happens when the user clicks on a Marker that is on the Map.

The **On Marker Press** block returns an **event** object. This is an object which can be used with [object blocks.](objects.md) The **event** block has the following properties:

**latitude:** returns the latitude of the selected Marker  
**longitude**: returns the longitude of the selected Marker

![Example of using On Marker Press block](.gitbook/assets/maponmarkerpressdemo.png)

