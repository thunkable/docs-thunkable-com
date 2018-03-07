#### **Thunkable for iOS **

# Realtime Database ![](/assets/iOSviewIconFirebaseDB.png) powered by Firebase

---

Realtime DB powered by Firebase is cloud storage component that stores and retrieves `keys` and their corresponding `values` in a database that can be accessed in real-time \(super fast\).

This version of the component supports storing app data in unique project buckets associated with a user's project. You can add your own private database instance by following the instructions below.

IMPORTANT As a general rule, user data should always be kept secure.  We strongly advise that you use own Firebase account both to ensure the privacy of your user data and to give you visibility into the database itself. We provide our database for your convenience but we may also clean out our shared account periodically.

* [Save, Retrieve and Update Data in Realtime](#save-retrieve--update-data-in-realtime)

* [Using Your Own Private Firebase Account](#private-firebase) \(recommended\)

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

#### Use Your Own Private Firebase Account \(recommended\) {#private-firebase}

IMPORTANT As a general rule, user data should always be kept secure.  We strongly advise that you use own Firebase account both to ensure the privacy of your user data and to give you visibility into the database itself.  Firebase Realtime Database also pairs well with [Sign in](/ios/components/screen-layout/authentication/sign-in.md) and you can use a single Firebase project for both services.

#### Step 1 / Create an account with [Firebase](https://firebase.google.com/) for free \(you can upgrade to a paid plan later\)

#### Step 2 / After creating your project, retrieve the API key and database URL for your project from the Firebase console.  One way to retrieve those values is illustrated below.

#### ![](/assets/firebase-ios-fig-3.png)![](/assets/firebase-ios-fig-4.png)

#### Step 3 / On Thunkable, you can simply copy the API key and database URL into App Settings \(which you can find by clicking on your project app icon on the top left. ![](/assets/firebase-ios-fig-5.png)

#### Step 4 / If you are using Firebase with a [Sign In](/ios/components/screen-layout/authentication/sign-in.md), you can leave the database rules as they are by default.

![](/assets/firebase-ios-fig-6.png)

#### If you do not want to require users to sign in, you'll need to change your database rules to accept users to save to your database.

![](/assets/firebase-ios-fig-7.png)

#### Congrats you should be all set up!  You can view and manage your data in Firebase



