---
description: >-
  With the camera component, you can open up your phone’s camera to take a
  picture.
---

# Camera

## Video Tutorial

{% embed url="https://youtu.be/3UWbWPlkjw8" %}



## Overview

* [Take Photo](camera.md#take-photo)

![](.gitbook/assets/camera-fig-1%20%281%29.png)

## Take Photo

The camera block has three outputs:

 **i\) Photo:** This saves the photo taken by the user.

**ii\) DidUserCancel:** This is either true or false depending on whether the user cancelled taking the picture

**iii\) Error:** Indicates if there was an error when the photo was taken

![These blocks say that when Button1 is clicked, open the camera. Then set the photo taken to be displayed in an Image component. ](.gitbook/assets/camera.png)

![These blocks say that when Button1 is clicked, open the camera. If the user does not cancel the action, one of two things will happen: if there is an error, display the error message on a Label. If there is not an error, set the photo taken to be displayed in an Image component. ](.gitbook/assets/cameraqualified.png)

