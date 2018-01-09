#### **Thunkable for iOS **

# Realtime Database ![](/assets/firebase-ios-icon.png) powered by Firebase

---

Realtime DB powered by Firebase is cloud storage component that stores and retrieves `keys` and their corresponding `values` in a database that can be accessed in real-time \(super fast\).

This version of the component supports storing app data in unique project buckets associated with a user's project. You can add your own private database instance by following the instructions below.

---

#### Save Data to Firebase

![](/assets/firebase-ios-fig-1.png)

---

#### Update Data in Realtime

![](/assets/firebase-ios-fig-2.png)

---

#### Save, Retrieve & Update Data in Realtime

| Event | Description |
| :--- | :--- |
| Save \(`key`, `value`\) | Asks Firebase to save a given `value` under the given `key` |
| Get \(`key`, `value`\) | Asks Firebase to get the `value` stored under the given `key` |
| Add Listener \(`key`\) | Asks Firebase to listen to a specific `key` for changes in the database. Required for Data Changed block. |
| Data Changed \(`key`, `value`\) | Asks Firebase for updates to `value` for specified `key`. Requires an Add Listener block. |
| Remove Listener \(`key`\) | Ask Firebase to stop listening to a specific `key` for changes in the database |

---

#### Use Your Own Firebase Instance

#### Step 1 Create an account with Firebase for free \(you can upgrade to a paid plan later\) and a new app project. In Database 'Rules', set "read" and "write" to 'true' \(they will be set to 'false' by default\). 

#### ![](/assets/firebase-ios-fig-6.png)

#### 

#### Step 2 Add Firebase to your iOS app and generate a plist file by following the steps below. Note that you can use the same Firebase project for your Android and iOS app.

![](/assets/firebase-ios-fig-3.png)![](/assets/firebase-ios-fig-4.png)![](/assets/firebase-ios-fig-5.png)

#### Step 3 Drag and drop the plist in you assets folder on Thunkable

![](/assets/firebase-ios.gif)

#### Step 4 After Downloading or Publishing Your App, View and Edit Database Contents

IMPORTANT: Private database instance will not work during live testing

