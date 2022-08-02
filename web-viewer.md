---
description: Display websites in your app
---

# Web Viewer

## Web Viewer Overview

{% hint style="info" %}
Some websites may not appear when previewing your app on the web. You may need to [Live Test](live-test.md#live-test) the app on a device, or [download](download.md) and install the app, to see your web page.
{% endhint %}

![](.gitbook/assets/web-viewer-fig-1.png)

## Properties

### Web Viewer

| Property | Description                                                                                                                                                                                     | Data Type |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| URL      | Set initial URL to be displayed in the Web Viewer. URL should begin with HTTPS://. Can also type in the name of a HTML file that has been uploaded to the project to display in the Web Viewer. | URL       |

### Advanced Properties

| Property                           | Description                                                              | Data Type  |
| ---------------------------------- | ------------------------------------------------------------------------ | ---------- |
| Geolocation Enabled (Android only) | Select if you want to enable geolocation functionality for Android apps. | True/False |

### Layout

| Property    | Description                                                                          | Data Type                                    |
| ----------- | ------------------------------------------------------------------------------------ | -------------------------------------------- |
| X           | Location of top left corner of Web Viewer on X-axis, where the left hand side is X=0 | Number                                       |
| Y           | Location of top left corner of Web Viewer on Y-axis, where the top side is Y=0       | Number                                       |
| Height      | Height of Web Viewer in pixels                                                       | Number                                       |
| Width       | Width of Web Viewer in pixels                                                        | Number                                       |
| Resize Mode | Define dimensions of the Web Viewer component/container                              | Select from list `[Stretch, Float in Place]` |

### **Style**

| Property       | Description                                                                             | Data Type                                  |
| -------------- | --------------------------------------------------------------------------------------- | ------------------------------------------ |
| Visible        | Toggle whether your end users can see the Web Viewer                                    | True/False                                 |
| Border Style   | Set whether border style is solid, dotted or dashed  (only visible if border width > 0) | Select from list `[solid, dotted, dashed]` |
| Border Color   | Color of border (only visible if border width > 0)                                      | Color                                      |
| Border Width   | Width of border around Web Viewer in pixels                                             | Number                                     |
| Border Radius  | Radius of corners of border on Web Viewer in degrees                                    | Number                                     |
| Shadow Color   | Color of Web Viewer's  shadow                                                           | Color                                      |
| Shadow Opacity | Opacity of Web Viewer's shadow                                                          | Number between 0 and 100                   |
| Shadow Radius  | Radius of corners of Web Viewer's shadow in pixels                                      | Number                                     |
| Shadow Offset  | How far Web Viewer's shadow should be offset, in height and width, in pixels            | Number                                     |

## Blocks

### Post Message/Receive Message

If you own the website being displayed in your Web Viewer, you can send and receive messages between your website and the Web Viewer using Javascript.

![](.gitbook/assets/wv\_post.png)

![](.gitbook/assets/wv\_receives.png)

You can see examples of sending/receiving messages and get further setup instructions [here](https://github.com/thunkable/webviewer-extension/).

#### See Also

You may also find the [Web API](web-api.md) component useful for sending/receiving information between your app and a website.

### Events

#### Receives Message

![](<.gitbook/assets/image (202).png>)

Fires when the Web Viewer receives a message from the web page it's displaying. Returns `message` output. This is a piece of text that contains the message that was returned.

### Functions

#### Reload&#x20;

![](.gitbook/assets/reload.png)

Reload the Web Viewer.

#### Back&#x20;

![](.gitbook/assets/back.png)

Go back to the previous page visited.

#### Forward&#x20;

![](.gitbook/assets/fwd.png)

Move forward to the next page in your browser history.

#### Post Message&#x20;

![](.gitbook/assets/screen-shot-2021-08-23-at-12.59.10-pm.png)

Post a message.

#### Value from Post

![](.gitbook/assets/screen-shot-2021-08-23-at-1.02.00-pm.png)

Returns any message that was received after calling the Post Message function.

### Properties

#### Computed Height&#x20;

![](.gitbook/assets/height.jpg)

Returns the on-screen dimensions of the web viewer, after it has been rendered on-screen.&#x20;

The value returned is an integer, representing the size of the Web Viewer in pixels.

#### Computed Width&#x20;

![](<.gitbook/assets/width (10).png>)

Returns the on-screen dimensions of the web viewer, after it has been rendered on-screen.&#x20;

The value returned is an integer, representing the size of the Web Viewer in pixels.

#### Visible

![](<.gitbook/assets/visible (3).png>)



Show or hide the Web Viewer.

#### URL

![](.gitbook/assets/url.png)

Change the web address that is displayed in the web viewer. Use **HTTPS://** URLs with this block.
