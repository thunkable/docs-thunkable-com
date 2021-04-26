# Web API

Great data is an essential part of many apps built today and the Web API component enables apps to retrieve data from any public or private API \(application programming interface\) service on the web. For more advanced developers who have write access to a private API, this component also enables you to upload and delete data.

To see what public APIs are available, we recommend [this list from Todd Motto](https://github.com/toddmotto/public-apis)

## Adding a Web API to your app

To add a Web API component to your app:

* Go to your Blocks tab
* Find the `Advanced` drawer of blocks. Click the drop-down menu icon to show the Advanced invisible components
* Click the ⊕ icon next to the `Web APIs` drawer

![](.gitbook/assets/advanced-components%20%281%29.png)

You will see a dialog with options to enter certain properties for your Web API component. Click Submit to create the Web API component, or Delete to dismiss the dialog without creating the component.

![](.gitbook/assets/web-api-contents.png)

For most public APIs, you'll likely have to first create an account to get your own unique API key. This is usually to prevent individuals from making too many requests or to charge developers when they exceed certain free limits.

Once you have the API key, you'll need to enter the unique URL into the property field of the Web API component

| Property | Description | Required? |
| :--- | :--- | :--- |
| URL | The url for the web request which usually contains an API key | Required |
| Query Parameter | Specifies some parameters of the data | Optional |
| Body | Body of your API call | Optional |
| Headers | Specifies some meta-data, eg: usernames and passwords | Optional |

### Change properties of your Web API

Once you have added at least one Web API component to your app, you will be able to view all of your Web API components under the `Web APIs` drawer in the Advanced section of the Blocks tab. 

To edit the properties of a Web API component, click on the ⚙ icon next to the component's name to bring up the properties dialog. You will be able to change the properties and click Submit to save your changes, or click Delete to delete the component.

![](.gitbook/assets/web-apis-blicks.png)

## Setting Query Parameters and Headers

Query parameters and headers can be set in the designer or in the blocks editor. In the example below you can add any property:value pair you want. You can add as many params to your app as you need, but each parameter has to be added one at a time. 

![](.gitbook/assets/wvd0.png)

In the blocks editor, it is possible to use the `create object` block to add multiple property:value pairs simultaneously. 

![](.gitbook/assets/screen-shot-2021-04-12-at-8.59.11-am.png)

In addition to creating your own objects, it is also possible to use JSON to specify the property:value pairs for your query parameters or headers. 

![](.gitbook/assets/screen-shot-2021-04-12-at-9.00.03-am.png)

## Get and Format \(parse\) Data

![](.gitbook/assets/screen-shot-2021-04-12-at-9.01.33-am.png)

To retrieve data from an API, you simply need to use the `Get` block.

| Event | Description |
| :--- | :--- |
| Get \(`response`, `status`,`error`\) | Performs an HTTP GET request using the Url property and retrieves the `response`. Reports `status` of request and if request does not go through, will report an `error` |

Most APIs will return data in a less than usable format for your app so we'll take a few moments to walk through a few examples of how to format data \(also known as parsing\) using our [Object](objects.md) blocks

### Example 1: [Open Weather Map API](https://openweathermap.org/current)

You can find a working example of this in the sample app, [Office Weather & Traffic](https://docs.thunkable.com/sample-apps#office-weather).

One of the most common output formats for APIs is JSON, short for Javascript Object Notation. The Open Weather Map API returns a JSON file like the one below.

```text
{
    "coord":{"lon":85.17,"lat":26.67},
    "weather":[{"id":804,"main":"Clouds","description":"overcast clouds","icon":"04n"}],
    "base":"stations",
    "main":{
        "temp":298.312,
        "pressure":1005.31,
        "humidity":94,
        "temp_min":298.312,
        "temp_max":298.312,
        "sea_level":1011.47,
        "grnd_level":1005.31},
    "wind":{"speed":2.96,"deg":79.5005},
    "clouds":{"all":92},
    "dt":1533157826,
    "sys":{
        "message":0.0034,
        "country":"IN",
        "sunrise":1533080664,
        "sunset":1533128790},
    "id":1273043,
    "name":"Dhaka",
    "cod":200
}
```

#### **Convert JSON to Object**

![](.gitbook/assets/image%20%28105%29.png)

If you simply want to retrieve the temperature \(`"temp":` in line 6\), you will have to first convert the JSON response into objects, an _entity_ like a person that has _properties_ to describe them like smart. Objects can be embedded within another object.

In your JSON response, objects can be found within the `"` quotes `"` followed by a colon `:`. The properties of the object is follows the colon `:` but is within the `{` curly brackets`}`.

In the example above, `"coord":` , `"weather":`, `"base":` and `"main":` are both objects and properties of the overall object since they are contained within the `{` curly brackets `}`.

#### **Get Property of Object**

![](.gitbook/assets/image%20%2868%29.png)

Once you have converted the JSON into objects, you can then specify the `objects` and `property` that you are interested in. To get the temperature \(`"temp":` in line 6\), we'll want to find the `temp` property of the `main` object which is the property of the overall object

![](.gitbook/assets/screen-shot-2018-08-01-at-2.52.33-pm.png)

### Example 2: [Google Maps Distance Matrix API](https://developers.google.com/maps/documentation/distance-matrix/start)

You can find a working example of this in the sample app, [Ride](https://community.thunkable.com/t/advanced-sample-app-ride-a-private-uber-like-app-made-on-thunkable/30646).

The JSON output of the Google Maps Distance Matrix API seems similar to the Open Weather Map API with one notable exception: it includes objects, properties and _lists_. Lists are items bounded by `[` square brackets `]`.

```text
{
   "destination_addresses" : [ "Los Angeles, CA, USA" ],
   "origin_addresses" : [ "San Francisco, CA, USA" ],
   "rows" : [
      {
         "elements" : [
            {
               "distance" : {
                  "text" : "617 km",
                  "value" : 616620
               },
               "duration" : {
                  "text" : "5 hours 45 mins",
                  "value" : 20680
               },
               "status" : "OK"
            }
         ]
      }
   ],
   "status" : "OK"
}
```

If you want to retrieve the `"text"` property in line 13, you'll have to:

* convert the JSON to an object 
* select the `"rows"` property of the object
* select the first item in the list
* select the `"elements"` property of the rows object
* select the first item in the list
* select the `"duration"` property of the elements object
* select the `"text"` property of the duration object

You can see the example below for how this would look using the [Object](objects.md) and [List](lists.md) blocks

![](.gitbook/assets/screen-shot-2018-08-01-at-3.18.25-pm.png)

## Upload data

Uploading and deleting data is usually reserved for a private API that you or your organization owns

| Event | Description |
| :--- | :--- |
| Put \(`response`, `status`,`error`\) | Performs an HTTP PUT request using the Url property and retrieves the `response`. Reports `status` of request and if request does not go through, will report an `error` |
| Post \(`response`, `status`,`error`\) | Performs an HTTP POST request using the Url property and retrieves the `response`. Reports `status` of request and if request does not go through, will report an `error` |
| Patch \(`response, status, error`\) | Performs an HTTP PATCH request using the Url property and retrieves the `response`. Reports `status` of request and if request does not go through, will report an `error` |

## Delete data

| Event | Description |
| :--- | :--- |
| Delete \(`response`, `status`,`error`\) | Performs an HTTP DELETE request using the Url property and retrieves the `response`. Reports `status` of request and if request does not go through, will report an `error` |

## See Also

You can also post and receive messages between a web page and a [Web Viewer](web-viewer.md) using the Post Message function. Read more about that [here](web-viewer.md#post-message-receive-message).

