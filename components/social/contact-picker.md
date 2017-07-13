#### **Thunkable for Android **❤

# Contact Picker ![](/assets/contact-picker-icon.png) + Phone Number Picker ![](/assets/phone-number-picker-icon.png)

---

Contact Picker and Phone Number Picker are identical components that allow users to select from stored contacts on a user's phone and retrieve a set of information about those contacts like name, phone number and email address.

---

#### Information available from Contact Picker or Phone Number Picker

After a user has made a selection, the following properties will be set to information:

| Property | Description |
| :--- | :--- |
| Contact Name | The contact's name |
| Phone Number | The contact's primary phone number |
| Phone Number List | A list of the contact's phone numbers |
| Email Address | The contact's primary email address |
| Email Address List | A list of the contact's email addresses |
| Contact URI | The path to the contact on the phone |
| Picture | The name of the file containing the contact's image, which can be used as a Picture property value for the Image or ImageSprite component |

---

#### Selecting a contact

| Event | Description |
| :--- | :--- |
| Open | Launches the Contact or Phone Number Picker |
| View Contact \(uri\) | Views a contact given its URI or path on phone |
| Before Picking | When the component is clicked but before the picker activity is started |
| After Picking | After the picker activity returns its result and the properties have been filled in |
| Touch Down | User gently presses the button |
| Touch Up | User releases the button |
| Enabled | If checked, button functionality is enabled |
| Got Focus | User's finger is over the button, making it possible to click |
| Lost Focus | User's finger is away from the button, making it no longer possible to click |

---

#### Button Appearance

There are two elements to a Contact Picker and Phone Number Picker, a button that opens the Picker and the Picker itself. You can only modify the appearance of the button

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





