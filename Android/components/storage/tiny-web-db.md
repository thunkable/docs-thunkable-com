#### **Thunkable for Android **❤

# Tiny Web DB

---

Tiny Web DB is a non-visible component that communicates with a Web service to store and retrieve information.

**Important note**: Since the introduction of Firebase, we only recommend the Tiny Web DB component for specific cases where you want to own and manage your own database infrastructure

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



