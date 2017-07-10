#### **Thunkable for Android **❤

# Tiny DB ![](/assets/tiny-db-icon.png)

---

TinyDB is a non-visible component that stores data for an app.

Apps created with Thunkable are initialized each time they run. This means that if an app sets the value of a variable and the user then quits the app, the value of that variable will not be remembered the next time the app is run. In contrast, TinyDB is a persistent data store for the app. The data stored in a TinyDB will be available each time the app is run. An example might be a game that saves the high score and retrieves it each time the game is played.

Data items are strings stored under tags. To store a data item, you specify the tag it should be stored under. Subsequently, you can retrieve the data that was stored under a given tag.

Each app has its own data store. There is only one data store per app. Even if you have multiple TinyDB components, they will use the same data store. To get the effect of separate stores, use different keys. You cannot use the TinyDB to pass data between two different apps on the phone, although you can use the TinyDB to share data between the different screens of a multi-screen app.

---

#### Functionality

| Event | Description |
| :--- | :--- |
| Store Value \(tag, valueToStore\)  | Store the value under the given tag. The storage persists on the phone when the app is restarted |
| Get Value \(tag, valueIfTagNotThere\)  | Retrieve the value stored under the given tag. If there's no such tag, then return valueIfTagNotThere |
| Clear All | Clear the entire data store in the Tiny DB |
| Clear Tag \(tag\)  | Clear the entry with the given tag |
| Get Tags | Return a list of all the tags in the Tiny DB |





