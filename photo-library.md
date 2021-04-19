---
description: Allows the user to select a photo to upload from their device to the app
---

# Photo Library

## Blocks

### Select Photo

![](.gitbook/assets/screen-shot-2021-04-19-at-10.28.09-am.png)

Opens the photo library and allows the user to select and upload a photo.

#### Outputs

| Name | Data Type | Data |
| :--- | :--- | :--- |
| Photo | Image | Image the user selected |
| DidUserCancel | True/False | If user cancelled action, returns `true`; else returns `false` |
| Error | Text | If error, returns error; else returns `null` |

