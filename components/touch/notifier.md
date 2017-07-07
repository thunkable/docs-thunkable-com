#### **Thunkable for Android **❤

# Notifier

---

Notifiers are temporary messages usually displayed on top of the current screen to alert the user before she or he proceeds.  Notifier dialogs can also be used to prompt users to make an important selection.

Note that only Alerts and not Dialogs can not be customized in terms of appearance. Dialogs will default to the Material Design default.

|  | [Alerts](#alerts) | Dialog |
| :--- | :--- | :--- |
|  |  | ![](/assets/notifier.png) |
| Common use case | Notify the user of an important message | Confirm a selection |

---

### Alerts

---

#### **Appearance**

| Property | Description |
| :--- | :--- |
| Text Color \(Alerts only\) | Default \(White\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks edito |
| Background Color \(Alerts only\) | Default \(Dark Gray\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Notifier Length \(Alerts only\) | 'Short' or 'long'. Specifies the length of time that the alert is shown |

---

#### Functionality

| Event | Description |
| :--- | :--- |
| Show Alert \(notice\) | Displays a temporary notification |

---

### Dialogs

---

#### Functionality

| Event / Property | Description |
| :--- | :--- |
| Min Value | Sets the minimum value of the slider |
| Max Value | Sets the maximum value of the slider |
| Thumb Position | Sets the position of the slider thumb. Cannot be below the Min Value or exceed the Max Value |
| Thumb Enabled | Sets whether or not to display the slider thumb |
| Position Changed \(Thumb Position\) | If position of slider thumb has changed |

AfterChoosing\(text choice\)

Event after the user has made a selection for ShowChooseDialog.

AfterTextInput\(text response\)

Event raised after the user has responded to ShowTextDialog.

Notifier

• Methods

DismissProgressDialog\(\)

Dismiss a previously displayed ProgressDialog box

ShowChooseDialog\(text message, text title, text button1Text, text button2Text, boolean cancelable\)

Shows a dialog box with two buttons, from which the user can choose. If cancelable is true there will be an additional CANCEL button. Pressing a button will raise the AfterChoosing event. The "choice" parameter to AfterChoosing will be the text on the button that was pressed, or "Cancel" if the CANCEL button was pressed.

ShowMessageDialog\(text message, text title, text buttonText\)

Display an alert dialog with a single button that dismisses the alert.

ShowProgressDialog\(text message, text title\)

Shows a dialog box with an optional title and message \(use empty strings if they are not wanted\). This dialog box contains a spinning artifact to indicate that the program is working. It cannot be canceled by the user but must be dismissed by the Thunkable Program by using the DismissProgressDialog block.

ShowTextDialog\(text message, text title, boolean cancelable\)

Shows a dialog box where the user can enter text, after which the AfterTextInput event will be raised. If cancelable is true there will be an additional CANCEL button. Entering text will raise the AfterTextInput event. The "response" parameter to AfterTextInput will be the text that was entered, or "Cancel" if the CANCEL button was pressed.

