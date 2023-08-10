---
description: >-
  With the camera component, you can open up your phone’s camera to take a
  picture.
---

# Camera Blocks

You can find the Camera blocks in the Camera drawer of blocks.

![](../../.gitbook/assets/camera-drawer.png)

## Video tutorial

You can view a video tutorial that demonstrates all of the Camera blocks here:

{% embed url="https://www.youtube.com/watch?v=Zi17wTeUKXs" %}

## Advanced Blocks

For each block in this drawer, you can right-click the block and select **Show advanced block** to see an expanded block with additional outputs. Both the simple and advanced blocks will be explained in this document.

![](<../../.gitbook/assets/image (147).png>)

## Use Photo from Camera

This block will open the camera and allow the user to take a photo. The photo can then be used in the app.

![](<../../.gitbook/assets/image (130).png>)

#### Advanced Block

![](<../../.gitbook/assets/image (172).png>)

| Output Name   | Data Type  | Function                                            |
| ------------- | ---------- | --------------------------------------------------- |
| photo         | image      | if a photo was taken, returns the photo             |
| was cancelled | true/false | returns whether the user cancelled taking the photo |
| error         | text       | if there was an error, returns the error            |

## Record Timed Video

Opens user camera, films from selected camera for chosen amount of time, returns video file.

![](../../.gitbook/assets/video.png)

#### Advanced Block

![](<../../.gitbook/assets/advanced timed.png>)

<table><thead><tr><th width="253.47193347193343">Input</th><th width="199.93102570628662">Data Type</th><th>Function</th></tr></thead><tbody><tr><td>Number of Seconds</td><td>Number</td><td>Set how long to record for</td></tr><tr><td>Using [...] Camera</td><td>Select from menu</td><td>Select camera to record with</td></tr></tbody></table>

| Output    | Data Type  | Function                                                   |
| --------- | ---------- | ---------------------------------------------------------- |
| videoFile | Video file | The recorded video footage                                 |
| Error     | Text       | If there is an error, returns the error. Else returns NULL |

#### Record Untimed Video

![](<../../.gitbook/assets/untimed video.png>)

#### Advanced Block

![](<../../.gitbook/assets/advacned untimed.png>)

| Input               | Data Type        | Function                       |
| ------------------- | ---------------- | ------------------------------ |
| Using \[...] Camera | Select from menu | Select a camera to record with |

| Output     | Data Type  | Function                                                   |
| ---------- | ---------- | ---------------------------------------------------------- |
| video file | Video File | Returns the recorded video footage                         |
| Error      | Text       | If there is an error, returns the error. Else returns NULL |

## Image Recognition

{% embed url="https://youtu.be/tH4k9sXgzFY" %}

This block will generate a description of a given image. This block requires internet access.

This component is powered by [Microsoft Azure](https://blogs.microsoft.com/ai/azure-image-captioning/). You can get your own server URL and subscription key for Microsoft Azure [here](https://azure.microsoft.com/en-us/free/). You can add these details to your app in the [Project Settings panel](../../settings/project-settings/#api-keys), which you can access by clicking on your app icon.

![](<../../.gitbook/assets/image (176).png>)

#### Advanced Block

![](<../../.gitbook/assets/image (158).png>)

| Output           | Data Type              | Function                                                               |
| ---------------- | ---------------------- | ---------------------------------------------------------------------- |
| description      | text                   | description of the image                                               |
| tags             | list of text           | returns tags used to identify the image                                |
| confidence level | number between 0 and 1 | returns calculated confidence level that given description is accurate |
| error            | text                   | if there was an error, returns the error                               |

## Barcode/QR Code scanner

This block will scan a barcode or a QR code and return its value.

![](<../../.gitbook/assets/image (168).png>)

#### Advanced Block

![](<../../.gitbook/assets/image (134).png>)

| Output        | Data Type  | Function                                           |
| ------------- | ---------- | -------------------------------------------------- |
| value         | text       | value of scanned barcode/QR code                   |
| type          | text       | returns whether bar code or QR code was scanned    |
| was cancelled | true/false | returns whether the user cancelled scanning a code |
| error         | text       | if there was an error, returns the error           |
