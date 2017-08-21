#### **Thunkable for Android **❤

# DatePicker ![](/assets/datepicker-icon.png) + TimePicker ![](/assets/timepicker-icon.png)

---

Date and TimePicker are components that make it easier for users to select dates and times in a consistent format

|  | ![](/assets/datepicker-icon.png) | ![](/assets/timepicker-icon.png) |
| :--- | :--- | :--- |
|  | [DatePicker](#datepicker) | [TimePicker](#aloha) |
|  | ![](/assets/datepicker.png) | ![](/assets/timepicker.png) |
| Common use case | Selecting day | Selecting time |

---

### DatePicker ![](/assets/datepicker-icon.png) {#datepicker}

---

#### **Appearance**

There are two elements to a DatePicker, a button that opens the DatePicker and the DatePicker itself. The button you can customize but the DatePicker design is set to the Material Design default.

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

| Property / Event | Description |
| :--- | :--- |
| SetDate to Display \(day, month, year\) | Sets a specific date to display when user opens DatePicker. The current date is the default |
| SetDate to Display from Instant \(instant\) | Sets a specific instant \(using the Clock component\) to use as date when user opens DatePicker. The current date is the default |
| Launch Picker | Opens the DatePicker |
| Touch Down | User gently presses the button |
| Touch Up | User releases the button |
| Enabled | If checked, button functionality is enabled |
| Got Focus | User's finger is over the button, making it possible to click |
| Lost Focus | User's finger is away from the button, making it no longer possible to click |
| After Date Set | Event after user selects a date |
| Day | Day selected by user \(1-31\) |
| Month | Month selected by user \(1-12\) |
| Year | Year selected by user |

---

### TimePicker ![](/assets/timepicker-icon.png) {#timepicker}

---

#### **Appearance**

There are two elements to a TimePicker, a button that opens the TimePicker and the TimePicker itself. The button you can customize but the TimePicker design is set to the Material Design default.

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

| Property / Event | Description |
| :--- | :--- |
| SetTime to Display \(hour, minute\) | Sets a specific time to display when user opens TimePicker. The current time is the default |
| SetTime to Display from Instant \(instant\) | Sets a specific instant \(using the Clock component\) to use as date when user opens TimePicker. The current time is the default |
| Launch Picker | Opens the TimePicker |
| Touch Down | User gently presses the button |
| Touch Up | User releases the button |
| Enabled | If checked, button functionality is enabled |
| Got Focus | User's finger is over the button, making it possible to click |
| Lost Focus | User's finger is away from the button, making it no longer possible to click |
| After Time Set | Event after user selects a time |
| Instant | Instant of time selected by user. Can be formatted using the Clock component |
| Minute | Minute selected by user |
| Hour | Hour selected by user in 24 hour format e.g. 11 pm is 23 |



