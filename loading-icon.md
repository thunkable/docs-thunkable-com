# Loading Icon

## Video Tutorial

{% embed url="https://youtu.be/y7WnblzAt2c" %}

## Loading Icon Overview

* [Style the Icon](loading-icon.md#style-the-loading-icon)
* [Show or Hide the Icon](loading-icon.md#showing-and-hiding-the-loading-icon)
* [Properties](loading-icon.md#properties)

For activities that take more than a few seconds, loading icons can be helpful to tell your app users that an activity is happening in the background, such as retrieving or uploading data.

![The large loading icon is on the top; the small is on the bottom on a Pixel 3](.gitbook/assets/ezgif.com-crop.gif)

## Style the Loading Icon 

| Property | Description |
| :--- | :--- |
| Color | The color of the loading icon |
| Size | `Small` or `large` |

## Showing and Hiding the Loading Icon

The loading icon should be displayed when the app is performing an activity in the background and hidden when it is not. 

One way to show and hide the icon is to use the `visible` property of the component.

In the following example the loading icon shows up when the app opens but disappears after data is retrieved from Airtable.

![](.gitbook/assets/li_legacy.png)

When the visibility is set to true, the loading icon will be seen on the app screen. If set to false, the loading icon will not be seen on the app screen.

## Properties

### Color 

![](.gitbook/assets/color%20%282%29.png)

### Height 

![](.gitbook/assets/height%20%286%29.png)

### Size 

![](.gitbook/assets/size%20%281%29.png)

### Visible 

![](.gitbook/assets/visible%20%288%29.png)

### Width

![](.gitbook/assets/width%20%288%29.png)

