---
description: The sound component plays a designated sound.
---

# Sound

## Set Source

There are a few ways you can set a sound source in your app:

1. **Upload a sound to your app. **Be careful of the Thunkable 50 MB [app size limit](projects/assets.md#app-size-limits-50-mb-per-app)
2. **Provide a link to the sound. **The link has to end in `.mp3`, `.wav`, etc

## Volume

You can set a volume for the Sound component between 0 and 100.

## Blocks

### Events

#### On Source Loaded

This block will be triggered when the source of a Sound component is loaded. It is recommended to use this block if changing a Sound component's source during app runtime.

![](.gitbook/assets/sourceloaded.png)

If a given audio is already the source of a Sound component, and you use a block to set the same audio as the source of the Sound component, this block will not be triggered. We recommend using an [if statement](control.md#if-this-do-that) to say that if the audio is already the source of the Sound component, execute the action you would take when the source is loaded.&#x20;

In the following screenshot, we want this audio to play when the Button is pressed. If this audio is already the source for the Sound component, we play the sound. If not, we set the audio to be the Sound's source. Once the source is loaded, we play the audio.

![](.gitbook/assets/screen-shot-2021-05-11-at-2.38.35-pm.png)

#### On Error

This block will be triggered if there is an error with the Sound component.

![](.gitbook/assets/error.png)

### Functions

Play, Pause, Resume or Stop a sound.

![](.gitbook/assets/functions.png)

A sound can only be resumed if it has been paused.

### Set/Get Source

Set the Sound's source using the drop-down menu or by using a [Text](text.md) block to specify a filename or URL.

Get the name of the Sound source.

![](<.gitbook/assets/source (1).png>)

### Set/Get Volume

Set Sound volume to value between 0 and 100.

Get Sound volume.

![](.gitbook/assets/screen-shot-2021-04-19-at-11.08.59-am.png)

