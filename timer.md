# Timer

## Properties

You can set:

* The **Name **of the Timer
* The **Interval **of the Timer, in seconds or milliseconds
* Whether or not the Timer should **Count Up**
* Whether the Timer should **Loop**, ie. if the Timer should reset itself once it fires
* Whether the Timer is **Enabled **(this can be changed with blocks)

## Event Blocks

### When Timer Fires

![](.gitbook/assets/whentimerfires.png)

Set something to happen when the Timer fires.

## Function Blocks

### Start Timer

![](.gitbook/assets/newtimerblocks-start.png)

Starts the Timer.

### Stop Timer

![](.gitbook/assets/newtimerblocks-stop.png)

Stops the Timer.

## Properties Blocks

### Get Time

#### Get time in seconds

![](.gitbook/assets/newtimerblocks-get-time-seconds.png)

If `Count Up` is `false`, returns remaining time from the Timer's interval in seconds.

If `Count Up` is `true`, returns elapsed time from the Timer's interval in seconds.

#### Get time in milliseconds

![](.gitbook/assets/newtimerblocks-get-time-milliseconds.png)

If `Count Up` is `false`, returns remaining time from the Timer's interval in milliseconds.

If `Count Up` is `true`, returns elapsed time from the Timer's interval in milliseconds.

### Interval

#### Set Interval

![](.gitbook/assets/newtimerblocks-set-interval.png)

Set interval of Timer in milliseconds.

#### Get Interval of Timer

![](<.gitbook/assets/image (170).png>)

Returns interval of Timer in milliseconds.

### Count Up

#### Set Count Up

![](.gitbook/assets/newtimerblocks-set-countup.png)

Set whether Count Up** **is enabled for this Timer.

#### Get Count Up

![](.gitbook/assets/newtimerblocks-get-countup.png)

Returns `true` or `false` value for whether Count Up is enabled for this Timer.

### Loops

#### Set Loops

![](.gitbook/assets/newtimerblocks-setloops.png)

If `Loops = true`, the timer will reset itself after it fires. If your interval is 10 seconds, the Timer will fire every 10 seconds.

If `Loops = false`, the timer will finish its current interval if it is in the middle of one, and will no longer fire. If your interval is 10s, the timer will finish its current 10 second interval, fire, and then stop.

#### Get Loops

![](.gitbook/assets/newtimerblocks-get-loops.png)

Returns `true` or `false` value for whether Loops is enabled for this Timer.

### Enabled

#### Set Enabled

![](.gitbook/assets/newtimerblocks-set-enabled.png)

Set whether the Timer is enabled.

#### Get Enabled

![](.gitbook/assets/newtimerblocks-get-enabled.png)

Returns `true` or `false` value for whether this Timer is enabled.
