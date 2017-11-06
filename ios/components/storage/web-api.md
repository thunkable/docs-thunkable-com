#### **Thunkable for iOS **

# Web API ![](/assets/web-api-ios-icon.png)

---

The Web API component provides functions for HTTP GET, POST, PUT, and DELETE requests used mainly to retrieve data from an open Web API service like Yahoo Finance for stock quotes or Weather Underground for weather information.

APIs unfortunately usually speak the language of code and not of humans so it is helpful to format these requests using our new [Object](/ios/blocks/objects.md) blocks.

---

#### Web API service settings

| Property | Description |
| :--- | :--- |
| Url | The url for the web request |
| Body |  |
| Query Parameters \(`property`, `value`\) |  |
| Headers \(`property`, `value`\) |  |

---

#### Retrieve data from a Web API

| Event | Description |
| :--- | :--- |
| Get \(`response`, `status`,`error`\) | Performs an HTTP GET request using the Url property and retrieves the `response`. Reports `status` of request and if request does not go through, will report an `error` |

---

#### Upload data to a Web API

| Event | Description |
| :--- | :--- |
| Put \(`response`, `status`,`error`\) | Performs an HTTP PUT request using the Url property and retrieves the `response`. Reports `status` of request and if request does not go through, will report an `error` |
| Post \(`response`, `status`,`error`\) | Performs an HTTP POSTT request using the Url property and retrieves the `response`. Reports `status` of request and if request does not go through, will report an `error` |

---

#### Delete data from a Web API

| Event | Description |
| :--- | :--- |
| Delete \(`response`, `status`,`error`\) | Performs an HTTP DELETE request using the Url property and retrieves the `response`. Reports `status` of request and if request does not go through, will report an `error` |



