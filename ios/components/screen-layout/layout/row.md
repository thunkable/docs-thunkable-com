#### **Thunkable for iOS **

# Row \(aka Horizontal Arrangement\) ![](/assets/iOSviewIconRow.png)

---

Row components are containers that can arrange elements horizontally within a screen. They can also be used to provide a margin on the top, bottom or in between vertical elements in your app![](/assets/row-ios-1.png)

* [Set the size of the container](#set-size-of-the-container)
* [Arrange the elements horizontally](#arrange-the-elements-horizontally-justification-)
* [Align the elements vertically](#align-the-elements-vertically-alignment)
* [Add a background color or picture](#add-a-background-color-or-picture)

---

#### Set size of the row container

| Property | Description |
| :--- | :--- |
| Height | `Fit contents` Container is just as large as the contents; `Fill container` Container is as large as it can be on the Screen; `Relative size` Size of the container in percent of the Screen; `Absolute size` Size of the container in pixels |
| Width | `Fit contents` Container is just as large as the contents; `Fill container` Container is as large as it can be on the Screen; `Relative size` Size of the container in percent of the Screen; `Absolute size` Size of the container in pixels |

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
| Background Picture Resize Mode | Determines how to resize the image when the frame doesn't match the raw image dimensions;`cover`\(default\) Scale the image uniformly \(maintain the image's aspect ratio\) so that both dimensions \(width and height\) of the image will be equal to or larger than the corresponding dimension of the view \(minus padding\);`contain`Scale the image uniformly \(maintain the image's aspect ratio\) so that both dimensions \(width and height\) of the image will be equal to or less than the corresponding dimension of the view \(minus padding\);`stretch`Scale width and height independently, This may change the aspect ratio of the src;`repeat`Repeat the image to cover the frame of the view. The image will keep it's size and aspect ratio;`center`Centers the image in the frame |



