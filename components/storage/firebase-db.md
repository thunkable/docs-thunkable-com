#### **Thunkable for Android **❤

# Firebase DB ![](/assets/firebase-icon.png)

---

Tiny Web DB is a non-visible component that communicates with a Web service to store and retrieve information.

**Important Note** This database was created initial for prototyping and the data is public to all other users. We highly recommend using an alternate database like Firebase DB or Spreadsheets for storing and retrieving data in the cloud

---

#### Functionality

| Event | Description |
| :--- | :--- |
| Service URL | The URL to the database with which the component should communicate |
| Store Value \(tag, valueToStore\) | Sends a request to the Web service to store the given value under the given tag |
| Value Stored | Indicates that a StoreValue server request has succeeded |
| Get Value \(tag\) | Sends a request to the Web service to get the value stored under the given tag. The Web service must decide what to return if there is no value stored under the tag. This component accepts whatever is returned |
| Got Value \(tagFromWebDB, valueFromWebDB\) | Indicates that a GetValue server request has succeeded |
| Web Service Error \(message\) | Indicates that there was an error communicating with the Web service |



