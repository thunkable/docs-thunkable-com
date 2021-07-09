---
description: >-
  The text input allows the person using your app to type in anything that they
  want such as words, passwords or numbers.
---

# Text Input

## Text Input Overview

![](.gitbook/assets/text-input-fig-1.png)

## Set Keyboard type

![](.gitbook/assets/text-input-fig-2.png)

You can choose from the following types of keyboards:

* **Default keyboard:** Displays your device’s default keyboard
* **Email Address:** Displays an alphanumeric keyboard to accept email addresses
* **Numeric:** Displays a keypad with only numbers; It is similar to the phone pad keyboard
* **Phone Pad:** Displays a telephone keypad; It is similar to the numeric keyboard

## Set up for Passwords



![](.gitbook/assets/text-input-fig-3.png)

You can also set up Text Input for passwords as shown below using the Secure Text Entry Switch. This switch will replace text with \* as users type.

To activate Secure Text Entry, look for the Text Input Style properties and make sure that the  Secure Text Entry switch is set to true.

![](.gitbook/assets/secure_text_entry.png)



## Style the Text Input

You can customize the Text Input component with the following properties: 

* **Hint:** Hint text that disappears when the user starts typing into the Text Input
* **Text:** Text that appears on the text input 
* **Visible:** To see the text input in your app, set the switch to true
* **Border**
  * **Width:** Enter how wide you want the border outline of the text input to be
  * **Color:** Pick a color for the border of the text input
  * **Style:** Select if you want the border to be a dotted, dashed or solid line
  * **Radius:** Enter how round you want the edges of the border for the text input to be

## Edit size and position

You can drag and drop your component into position, and set its size.   
You can set exact values for the component's Height and Width, and X and Y coordinates, in its properties.

**Height:** Height of Button in pixels  
**Width:** Width of Button in pixels

**X:** position of top left corner of Button on X-axis  
**Y:** position of top right corner of component on Y-axis

## Events

### Click

![](.gitbook/assets/ti_click.png)

This event fires when the user clicks on the Text Input component.

### Unfocus 

![](.gitbook/assets/ti_unfocus.png)

This event fires when the component looses focus, i.e the user clicks on another component.

### Submit 

![](.gitbook/assets/ti_submit.png)

This event fires when the enter or submit button is pressed on the device keyboard.

### Changes

![](.gitbook/assets/ti_changes.png)

This event fires every time a character is added or removed to the Text Input.



## Properties

### Border Width

![](.gitbook/assets/boder_width.png)

The border width value corresponds to the size of the border around the Text Input. Changes to the color and style of the border must be done in the[ designer.](text-input.md#style-the-text-input) 

### Height 

![](.gitbook/assets/height%20%281%29.png)

The set and get height blocks work with the Height property of the Text Input component. Acceptable input values are. 

* Number of Pixels
* Percentage Height
* "Fit Contents"
* "Fill Container"

The `Computed Height` block returns the on-screen dimensions of the Text Input, after it has been rendered on the device screen. The value returned is an integer, representing the size of the component, in pixels.

### Hint 

![](.gitbook/assets/hint.png)

The set and get hint work with the prompt that is displayed in the Text Input, before the user starts typing. Any string of text or number can be used as the hint.

### Keyboard Type 

![](.gitbook/assets/keyboard.png)

The set and get keyboard type property gives you control over what version of the keyboard is displayed on-screen when the user starts typing. Acceptable values are:  


* default
* email address
* numeric
* phone pad

### Text 

![](.gitbook/assets/text%20%281%29.png)

The set and get text property works with the string of text that displayed in the Text Input. 

### Visible 

![](.gitbook/assets/visible%20%282%29.png)

The set and get visible blocks are used to show or hide the entire Text Input component. Acceptable values are:

* True
* False

### Width

![](.gitbook/assets/width%20%282%29.png)

The set and get width blocks work with the Width property of the Text Input component. Acceptable values are.‌

* Number of Pixels
* Percentage Width
* "Fit Contents"
* "Fill Container"

The `Computed Width` block returns the on-screen dimensions of the Text Input, after it has been rendered on the device screen. The value returned is an integer, representing the size of the component, in pixels.





