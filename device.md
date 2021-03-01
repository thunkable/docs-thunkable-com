# Device

The Device blocks gather useful data from the device \(Android / iOS, online / offline, time and date\) as well as set the phone to vibrate.

* [Vibrate device](device.md#vibrate-device)
* [Get current time and date](device.md#get-current-time-and-date)
* [Get Seconds since 1970](device.md#seconds-since-1970)
* [Get online/offline status](device.md#get-online-offline-status)
* [Get Screen Height/Width](device.md#screen-height-width)
* [Get mobile operating system](device.md#get-mobile-operating-system)
* [Dismiss Keyboard](device.md#dismiss-keyboard)
* [Keep Screen Awake](device.md#keep-screen-awake)
* [Get Device Color Scheme](device.md#get-device-color-scheme)

## Vibrate Device

![](.gitbook/assets/vibrate.png)

This block will vibrate the device.

## Get Current Time and Date

![](.gitbook/assets/thunkable-docs-exhibits-93.png)

![](.gitbook/assets/screen-shot-2018-12-13-at-12.58.32-pm.png)

At the moment, all the dates and times are in numerical format i.e. month = 1 rather than month = Jan. If you want to convert the numbers into names, we suggest you to add a [Local DB](local-db.md) component and a simple table like the ones shown below.

![Add a Local DB component that maps the numerical month with the names ](.gitbook/assets/screen-shot-2018-12-13-at-2.08.44-pm.png)

![Because the minutes can be less than one digit and digital clocks always show two, there&apos;s an additional conditional block to account for the case when the minute is less than double digits](.gitbook/assets/screen-shot-2018-12-13-at-2.10.33-pm.png)

## Get Seconds since 1970

![](.gitbook/assets/unix.png)

Measures seconds since 00:00:00 UTC on 1 January 1970. This timestamp is also known as Unix time or Epoch time. You can read about its use in computer programming at the [Unix time Wikipedia page](https://en.wikipedia.org/wiki/Unix_time).

## Get Online/Offline Status

There may be times you may want to design a different experience when a user is offline. To detect a user's connection, you can simply use the blocks below:

![](.gitbook/assets/screen-shot-2018-12-13-at-2.16.48-pm.png)

This block will return `true` or `false`.

## Get Screen Height/Width

![](.gitbook/assets/size.png)

Returns the height or width of the screen running the app in pixels.

## Get Mobile Operating System

Since Thunkable can build apps for Android, iOS and web, there may be times when you want to modify your user experience depending on their mobile operating system. To do so, you can use the block below:

![](.gitbook/assets/platform.png)

This block will return `true` or `false`.

## Dismiss Keyboard

If you have a Text Input in your app, there may be situations when you want to dismiss the keyboard for the user. The block below will help with that:

![](.gitbook/assets/screen-shot-2019-07-19-at-4.34.21-pm.png)

## Keep Screen Awake

![](.gitbook/assets/awake.png)

Some devices will auto-sleep if there is no user activity in an app for a certain period of time.  
The Keep Screen Awake block can be used to keep the screen awake even if the user is not actively interacting with the app.  
This block can be set to `true` or `false`.

## Get Device Color Scheme

![](.gitbook/assets/theme.png)

Having dark mode and light mode available is a popular choice for apps and device operating systems.  
This block can be used to detect whether the user's device has a light or dark theme on their device.   
You can then use blocks to change the color scheme of components in your app to match the user's preferences.  
This block will return `true` or `false`.

