# Server Logs

These should be created and deployed like the previous 3 functions



### 1. To get started, go to[ console.google.cloud.com/functions](https://console.cloud.google.com/functions/list)

### 2. Click Create Function

### 3. Give your new function  a meaningful name

**serverLog** should be the  name you use here

### 4. Save the trigger type

### 5. Copy the code below and click the blue "next" button

### 6. Clear the default and paste the copied code into the code

### 7. Update the package.json file

### 8. Set the name of the functions entry point

the name used here should match the name used in **Step 3** above

### 11. Deploy the function

### 12. Set function invocation privacy permissions

This allows any device with your endpoint URL the ability to verify purchases made via your app

1. Go to [https://console.cloud.google.com/functions/list](https://console.cloud.google.com/functions/list)
2. Select the function you want to make public. (the function you just created)
3. Click the **Permissions** tab.
4. Click **Add Principle**
5. In the **Add members** field, type `allUsers`
6. Select the **Cloud Function Invoker** role from the **Select a role** drop-down menu.
7. Click **Add**.

<details>

<summary>Code</summary>

```
const functions = require("firebase-functions");
const admin = require("firebase-admin");
admin.initializeApp();


exports.purchaseInfo = functions.https.onRequest((request, response) => {
  const dbRef = admin.database().ref("purchases")
  const data = request.body;
  const queryTerms = request.query;
  const objToSave = {
    data, queryTerms, timestamp: admin.firestore.FieldValue.serverTimestamp(),
  };

  //add this objToSave the realtime database
  dbRef.push(objToSave);

  
  response.send("success").status(200);
});
```

</details>

<details>

<summary>package.json</summary>

```
{
  "name": "functions",
  "description": "Cloud Functions for Firebase",
  "version": "1.0.0",
  "dependencies": {
    "firebase-admin": "^9.8.0",
    "firebase-functions": "^3.14.1"
  }
}

```

</details>
