#### **Thunkable for Android **❤

# Web Viewer

---

Web Viewers are powerful components for not only displaying websites but also images and custom html.  Displaying custom html within a Web Viewer can enable Material Design effects or displaying simple websites when an internet connection is not available.

### 

---

#### Functionality

| Property | Description |
| :--- | :--- |
| **Home URL** | Accepts website or image urls that must include 'https://' or 'http://'. Can also accept image \(e.g. .png\) or html assets \(e.g. .html\) that have been uploaded to the app project |
| Follow Links | If checked, enables users to follow links when tapped in the WebViewer.   |
| Use External Browser | If checked, opens an external browser when links are followed |
| Uses Location\* | If checked, gives app permission to use the geolocation API |
| Prompt for Permission | If checked, prompts the user to give permission to use the geolocation API |
| Ignore SSL Errors | If checked, ignores SSL errors.  Use this to accept self-signed certificates from websites |

---

#### **Appearance**

| Property | Description |
| :--- | :--- |
| Height | Height in pixels, percent, 'Automatic' or 'Fill' |
| Width | Width in pixels, percent, 'Automatic' or 'Fill' |
| Visible | If checked, the Web Viewer will be visible on the screen |
| Zoom Display | Recommend to uncheck, which disables zoom control.  if checked, enables zoom control |

---

#### Events \(Websites Only\)

CurrentPageTitle

Title of the page currently viewed

IgnoreSslError

Determine whether or not to ignore SSL errors. Set to true to ignore errors. Use this to accept self signed certificates from websites.

WebViewString

Gets the WebView's String, which is viewable through Javascript in the WebView as the window.AppInventor object

Boolean CanGoBack\(\)

Returns true if the WebViewer can go back in the history list.

Boolean CanGoForward\(\)

Returns true if the WebViewer can go forward in the history list.

ClearCaches\(\)

Clear the WebViewer caches

ClearLocations\(\)

Clear stored location permissions.

GoBack\(\)

Go back to the previous page in the history list. Does nothing if there is no previous page.

GoForward\(\)

Go forward to the next page in the history list. Does nothing if there is no next page.

GoHome\(\)

Loads the home URL page. This happens automatically when the home URL is changed.

GoToUrl\(text url\)

Load the page at the given URL.



