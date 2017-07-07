#### **Thunkable for Android **❤

# Button

---

Buttons are a key input for many apps and one of the most popular components on Thunkable. Many aspects of its appearance can be changed and different events can be triggered with different types of clicks - regular, long and touch up or touch down.

|  | Default | Material Icon |
| :--- | :--- | :--- |
|  | ![](/assets/button.png) | ![](/assets/button-material-icon.png) |
| Common use case | Start an event | Navigation or settings |

---

#### Pro-tip: Buttons and Icon Fonts {#button-pro-tip}

One of the most common customizations of buttons is to add an image to them but this can both take time to generate and also take up valuable space in your app.  One way to avoid this is to use one of the many icon fonts available to substitute a custom font for images.

For navigation menus, we highly recommend the [Material Design Icon Font](https://material.io/icons/)

For social media bars, we recommend the [Mono Social Font](http://drinchev.github.io/monosocialiconsfont/)

The sample app [Thunkableagram: AI-powered Instagram](#) uses the Material Design Icon Font for the bottom navigation bar

---

#### **Appearance**

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
| Lost Focus | User's finger is away from the button, making it no longer possible to click |



