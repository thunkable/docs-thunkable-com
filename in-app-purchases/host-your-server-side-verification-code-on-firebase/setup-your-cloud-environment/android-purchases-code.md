---
description: >-
  Please be mindful. This page is almost identical to the previous with
  exceptions in the function name and code.
---

# Android Purchases Code

These codes will allow you to acknowledge and verify purchases or subscriptions. There is 1 call for each type of transaction.&#x20;

### 1. To get started, go to[ console.google.cloud.com/functions](https://console.cloud.google.com/functions/list)

### 2. Click Create Function

<div align="left">

<figure><img src="../../../.gitbook/assets/2 (2).png" alt=""><figcaption></figcaption></figure>

</div>

### 3. Give your new function  a meaningful name

**androidPurchaseHandler** should be the name you use here

<div align="left">

<figure><img src="../../../.gitbook/assets/3 (2) (1).png" alt=""><figcaption></figcaption></figure>

</div>

### 4. Save the trigger type

<div align="left">

<figure><img src="../../../.gitbook/assets/4 (3) (1) (1).png" alt=""><figcaption></figcaption></figure>

</div>

### 5. Copy the code below and click the blue "next" button

<details>

<summary>Copy Me</summary>

{% code title="androidPurchaseHandler." %}
```
///purchase handler
const functions = require("firebase-functions");
const admin = require("firebase-admin");
const googleServiceAccountKey = require("./serviceAccount.json");
admin.initializeApp({
  credential: admin.credential.cert(googleServiceAccountKey),
});
const {google} = require("googleapis");
const axios = require("axios");

exports.androidPurchaseHandler = functions.https.onRequest((request, response) => {
 
  const {purchaseObject, type} = request.body;
  // get the token and product id from the request
  const purchaseToken = purchaseObject.purchaseToken;
  const productId = purchaseObject.productId;
  functions.logger.info(`trying to handle ${type} for the follow ${JSON.stringify(purchaseObject)}`);
  // set your package id
  const packageID = "edu.fit.my.jgibb2018.pob";

  const returnTheResponse = (data) => {
    response.status(200).send(data);
  };

  const acknowledgePurchase = (err, tokens) => {
    functions.logger.info("acknowledging purchase");
    const config = {
      method: "post",
      url: `https://androidpublisher.googleapis.com/androidpublisher/v3/applications/${packageID}/purchases/products/${productId}/tokens/${purchaseToken}:acknowledge`,
      headers: {
        "Authorization": `Bearer ${tokens.access_token}`,
      },
    };

    axios(config)
        .then(function(r) {
          functions.logger.info("acknowledge success. returning ", JSON.stringify(r.data));

          returnTheResponse(r.data);
        })
        .catch(function(e) {
          returnTheResponse(JSON.stringify({error: e.data, status: e.status, message: e.message}));
        });
  };

  const verifyPurchase = (err, tokens) => {
    functions.logger.info("verifying purchase");
    const config = {
      method: "get",
      url: `https://androidpublisher.googleapis.com/androidpublisher/v3/applications/${packageID}/purchases/products/${productId}/tokens/${purchaseToken}`,
      headers: {
        "Authorization": `Bearer ${tokens.access_token}`,
      },
    };

    axios(config)
        .then(function(r) {
          functions.logger.info("verify success. returning ", JSON.stringify(r.data));
          returnTheResponse(r.data);
        })
        .catch(function(e) {
          returnTheResponse(JSON.stringify({error: e.data, status: e.status, message: e.message}));
        });
  };

  const getAccessToken = () => {
    const jwtClient = new google.auth.JWT(
        googleServiceAccountKey.client_email,
        null,
        googleServiceAccountKey.private_key,
        ["https://www.googleapis.com/auth/androidpublisher"],
        null,
    );
    try {
      functions.logger.info("type is ", type);
      if (type == "purchaseAcknowledge") {
        jwtClient.authorize(acknowledgePurchase);
      } else {
        jwtClient.authorize(verifyPurchase);
      }
    } catch (error) {
      functions.logger.log(error);
      response.status(500).send("getting auth", error);
    }
  };

  getAccessToken();
});


```
{% endcode %}



</details>

<div align="left">

<figure><img src="../../../.gitbook/assets/5 (3) (1).png" alt=""><figcaption></figcaption></figure>

</div>

### 6. Clear the default and paste the copied code into the code

{% embed url="https://vimeo.com/698771346" %}

### 7. Update the package.json file

<details>

<summary>copy and paste this over  the default code</summary>

```
{
  "name": "sample-http",
  "version": "0.0.1",
  "dependencies": {
     "axios": "^0.26.0",
     "googleapis": "^97.0.0",
     "firebase-functions": "^3.18.0",
     "firebase-admin": "^10.0.2"
   }
}

```

</details>

{% embed url="https://player.vimeo.com/video/698770935" %}

### 8. Set the name of the functions entry point

the name used here should match the name used in **Step 3** above

<div align="left">

<figure><img src="../../../.gitbook/assets/9.1 (1).png" alt=""><figcaption></figcaption></figure>

</div>

### 9. Click the plus icon to create a new file and name it "serviceAccount.json"

<div align="left">

<figure><img src="../../../.gitbook/assets/9.1 (1).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/9.2 (1).png" alt=""><figcaption></figcaption></figure>

</div>

### 10. Copy and paste the content of this projects [service account](http://127.0.0.1:5000/s/KrMxDvAEx21XNB81zaoj/in-app-purchases/overview/android-play-store-setup#download\_your\_service\_key) file from your computer into this newly created file.&#x20;

<div align="left">

<figure><img src="../../../.gitbook/assets/10 (1).png" alt=""><figcaption></figcaption></figure>

</div>

### 11. Deploy the function

<div align="left">

<figure><img src="../../../.gitbook/assets/11 (1).png" alt=""><figcaption></figcaption></figure>

</div>

### 12. Set function invocation privacy permissions

This allows any device with your endpoint URL the ability to verify purchases made via your app

1. Go to [https://console.cloud.google.com/functions/list](https://console.cloud.google.com/functions/list)
2. Select the function you want to make public. (the function you just created)
3. Click the **Permissions** tab.
4. Click **Add Principle**
5. In the **Add members** field, type `allUsers`
6. Select the **Cloud Function Invoker** role from the **Select a role** drop-down menu.
7. Click **Add**.
