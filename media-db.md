# Media DB by Cloudinary

## Media DB Overview

{% hint style="info" %}
No set up is required but creating your free Cloudinary account is highly recommended
{% endhint %}

## Getting Started

No set up is required but creating your free Cloudinary account is highly recommended. Thunkable provides its own subscription key for your convenience but we strongly recommend creating your own account to ensure privacy for your uploaded media. We also have a current media size limit of 10MB per app and we may periodically clean out our default Cloudinary account

### Create a [free Cloudinary](https://cloudinary.com/) account

![](.gitbook/assets/media-db-cloudinary-fig-1.png)

### Connect your Cloudinary cloud to Thunkable

To connect your Cloudinary cloud to Thunkable, simply retrieve the following fields from the Cloudinary dashboard: `Cloud name`, `API key`, and `API secret.` You can add these details to your app in the [Project Settings panel](projects/settings.md#api-keys), which you can access by clicking on your app icon.

![](.gitbook/assets/media-db-cloudinary-fig-4.png)

![](.gitbook/assets/media-db-cloudinary-fig-2.png)

## Upload Media

You can upload any media file from your phone to your Cloudinary account with the mediaDB component. In this case we do some additional checking with the [if do else](control.md#if-this-do-that) block to make sure that the user has attached an image and that neither the photo library nor the mediaDB components encounter an error. 

![](.gitbook/assets/mediadb_upload.png)

<table>
  <thead>
    <tr>
      <th style="text-align:left">Event</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Upload (<code>media</code>)</td>
      <td style="text-align:left">
        <p>Uploads the image to the Cloudinary cloud. Returns a <code>mediaURL</code> if
          successful.</p>
        <p>Else returns <code>error</code>.</p>
      </td>
    </tr>
  </tbody>
</table>

