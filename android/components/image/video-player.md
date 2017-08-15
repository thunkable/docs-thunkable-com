#### **Thunkable for Android **❤

# Video Player ![](/assets/video-player-icon.png)

---

The Video Player plays video in 3GPP \(.3gp\) or MPEG-4 \(.mp4\) formats that under 1 MB. If your media files are too large, you may get errors when packaging or installing your application, in which case you should reduce the number of media files or their sizes

If you want to avoid the video format size limit, you can also set the media source to a URL that points to a streaming video, but the URL must point to the video file itself, not to a program that plays the video.

---

#### Appearance

| Property | Description |
| :--- | :--- |
| Height | Height in pixels, percent, 'Automatic' or 'Fill' |
| Width | Width in pixels, percent, 'Automatic' or 'Fill' |
| Source | The path to the video, either the name of the video if uploaded \(e.g. hello.mp4\) or a URL that links to the video file itself |
| Full Screen | If checked, the video will play in full screen |
| Volume | Sets the volume to a number between 0 and 100. Values less than 0 will be treated as 0, and values greater than 100 will be treated as 100 |
| Visible | If checked, the button will be visible on the screen |

---

#### Functionality

| Event | Description |
| :--- | :--- |
| Start | Starts playback of the video |
| Pause | Pauses playback of the video. Playback can be resumed at the same location by calling the Start event |
| Seek To \(milliseconds\) | Seeks to the requested time \(specified in milliseconds\) in the video. Note that if the video is paused, the frame shown will not be updated by the seek |
| Completed | Indicates that the video has reached the end |
| Get Duration | Returns duration of the video in milliseconds |



