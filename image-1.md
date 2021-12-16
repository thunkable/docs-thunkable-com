---
description: The image component lets you display pictures in your app.
---

# Image

## Image Overview

The Image component lets you display pictures in your app and pairs nicely with image based components like the [Camera](camera.md), [Photo Library](camera.md#use-image-from-photo-library), [Image Recognizer](camera.md#image-recognition) and [Media DB](camera.md#upload-image-to-the-cloud)

![](.gitbook/assets/image-fig-1.png)

## Set Image

There are a few ways you can display an image in your app:\
****

1. **Upload a picture to your project's Assets**\
   ****\
   ****![](.gitbook/assets/assets\_upload.png)\

2. **Provide a link in the Image properties:**\
   ****\
   ****![](.gitbook/assets/img\_type\_in\_url.png)\

3. **Take a picture with the Camera component**

![](.gitbook/assets/take\_photo.png)

The blocks above open up your phone’s camera and set the Image component to the picture that you took.&#x20;

## Edit size and position

You can drag and drop your component into position, and set its size. \
You can set exact values for the component's Height and Width, and X and Y coordinates, in its properties.

**Height:** Height of Button in pixels\
**Width:** Width of Button in pixels

**X:** position of top left corner of Button on X-axis\
**Y:** position of top right corner of component on Y-axis

## Resizing the Image

![](.gitbook/assets/image-fig-3.png)

With the Resize Mode property, you can do the following:

* **Cover:** Resizes the picture to its max height or width regardless without changing the image quality.
* **Contain:** Resizes the picture to fit the area without changing its quality
* **Stretch:** The picture’s height will change to fill the image component length-wise
* **Repeat:** Repeats the picture at its original quality within the image component area
* **Center:** Positions the picture in the middle of the image component

## Add a Border

You can style the image with the following properties:

* **Border**
  * **Width:** Enter how wide you want the border outline of the image to be&#x20;
  * **Color:** Pick a color for the border of the image
  * **Radius:** Enter how round you want the edges of the border for the image to be ****&#x20;

## Events

### Click

![](.gitbook/assets/image\_click.png)

This event handler is fired when the user clicks on the image.

## Properties

### Computed Dimensions

![](<.gitbook/assets/screen-shot-2021-04-08-at-4.19.37-pm-copy (2).jpg>)

![](<.gitbook/assets/screen-shot-2021-04-08-at-4.19.37-pm-copy (1).jpg>)

The `Computed Height` and `Computed Width` blocks return the on screen dimensions of the image, after it has been rendered on-screen. The value returned is an integer, representing the size of the image in pixels.

### Height&#x20;

![](<.gitbook/assets/screen-shot-2021-04-08-at-4.19.37-pm-copy (3).jpg>)

The set and get height blocks work with the Height property of the image component. Acceptable input values are.&#x20;

* Number of Pixels
* Percentage Height
* "Fit Contents"
* "Fill Container"

### Picture&#x20;

![](.gitbook/assets/picture.png)

The set and get picture blocks work with picture property of the image component. Pictures can be uploaded as local assets or specified as URLs&#x20;

### Resize Mode&#x20;

![](<.gitbook/assets/resize\_mode (1).png>)

The set and get resize mode blocks work with how the picture is scaled within the image component. Acceptable values are:

* Cover
* Contain
* Stretch
* Repeat
* Center

### Visible&#x20;

![](<.gitbook/assets/visible (12).png>)

The set and get visible blocks are used to show or hide the entire image component. Acceptable values are:

* True
* False

### Width

![](.gitbook/assets/screen-shot-2021-04-08-at-4.19.37-pm-copy.jpg)

\
The set and get width blocks work with the Width property of the image component. Acceptable values are.‌

* Number of Pixels
* Percentage Width
* "Fit Contents"
* "Fill Container"

