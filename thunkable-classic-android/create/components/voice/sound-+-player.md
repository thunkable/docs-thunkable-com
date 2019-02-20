# Sound + Player

#### ![](../../../../.gitbook/assets/sound-icon.png) + ![](../../../../.gitbook/assets/player-icon.png)

The Sound component is recommended for short sound files like sound effects while the Player is recommended for longer sound files like songs

|  | ![](../../../../.gitbook/assets/sound-icon.png) | ![](../../../../.gitbook/assets/player-icon.png) |
| :--- | :--- | :--- |
|  | Sound | Player |
| Common use case | Short sound files like sound effects | Long sound files like songs |

### Sound ![](../../../../.gitbook/assets/sound-icon.png)

#### Functionality

| Property / Event | Description |
| :--- | :--- |
| Source | The name of the sound file. Only certain formats are supported. See [https://developer.android.com/guide/appendix/media-formats.html](sound-+-player.md) |
| Play | Plays the sound |
| Pause | Pauses the sound |
| Resumes | Resumes playing the sound after a pause |
| Stop | Stops playing the sound |
| Vibrate \(milliseconds\) | Vibrates for the specified number of milliseconds e.g. 1000 is 1 second |
| Minimum Interval \(milliseconds\) | The minimum interval between sounds. If you play a sound, all further play events will be ignored until the interval has passed |

### Player ![](../../../../.gitbook/assets/player-icon.png)

#### Functionality

| Property / Event | Description |
| :--- | :--- |
| Source | The name of the sound file. Only certain formats are supported. See [https://developer.android.com/guide/appendix/media-formats.html](sound-+-player.md) |
| Volume | Sets the volume between 0 and 100 |
| Start | Plays the sound |
| Pause | Pauses the sound |
| Stop | Stops playing the sound |
| Loop | If checked, the sound will play on a loop |
| Vibrate \(milliseconds\) | Vibrates for the specified number of milliseconds e.g. 1000 is 1 second |
| Plays Only in Foreground | If checked, the player will pause playing when leaving the current screen. If unchecked \(default\), the player will continue playing even if the user leaves the current screen |
| IsPlaying | Indicates whether the sound is playing |
| Completed | Indicates that the sound has reached the end |
| Other Player Started | This event is signaled when another player has started \(and the current player is playing or paused but not stopped\) |

