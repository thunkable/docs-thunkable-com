---
description: The label component allows you to display text in your app.
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

# Label Component

## Overview

The label component in mobile app development is a fundamental user interface element that displays static text or information on the screen. Labels work alongside other user interface components like buttons, images, and text inputs to create a cohesive and intuitive user experience.&#x20;

<figure><img src="../../../.gitbook/assets/label component overview.png" alt=""><figcaption></figcaption></figure>

## Properties

You can customize your label using the following properties:&#x20;

### Label

<table><thead><tr><th width="216.69525053355846">Property</th><th width="183.58335031860162">Value</th><th>Description</th></tr></thead><tbody><tr><td>Text</td><td>Text</td><td>Text that appears on the label</td></tr><tr><td>Font</td><td>Select from menu</td><td>Font used to display label's text</td></tr><tr><td>Custom Font (mobile only)*</td><td>OTF or TTF file</td><td>Font used to display label's text</td></tr><tr><td>Color</td><td>Color</td><td>Color of the text that appears on the label</td></tr><tr><td>Font Weight</td><td>True/False</td><td>Make the label's text bold</td></tr><tr><td>Font Style</td><td>True/False</td><td>Make the label's text italicized</td></tr><tr><td>Underline</td><td>True/False</td><td>Underline the label's text</td></tr><tr><td>Strikethrough</td><td>True/False</td><td>Apply strikethrough formatting to the label's text. You can further select the strikethrough's color and style. </td></tr><tr><td>Text Align</td><td>Select from menu</td><td>Set alignment of the text relative to the label's outline</td></tr><tr><td>Font Size</td><td>Number</td><td>Size of the text that appears on the label</td></tr><tr><td>Number Of Lines</td><td>Number</td><td>Maximum amount of lines of text that your label will display</td></tr></tbody></table>

{% hint style="info" %}
Uploading a custom font is available on Thunkable's Business and Enterprise plans.\
[Read more about our pricing plans here.](https://thunkable.com/#/pricing)
{% endhint %}

### Advanced Properties

| Property                                           | Value                                             | Description                            |
| -------------------------------------------------- | ------------------------------------------------- | -------------------------------------- |
| <p>Writing Direction </p><p>(iOS and web only)</p> | Select from list `[left-to-right, right-to-left]` | Writing direction of your label's text |
| <p>Letter Spacing </p><p>(iOS and web only)</p>    | number                                            | Spacing between letters of your label  |

### **Layout**

<table><thead><tr><th width="160.57888762769582">Property</th><th width="173">Value</th><th>Description</th></tr></thead><tbody><tr><td>X</td><td>coordinate value</td><td>Position of the upper left corner of the label on the X-axis, where the left side of the screen is X=0.</td></tr><tr><td>Y</td><td>coordinate value</td><td>Position of the upper left corner of the label on the Y-axis, where the top of the screen is Y=0.</td></tr><tr><td>Height</td><td>number in pixels</td><td>The label's height is defined by a custom number of pixels.</td></tr><tr><td>Width</td><td>number in pixels</td><td>The label's width is defined by a custom number of pixels.</td></tr><tr><td>Resize Mode</td><td>Stretch</td><td>Stretches the label's to fit the dimensions of the device's screen.</td></tr><tr><td>Resize Mode</td><td>Float in Place</td><td>Renders the label in the same aspect ratio as the design, regardless of the device size.</td></tr></tbody></table>

### Style

<table><thead><tr><th width="197.33333333333331">Property</th><th width="252">Value</th><th>Description</th></tr></thead><tbody><tr><td>Visible</td><td>visible</td><td>Users can see the label.</td></tr><tr><td>Visible</td><td>invisible</td><td>Users cannot see the label.</td></tr><tr><td>Background Color</td><td>color</td><td>The background color of the label.</td></tr><tr><td>Border: Style</td><td>solid</td><td>The label's border is a solid line.</td></tr><tr><td>Border: Style</td><td>dotted</td><td>The label's border is a dotted line.</td></tr><tr><td>Border: Style</td><td>dashed</td><td>The label's border is a dashed line.</td></tr><tr><td>Border: Color</td><td>color</td><td>The label's border is the color selected. </td></tr><tr><td>Border: Width</td><td>number in pixels</td><td>The width of the label's border is defined by a custom number of pixels.</td></tr><tr><td>Border: Radius</td><td>number in pixels</td><td>The radius of the label border’s corners is defined by a custom number of pixels.</td></tr><tr><td>Shadow: Color</td><td>color</td><td>The label's shadow is the color selected. </td></tr><tr><td>Shadow: Opacity</td><td>number between 0 and 100</td><td>The opacity of the label's shadow. </td></tr><tr><td>Shadow: Radius</td><td>number in pixels</td><td>The radius of the label shadow’s corners is defined by a custom number of pixels.</td></tr><tr><td>Shadow: Offset</td><td>number in pixels</td><td>How far the label's shadow should be offset, in height and width, is defined by a custom number of pixels.</td></tr></tbody></table>

