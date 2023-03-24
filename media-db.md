# Media DB by Cloudinary

{% hint style="info" %}
No set up is required but creating your free Cloudinary account is highly recommended
{% endhint %}

* [Set up](media-db.md#set-up)
* [Upload media](media-db.md#upload-media)

## Set up

No set up is required but creating your free Cloudinary account is highly recommended. Thunkable provides its own subscription key for your convenience but we strongly recommend creating your own account to ensure privacy for your uploaded media. We also have a current media size limit of 10MB per app and we may periodically clean out our default Cloudinary account

### Create a [free Cloudinary](https://cloudinary.com/) account

![](.gitbook/assets/media-db-cloudinary-fig-1.png)

### Connect your Cloudinary cloud to Thunkable

To connect your Cloudinary cloud to Thunkable, simply retrieve the following fields from the Cloudinary dashboard: `Cloud name`, `API key`, and `API secret`

![](.gitbook/assets/media-db-cloudinary-fig-4.png)

![](.gitbook/assets/media-db-cloudinary-fig-2.png)

## Upload media

![](.gitbook/assets/media-db-cloudinary-fig-3.png)

| Event | Description |
| :--- | :--- |
| Upload \(`media`\) | Uploads the image to the Cloudinary cloud and returns a `mediaURL` if successful |

