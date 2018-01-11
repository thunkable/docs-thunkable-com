#### **Thunkable for iOS **

# Screen ![](/assets/screen-icon.png)

---

Screens are the main organizing containers of an app. They can themselves be organized by [navigators](/ios/components/screen-layout/navigators/README.md) or subdivided by row and column containers.

* [Arrange the elements horizontally](#arrange-the-elements-horizontally-justification-)
* [Align the elements vertically](#align-the-elements-vertically-alignment)
* [Add a background color or picture](#add-a-background-color-or-picture)
* [Enable scrolling](#enable-scrolling)
* [Hide \(or show\) status bar](#hide-status-bar)

---

#### Arrange the elements horizontally \(Justification\)![](/assets/row-ios-2.png)

---

#### Align the elements vertically \(Alignment\)

![](/assets/row-ios-3.png)

---

#### Add a background color or picture

| Property | Description |
| :--- | :--- |
| Background Color | Default \(none\). Select any color using the color picker, RGBA or HEX value |
| Background Picture | You can upload a background image to your app or reference an image url e.g.`beaver-yellow.png` |
| Background Picture Resize Mode | Determines how to resize the image when the frame doesn't match the raw image dimensions; `cover` \(default\) Scale the image uniformly \(maintain the image's aspect ratio\) so that both dimensions \(width and height\) of the image will be equal to or larger than the corresponding dimension of the view \(minus padding\);`contain` Scale the image uniformly \(maintain the image's aspect ratio\) so that both dimensions \(width and height\) of the image will be equal to or less than the corresponding dimension of the view \(minus padding\); `stretch` Scale width and height independently, This may change the aspect ratio of the src; `repeat` Repeat the image to cover the frame of the view. The image will keep it's size and aspect ratio; `center` Centers the image in the frame |

---

#### Enable scrolling

| Property | Description |
| :--- | :--- |
| Scrollable | Default \(false\). Indicates whether the screen is scrollable |

---

#### Hide \(or show\) status bar

| Property | Description |
| :--- | :--- |
| Show Status Bar | Default \(true\). If set to 'false', hides the top status bar |



