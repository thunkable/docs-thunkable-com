#### **Thunkable for Android **❤

# Notifier

---

Notifiers are temporary messages to alert the user before she or he proceeds.  Notifiers come in two flavors - alerts, which are more passive but whose appearance can be customized and dialogs which default to the Material Design design but prompt users to confirm \(Message Dialog\), make a choice \(Choose Dialog\), enter text \(Text Dialog\) or wait \(Progress Dialog\) for a certain event before proceeding.

|  | [Alerts](#alerts) | [Dialogs](#dialogs) |
| :--- | :--- | :--- |
|  | ![](/assets/notifier-alert.png) | ![](/assets/notifier.png) |
| Common use case | Passive notification that an event has or is about to occur | Active notification that requires the user to tap, wait or input text before proceeding |

---

### Alerts

Alerts are useful as passive messages as the user is navigating your app but no action is required such as "Login successful"

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

Dialogs are useful when a message requires the user's attention and in some cases, a choice before proceeding

|  | Message Dialog | Progress Dialog | Choose Dialog | Text Dialog |
| :--- | :--- | :--- | :--- | :--- |
|  | ![](/assets/notifier.png) | ![](/assets/dialog-progress.png) | ![](/assets/dialog-choose.png) | ![](/assets/dialog-text.png) |

---

#### Functionality

| Event / Property | Description |
| :--- | :--- |
| Show Message Dialog \(message, title, button text\) | Displays a dialog with a single button that dismisses the alert |
| Show Progress Dialog \(message, title\) | Shows a dialog with an optinal title and message and a spinning animation to indicate that the program is working. Cannot be dismissed by the user and must be dismissed by the Dismiss Progress Dialog block |
| Dimiss Progress Dialog | Dismisses a Progress Dialog |
| Show Choose Dialog \(message, title, button1 text, button2 text, cancelable\) | Shows a dialog with two buttons, from which a user can choose. Pressing a button will start the After Choosing event. If cancelable is set to 'true', there will be an additional 'cancel' button, which if pressed, will dismiss the dialog |
| After Choosing \(choice\) | Starts event after a choice is selected in a Choose Dialog |
| Show Text Dialog \(message, title, cancelable\) | Shows a dialog button where user can enter text, which will start the After Text Input event. If cancelable is set to 'true', there will be a cancel button, which if pressed, will dismiss the dialog |
| After Text Input \(response\) | Starts event after text is input in a Text Dialog |



