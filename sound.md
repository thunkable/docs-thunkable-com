---
description: The sound component plays a designated sound.
---

# Sound

## Play

Play a selected sound. This can be an audio file that has been uploaded to your project, or a URL that streams audio.

![](.gitbook/assets/image%20%28133%29.png)

## Pause

Pause a selected audio file that is currently playing.

![](.gitbook/assets/image%20%28162%29.png)

## Resume

Resume a selected audio file that has been previously paused.

![](.gitbook/assets/image%20%28169%29.png)

## Stop

Stop a selected audio file that is currently playing. A sound that has been 'stopped' cannot be resumed using the [resume](sound.md#resume) block.

![](.gitbook/assets/image%20%28143%29.png)

## Is Sound Paused?

![](.gitbook/assets/image%20%28140%29.png)

Returns **true** if named sound file has been partially played, then paused.   
Returns **false** otherwise.

## Sound File from Recording

Records for the specified amount of seconds, then returns the recorded audio.

![](.gitbook/assets/image%20%28175%29.png)

## Untimed Recording

The **start recording** block begins a recording.

![](.gitbook/assets/image%20%28174%29.png)

The **sound file from stopped recording** block will stop the recording initiated by the **start recording** block, and return the recorded sound file.

![](.gitbook/assets/image%20%28142%29.png)

