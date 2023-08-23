# Timer Blocks

## Adding Timers to your app

### Create a Timer

You can add a Timer to your app from the Blocks tab of your Thunkable project. Under the App Features header, click the ⊕ icon next to Timers to add a Timer to your app.

![](../../.gitbook/assets/timers.png)

### Properties

The Timer's properties are initially set when you add a Timer to your project.&#x20;

| Property | Description                                                                                                                                                    | Data Type  |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- |
| Interval | How regularly the Timer fires, in seconds or milliseconds                                                                                                      | Number     |
| Count Up | Toggle whether the Timer's [time blocks](timer.md#get-time-in-seconds) return the current time as counted up from 0 or counted down from the interval duration | True/False |
| Loops    | Toggle whether the Timer will start again once it has fired                                                                                                    | True/False |
| Enabled  | Toggle whether the Timer is active in your app                                                                                                                 | True/False |

### Edit or Delete a Timer

You will see the Timers you have added to your app underneath the Timers section of your blocks. To edit the properties after the fact or delete a timer, click the gear icon next to the Timer's name in the left panel of the Blocks tab.&#x20;

![](../../.gitbook/assets/timers-menu.png)

## Blocks

### Events

#### When Timer Fires

![](../../.gitbook/assets/whentimerfires.png)

Set something to happen when the Timer fires.

### Functions

#### Start Timer

![](../../.gitbook/assets/timst.png)

Starts the Timer.

#### Stop Timer

![](../../.gitbook/assets/timstop.png)

Stops the Timer.

### Property Blocks

#### Get time in seconds

![](../../.gitbook/assets/gets.png)

If `Count Up` is `false`, returns remaining time from the Timer's interval in seconds.

If `Count Up` is `true`, returns elapsed time from the Timer's interval in seconds.

#### Get time in milliseconds

![](../../.gitbook/assets/getms.png)

If `Count Up` is `false`, returns remaining time from the Timer's interval in milliseconds.

If `Count Up` is `true`, returns elapsed time from the Timer's interval in milliseconds.

#### Set Interval

![](../../.gitbook/assets/setint.png)

Set interval of Timer in milliseconds.

#### Get Interval of Timer

![](../../.gitbook/assets/getint.png)

Returns interval of Timer in milliseconds

#### Set Count Up

![](../../.gitbook/assets/setcount.png)

Set whether Count Up is enabled for this Timer.

#### Get Count Up

![](../../.gitbook/assets/getcount.png)

Returns `true` or `false` value for whether Count Up is enabled for this Timer.

#### Set Loops

![](../../.gitbook/assets/setloops.png)

\
If `Loops = true`, the timer will reset itself after it fires. If your interval is 10 seconds, the Timer will fire every 10 seconds.‌

If `Loops = false`, the timer will finish its current interval if it is in the middle of one, and will no longer fire. If your interval is 10s, the timer will finish its current 10 second interval, fire, and then stop.

#### Get Loops

![](../../.gitbook/assets/getloops.png)

Returns `true` or `false` value for whether Loops is enabled for this Timer.

#### Set Enabled

![](../../.gitbook/assets/setenabled.png)

Set whether the Timer is enabled.

#### Get Enabled

![](../../.gitbook/assets/screen-shot-2021-04-12-at-8.52.24-am.png)

Returns `true` or `false` value for whether this Timer is enabled.