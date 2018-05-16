---
description: >-
  There are a variety of Android emulators out there, but Thunkable works best
  with Genymotion
---

# Test via Emulator



Here are the steps involved in installing and using Genymotion

### Install Genymotion and creating an Android Virtual Device \(AVD\) {#step-1-installing-genymotion-and-creating-an-android-virtual-device-avd}

1. Click [here](https://www.genymotion.com/account/create/) to create a Genymotion user account.
2. Download Genymotion's [user guide](https://docs.genymotion.com/Content/Home.htm) \(under the\_PDF Guides\_section\) and follow the\_Installation\_section. Then scroll down to the Virtual Devices section to set up an Android Virtual Device \(AVD\) \(You need not worry about other pages\).

### Deploy an APK file into an AVD {#step-2-deploying-an-apk-file-into-an-avd}

Once Genymotion is installed, you can use it to run packages apps \(APK files\), including apps that you have built and packaged with Thunkable. Here is an example:

1. Start an AVD in Genymotion:

   ![](https://thunkable.com/explore/img/emulator/start-avd.png)

2. Go back to Thunkable and download your app as an APK file.

   ![](https://thunkable.com/explore/img/emulator/download-thunkable-apk.png)

3. Drag and drop the APK file to the window of the running AVD. The application should launch:

   ![](https://thunkable.com/explore/img/emulator/genymotion-with-apk.png)

### Connect Genymotion to Thunkable through the Thunkable App {#step-3-connecting-genymotion-to-thunkable-through-the-thunkable-app}

You can also use Genymotion in live development in Thunkable. In order to do that, the computer you are using and the Genymotion emulator must be within the same subnet in the network. In the default setting, the Genymotion emulator and the computer are on different subnets. However, you can change the default settings to get them on the same subnet by doing the following:

1. Open the VirtualBox you have installed in Step 1
2. Identify and select the virtual machine you have made for the emulator
3. In the Network setting of that emulator, select_Adapter 2_, and select\_Bridge Adapter\_in the\_Attached to\_option. Underneath that, select either Wi-Fi or Ethernet, based on how you connect to the Internet.

   ![](https://thunkable.com/explore/img/emulator/genymotion-settings.png)

4. Load the Thunkable Live .apk into the emulator. You will need to manually update the app when Thunkable releases new versions of the app. You can download the [most recent version here](http://thunkable.com/live/Thunkable.apk).
5. Launch the Thunkable app within the emulator and connect with the Thunkable platform using the 6 digit code.
6. The project application should appear in Genymotion after 10 or 20 seconds.

### Going more in-depth

[How do you install Google frameworks \(Play, Accounts, etc.\) on a Genymotion virtual device?](http://stackoverflow.com/a/20013322/395857)  
[How to use adb with a Genymotion virtual device?](http://stackoverflow.com/a/17530410/395857)  
[How to solve the "failure install failed cpu api incompatible" error message when installing an APK file in Genymotion?](http://stackoverflow.com/a/24076795/395857)   
[How to copy virtual devices downloaded by Genymotion to another machine?](http://stackoverflow.com/q/17538686/395857)   
[How to transfer folder/files from your computer to the Genymotion instance?](http://stackoverflow.com/a/22803803/395857)

