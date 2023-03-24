# Device

The Device blocks gather useful data from the device \(Android / iOS, online / offline, time and date\) as well as set the phone to vibrate.

* [Get current time and date](device.md#get-current-time-and-date)
* [Get mobile operating system](device.md#get-mobile-operating-system)
* [Get online/offline status](device.md#get-online-offline-status)
* [Set device to vibrate](device.md#set-device-to-vibrate)
* Dismiss keyboard

## Get current time and date

![](.gitbook/assets/thunkable-docs-exhibits-93.png)

![](.gitbook/assets/screen-shot-2018-12-13-at-12.58.32-pm.png)

At the moment, all the dates and times are in numerical format i.e. month = 1 rather than month = Jan. If you want to convert the numbers into names, we suggest you to add a [Local DB](local-db.md) component and a simple table like the ones shown below.

![Add a Local DB component that maps the numerical month with the names ](.gitbook/assets/screen-shot-2018-12-13-at-2.08.44-pm.png)

![Because the minutes can be less than one digit and digital clocks always show two, there&apos;s an additional conditional block to account for the case when the minute is less than double digits](.gitbook/assets/screen-shot-2018-12-13-at-2.10.33-pm.png)

## Get mobile operating system

Since Thunkable Cross Platform ✕ works on both Android and iOS from a single project, there may be times when you want to modify your user experience depending on their mobile operating system. To do so, you can use the block below:

![](.gitbook/assets/screen-shot-2018-12-13-at-2.17.26-pm.png)

To see how this might work in your app, take a look at the blocks below:

![](.gitbook/assets/screen-shot-2018-12-13-at-2.16.39-pm.png)

## Get online/offline status

There may be times you may want to design a different experience when a user is offline. To detect a user's connection, you can simply use the blocks below:

![](.gitbook/assets/screen-shot-2018-12-13-at-2.16.48-pm.png)

## Set device to vibrate

Apps often work in the background and vibrating a device is a popular way of notifying a user of a certain event. To set your device to vibrate, you can use the block sample below:

![](.gitbook/assets/screen-shot-2018-12-13-at-2.21.45-pm.png)

## Dismiss keyboard

If you have a Text Input in your app, there may be situations when you want to dismiss the keyboard for the user. The block below will help with that:

![](.gitbook/assets/screen-shot-2019-07-19-at-4.34.21-pm.png)

