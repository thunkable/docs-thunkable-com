---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Switch Component

## Overview​ <a href="#switch-overview" id="switch-overview"></a>

The switch component is a two-state toggle that allows users to select between two options. It is commonly used in selecting on/off for things like sound, Bluetooth, WiFi etc.

<div align="left">

<figure><img src="../../../.gitbook/assets/switch (web preview - cropped).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

## Properties <a href="#getting-started" id="getting-started"></a>

### Switch

| Property         | Value      | Description                                        |
| ---------------- | ---------- | -------------------------------------------------- |
| Value            | True/False | Initial value of Switch                            |
| Tint Color       | Color      | Color of background when Switch is **false**       |
| On Tint Color    | Color      | Color of background when Switch is **true**        |
| Thumb Tint Color | Color      | Color of the Switch's slider                       |
| Disabled         | True/False | Toggle whether value Switch can be changed by user |

### Layout

| Property    | Value            | Desciption                                                                                               |
| ----------- | ---------------- | -------------------------------------------------------------------------------------------------------- |
| X           | coordinate value | Position of the upper left corner of the switch on the X-axis, where the left side of the screen is X=0. |
| Y           | coordinate value | Position of the upper left corner of the switch on the Y-axis, where the top of the screen is Y=0.       |
| Height      | number in pixels | The switch's height is defined by a custom number of pixels.                                             |
| Width       | number in pixels | The switch's width is defined by a custom number of pixels.                                              |
| Resize Mode | Stretch          | Stretches the switch to fit the dimensions of the device's screen.                                       |
| Resize Mode | Float in Place   | Renders the switch in the same aspect ratio as the design, regardless of the device size.                |

## Blocks <a href="#events" id="events"></a>

To access the blocks specific to the switch component:

1. On the Design tab, add a **Image** component to a screen.
2. Navigate to the **Blocks** tab.
3. In the component tree on the left, click the name of the image component.
4. A drawer of image-specific blocks opens.

| Block Image                                              | Description                                                                                                        |
| -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| ![](<../../../.gitbook/assets/image (226).png>)          | This event will fire when the user clicks on the image.                                                            |
| ![](../../../.gitbook/assets/setImage.png)               | Set the image component's Picture.                                                                                 |
| ![](../../../.gitbook/assets/getImage.png)               | Get the image component's Picture.                                                                                 |
| ![](../../../.gitbook/assets/setImageResize.png)         | Set the image component's [resize mode](switch.md#picture-resize-mode)                                             |
| ![](<../../../.gitbook/assets/getImageResize (1).png>)   | Get the image component's [resize mode](switch.md#picture-resize-mode)                                             |
| ![](../../../.gitbook/assets/setImageHeight.png)         | Set the image component's height.                                                                                  |
| ![](../../../.gitbook/assets/getImageHeight.png)         | Get the image component's height.                                                                                  |
| ![](../../../.gitbook/assets/getImageComputedHeight.png) | Returns the height of the image component in pixels after it has been rendered on-screen.                          |
| ![](../../../.gitbook/assets/setImageWidth.png)          | Set the image component's width.                                                                                   |
| ![](../../../.gitbook/assets/getImageWidth.png)          | Get the image component's width.                                                                                   |
| ![](../../../.gitbook/assets/getImageComputedWidth.png)  | Returns the width of the image component in pixels after it has been rendered on-screen                            |
| ![](../../../.gitbook/assets/setImageVisible.png)        | Set whether the image component is visible on the screen.                                                          |
| ![](../../../.gitbook/assets/getImageVisible.png)        | Get whether the image component is visible on the screen.                                                          |
| ![](../../../.gitbook/assets/setImageX.png)              | Set the position image the upper left corner of the image on the X-axis, where the left side of the screen is X=0. |
| ![](../../../.gitbook/assets/getImageX.png)              | Get the position of the upper left corner of the image on the X-axis, where the left side of the screen is X=0.    |
| ![](../../../.gitbook/assets/setImageY.png)              | Set the position of the upper left corner of the image on the Y-axis, where the top of the screen is Y=0.          |
| ![](../../../.gitbook/assets/getImageY.png)              | Get the position of the upper left corner of the image on the Y-axis, where the top of the screen is Y=0.          |

### Events&#x20;

#### On Value Change

![](../../../.gitbook/assets/screen-shot-2021-08-23-at-12.51.10-pm.png)

This event fires every time the switch is clicked.

Returns `newValue` output block, which returns the new value of the Switch (`true` or `false`).

### Properties

Use these blocks to set and get the named [properties](switch.md#getting-started) of the Switch.

#### Value&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZGFgk\_NS1U31Z65lg%2Fvalue.png?alt=media\&token=1e299ebf-80b0-4eca-9de1-bffa49bf40da)

#### Tint Color&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZGEHN\_gpbrhgSKHxM%2Ftint\_color.png?alt=media\&token=39b92335-6977-4768-9a67-d874838f9425)

#### On Tint Color&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZG6DZJ4tRxXoh61Dy%2Fon\_tint\_color.png?alt=media\&token=c980b50b-8eeb-4732-a802-1eb3d60fd05f)

#### Thumb Tint Color&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZG7d5VsHWrnTT99VE%2Fthumb\_tint\_color.png?alt=media\&token=223e8e93-175c-489f-bc04-2df46398601a)

#### Disabled&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZG3NqO-Qepj7sp5hj%2Fdisabled.png?alt=media\&token=ef01971d-5acc-4fa7-99a8-80d9e73c2b19)

#### X&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZGJHPWiFk0A6jxttz%2Fx.png?alt=media\&token=970de731-7f9d-4377-a161-a47889826d95)

#### Y

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZGKPvI15ZDZMgD4dU%2Fy.png?alt=media\&token=5f8c09a0-48a7-46a9-884d-742f1f984b3a)

#### Height&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZG4gitjHowTsf\_j\_L%2Fheight.png?alt=media\&token=8d69e6cd-4c36-45cc-a9ba-5c0d85afb8b2)

#### Width&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZGI49tqFn8CnxjOQa%2Fwidth.png?alt=media\&token=9e21c30e-8e20-4b01-830d-1c4f720cd4da)

####

#### Visible&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZGGpog3cyq9npq5Qo%2Fvisible.png?alt=media\&token=e0f07925-562e-41ac-8476-cf92eda91461)
