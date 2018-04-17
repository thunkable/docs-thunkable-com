#### **Thunkable Cross-Platform **✕

# Button ![](/assets/iOSviewIconButton.png)

---

Buttons are the most commonly used app components and can be styled to take the shape of anything from a blue oval to a hardworking beaver.

* [Style the Button](#style-the-button)
* [Edit size](#edit-size)
* [Start an event from a Button click](#start-an-event-from-a-button-click)

![](/assets/button-✕-fig-1.png)

---

### Style the Button

| Property | Description |
| :--- | :--- |
| Text | Default \(`Button`\); Optional text that appears on the button |
| Text Color | Default \(`#007AFF`\); Color of the optional text that appears on the button |
| Font Bold | Default \(`false`\); If `true`, text font will be **bold** |
| Font Italic | Default \(`false`\);  If `true`, text font will be _italic_ |
| Font Size | Default \(`16`\); Size of the optional text that appears on the button |
| Background Picture | Default \(`none`\); Optional background picture that appears in the button; You can upload a background image to your app or reference an image url e.g.`beaver-yellow.png` |
| Background Picture Resize Mode | Sets how an image is resized when the frame doesn't match the raw image dimensions; `cover` \(default\) Scale the image uniformly \(maintain the image's aspect ratio\) so that both dimensions \(width and height\) of the image will be equal to or larger than the corresponding dimension of the view \(minus padding\);`contain` Scale the image uniformly \(maintain the image's aspect ratio\) so that both dimensions \(width and height\) of the image will be equal to or less than the corresponding dimension of the view \(minus padding\); `stretch` Scale width and height independently, This may change the aspect ratio of the src; `repeat` Repeat the image to cover the frame of the view. The image will keep it's size and aspect ratio; `center` Centers the image in the fram |
| Background Color | Default \(`none`\); Sets the background color of the button |
| Border | Default \(`none`\); You can set the `width`, `color` and `style` of the button border |
| Corner Radius | Default \(`not rounded`\); You can round up the button corners by increasing this value |
| Raised | Default \(`false`\); If `true`, button will cast a shadow |

---

### Edit size

| Property | Description |
| :--- | :--- |
| Height | Default \(`Fit contents`\); Four options: 1\) `Fit contents` which auto-sizes to the content size or 2\) `Fill container` which auto-sizes to the container 3\) `Relative size` in percent of Screen, 4\) `Absolute size` in pixels |
| Width | Default \(`Fit contents`\); Four options: 1\) `Fit contents` which auto-sizes to the content size or 2\) `Fill container` which auto-sizes to the container 3\) `Relative size` in percent of Screen, 4\) `Absolute size` in pixels |

---

### Start an event from a Button click

![](/assets/button-✕-fig-2.png)

| Event | Description |
| :--- | :--- |
| Click | User tapped and releases the button |
| Long Click | User holds the button down |
| Touch Up | User releases the button |
| Touch Down | User gently presses the button |
| Disabled | If `true`, button will be disable |



