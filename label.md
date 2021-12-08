---
description: The label component allows you to display text in your app.
---

# Label

## Style the Label <a href="#style-the-label" id="style-the-label"></a>

You can customize your label using the following properties:

### Properties <a href="#properties-1" id="properties-1"></a>

* **Text:** Text that appears on the label
* **Font Size:** Size of the text that appears on the label
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

![](https://docs.thunkable.com/\~/files/v0/b/gitbook-28427.appspot.com/o/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MA5guzt3PT-bmFFNgtV%2F-MA5jXwBVyl0JQnJHoAV%2Fla\_click.png?alt=media\&token=9b19a208-53ce-4079-a5c5-b9a51416e0c5)

## Properties <a href="#properties" id="properties"></a>

The get and set background color properties work with the color of the label itself i.e. the region behind the label text. Best practice is to use one of the [color blocks](https://docs.thunkable.com/v/drag-and-drop/color) to set this value but HEX or RGB values may be used too.

### Background Color <a href="#background-color" id="background-color"></a>

![](https://docs.thunkable.com/\~/files/v0/b/gitbook-28427.appspot.com/o/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWYr390JU0vOfN\_ODXd%2F-MWYr8wphqyxcktI3LSs%2Fbg\_color.png?alt=media\&token=0c34d28a-233f-4faf-8e14-1bf1937903b2)

### Color <a href="#color" id="color"></a>

![](https://docs.thunkable.com/\~/files/v0/b/gitbook-28427.appspot.com/o/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWYr390JU0vOfN\_ODXd%2F-MWYrBE16\_5JDdFbvj6X%2Fcolor.png?alt=media\&token=79be07c2-c61d-43ff-bc6f-e36b157dc3ca)

### Font Size <a href="#font-size" id="font-size"></a>

![](https://docs.thunkable.com/\~/files/v0/b/gitbook-28427.appspot.com/o/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWYr390JU0vOfN\_ODXd%2F-MWYrEmf7fV\_kmMU-hZi%2Ffont\_size.png?alt=media\&token=7ca9c0cd-c915-4e90-8b63-35de1011e512)

### Font Style <a href="#font-style" id="font-style"></a>

![](https://docs.thunkable.com/\~/files/v0/b/gitbook-28427.appspot.com/o/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWYr390JU0vOfN\_ODXd%2F-MWYrI1eHAHeohhzDJ77%2Ffont\_style.png?alt=media\&token=97760c0e-3dfd-47f9-a699-e9bfd435c251)

### Font Weight <a href="#font-weight" id="font-weight"></a>

![](https://docs.thunkable.com/\~/files/v0/b/gitbook-28427.appspot.com/o/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWYr390JU0vOfN\_ODXd%2F-MWYrKDrUoRzlych2ekH%2Ffont\_weight.png?alt=media\&token=a2c0787d-ee53-4c3f-8a5f-b60300968e4c)

### Height <a href="#height" id="height"></a>

The set and get height blocks work with the Height property of the label component. Acceptable input values are:

![](https://docs.thunkable.com/\~/files/v0/b/gitbook-28427.appspot.com/o/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWYr390JU0vOfN\_ODXd%2F-MWYrMmKFgwAnBjxmaiF%2Fheight.png?alt=media\&token=d893f675-821e-4770-b4b6-cad8f7814311)

* Number of Pixels
* Percentage Height
* "Fit Contents"
* "Fill Container"

### Number of Lines <a href="#number-of-lines" id="number-of-lines"></a>

The get and set number of lines property is used to work with the maximum number of lines of text that should be displayed in a label before that label starts to scroll.

![](https://docs.thunkable.com/\~/files/v0/b/gitbook-28427.appspot.com/o/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWYr390JU0vOfN\_ODXd%2F-MWYrPOmCs6UlKCEC8ES%2Fnum\_lines.png?alt=media\&token=8fbcc095-5ec2-4189-a85c-0a957592384d)

### Text <a href="#text" id="text"></a>

This property corresponds to the text that is displayed in the label component.

![](https://docs.thunkable.com/\~/files/v0/b/gitbook-28427.appspot.com/o/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWYr390JU0vOfN\_ODXd%2F-MWYrRzONlpk0GaUmPmy%2Ftext.png?alt=media\&token=c7f514b6-b342-44b4-9b5f-9c4826ccc483)

### Text Align <a href="#text-align" id="text-align"></a>

Text Align can be any of the following values:

![](https://docs.thunkable.com/\~/files/v0/b/gitbook-28427.appspot.com/o/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWYr390JU0vOfN\_ODXd%2F-MWYrTtYaUaIyX321lJC%2Ftext\_align.png?alt=media\&token=6c5d7b68-336f-4e0c-8a51-4cb24ae77012)

* Auto
* Left
* Right
* Center
* Justify

### Visible <a href="#visible" id="visible"></a>

![](https://docs.thunkable.com/\~/files/v0/b/gitbook-28427.appspot.com/o/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWYr390JU0vOfN\_ODXd%2F-MWYrWC11aSImy7ieRQB%2Fvisible.png?alt=media\&token=99d0c092-43e8-4b21-977f-63be22157d4e)

* True
* False

### Width <a href="#width" id="width"></a>

The set and get width blocks work with the Width property of the label component.

![](https://docs.thunkable.com/\~/files/v0/b/gitbook-28427.appspot.com/o/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWYsAlosgFhvUhh0x6j%2F-MWYxsqSYJdVVHiqoIHb%2Fwidth.png?alt=media\&token=b2e7105e-8ff5-4963-a59c-22435376e96d)

* Number of Pixels
* Percentage Width
* "Fit Contents"
* "Fill Container"
