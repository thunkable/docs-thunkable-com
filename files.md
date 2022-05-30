# Files

## Advanced Blocks

For each block in this drawer, you can right-click the block and select **Show advanced block** to see an expanded block with additional outputs. Both the simple and advanced blocks will be explained in this document.

![](<.gitbook/assets/image from photo library.png>)

## Image from Photo Library

This block will open the user's photo library and allow the user to select a photo. The photo can then be used in the app.

![](<.gitbook/assets/image (141).png>)

#### Advanced Block

![](<.gitbook/assets/image (132).png>)

| Output        | Data Type  | Function                                             |
| ------------- | ---------- | ---------------------------------------------------- |
| photo         | image      | if a photo was taken, returns the photo              |
| was cancelled | true/false | returns whether the user cancelled selecting a photo |
| error         | text       | if there was an error, returns the error             |

## File from Device

This block will open the user's file library and allow the user to select a file. The file can then be used in the app.

You can allow the user to upload any kind of file, or limit their selection by file type using the drop down menu.

{% hint style="info" %}
Your end users may experience lags or delays if the size of the file the try to upload is larger than 5MB
{% endhint %}

![](.gitbook/assets/Untitled.png)

#### Advanced Block

![](<.gitbook/assets/file exp.png>)

| Output        | Description                                                                                                                 | Data Type                                                                                           |
| ------------- | --------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| file          | Points to the file that has been uploaded                                                                                   | <p>Data type of the file that has been uploaded.<br>Can also return address of the file as text</p> |
| name          | Name of the uploaded file                                                                                                   | Text                                                                                                |
| mime type     | Describes the type of file in [MIME format](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics\_of\_HTTP/MIME\_types) | Text                                                                                                |
| size          | Returns size of uploaded file in bytes                                                                                      | Number                                                                                              |
| was cancelled | Indicates whether the end user cancelled selecting a file                                                                   | True/False                                                                                          |
| error         | If there is an error, returns the error. Else returns `null`                                                                | Text                                                                                                |

## Upload file to the cloud

Cloudinary Media DB is a service that allows you to store media files in the cloud. Thunkable's `upload file` block allows you to send media directly from your Thunkable app to a linked Cloudinary account.

{% hint style="warning" %}
If you use Thunkable's default Cloudinary DB, your files will be deleted after 90 days. Please connect your own Cloudinary DB to your Thunkable project to keep your media safe.
{% endhint %}

#### Advanced block

![](<.gitbook/assets/file (1).png>)

| Output | Data Type | Function                                 |
| ------ | --------- | ---------------------------------------- |
| URL    | text      | returns a URL for the uploaded file      |
| error  | text      | if there was an error, returns the error |

### Connecting Your Cloudinary DB to Your Thunkable project

No set up is required but creating your free Cloudinary account is highly recommended. Thunkable provides its own subscription key for your convenience but we strongly recommend creating your own account to ensure privacy for your uploaded media. We also have a current media size limit of 10MB per app and we may periodically clean out our default Cloudinary account

#### Create a [free Cloudinary](https://cloudinary.com/) account

![](<.gitbook/assets/image (222).png>)

#### Connect your Cloudinary cloud to Thunkable

To connect your Cloudinary cloud to Thunkable, simply retrieve the following fields from the Cloudinary dashboard: `Cloud name`, `API key`, and `API secret.` You can add these details to your app in the [Project Settings panel](project-settings.md#api-keys).

![](<.gitbook/assets/image (220).png>)

![](https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-LAn5scXl2uqUJUOqkJo-84897653%2Fuploads%2F7dZE50mYtYJaQjI0sdeZ%2FScreen%20Shot%202022-02-16%20at%2010.04.27%20AM.png?alt=media\&token=65c825f8-3aad-4b5e-b6be-8cc9bb552b1f)

## Resize Image

This block will take an image file and return it in the given dimensions, quality and format.

![](<.gitbook/assets/Screen Shot 2021-11-02 at 3.33.23 PM.png>)

#### Advanced Block

![](.gitbook/assets/advanced.png)

| Input            | Data Type        | Function                                                                 |
| ---------------- | ---------------- | ------------------------------------------------------------------------ |
| \[resize] image  | Any image file   | The image to be resized                                                  |
| Width            | Number           | Width in pixels to resize image file to                                  |
| Height           | Number           | Height in pixels to resize image file to                                 |
| Quality          | Number           | Quality of resulting image, as a percentage of quality of original image |
| using ... format | Select from menu | Select image type for resulting image                                    |

| Output        | Data Type | Function                                                    |
| ------------- | --------- | ----------------------------------------------------------- |
| Resized Image | Image     | The resized image in the selected format and quality level  |
| Error         | Text      | If there was an error, returns the error. Else returns NULL |

