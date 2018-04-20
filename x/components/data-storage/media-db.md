#### T**hunkable Cross-Platform **✕

# Media Database ![](/assets/cloudinary-icon.png) powered by Cloudinary

---

Media Database powered by Cloudinary stores your favorite images, audio files and videos into the cloud and returns a url for where it can be retrieved later

`IMPORTANT No set up is required but creating your free Cloudinary account is highly recommended`

* [Set up](#set-up)
* [Upload media](#upload-media)

---

### Set up

No set up is required but creating your free Cloudinary account is highly recommended. Thunkable provides its own subscription key for your convenience but we strongly recommend creating your own account to ensure privacy for your uploaded media. We also have a current media size limit of 10MB per app and we may periodically clean out our default Cloudinary account

#### Step ① / Create a [free Cloudinary](https://cloudinary.com/) account

#### ![](/assets/media-db-cloudinary-✕-fig-1.png)

#### Step ② / Connect your Cloudinary cloud to Thunkable

To connect your Cloudinary cloud to Thunkable, simply retrieve the following fields from the Cloudinary dashboard: `Cloud name`, `API key`, and `API secret`

![](/assets/media-db-cloudinary-✕-fig-4.png)

![](/assets/media-db-cloudinary-✕-fig-2.png)

---

### Upload media

#### ![](/assets/media-db-cloudinary-✕-fig-3.png)

| Event | Description |
| :--- | :--- |
| Upload \(`media`\) | Uploads the image to the Cloudinary cloud and returns a `mediaURL` if successful |



