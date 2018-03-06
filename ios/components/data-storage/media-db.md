#### **Thunkable for iOS **

# Media Database ![](/assets/cloudinary-icon.png) powered by Cloudinary

---

Media Database powered by Cloudinary is an easy-to-use service for uploading your images, audio files and videos in the cloud and returning a url where you can retrieve the image. 

IMPORTANT Thunkable provides its own API key by default for your convenience but if you may want to use your own Cloudinary key to ensure more privacy for your user's images or increase the 10MB image file size limit

---

#### Pick a photo from the library, upload it to the Cloudinary cloud and store its url in Firebase

#### ![](/assets/media-db-cloudinary-fig-1.png)

---

#### Set up

No set up is required. Thunkable provides its own subscription key as default. The current image size limit is 10MB.

You may want to create your own free account with [Cloudinary](http://cloudinary.com/) if you want to upload larger images or if you want to ensure better privacy for your user's images

`default`

| Property | Description |
| :--- | :--- |
| Cloud Name | Thunkable provides its own as `default`. Do not change unless you want to replace it with your own |
| API Key | Thunkable provides its own as `default`. Do not change unless you want to replace it with your own |
| API Secret | Thunkable provides its own as `default`. Do not change unless you want to replace it with your own |

![](/assets/cloudinary-account.png)

If you do create your own account, the API key corresponds to the 'subscription key', the API secret corresponds to the 'subscription secret' and the cloud name corresponds to the 'cloud name'

---

#### Upload media and return a URL

| Event | Description |
| :--- | :--- |
| Upload \(`media`\) | Uploads the image to the Cloudinary cloud and returns a `mediaURL` if successful |



