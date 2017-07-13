#### **Thunkable for Android **❤

# Clock ![](/assets/clock-icon.png)

---

The Clock component uses the internal clock on a phone to both set a Timer \(to trigger an event\) or to get the current time in a variety of date and time formats

---

#### Set a Timer \(to Turn Off a Splash Screen\)

![](/assets/clock-blocks-1.png)

[Watch the Branding Screen tutorial](https://www.youtube.com/watch?v=9u365ejwTqg&t=1s)

| Property / Event | Description |
| :--- | :--- |
| Timer Enabled | If 'true', timer will fire. If 'false', turns off timer so it no longer fires |
| Timer Interval \(milliseconds\) | Interval between timer events in milliseconds |
| Timer | When timer has gone off |
| Timer Always Fires | If 'true', timer will fire even if the application is not showing on the screen |

---

#### Get the Current Time

![](/assets/clock-blocks-2.png)

| Property | Description |
| :--- | :--- |
| Now | Returns an instant of the current time read from phone's clock |
| System Time | Returns the phone's internal time |
| Format Date \(instant, pattern\) | Returns text representing the date of an instant in the specified pattern |
| Format Date Time \(instant, pattern\) | Returns text representing the date and time of an instant in the specified pattern |
| Format Time \(instant, pattern\) | Return text representing the time of an instant |
| Month \(instant\) | Returns the month of the year \(1-12\) from the instant |
| Month Name \(instant\) | Returns the name of the month from the instant E.g. January, February, March... |
| Day Of Month \(instant\) | Returns the day of the month\(1-31\) from the instant |
| Weekday \(instant\) | Returns the day of the week represented as a number from 1 \(Sunday\) to 7 \(Saturday\) |
| Weekday Name \(instant\) | Returns the name of the day of the week from the instant |
| Year \(instant\) | Returns the year from the instant |
| Hour \(instant\) | Returns the hour of the day \(0-23\) from the instant |
| Minute \(instant\) | Returns the minute of the hour \(0-59\) from the instant |
| Second \(instant\) | Returns the second of the minute \(0-59\) from the instant |
| Get Millis \(instant\) |  |  Returns the instant in time measured as milliseconds since 1970 |  |

---

#### Set a Future Time

| Property | Description |
| :--- | :--- |
| Add Days \(instant, number days\) | Returns an instant in time some days after the argument |
| Add Weeks \(instant, weeks\) | Returns an instant in time some weeks after the argument |
| Add Months \(instant, months\) | Returns an instant in time some months after the argument |
| Add Years \(instant, years\) | Returns an instant in time some years after the argument |
| Add Seconds \(instant, seconds\) | Returns an instant in time some seconds after the argument |
| Add Minutes \(instant, minutes\) | Returns an instant in time some minutes after the argument |
| Add Hours \(instant, hours\) | Returns an instant in time some hours after the argument |
| Add Duration \(instant, duration\) | Returns an instant in time some time after the argument. Duration can be obtained from Clock.Duration |

---

#### Calculate Duration

| Property | Description |
| :--- | :--- |
|  Duration \(start, end\) |  Returns duration, which is milliseconds elapsed between instants |
|  Duration To Seconds \(duration\) |  Converts the duration to the number of seconds |
|  Duration To Minutes \(duration\) |  Converts the duration to the number of minutes |
|  Duration To Hours \(duration\) |  Converts the duration to the number of hours |
|  Duration To Days \(duration\) |  Converts the duration to the number of days |
|  Duration To Weeks \(duration\) | Converts the duration to the number of weeks |



