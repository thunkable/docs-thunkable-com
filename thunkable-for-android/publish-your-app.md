#### **Thunkable for Android **❤

# Step 4 `Publish`

|  Requirements |  |  |  |  |
| :--- | :--- | :--- | :--- | :--- |


---

### Requirements

Here are the _minimum_ requirements for publishing to the Google Play Store:

* [Google Play Developer account](https://play.google.com/apps/publish/signup/) \($25 one-time registration fee\)
* Assets
  * App icon at 512 px by 512 px
  * Feature graphic at 1024 px by 500 px
  * Screenshots

---

### Package name

The package name for all apps built completely on Thunkable:

* com.thunkable.android.{username}.{appname}

Currently, there is no way to customize your package name \(which is visible on the Google Play store url\)

---

### **Version Your App**

Every app you publish must have a`VersionCode`and a`VersionName`. You can set these in the designer under the properties panel for the`Screen1`component.

`VersionCode`is an integer value that will not be visible to Google Play Store users. It is used by other apps to check if your app has been upgraded or downgraded. It defaults to 1 and should be increased by one with every successive change whether it is a major change or a minor change.

`VersionName`is a String which can be anything you would like. It is defaulted to`1.0`. A common structure is a decimal number which is increased by 1 for every major change and`0.1`for every minor change. For example, an initial`VersionName`could be`1.0`which can be updated to`1.1`after a small change and`2.0`after a larger change.

You will need to increase the`VersionCode`and change the`VersionName`of your application when you upload a new version to the Play Store.

---

### Download app \(.apk\) to your computer {#exporting-your-keystore-from-mit-app-inventor}

Package the app \(.apk file\) by going to the "Export" menu on the Thunkable toolbar

![](https://thunkable.com/explore/img/share/Build_Dropdown.png)

Select "App \(save .apk to my computer\)." A pop-up box \(seen below\) should alert you that your download has begun. Note: The other option \(provide QR code for .apk\) produces a scannable QR code that will download the app for two hours. You can share this code with others, but they have to use it within 2 hours of your generating it.

![](https://thunkable.com/explore/img/share/Build_Popup.png)

You can also download the apk directly from your apps home page by clicking on the download arrow next to any app project.

![](https://thunkable.com/explore/img/share/download_apk.png)

---

### Publish Your App

You can now go to [Google Play Publishing Home](https://play.google.com/apps/publish/signup/) and follow the steps to publish your app to Google Play.

For more details, you may want to start with [Introduction to Publishing on Google Play](https://developer.android.com/distribute/tools/launch-checklist.html) and [Google Support on Uploading to Google Play](https://support.google.com/googleplay/android-developer/answer/113469?hl=en&topic=2365624&ctx=topic).

---

### Package name

The package name for all apps built completely on Thunkable:

* com.thunkable.android.{username}.{appname}

Currently, there is no way to customize your package name \(which is visible on the Google Play store url\)

---

### Backups

Once you publish your application in the Google Play Store, other people will now be depending upon you to fix bugs and otherwise maintain your application. It is therefore very important that you backup your application's source code. To do this, click on "Project--&gt;My Projects", check the box next to the name of your project and then select "Project--&gt;Export selected project \(.aia\) to my computer." This will download a zip file which contains your projects source code. Store it in a safe place!

Thunkable and Google, which operate the App Engine service on which Thunkable relies, make best efforts to ensure that Thunkable does not lose projects. HOWEVER WE CAN OFFER NO GUARANTEE THAT DATA \(LIKE YOUR PROJECTS\) WILL NEVER BE LOST. IT IS IMPERATIVE THAT YOU MAKE YOUR OWN BACKUPS!

---

### Keystores

During the .apk building process your application is signed with a digital private key which is associated with your account. Whenever you build a new version this same key is used to sign the new version. When an android phone has an application installed on it, it remembers the key that was used to sign it. In order to install an updated version of an application, the new application must be signed by the same key. It is therefore important that you not lose this key!

Your private digital key is stored in a keystore file. Normally the Thunkable server will create this file when needed and store it for you so you do not need to worry about it. Although we do not anticipate losing your keystore file, we recommend that you back it up. From the designer under the "Projects" menu there is a choice labeled "Export Keystore". Select this option. This will download your keystore file to your local computer. Save it in a safe place. It should not be publicly readable as your private digital key is a secret which should not be shared.

If you move your project to another Thunkable server, you will want to upload your keystore to that server \(you will see that under "Projects" there is a "Import Keystore" option as well\). You only need to do this if you are publishing .apk files to Google Play or if you intend to share your application with other people in general.

IF YOUR keyfile IS LOST OR DELETED IT CANNOT BE RECOVERED. If you were to lose your project's source code, you could always re-enter it from scratch \(this may be a lot of work, but is something you can do\). NEITHER YOU NOR THUNKABLE CAN RECOVER A LOST keyfile. NO AMOUNT OF EFFORT WILL RECOVER IT, SO BE SURE TO BACK IT UP!!!

