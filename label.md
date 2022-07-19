---
description: The label component allows you to display text in your app.
---

# Label

## Style the Label <a href="#style-the-label" id="style-the-label"></a>

You can customize your label using the following properties:

### Properties <a href="#properties-1" id="properties-1"></a>

* **Text:** Text that appears on the label
* **Font Size:** Size of the text that appears on the label
*   **Custom Font (mobile only)**: Upload a TTF or OTF font file to use as your Button's font

    {% hint style="info" %}
    Uploading a custom font file is available to accounts with Business and Enterprise plans.\
    Check out our [pricing page](https://thunkable.com/#/pricing) for more information about these plans
    {% endhint %}
* **Color:** Color of the text that appears on the label
* **Background Color:** Sets the background color of the label
* **Text Align**
  * **Auto -** Aligns the text automatically
  * **Left -** Displays the text starting from the left of the label
  * **Right -** Displays the text starting from the right of the label
  * **Center -** Displays the text starting from the middle of the label
  * **Justify -** Aligns both the right and left side of the text equally
* **Font Style**
  * **Normal:** Default text display
  * **Italic:** Display the text in italics
* **Font Weight:** Select how bold the text on the label will be
* **Number of Lines:** set a maximum amount of lines of text that your Label will display
* **Background Color:** set the color of your Label's background
* **Border Width:** Enter how wide you want the border outline of the label to be
* **Border** **Radius:** Enter how round you want the edges of the border for the label to be
* **Border Color:** Pick a color for the border of the label
* **Border Style:** Select if you want the border of the label to be a dotted, dashed or solid line
* **Background Color:** set the color of your Label's background
* **Border Width:** Enter how wide you want the border outline of the label to be
* **Border** **Radius:** Enter how round you want the edges of the border for the label to be
* **Border Color:** Pick a color for the border of the label
* **Border Style:** Select if you want the border of the label to be a dotted, dashed or solid line

### Advanced Properties <a href="#advanced-properties" id="advanced-properties"></a>

* **Letter Spacing (iOS and web only):** increase spacing between letters of your Label
* **Text Decoration Line:** add a line through, underline, or both with underline line-through
* **Text Decoration Style (iOS and web only):** set your Text Decoration line to be solid, dotted, dashed, or double
* **Text Decoration Color (iOS and web only):** set the color of your Text Decoration Line
* **Writing Direction (iOS and web only):** set the writing direction of your Label's text
* **Letter Spacing (iOS and web only):** increase spacing between letters of your Label
* **Text Decoration Line:** add a line through, underline, or both with underline line-through
* **Text Decoration Style (iOS and web only):** set your Text Decoration line to be solid, dotted, dashed, or double
* **Text Decoration Color (iOS and web only):** set the color of your Text Decoration Line
* **Writing Direction (iOS and web only):** set the writing direction of your Label's text

## Events <a href="#events" id="events"></a>

### Click <a href="#click" id="click"></a>

This event will fire when the user clicks on the label.

![](.gitbook/assets/la\_click.png)

## Properties <a href="#properties" id="properties"></a>

The get and set background color properties work with the color of the label itself i.e. the region behind the label text. Best practice is to use one of the [color blocks](https://docs.thunkable.com/v/drag-and-drop/color) to set this value but HEX or RGB values may be used too.

### Background Color <a href="#background-color" id="background-color"></a>

![](.gitbook/assets/la\_bg\_color.png)

### Color <a href="#color" id="color"></a>

![](.gitbook/assets/la\_color.png)

### Font Size <a href="#font-size" id="font-size"></a>

![](.gitbook/assets/la\_font\_size.png)

### Font Style <a href="#font-style" id="font-style"></a>

![](.gitbook/assets/la\_font\_style.png)

### Font Weight <a href="#font-weight" id="font-weight"></a>

![](.gitbook/assets/la\_font\_weight.png)

### Height <a href="#height" id="height"></a>

The set and get height blocks work with the Height property of the label component. Acceptable input values are:

![](.gitbook/assets/la\_height.png)

* Number of Pixels
* Percentage Height
* "Fit Contents"
* "Fill Container"

### Number of Lines <a href="#number-of-lines" id="number-of-lines"></a>

The get and set number of lines property is used to work with the maximum number of lines of text that should be displayed in a label before that label starts to scroll.

![](.gitbook/assets/la\_num\_lines.png)

### Text <a href="#text" id="text"></a>

This property corresponds to the text that is displayed in the label component.

![](.gitbook/assets/la\_text.png)

### Text Align <a href="#text-align" id="text-align"></a>

Text Align can be any of the following values:

![](.gitbook/assets/la\_text\_align.png)

* Auto
* Left
* Right
* Center
* Justify

### Visible <a href="#visible" id="visible"></a>

![](.gitbook/assets/la\_visible.png)

* True
* False

### Width <a href="#width" id="width"></a>

The set and get width blocks work with the Width property of the label component.

![](.gitbook/assets/la\_widrth.png)

* Number of Pixels
* Percentage Width
* "Fit Contents"
* "Fill Container"
