#### **Thunkable for iOS **

# Timer ![](/assets/timer-ios-icon.png)

---

The Timer is a popular component that uses the internal clock on a phone to to trigger an event in the app after a certain period of time. Unlike on Android, the Timer fires only once by default but you can set it to fire continuously by enabling a loop.

---

#### Set the Timer interval

| Property | Enabled |
| :--- | :--- |
| Interval \(milliseconds\) | Timer interval in milliseconds. Default is 3 seconds |

---

#### Determine how often you want the Timer to trigger an event

| Frequency | Use case | Enabled | Loops |
| :--- | :--- | :--- | :--- |
| Just once when app starts | Splash screen | `true` \(default\) | `false` \(default\) |
| Just once but after app starts | Loading data when opening a new screen | Set to `false`initially. Set to `true `when you want to start the Timer | `false` |
| Looping when app starts | Playing background music in a game | `true` \(default\) | `true`  |
| Looping during certain intervals of the app | Collecting location data | Set to `false`initially. Set to `true `when you want to start the Timer and then `false`when you want the looping to stop. | `true`   |

---

#### Starting the Timer

If 'enabled' is set to `true`, the Timer will trigger on its own when the app starts. If you want to start the timer at a later point in your app based on another event, you can set 'enabled' is set to `true`

---

#### Triggering an Event

To trigger an event, you'll need to set up the blocks like the example below

![](/assets/timer-ios-fig-1.png)



