---
description: >-
  When you tap on the play icon to hear your favourite music, you are using a
  button.
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

# Button Component

## Overview

The button component gives your user familiar ways to start actions in your app. Examples include navigating between app screens, submitting user inputs, and triggering a device’s camera to take a photo.&#x20;

In the block combination below, when a user clicks Button1 they will be taken to, or navigate to, Screen2.

<div align="left">

<img src="../../../.gitbook/assets/btn_click_1.png" alt="Navigate to a different screen" width="375">

</div>

## Properties

### Button

<table><thead><tr><th width="214.33333333333331">Property</th><th width="198">Value</th><th>Description</th></tr></thead><tbody><tr><td>Text</td><td>Text</td><td>Text displayed on the button.</td></tr><tr><td>Font</td><td>Select from font menu</td><td>Font for the button's text.</td></tr><tr><td>Custom Font (mobile only)*</td><td>Upload TTF or OTF file</td><td>Font for the button's text.</td></tr><tr><td>Text Color</td><td>Color</td><td>Color the button's text.</td></tr><tr><td>Font Bold</td><td>True/False</td><td>True = button's text is <strong>bold</strong>.<br>False = button's text is not bold.</td></tr><tr><td>Font Italic</td><td>True/False</td><td>True = button's text is <em>italic.</em><br>False = button's text is not <em>italic.</em></td></tr><tr><td>Raised</td><td>True/False</td><td>True = button has a shadow.<br>False = button does not have a shadow.</td></tr><tr><td>Font Size</td><td>Number</td><td>Font size of the button's text.</td></tr><tr><td>Disabled</td><td>True/False</td><td>True = button is disabled for the user by default.<br>False = button is enabled for the user by default.</td></tr></tbody></table>

{% hint style="info" %}
Uploading a custom font may only be available for Creators on certain Thunkable plans. Please refer to our [pricing page](https://thunkable.com/#/pricing) for more information.
{% endhint %}

### Layout

<table><thead><tr><th width="158.66666666666666">Property</th><th width="186">Value</th><th>Description</th></tr></thead><tbody><tr><td>X</td><td>coordinate value</td><td>Position of the upper left corner of the button on the X-axis, where the left side of the screen is X=0.</td></tr><tr><td>Y</td><td>coordinate value</td><td>Position of the upper left corner of the button on the Y-axis, where the top of the screen is Y=0.</td></tr><tr><td>Height</td><td>number in pixels</td><td>The button's height is defined by a custom number of pixels.</td></tr><tr><td>Width</td><td>number in pixels</td><td>The button's width is defined by a custom number of pixels.</td></tr><tr><td>Resize Mode</td><td>Stretch</td><td>Stretches the button to fit the dimensions of the device's screen.</td></tr><tr><td>Resize Mode</td><td>Float in Place</td><td>Renders the button in the same aspect ratio as the design, regardless of the device size.</td></tr></tbody></table>

### Style

| Property                    | Description                                                           | Data Type                                  |
| --------------------------- | --------------------------------------------------------------------- | ------------------------------------------ |
| Visible                     | Toggle whether your end users can see the Button                      | True/False                                 |
| Background (Color or Image) | Button's background color or the image displayed on the button        | Color or uploaded image file               |
| Border Style                | Style of Button's border                                              | Select from list `[solid, dotted, dashed]` |
| Border Color                | Color of Button's border                                              | Color                                      |
| Border Width                | Width of Button's border in pixels                                    | Number                                     |
| Border Radius               | Radius of corners of Button's border in pixels                        | Number                                     |
| Shadow Color                | Color of Button's shadow                                              | Color                                      |
| Shadow Opacity              | Opacity of Button's shadow                                            | Number between 0 and 100                   |
| Shadow Radius               | Radius of corners of Button's shadow in pixels                        | Number                                     |
| Shadow Offset               | How far the Button's shadow is offset, in Height and Width, in pixels | Number                                     |

## Blocks

### Events

You can use the following blocks to listen for when a specific event occurs

#### Click

![](../../../.gitbook/assets/click.png)

Performs an action when the user taps the button.

#### Long Click

![](../../../.gitbook/assets/long\_click.png)

Performs an action when the user holds down the button.

#### Touch Down

![](../../../.gitbook/assets/touch\_down.png)

Performs an action when a user pressed down on the button

#### Touch Up

![](../../../.gitbook/assets/touch\_up.png)

Performs an action after the user releases the button

### Properties

#### Background Color

![](<../../../.gitbook/assets/bg\_color (1).png>)

The get and set background color properties work with the color of the button itself i.e. the region behind the button text. Best practice is to use one of the built [color blocks](../../../blocks/blocks/color.md) to set this value, but you can use HEX and RGB values too.

#### Background Picture

![](../../../.gitbook/assets/bg\_picture.png)



#### Background Picture Resize Mode

![](../../../.gitbook/assets/resize\_mode.png)

The set and get resize mode blocks work with how the background picture is scaled within the button component. Acceptable values are:

* Cover
* Contain
* Stretch
* Repeat
* Center

#### Disabled

![](../../../.gitbook/assets/disabled.png)

The disabled property is used to set whether or not the button is "clickable". Expected values for this property are:

* True
* False



#### Font

![](<../../../.gitbook/assets/bold (1).png>)

![](../../../.gitbook/assets/italic.png)

![](../../../.gitbook/assets/raised.png)

The font style properties of the button text can be "**Bold**",  "_Italic",_ or Raised. Expected values for each property are:

* True
* False

#### Font Size

![](../../../.gitbook/assets/font\_size.png)

The get and set font size blocks are used to work with the size of the text that is displayed in the button. This value must be a number.

#### Height

![](../../../.gitbook/assets/height.png)



The set and get height blocks work with the Height property of the button component. Acceptable input values are.&#x20;

* Number of Pixels
* Percentage Height
* "Fit Contents"
* "Fill Container"

The `Computed Height`block returns the on-screen dimensions of the button, after it has been rendered on-screen. The value returned is an integer, representing the size of the button in pixels.

#### Text

![](../../../.gitbook/assets/text.png)

This property corresponds to the text that is displayed in the button component.

#### Text Color

![](../../../.gitbook/assets/text\_color.png)

The get and set text color properties can be used to work with the color of the text displayed on the button. Best practice is to use one of the [color blocks](../../../blocks/blocks/color.md) to set this value but you can use HEX and RGB values too.

#### Visible

![](../../../.gitbook/assets/visible.png)



The set and get visible blocks are used to show or hide the entire button component. Acceptable values are:

* True
* False

#### Width

![](../../../.gitbook/assets/width.png)

The set and get width blocks work with the Width property of the button component. Acceptable input values are.&#x20;

* Number of Pixels
* Percentage Width
* "Fit Contents"
* "Fill Container"

The `Computed Width`block returns the on-screen dimensions of the button, after it has been rendered on-screen. The value returned is an integer, representing the size of the button in pixels.

{% hint style="success" %}
**Have feedback on this doc?** Please take a moment to share your feedback here: [Thunkable Docs Feedback](https://docs.google.com/forms/d/e/1FAIpQLSfCwn5L2xyla-LSLZX0DSWFcFeJ43qp-r1tELCacuVS2zduLA/viewform?usp=sf\_link). Your valuable insights will help us improve and better serve you in the future.
{% endhint %}
