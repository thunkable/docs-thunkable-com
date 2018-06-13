# Screen

## Screen starts and opens

| Event | Description |
| --- | --- | --- |
| Starts | Triggers an event / set of events when the Screen is first opened |
| Opens | Triggers an event / set of events whenever the Screen is opened |

## Space elements horizontally

The `Justification` property allows you to space elements in a Screen horizontally

![](../../../../.gitbook/assets/thunkable-documentation-exhibits-64%20%281%29.png)

## Space elements vertically

The `Alignment` property allows you to space elements in a Screen vertically

![](../../../../.gitbook/assets/spacing-fig-2.png)

## Add a background color or picture

| Property | Description |
| :--- | :--- |
| Background Color | Default \(`none`\). Select any color using the color picker, RGBA or HEX value |
| Background Picture | You can upload a background image to your app or reference an image url e.g.`beaver-yellow.png` |
| Background Picture Resize Mode | Determines how to resize the image when the frame doesn't match the raw image dimensions;`cover`\(default\) Scale the image uniformly \(maintain the image's aspect ratio\) so that both dimensions \(width and height\) of the image will be equal to or larger than the corresponding dimension of the view \(minus padding\);`contain`Scale the image uniformly \(maintain the image's aspect ratio\) so that both dimensions \(width and height\) of the image will be equal to or less than the corresponding dimension of the view \(minus padding\);`stretch`Scale width and height independently, This may change the aspect ratio of the src;`repeat`Repeat the image to cover the frame of the view. The image will keep it's size and aspect ratio;`center`Centers the image in the frame |

## Enable scrolling

| Property | Description |
| :--- | :--- |
| Scrollable | Default \(`false`\). Indicates whether the screen is scrollable. For scrollable to work, one or more of your components must have fixed heights that exceed the height of the screen |

## Hide \(or show\) status bar

| Property | Description |
| :--- | :--- |
| Show Status Bar | Default \(`true`\). If set to `false`, hides the top status bar |

## Set Orientation

Coming Soon.

