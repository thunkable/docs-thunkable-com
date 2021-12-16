---
description: The video component lets you play videos in your app.
---

# Video

## Video Overview

{% hint style="warning" %}
Please note that video files can be quite large and might exceed the 50 MB [size limit](projects/assets.md#app-size-limits-50-mb-per-app) for your project.&#x20;
{% endhint %}

The Video component lets you play videos in your app that are stored in the cloud or in your app. App users can easily pause, rewind or fast-forward the video with the built in player.



![](.gitbook/assets/screen-shot-2019-10-17-at-2.52.02-pm.png)

## Set Video

There are a few ways you can set a video source in your app:

1. **Upload a video to your app.** Be careful of the Thunkable 50 MB [app size limit](projects/assets.md#app-size-limits-50-mb-per-app)
2. **Provide a link to the video.** The link has to end in `.mp4`, `.mov`, …so videos uploaded to YouTube and other video sharing sites may not work.

Please note that the Video component is not recommended for streaming live video content.&#x20;

## Edit Video size

You can set how tall the Video is using the `height` property and set how wide it is using the `width` property.

**`Height`**

* **Fill container (default)-** The Video fills the entire screen vertically
* **Fit contents -** The Video’s height changes to fit the contents it contains
* **Relative size -** The Video fills the specified percentage of the screen
* **Absolute size -** Sizes the Video to a specified number of pixels

**`Width`**

* **Fill container (default) -** The Video fills the entire screen horizontally
* **Fit contents -** The Video’s width changes to fit the contents it contains
* **Relative size -** The Video fills the specified percentage of the screen
* **Absolute -** Sizes the Video to a specified number of pixels

## Set to Auto-Play

To set a video to play automatically, just toggle the Play property to `true`&#x20;

![](.gitbook/assets/screen-shot-2019-10-29-at-2.03.22-pm.png)

## Blocks

### Set Video

![](.gitbook/assets/screen-shot-2021-04-08-at-4.16.23-pm.png)

### Get Video

See what video is currently set as the Video component's source

![](.gitbook/assets/screen-shot-2021-04-08-at-4.17.34-pm.png)

