#### **Thunkable for Android **❤

# Texting ![](/assets/texting-icon.png)

---

The Texting component send, receives and can be set up to automatically respond to texts \(like during driving\).  Standard messaging rates apply for the user.

---

#### Send a text

![](/assets/texting-blocks-1.png)

| Property / Event | Description |
| :--- | :--- |
| Phone Number | The number that the message will be sent to when the SendMessage method is called. The number is a text string with the specified digits \(e.g., 6505551212\). Dashes, dots, and parentheses may be included \(e.g., \(650\)-555-1212\) but will be ignored; spaces should not be included |
| Message | The message that will be sent when the Send Message method is called |
| Send Message | Sends a text message |
| Receiving Enabled | If set to 1 \(OFF\) no messages will be received. If set to 2 \(FOREGROUND\) or 3 \(ALWAYS\) the component will respond to messages if it is running. If the app is not running then the message will be discarded if set to 2\(FOREGROUND\). If set to 3 \(ALWAYS\) and the app is not running the phone will show a notification. Selecting the notification will bring up the app and signal the MessageReceived event. Messages received when the app is dormant will be queued, and so several MessageReceived events might appear when the app awakens. As an app developer, it would be a good idea to give your users control over this property, so they can make their phones ignore text messages when your app is installed |
|  |  |
| Google Voice Enabled | If true, then Send Message will attempt to send messages over Wifi using Google Voice. This requires that the Google Voice app must be installed and set up on the phone or tablet, with a Google Voice account. If Google Voice Enabled is false, the device must have phone and texting service in order to send or receive messages with this component |

---

#### Send a text automatically











