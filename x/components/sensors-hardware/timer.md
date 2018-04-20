#### T**hunkable Cross-Platform **✕

# Timer ![](/assets/iOSviewIconTimer.png)

---

The Timer uses the internal clock on a phone to to trigger an event in the app after a certain period of time. The Timer fires only once by default but you can set it to fire continuously by enabling a loop

* [Set up](#set-up)
* [Start an event with a Timer](#start-an-event-with-a-timer)

---

### Set up

| Property | Enabled |
| :--- | :--- |
| Interval \(milliseconds\) | Default \(`3000`\); Timer interval is in milliseconds |

#### Determine how often you want the Timer to trigger an event

| Frequency | Use case | Enabled | Loops |
| :--- | :--- | :--- | :--- |
| Just once when app starts | Splash screen | `true` \(default\) | `false` \(default\) |
| Just once but after app starts | Loading data when opening a new screen | Set to `false`initially. Set to `true`when you want to start the Timer | `false` |
| Looping when app starts | Playing background music in a game | `true` \(default\) | `true` |
| Looping during certain intervals of the app | Collecting location data | Set to `false`initially. Set to `true`when you want to start the Timer and then `false`when you want the looping to stop. | `true` |

#### Starting the Timer

If 'enabled' is set to `true`, the Timer will trigger on its own when the app starts. If you want to start the timer at a later point in your app based on another event, you can set 'enabled' is set to `true`

---

### Start an event with a Timer

You can start an event--such as opening a new Screen--when the Timer fires based on its given `interval`

![](/assets/timer-✕-fig-1.png)



