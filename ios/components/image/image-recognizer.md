#### **Thunkable for iOS **

# Image Recognizer ![](/assets/microsoft-icon.png) powered by Microsoft

---

Microsoft's Image Recognizer services puts the power of some of the most advanced open artificial intelligence tools into your image-based apps.

The Image Recognizer returns a description and tags about visual content found in an image![](/assets/image-recognizer-ios-fig-2.png)

---

#### Auto-caption a picture

![](/assets/image-recognizer-ios-fig-1.png)

| Event | Description |
| :--- | :--- |
| Upload \(`photo`\) | Sends a `photo` to Microsoft's Image Recognizer and returns a one-line `description` , a `confidenceLevel` for that description, and description `tags`.  It will also return an `error` if there is a problem returning a description for a given image. |

---

#### Set up

No set up is required.

Thunkable provides its own API key by default for your convenience but if you expect your users to upload more than 1,000 images per month, please create your own free account with [Microsoft Cognitive Services](https://azure.microsoft.com/en-us/services/cognitive-services/) \(current free limit is 30,000 images per month\)

| Property | Description |
| :--- | :--- |
| Subscription Key | Thunkable provides its own subscription key as `default`. You can add your own if you expect your users to upload more than 1,000 images per month |
| Server Url | Distinct Url required for the Computer Vision API. Do not change the `default` unless you are trying to access this component from China, in which case you need to provide a different server Url |



