---
description: Preview your Thunkable project with our Thunkable live app, or on the Web
---

# Live Test your App

## **What is the Thunkable Live App?**

The Thunkable Live app connects the projects in your web browser directly to your mobile device. It allows you to do two things:

1. You can [**Live Test**](live-test.md#live-test) your project. Any changes you make in your browser are displayed on your device immediately.&#x20;
2. You can [**Live Preview**](live-test.md#live-preview) any of your projects, directly on your device, without the need to be logged in to your computer.

## **Download the Thunkable Live App**

The Thunkable Live app allows you to live test your app on your device, in real-time, while you are building it. Not even hard core developers have this super power. You can also preview all your app projects from the comfort of your mobile device.

| [**Download for Android**](https://play.google.com/store/apps/details?id=com.thunkable.live) | [**Download for iOS**](http://appstore.com/thunkablelive) |
| -------------------------------------------------------------------------------------------- | --------------------------------------------------------- |

![](../.gitbook/assets/appstorepic\_email\_small.png)

If you don't have an iOS or Android device, you can also [set up an emulator](../emulators.md) on your computer that will mimic what you would see on an actual device.‌

With Thunkable Live installed on your device, you are now ready to live test or to live preview.‌

## **Live Test**

While live testing, any changes that you make to your project should be reflected in your app. Bear in mind that the Thunkable Live app doesn't check your project for errors. Some changes that you make may crash the app. If this happens simply exit out of the app and re-open it.

### **Getting started**

From any of your Thunkable projects, click on the **Live Test** button at the top of the screen to begin live testing.

![](../.gitbook/assets/live\_test\_icon.png)

‌The next pop-up you see depends on if you are [signed in with Google](live-test.md#if-you-are-signed-in-with-google) or if you have [signed in by email](live-test.md#if-you-are-signed-in-by-email).‌

### **If you are signed in with Google:**

Clicking on the Live Test button will remind you to open Thunkable Live on your device.

![](../.gitbook/assets/lt\_gmail.png)

Sign in with the same Google account in Thunkable Live to preview your projects directly on your device.

### **If you are signed in by Email:**

When you click the Live Test button you will be prompted to enter a code into your computer.

![](../.gitbook/assets/lt\_email.png)

To find this code, open Thunkable Live on your device and click **Email sign in - Generate Test Code.**

![](../.gitbook/assets/img\_1315.png)

Enter this code into the first prompt and you will be able to live test your app.

## **Live Preview**

For the first time, you can live preview all your app projects from the comfort of your mobile device. Simply login and you should see a list of all your projects on your Thunkable Live app.

![](<../.gitbook/assets/live-preview-fig-1 (1).gif>)

## Troubleshooting

Common issues with the Thunkable Live app

### **You see a blank / white screen when you live test (even if there are items in your app)**

* If you have a Navigator as the first item in your tree, make sure your screen is dropped within it
* Your have unconnected blocks
* You have an event triggered by a Screen.Start which may be causing the screen to crash
* Your app and desktop may not be logged into the same account

### **App is crashing because of a bug on our end; we are trying to fix it as soon as we can**

* (Android only) You are trying to set the value of a Slider in your blocks&#x20;
* (Android only) You are trying to set the latitude and longitude of a Map in your blocks

### **Image is not showing up on your phone**

* The height or width of the image may be set to 'Fit contents'

## Preview your App on the Web

Preview on the Web allows you to live preview your own project directly from your browser. Simply click on "Live Test" to preview your own app in a pop-up window. &#x20;

![](../.gitbook/assets/live\_preview.gif)

&#x20;You can also preview any _public _app, directly from the Project Detail Page. Here's [one example](https://x.thunkable.com/projectPage/5ea6ed029ce3d64d1d3a27dc) but you can find thousands of others in the public gallery.

![](../.gitbook/assets/project\_preview.gif)

### Unsupported Components

Not all components are supported on the web at this time so please see the list below of components that are **`not supported`**:

| Component                | Category       | Status                                       |
| ------------------------ | -------------- | -------------------------------------------- |
| **Map**                  | Location       | **`Not supported yet`**                      |
| **Share**                | Social         | **`Not supported yet`**                      |
| **Push Notification**    | Social         | **`Not supported yet`**                      |
| **AdMob**                | Monetization   | **`Can not be supported`**                   |
| **Bluetooth Low Energy** | Sensors        | **`Not supported yet`**                      |
| **Accelerometer**        | Sensors        | **`Supported but may not work as expected`** |
| **Gyroscope**            | Sensors        | **`Supported but may not work as expected`** |
| **Magnetometer**         | Sensors        | **`Supported but may not work as expected`** |
| **Alert**                | User Interface | **`Not supported yet`**                      |
| **Speech Recognizer**    | Voice          | **`Not supported yet`**                      |
| **Assistant**            | Voice          | **`Not supported yet`**                      |
| **Photo Library**        | Image          | **`Not supported yet`**                      |
| **Barcode Scanner**      | Image          | **`Not supported yet`**                      |
| **Local Storage**        | Data           | **`Not supported yet`**                      |

