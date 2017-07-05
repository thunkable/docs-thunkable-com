#### **Thunkable for Android **❤

# Touch

---

**One of the first defining features of smartphones was the touch screen interface, which enabled developers to utilize all parts of a screen to perform distinct actions, unleashing an almost limitless number of user interface options.**

Below are the different touch interface components and what they look like on a Samsung S6 phone by default

|  |  |  |  |
| :--- | :--- | :--- | :--- |
| [Button](/components/touch/button.md) | ![](/assets/button.png) | [Label](#label) | ![](/assets/label.png) |
| TextBox | ![](/assets/textbox.png) | Password TextBox | ![](/assets/password-textbox.png) |
| ListPicker | ![](/assets/listpicker.png) | ListView | ![](/assets/listview.png) |
| Spinner | ![](/assets/spinner.png) | CheckBox | ![](/assets/checkbox.png) |
| Slider | ![](/assets/slider.png) | Notifier | ![](/assets/notifier.png) |
| DatePicker | ![](/assets/datepicker.png) | TimePicker | ![](/assets/timepicker.png) |

---

# Button

---

**Buttons are a key input for many apps and one of the most popular components on Thunkable**. Many aspects of its appearance can be changed and different events can be triggered with different types of clicks - regular, long and touch up or touch down.

---

#### Pro-tip: Buttons and Icon Fonts

One of the most common customizations of buttons is to add an image to them but this can both take time to generate and also take up valuable space in your app.  One way to avoid this is to use one of the many icon fonts available to substitute a custom font for images.

For navigation menus, we highly recommend the [Material Design Icon Font](https://material.io/icons/)

For social media bars, we recommend the [Mono Social Font](http://drinchev.github.io/monosocialiconsfont/)

The sample app [Thunkableagram: AI-powered Instagram](#) uses the Material Design Icon Font for the bottom navigation bar

---

### **Appearance**

| Property | Description |
| :--- | :--- |
| Height | Height in pixels, percent, 'Automatic' or 'Fill' |
| Width | Width in pixels, percent, 'Automatic' or 'Fill' |
| Shape\* | Default \(rectangle\), rounded, rectangular or oval.  The shape will not be visible if an Image is being displayed |
| Background Color | Default \(Gray\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Image | You can upload an image to your app or reference an image url. If an image is uploaded, it will negate the background color and shape properties |
| Text | Optional text that will display on the button |
| Text Color | Default \(Black\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Text Alignment\* | Left, center \(recommended\) or right |
| Font Bold | If checked, button text is displayed in **bold** |
| Font Italic | If checked, button text is displayed in _italic_ |
| Font Size | Point size for button text |
| Font Typeface\* | Default \(Roboto\), Roboto Regular, Roboto Thin, Sans Serif, Serif, and Monospace. You can upload your own custom font \(.ttf\) |
| Show Feedback | If checked, shows visual feedback for a button with an image displayed |
| Visible | If checked, the button will be visible on the screen |

\*Can only be set in the Designer

---

#### Functionality

| Event | Description |
| :--- | :--- |
| Click | User tapped and releases the button |
| Long Click | User holds the button down |
| Touch Down | User gently presses the button |
| Touch Up | User releases the button |
| Enabled | If checked, button functionality is enabled |
| Got Focus | User's finger is over the button, making it possible to click |
| Lost Focus | User's finder is away from the button, making it no longer possible to click |

# Label

---

Labels are components used to display text.  Empty labels are used to provide horizontal and vertical padding between elements.

---

#### Pro-tip: Labels and HTML formatting

Labels are the only component so far that supports HTML formatting, which can be helpful if you want to add a line break or bold only a few words.

Example:

`<br>Example: Hello World<br><b>How are you?<b/>`

---

### **Appearance**

| Property | Description |
| :--- | :--- |
| Height | Height in pixels, percent, 'Automatic' or 'Fill' |
| Width | Width in pixels, percent, 'Automatic' or 'Fill' |
| Background Color | Default \(Gray\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Text | Optional text that will display on the button |
| Text Color | Default \(Black\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Text Alignment\* | Left, center \(recommended\) or right |
| Font Bold | If checked, button text is displayed in **bold** |
| Font Italic | If checked, button text is displayed in _italic_ |
| Font Size | Point size for button text |
| Font Typeface\* | Default \(Roboto\), Roboto Regular, Roboto Thin, Sans Serif, Serif, and Monospace. You can upload your own custom font \(.ttf\) |
| HTML Format | If checked, enables label to read html formatting. Not all HTML format is supported |
| Has Margins | If checked, adds a consistent margin around the label |
| Visible | If checked, the button will be visible on the screen |

\*Can only be set in the Designer

