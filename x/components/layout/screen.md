#### **Thunkable Cross-Platform **✕

# Screen ![](/assets/iOSviewIconScreen.png)

---

Screens are the main organizing containers of an app. They can themselves be organized by navigators or subdivided by row and column components.

* Spacing the elements in a Screen horizontally
* Spacing the elements in a Screen vertically
* Adding a background color or picture
* Enable scrolling
* Hide status bar

---

#### Spacing the elements horizontally



---

#### Spacing the elements vertically

---

#### Add a background color or picture

| Property | Description |
| :--- | :--- |
| Background Color | Default \(none\). Select any color using the color picker, RGBA or HEX value |
| Background Picture | You can upload a background image to your app or reference an image url e.g.`beaver-yellow.png` |
| Background Picture Resize Mode | Determines how to resize the image when the frame doesn't match the raw image dimensions;`cover`\(default\) Scale the image uniformly \(maintain the image's aspect ratio\) so that both dimensions \(width and height\) of the image will be equal to or larger than the corresponding dimension of the view \(minus padding\);`contain`Scale the image uniformly \(maintain the image's aspect ratio\) so that both dimensions \(width and height\) of the image will be equal to or less than the corresponding dimension of the view \(minus padding\);`stretch`Scale width and height independently, This may change the aspect ratio of the src;`repeat`Repeat the image to cover the frame of the view. The image will keep it's size and aspect ratio;`center`Centers the image in the frame |

---

#### Enable scrolling

| Property | Description |
| :--- | :--- |
| Scrollable | Default \(false\). Indicates whether the screen is scrollable. For scrollable to work, one or more of your components must have fixed heights that exceed the height of the screen |

---

#### Hide \(or show\) status bar

| Property | Description |
| :--- | :--- |
| Show Status Bar | Default \(true\). If set to 'false', hides the top status bar |



