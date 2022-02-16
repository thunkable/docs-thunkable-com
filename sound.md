---
description: The sound component plays a designated sound.
---

# Sound

## Advanced Blocks

You can right-click any block to show an advanced version of the block.

These blocks will return an `error` output block. If there is en error with executing the block, the error block will return an error message. If not, the error block will return a null value.

![](.gitbook/assets/playadv.png)

## Play

Play a selected sound. This can be an audio file that has been uploaded to your project, or a URL that streams audio.

![](<.gitbook/assets/image (133).png>)

## Pause

Pause a selected audio file that is currently playing.

![](<.gitbook/assets/image (162).png>)

## Resume

Resume a selected audio file that has been previously paused.

![](<.gitbook/assets/image (169).png>)

## Stop

Stop a selected audio file that is currently playing. A sound that has been 'stopped' cannot be resumed using the [resume](sound.md#resume) block.

![](<.gitbook/assets/image (143).png>)

## Is Sound Paused?

![](<.gitbook/assets/image (140).png>)

Returns **true** if named sound file has been partially played, then paused. \
Returns **false** otherwise.

## Sound File from Recording

Records for the specified amount of seconds, then returns the recorded audio.

![](<.gitbook/assets/image (175).png>)

## Untimed Recording

The **start recording** block begins a recording.

![](<.gitbook/assets/image (174).png>)

The **sound file from stopped recording** block will stop the recording initiated by the **start recording** block, and return the recorded sound file.

![](<.gitbook/assets/image (142).png>)
