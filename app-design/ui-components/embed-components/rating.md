# Rating Component

## Rating Overview

The Rating component is a visible component which can be used to display the rating of a product or content in your app, and allow the user to leave their own rating.

A Rating component is made up of 5-10 _icons_. An icon can be filled, partially filled, or empty, as seen below:

![A Rating component displaying a rating of 3.5/5](../../../.gitbook/assets/rating.png)

## Properties

### Rating

| Property         | Description                                            | Data Type                                   |
| ---------------- | ------------------------------------------------------ | ------------------------------------------- |
| Value            | Initial value of your rating                           | Number                                      |
| Count            | Max value of your rating                               | Number between 5 and 10                     |
| Image\*          | Shape of the icons in your Rating component            | Select from menu (Pick One or Custom Image) |
| Read Only        | Toggle whether or not the user can edit the rating     | True/False                                  |
| Rating Color     | Color of filled-in icons to reflect the current rating | Color                                       |
| Background Color | Color of unfilled icons                                | Color                                       |

There are two ways to set an Image for your Rating component:

#### Select from Menu

Thunkable provides a menu of pre-set icons from Expo that you can choose from. [Preview these icons here.](https://icons.expo.fyi/)

#### Custom Image

If you set the Image property to Custom Image, you will be able use your own images as icons for the Rating component.&#x20;

Selecting Custom Image will show two new properties:

| Property     | Description                                                       | Data Type       |
| ------------ | ----------------------------------------------------------------- | --------------- |
| Filled Image | Images to reflect 'filled-in' icons to reflect the current rating | Image file name |
| Empty Image  | Images to reflect 'unfilled' icons                                | Image file name |

You can upload your images as [assets](../../../settings/assets.md) to your project, or provide URLs that point to your chosen images.

These URLs must end in a file extension, such as .jpg or .png.

### Layout

| Property    | Description                                                                                | Data Type                                    |
| ----------- | ------------------------------------------------------------------------------------------ | -------------------------------------------- |
| X           | Location of top left corner of Rating component on X-axis, where the left hand side is X=0 | Number                                       |
| Y           | Location of top left corner of Rating component on Y-axis, where the top side is Y=0       | Number                                       |
| Height      | Height of Rating component in pixels                                                       | Number                                       |
| Width       | Width of Rating component in pixels                                                        | Number                                       |
| Resize Mode | Define dimensions of the Rating component/container                                        | Select from list `[Stretch, Float in Place]` |

## Blocks

### Events

#### On Rate

This block fires when a user enters a rating in the Rating component.

![](../../../.gitbook/assets/rating-on-rate.png)

### Properties

Set and get [properties](rating.md#properties) of the Rating component

#### Count

![](../../../.gitbook/assets/count.png)

#### Direction

Select how the Rating component is displayed: as a **row** (left-right), **row-reverse** (right-left), **column** (top-bottom), or **column-reverse** (bottom-top).

![](../../../.gitbook/assets/direction.png)

#### Font Size

Change the size of the icons that make up the Rating component.

![](<../../../.gitbook/assets/font\_size (3).png>)

###

#### Height&#x20;

![](<../../../.gitbook/assets/height (8).png>)

#### Icon Margin&#x20;

Get or change the size of the margin between the icons of the Rating component.

![](../../../.gitbook/assets/icon\_margin.png)

#### Icon

You can select an image from the list available. All of the image options are suitable for any platform. You can preview the image options [here](https://icons.expo.fyi/).

You can upload your own images to be displayed for filled and empty icons.

![](../../../.gitbook/assets/icon.png)

#### Read Only

![](../../../.gitbook/assets/read\_only.png)

#### Rating Background Color

![](../../../.gitbook/assets/rating\_bg\_color.png)

#### Rating Color

![](../../../.gitbook/assets/rating\_color.png)

#### Value

![](<../../../.gitbook/assets/value (2).png>)

#### Visible

![](<../../../.gitbook/assets/visible (9).png>)

#### Width&#x20;

![](<../../../.gitbook/assets/width (9).png>)

#### X&#x20;

![](<../../../.gitbook/assets/x (1).png>)

#### Y

![](<../../../.gitbook/assets/y (1).png>)