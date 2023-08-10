---
description: The label component allows you to display text in your app.
---

# Label Component

## Properties

You can customize your label using the following properties:&#x20;

### Label

<table><thead><tr><th width="216.69525053355846">Property</th><th>Description</th><th>Data Type</th></tr></thead><tbody><tr><td>Text</td><td>Text that appears on the label</td><td>Text</td></tr><tr><td>Font</td><td>Font used to display Label's text</td><td>Select from menu</td></tr><tr><td>Custom Font (mobile only)*</td><td>Font used to display Label's text</td><td>OTF or TTF file</td></tr><tr><td>Color</td><td>Color of the text that appears on the label</td><td>Color</td></tr><tr><td>Font Weight</td><td>Make the label's text bold</td><td>True/False</td></tr><tr><td>Font Style</td><td>Make the label's text italicized</td><td>True/False</td></tr><tr><td>Underline</td><td>Underline the label's text</td><td>True/False</td></tr><tr><td>Strikethrough</td><td>Apply strikethrough formatting to the label's text. You can further select the strikethrough's color and style. </td><td>True/False</td></tr><tr><td>Text Align</td><td>Set alignment of the text relative to the Label's outline</td><td>Select from menu</td></tr><tr><td>Font Size</td><td>Size of the text that appears on the label</td><td>Number</td></tr><tr><td>Number Of Lines</td><td>Maximum amount of lines of text that your Label will display</td><td>Number</td></tr></tbody></table>

{% hint style="info" %}
Uploading a custom font is available on Thunkable's Business and Enterprise plans.\
[Read more about our pricing plans here.](https://thunkable.com/#/pricing)
{% endhint %}

### Advanced Properties

| Property                                           | Description                            | Data Type                                         |
| -------------------------------------------------- | -------------------------------------- | ------------------------------------------------- |
| <p>Writing Direction </p><p>(iOS and web only)</p> | Writing direction of your Label's text | Select from list `[left-to-right, right-to-left]` |
| <p>Letter Spacing </p><p>(iOS and web only)</p>    | Spacing between letters of your Label  | Number                                            |

### **Layout**

<table><thead><tr><th width="187.33333333333331">Property</th><th>Description</th><th>Data Type</th></tr></thead><tbody><tr><td>X</td><td>Location of your Label on the X-axis in pixels</td><td>Number</td></tr><tr><td>Y</td><td>Location of your Label on the Y-axis in pixels</td><td>Number</td></tr><tr><td>Height</td><td>Height of your Label in pixels</td><td>Number</td></tr><tr><td>Width</td><td>Width of your Label in pixels</td><td>Number</td></tr><tr><td>Resize Mode</td><td>Stretch the label to fit the device screen or render it the same as the design, regardless of the device (float in place).</td><td>Select from menu (Stretch, Float in Place)</td></tr></tbody></table>

### Style

| Property         | Description                                                          | Data Type                                  |
| ---------------- | -------------------------------------------------------------------- | ------------------------------------------ |
| Visible          | Toggle whether your end users can see the Label                      | True/False                                 |
| Background Color | Color of your Label's background                                     | Color                                      |
| Border Style     | Style of Label's Border                                              | Select from list `[solid, dotted, dashed]` |
| Border Color     | Color of the Label's Border                                          | Color                                      |
| Border Width     | Width of border outline in pixels                                    | Number                                     |
| Border Radius    | Radius of corners of Label                                           | Number                                     |
| Shadow Color     | Color of Label's shadow                                              | Color                                      |
| Shadow Opacity   | Opacity of Label's shadow                                            | Number between 0 and 100                   |
| Shadow Radius    | Radius of corners of Label's shadow in pixels                        | Number                                     |
| Shadow Offset    | How far the Label's shadow is offset, in Height and Width, in pixels | Number                                     |

## Blocks

### Events

#### Click

![](../../../.gitbook/assets/la\_click.png)

This event will fire when the user clicks on the label.

### Properties

#### Background Color&#x20;

![](<../../../.gitbook/assets/bg\_color (2).png>)

The get and set background color properties work with the color of the label itself i.e. the region behind the label text. Best practice is to use one of the [color blocks](../../../blocks/blocks/color.md) to set this value but HEX or RGB values may be used too.

#### Color&#x20;

![](../../../.gitbook/assets/color.png)

The get and set color properties can be used to work with the color of the text that is displayed in the label. Best practice is to use one of the [color blocks](../../../blocks/blocks/color.md) to set this value but HEX or RGB values may be used too.&#x20;

#### Font Size&#x20;

![](<../../../.gitbook/assets/font\_size (1).png>)

The get and set font size blocks are used to work with the size of the text that is displayed in the label. This value must be a number.

#### Font Style&#x20;

![](../../../.gitbook/assets/font\_style.png)

The font style property can be either "Normal" or "_Italic"._

#### Font Weight&#x20;

![](../../../.gitbook/assets/font\_weight.png)

The font weight value can be either; "Normal", "**Bold**" or a a value from 100 to 900

#### Height&#x20;

![](<../../../.gitbook/assets/height (2).png>)

The set and get height blocks work with the Height property of the label component. Acceptable input values are.&#x20;

* Number of Pixels
* Percentage Height
* "Fit Contents"
* "Fill Container"

The `Computed Height` block returns the on-screen dimensions of the label, after it has been rendered on-screen. The value returned is an integer, representing the size of the label in pixels.

#### Number of Lines&#x20;

![](../../../.gitbook/assets/num\_lines.png)

The get and set number of lines property is used to work with the maximum number of lines of text that should be displayed in a label before that label starts to scroll.

#### Text&#x20;

![](<../../../.gitbook/assets/text (2).png>)

This property corresponds to the text that is displayed in the label component.

#### Text Align

![](../../../.gitbook/assets/text\_align.png)

Text Align can be any of the following values:

* Auto
* Left
* Right
* Center
* Justify

#### Visible

![](<../../../.gitbook/assets/visible (1).png>)

The set and get visible blocks are used to show or hide the entire image component. Acceptable values are:

* True
* False

#### Width&#x20;

![](<../../../.gitbook/assets/width (1).png>)

The set and get width blocks work with the Width property of the label component. Acceptable values are.‌

* Number of Pixels
* Percentage Width
* "Fit Contents"
* "Fill Container"

The `Computed Width` block returns the on-screen dimensions of the label, after it has been rendered on-screen. The value returned is an integer, representing the size of the label in pixels.

