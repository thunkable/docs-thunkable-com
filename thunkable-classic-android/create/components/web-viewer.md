# Web Viewer

###  ![](../../../.gitbook/assets/web-viewer-icon.png)

Web Viewers are powerful components for not only displaying websites but also images and custom html. Displaying custom html within a Web Viewer can enable Material Design effects or displaying simple websites when an internet connection is not available.

Users of Android 4.4 and above should have access to the latest Web Viewer available.

The current Web Viewer does support image uploading but not full screen video playing within a browser.

|  | Web Viewer Use 1 | Web Viewer Use 2 | Web Viewer Use 3 | Web Viewer Use 4 |
| :--- | :--- | :--- | :--- | :--- |
| Common use case | Display a website from a url | Display an image from url or file source. Supports .gifs unlike the Image component | Display an offline website from html | Display a Material Design element from html |

### Functionality

| Property | Description |
| :--- | :--- |
| Home URL | Accepts website or image urls that must include 'https://' or 'http://'. Can also accept image \(e.g. .png\) or html assets \(e.g. .html\) that have been uploaded to the app project |
| Follow Links | If checked, enables users to follow links when tapped in the WebViewer. |
| Use External Browser | If checked, opens an external browser when links are followed |
| Uses Location | If checked, gives app permission to use the geolocation API |
| Prompt for Permission | If checked, prompts the user to give permission to use the geolocation API |
| Ignore SSL Errors | If checked, ignores SSL errors.  Use this to accept self-signed certificates from websites |
| Go to URL | Loads the Web Viewer to a given url or source file |
| Go Home | Loads the Home URL |
| Go Back | Goes back to the previous page \(if available\) |
| Go Forward | Goes forward to next page \(if available\) |
| Clear Caches | Clears the Web Viewer caches |
| Clear Locations | Clears stored location permissions |

### **Appearance**

| Property | Description |
| :--- | :--- |
| Height | Height in pixels, percent, 'Automatic' or 'Fill' |
| Width | Width in pixels, percent, 'Automatic' or 'Fill' |
| Visible | If checked, the Web Viewer will be visible on the screen |
| Zoom Display | Recommend to uncheck, which disables zoom control.  if checked, enables zoom control |

