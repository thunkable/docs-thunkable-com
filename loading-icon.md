# Loading Icon

## Loading Icon Overview

For activities that take more than a few seconds, loading icons can be helpful to tell your app users that an activity is happening in the background, such as retrieving or uploading data.

![The large loading icon is on the top; the small is on the bottom on a Pixel 3](.gitbook/assets/ezgif.com-crop.gif)

## Style the Loading Icon 

| Property | Description |
| :--- | :--- |
| Color | The color of the loading icon |

## Edit size and position

You can drag and drop your component into position, and set its size.   
You can set exact values for the component's Height and Width, and X and Y coordinates, in its properties.

**Height:** Height of Button in pixels  
**Width:** Width of Button in pixels

**X:** position of top left corner of Button on X-axis  
**Y:** position of top right corner of component on Y-axis

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

