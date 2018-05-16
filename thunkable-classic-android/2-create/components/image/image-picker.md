---
description: >-
  The Image Picker accesses all the images stored on the phone and in the cloud
  via other services
---

# Image Picker

###  ![](../../../../.gitbook/assets/image-picker-icon.png)

![](../../../../.gitbook/assets/image-picker-fig-1.png)

### **Appearance**

There are two elements to an ImagePicker, a button that opens the ImagePicker and the ImagePicker itself. The button you can customize but the ImagePicker design is the Android default.

| Property | Description |
| :--- | :--- |
| Height | Height in pixels, percent, 'Automatic' or 'Fill' |
| Width | Width in pixels, percent, 'Automatic' or 'Fill' |
| Shape | Default \(rectangle\), rounded, rectangular or oval.  The shape will not be visible if an Image is being displayed |
| Background Color | Default \(Gray\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Image | You can upload an image to your app or reference an image url. If an image is uploaded, it will negate the background color and shape properties |
| Text | Optional text that will display on the button |
| Text Color | Default \(Black\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Text Alignment | Left, center \(recommended\) or right |
| Font Bold | If checked, button text is displayed in **bold** |
| Font Italic | If checked, button text is displayed in _italic_ |
| Font Size | Point size for button text |
| Font Typeface | Default \(Roboto\), Roboto Regular, Roboto Thin, Sans Serif, Serif, and Monospace. You can upload your own custom font \(.ttf\) |
| Show Feedback | If checked, shows visual feedback for a button with an image displayed |
| Visible | If checked, the button will be visible on the screen |

### Functionality

| Event | Description |
| :--- | :--- |
| Open | Opens the Image Picker |
| Touch Down | User gently presses the button |
| Touch Up | User releases the button |
| Selection | The selected image |
| After Picking | Event after user selects an image |
| Before Picking | Event before a user selects an image |
| Enabled | If checked, button functionality is enabled |
| Got Focus | User's finger is over the button, making it possible to click |
| Lost Focus | User's finger is away from the button, making it no longer possible to click |

