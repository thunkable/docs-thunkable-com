---
description: >-
  With the camera component, you can open up your phone’s camera to take a
  picture.
---

# Camera

You can find the Camera blocks in the Camera drawer of blocks.

![](.gitbook/assets/camera-drawer.png)

## Video tutorial

You can view a video tutorial that demonstrates all of the Camera blocks here:

{% embed url="https://www.youtube.com/watch?v=Zi17wTeUKXs" %}

## Advanced Blocks

For each block in this drawer, you can right-click the block and select **Show advanced block** to see an expanded block with additional outputs. Both the simple and advanced blocks will be explained in this document.

![](<.gitbook/assets/image (147).png>)

## Use Photo from Camera

This block will open the camera and allow the user to take a photo. The photo can then be used in the app.

![](<.gitbook/assets/image (130).png>)

#### Advanced Block

![](<.gitbook/assets/image (172).png>)

| Output Name   | Data Type  | Function                                            |
| ------------- | ---------- | --------------------------------------------------- |
| photo         | image      | if a photo was taken, returns the photo             |
| was cancelled | true/false | returns whether the user cancelled taking the photo |
| error         | text       | if there was an error, returns the error            |

## Record Timed Video

Opens user camera, films from selected camera for chosen amount of time, returns video file.

![](.gitbook/assets/video.png)

#### Advanced Block

![](<.gitbook/assets/advanced timed.png>)

| Input               | Data Type        | Function                     |
| ------------------- | ---------------- | ---------------------------- |
| Number of Seconds   | Number           | Set how long to record for   |
| Using \[...] Camera | Select from menu | Select camera to record with |

| Output    | Data Type  | Function                                                   |
| --------- | ---------- | ---------------------------------------------------------- |
| videoFile | Video file | The recorded video footage                                 |
| Error     | Text       | If there is an error, returns the error. Else returns NULL |

#### Record Untimed Video

![](<.gitbook/assets/untimed video.png>)

#### Advanced Block

![](<.gitbook/assets/advacned untimed.png>)

| Input               | Data Type        | Function                       |
| ------------------- | ---------------- | ------------------------------ |
| Using \[...] Camera | Select from menu | Select a camera to record with |

| Output     | Data Type  | Function                                                   |
| ---------- | ---------- | ---------------------------------------------------------- |
| video file | Video File | Returns the recorded video footage                         |
| Error      | Text       | If there is an error, returns the error. Else returns NULL |

## Image Recognition

This block will generate a description of a given image. This block requires internet access.

This component is powered by [Microsoft Azure](https://blogs.microsoft.com/ai/azure-image-captioning/). You can get your own server URL and subscription key for Microsoft Azure [here](https://azure.microsoft.com/en-us/free/). You can add these details to your app in the [Project Settings panel](project-settings.md#api-keys), which you can access by clicking on your app icon.

![](<.gitbook/assets/image (176).png>)

#### Advanced Block

![](<.gitbook/assets/image (158).png>)



| Output           | Data Type              | Function                                                               |
| ---------------- | ---------------------- | ---------------------------------------------------------------------- |
| description      | text                   | description of the image                                               |
| tags             | list of text           | returns tags used to identify the image                                |
| confidence level | number between 0 and 1 | returns calculated confidence level that given description is accurate |
| error            | text                   | if there was an error, returns the error                               |

## Barcode/QR Code scanner

This block will scan a barcode or a QR code and return its value.

![](<.gitbook/assets/image (168).png>)

#### Advanced Block

![](<.gitbook/assets/image (134).png>)

| Output        | Data Type  | Function                                           |
| ------------- | ---------- | -------------------------------------------------- |
| value         | text       | value of scanned barcode/QR code                   |
| type          | text       | returns whether bar code or QR code was scanned    |
| was cancelled | true/false | returns whether the user cancelled scanning a code |
| error         | text       | if there was an error, returns the error           |

## Base64 Encoding

Provided an image, video or audio file, this block generates a Base64 encoded file. _(Alternate Description: This block receives an image, video or audio file, and returns it Base64 encoded.)_

Projects are restricted to 50MB total asset storage. Individual files using the Base64 block are subject to the same restrictions.  Based on our internal testing, maximum file size for Base64 encoding in web apps and web previewing is 10 MB, 40 MB in iOS and Android platforms.

{% hint style="info" %}
Keep in mind that while a file is encoding, your Thunkable app will not be able to navigate to other screens or engage in other functionality.  It is best to keep file sizes well below the maximum for best performance.
{% endhint %}

![](<.gitbook/assets/base64\_block (1).png>)

#### Advanced Block

![](<.gitbook/assets/base64\_advanced\_block (1).png>)

|            Input           | Data Type |         Function        |
| :------------------------: | :-------: | :---------------------: |
| Image, Video & Music Files |  Any File | The file to be encoded. |

|    Output    | Data Type |                      Function                     |
| :----------: | :-------: | :-----------------------------------------------: |
| Encoded File |    Text   |              The Base64 encoded file.             |
|     Error    |    Text   | Returns error if thrown.  Else returns undefined. |
