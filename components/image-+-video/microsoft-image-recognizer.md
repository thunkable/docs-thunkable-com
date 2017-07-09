#### **Thunkable for Android **❤

# Microsoft Image and Emotion Recognizer

---

Microsoft's Image and Emotion Recognizer services puts the power of some of the most advanced open artificial intelligence tools in your image-based apps.

The Image Recognizer returns information about visual content found in an image while the Emotion Recognizer detects emotions from images containing a single face.

|  | Image Recognizer | Emotion Recognizer |
| :--- | :--- | :--- |
| Recommended images | Any image | Images with a single face |
| Expected result | Single line 'description' with a 'description score' and image 'tags' | Most likely 'emotion' and 'emotion score' from anger, contempt, disgust, fear, happiness, neutral, sadness, and surprise. These emotions are understood to be cross-culturally and universally communicated with particular facial expressions |

The sample app [Thunkableagram: AI-powered Instagram](#) uses the Image Recognizer to auto-caption images

---

#### Set up

No set up is required.

Thunkable provides its own API key by default for your convenience but if you expect your users to upload more than 1,000 images per month, please create your own free account with [Microsoft Cognitive Services](https://azure.microsoft.com/en-us/services/cognitive-services/) \(current free limit is 30,000 images per month\).

| Property | Description |
| :--- | :--- |
| Subscription Key | Thunkable provides its own subscription key as DEFAULT. You can add your own if you expect your users to upload more than 1,000 images per month |
| Server Url | Distinct Url required for the Computer Vision API. Do not change the DEFAULT unless you are trying to access this component from China, in which case you need to provide a different server Url |

---

### Microsoft Image Recognizer

The Image Recognizer returns information about visual content found in an image and provides a set of tags and its best single line description.

![](/assets/image-recognizer1.jpg)

---

#### Select an image and let Microsoft's Image Recognizer detect its contents

![](/assets/image-recognizer-blocks.png)

---

#### Functionality

| Event | Description |
| :--- | :--- |
| Post Image \(path\) | Uploads the image \(specified by the path\) to the Microsoft Cognitive Service |
| Got Response \(description, descriptionScore, tags, responseCode, responseContent\) | If okay \('responseCode' = 200\), returns a one line 'description', a 'description score' \(confidence between 0 and 1\), and a set of image 'tags'. If not okay, will return an explanation for the error \('responseContent'\) |

---

### Microsoft Emotion Recognizer

The Image Recognizer returns information about visual content found in an image and provides a set of tags and its best single line description.

The Emotion API takes a facial expression in an image as an input, and returns the confidence across a set of emotions for each face in the image, as well as bounding box for the face, using the Face API. If a user has already called the Face API, they can submit the face rectangle as an optional input.

The emotions detected are anger, contempt, disgust, fear, happiness, neutral, sadness, and surprise. These emotions are understood to be cross-culturally and universally communicated with particular facial expressions

