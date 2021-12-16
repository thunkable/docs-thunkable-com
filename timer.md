# Timer

## Adding Timers to your app

### Create a Timer

You can add a Timer to your app from the Blocks tab of your Thunkable project.\
Find the **Timers** drawer of blocks and click on the ⊕ icon to add a Timer to your app.

![](.gitbook/assets/timers.png)

### Properties

You will see a settings panel that allows you to set:

* The **Name** of the Timer
* The **Interval** of the Timer, in seconds or milliseconds
* Whether or not the Timer should **Count Up**
* Whether the Timer should **Loop**, ie. if the Timer should reset itself once it fires
* Whether the Timer is **Enabled** (this can be changed with blocks)

You can also **Delete** the Timer.

![](.gitbook/assets/timerdialouge.png)

### Edit a Timer

You will see the Timers you have added to your app underneath the Timers section of your blocks.

![](.gitbook/assets/timers-menu.png)

## Event Blocks

### When Timer Fires

![](.gitbook/assets/whentimerfires.png)

Set something to happen when the Timer fires.

## Function Blocks

### Start Timer

![](.gitbook/assets/timst.png)

Starts the Timer.

### Stop Timer

![](.gitbook/assets/timstop.png)

Stops the Timer.

## Property Blocks

### Get Time

#### Get time in seconds

![](.gitbook/assets/gets.png)

If `Count Up` is `false`, returns remaining time from the Timer's interval in seconds.

If `Count Up` is `true`, returns elapsed time from the Timer's interval in seconds.

#### Get time in milliseconds

![](.gitbook/assets/getms.png)

If `Count Up` is `false`, returns remaining time from the Timer's interval in milliseconds.

If `Count Up` is `true`, returns elapsed time from the Timer's interval in milliseconds.

### Interval

#### Set Interval

![](.gitbook/assets/setint.png)

Set interval of Timer in milliseconds.

#### Get Interval of Timer

![](.gitbook/assets/getint.png)

Returns interval of Timer in milliseconds.

### Count Up

#### Set Count Up

![](.gitbook/assets/setcount.png)

Set whether Count Up **** is enabled for this Timer.

#### Get Count Up

![](.gitbook/assets/getcount.png)

Returns `true` or `false` value for whether Count Up is enabled for this Timer.

### Loops

#### Set Loops

![](.gitbook/assets/setloops.png)

\
If `Loops = true`, the timer will reset itself after it fires. If your interval is 10 seconds, the Timer will fire every 10 seconds.‌

If `Loops = false`, the timer will finish its current interval if it is in the middle of one, and will no longer fire. If your interval is 10s, the timer will finish its current 10 second interval, fire, and then stop.

#### Get Loops

![](.gitbook/assets/getloops.png)

Returns `true` or `false` value for whether Loops is enabled for this Timer.

### Enabled

#### Set Enabled

![](.gitbook/assets/setenabled.png)

Set whether the Timer is enabled.

#### Get Enabled

![](.gitbook/assets/screen-shot-2021-04-12-at-8.52.24-am.png)

Returns `true` or `false` value for whether this Timer is enabled.
