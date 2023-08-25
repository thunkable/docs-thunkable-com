# Location Blocks

## Web Geocoding API Key

If you intend to publish a web app, you need to enter your personal Web Geocoding API Key in your project's app settings. This step is unnecessary for publishing and downloading to mobile devices. It is only required when publishing a project as a web app.&#x20;

To learn how to create your Web Geocoding API Key, see here: [Use API Keys with Geocoding API](https://developers.google.com/maps/documentation/geocoding/get-api-key)

To add your own Google Maps Web Geocoding API Key to your Thunkable project:

1. Follow these instructions to create your Web Geocoding API Key: [Use API Keys with Geocoding API](https://developers.google.com/maps/documentation/geocoding/get-api-key).
2. Click the **gear icon** on the left of your Thunkable project's Design tab to access your Project Settings.
3. Scroll to the **Google Map Settings** section.
4. Input your **Web Geocoding API Key** into the corresponding field.

<div align="left">

<figure><img src=".gitbook/assets/Google Maps Web Geocoding API Key.png" alt="" width="352"><figcaption></figcaption></figure>

</div>

## Coordinates from address

Geocoding is the process of converting an address to a latitude-longitude pair. To access this functionality in Thunkable, you use the `coordinates from address` block in the Location drawer of blocks.&#x20;

<div align="left">

<figure><img src=".gitbook/assets/coordinates from address block2.png" alt="" width="327"><figcaption></figcaption></figure>

</div>

**Outputs:**

* latitude
* longitude
* error

{% hint style="warning" %}
For Android, geocoding requires the device’s location services to be enabled.&#x20;
{% endhint %}

### Sample Block Combination

In the sample block combination below, when the Geocode button (btnGeocode) is clicked, the `coordinates form address` block will geocode the address the user has input in the text input (textAddress), and output the address’s latitude and longitude or an error if applicable. If there is an error, the label (labelError) will populate with the error output text. If there isn’t an error, the label (labelLocation) text will be populated by the address’s latitude and longitude, separated by a comma.&#x20;

<div align="left">

<figure><img src=".gitbook/assets/coordinates from address block combination2.png" alt="" width="563"><figcaption></figcaption></figure>

</div>

### Possible Errors

| Returned Value            | Explanation                                               |
| ------------------------- | --------------------------------------------------------- |
| ZERO\_RESULTS             | The request was successful but returned no results.       |
| INVALID\_REQUEST          | The request was not successful due to invalid parameters. |
| E\_LOCATION\_UNAUTHORIZED | Location services must be enabled.                        |

Additional error values are available here: [Google Maps Platform Status Codes](https://developers.google.com/maps/documentation/javascript/geocoding#GeocodingStatusCodes).

## Address from coordinates

Reverse Geocoding is the process of converting a latitude-longitude pair into a human-readable street address or [Plus Code](https://maps.google.com/pluscodes/). To access this functionality in Thunkable, you use the `address from coordinates` block, which is in the Location drawer of blocks.&#x20;

<div align="left">

<figure><img src=".gitbook/assets/address from coordinates block2.png" alt="" width="563"><figcaption></figcaption></figure>

</div>

{% hint style="warning" %}
For Android, reverse geocoding requires the device’s location services to be enabled.&#x20;
{% endhint %}

### Sample Block Combination

In the sample block combination below, when the Reverse Geocode button (btnReverse) is clicked, the `address from coordinates` block will engage in reverse geocoding using the latitude and longitude the user has input in the text inputs (textLat and textLng), and output the coordinate’s address or an error if applicable. If there is an error, the label (labelError) will populate with the error output text. If there isn’t an error, the label (labelAddress) text will be populated by the latitude and longitude’s address.&#x20;

<div align="left">

<figure><img src=".gitbook/assets/address from coordinates block combination2.png" alt="" width="563"><figcaption></figcaption></figure>

</div>

**Note:** The `address from coordinates` block in the image above is the advanced version of the block. To access this version:

1. Drag and drop the block into your workspace.
2. Right click on the block.
3. Select **Show advanced block**.

### Possible Errors

| Returned Value            | Explanation                                               |
| ------------------------- | --------------------------------------------------------- |
| ZERO\_RESULTS             | The request was successful but returned no results.       |
| INVALID\_REQUEST          | The request was not successful due to invalid parameters. |
| E\_LOCATION\_UNAUTHORIZED | Location services must be enabled.                        |

Additional error values are available here: [Google Maps Platform Status Codes](https://developers.google.com/maps/documentation/javascript/geocoding#GeocodingStatusCodes).

{% hint style="info" %}
If a street address is unavailable, the block may return a [Plus Code](https://maps.google.com/pluscodes/).
{% endhint %}

{% hint style="success" %}
**Have feedback on this doc?** Please take a moment to share your feedback here: [Thunkable Docs Feedback](https://docs.google.com/forms/d/e/1FAIpQLSfCwn5L2xyla-LSLZX0DSWFcFeJ43qp-r1tELCacuVS2zduLA/viewform?usp=sf\_link). Your valuable insights will help us improve and better serve you in the future.
{% endhint %}