## Label Blocks

To access the blocks specific to the label component:

1. On the Design tab, add a **Label** component to a screen.
2. Navigate to the **Blocks** tab.
3. In the component tree on the left, click the name of the label component.
4. A drawer of label-specific blocks opens.

| Block Image                                     | Description                                                                                                                                                                                                                                            |
| ----------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ![](<../../../.gitbook/assets/image (223).png>) | This event will fire when the user clicks on the label.                                                                                                                                                                                                |
| ![](<../../../.gitbook/assets/image 13.png>)    | Set the label's color with the color of the label itself i.e. the region behind the label text. Best practice is to use one of the [color blocks](../../../blocks/blocks/color.md) to set this value but HEX or RGB values may be used too.            |
| ![](<../../../.gitbook/assets/image 12.png>)    | Get the label's color.                                                                                                                                                                                                                                 |
| ![](<../../../.gitbook/assets/image 2.png>)     | Set the label's background color with the color of the label itself i.e. the region behind the label text. Best practice is to use one of the [color blocks](../../../blocks/blocks/color.md) to set this value but HEX or RGB values may be used too. |
| ![](<../../../.gitbook/assets/image 1.png>)     | Get the label's background color.                                                                                                                                                                                                                      |
| ![](<../../../.gitbook/assets/image 3 (2).png>) | Set the label's font size.                                                                                                                                                                                                                             |
| ![](<../../../.gitbook/assets/image 4 (1).png>) | Get the label's font size.                                                                                                                                                                                                                             |
| ![](<../../../.gitbook/assets/image 6.png>)     | Set's the label's font style. The font style property can be either "Normal" or "_Italic"._                                                                                                                                                            |
| ![](<../../../.gitbook/assets/image 5 (2).png>) | Get the label's font style.                                                                                                                                                                                                                            |
| ![](<../../../.gitbook/assets/image 7.png>)     | Set's the label's font weight.The font weight value can be either "Normal", "**Bold**" or a a value from 100 to 900                                                                                                                                    |
| ![](<../../../.gitbook/assets/image 8.png>)     | Get the label's font weight.                                                                                                                                                                                                                           |
| ![](<../../../.gitbook/assets/image 10.png>)    | <p></p><p>Set's the label's font height. Acceptable input values are: Number of Pixels, Percentage Height, "Fit Contents", or "Fill Container."</p>                                                                                                    |
| ![](<../../../.gitbook/assets/image 9.png>)     | Get the label's font height.                                                                                                                                                                                                                           |
| ![](<../../../.gitbook/assets/image 11.png>)    | The `Computed Height` block gets the on-screen dimensions of the label, after it has been rendered on-screen. The value returned is an integer, representing the size of the label in pixels.                                                          |
| ![](<../../../.gitbook/assets/image 14.png>)    | Set the label's number of lines.The number of lines property is used to work with the maximum number of lines of text that should be displayed in a label before that label starts to scroll.                                                          |
| ![](<../../../.gitbook/assets/image 15.png>)    | Get the label's number of lines.                                                                                                                                                                                                                       |
| ![](<../../../.gitbook/assets/image 16.png>)    | Set the label's text. This property corresponds to the text that is displayed in the label component.                                                                                                                                                  |
| ![](<../../../.gitbook/assets/image 17.png>)    | Get the label's text.                                                                                                                                                                                                                                  |
| ![](<../../../.gitbook/assets/image 18.png>)    | <p></p><p>Set the label's Text Align. Text Align can be any of the following values: Auto, Left, Right, Center, or Justify.</p>                                                                                                                        |
| ![](<../../../.gitbook/assets/image 19.png>)    | Get the label's Text Align.                                                                                                                                                                                                                            |
| ![](<../../../.gitbook/assets/image 20.png>)    | Set the label's Visibility. The visible blocks are used to show or hide the entire image component. Acceptable values are: true or false.                                                                                                              |
| ![](<../../../.gitbook/assets/image 21.png>)    | Get the label's Visibility.                                                                                                                                                                                                                            |
| ![](<../../../.gitbook/assets/image 23.png>)    | Set the label's width. The width blocks work with the Width property of the label component. Acceptable values are.‌                                                                                                                                   |
| ![](<../../../.gitbook/assets/image 22.png>)    | Get the label's width.                                                                                                                                                                                                                                 |
| ![](<../../../.gitbook/assets/image 24.png>)    | The `Computed Width` block gets the on-screen dimensions of the label, after it has been rendered on-screen. The value returned is an integer, representing the size of the label in pixels.                                                           |
