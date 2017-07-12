#### **Thunkable for Android **❤

# Image Sprite ![](/assets/image-sprite-icon.png) + Ball ![](/assets/ball-icon.png)

---

A 'sprite' is an Image or a Ball that can be placed on a Canvas, where it can react to touches and drags, interact with other sprites  and the edge of the Canvas, and move according to its property values.

The difference between an Image Sprite and a Ball is that an Image Sprite can get its appearance from an image file, while a Ball's appearance can only be changed by varying its PaintColor and Radius properties.

---

#### Styling the Ball

| Property | Description |
| :--- | :--- |
| Paint Color | The color of the ball. Default \(Black\). You can choose any color on the Designer palette or customize the color to any RGB value in the Blocks editor |
| Radius | The radius of the ball |
| Visible | If checked, the ball will be visible on the screen |

---

#### Styling the Image Sprite

| Property | Description |
| :--- | :--- |
| Height | Height in pixels, percent, 'Automatic' or 'Fill' |
| Width | Width in pixels, percent, 'Automatic' or 'Fill' |
| Picture | You can upload an image to your app for the sprite |
| Rotates | If checked, the sprite image rotates to match the sprite's heading. If unchecked, the sprite image does not rotate when the sprite changes heading. The sprite rotates around its center point. |
| Visible | If checked, the image sprite will be visible on the scree |

---

#### Setting the initial position and speed of the Ball or Image Sprite

| Property | Description |
| :--- | :--- |
| Heading | Returns the sprite's heading in degrees above the positive x-axis. Zero degrees is toward the right of the screen; 90 degrees is toward the top of the screen. |
| X | In pixels from left. The horizontal coordinate of the left edge of the sprite, increasing as the sprite moves to the right |
| Y | In pixels from top. The vertical coordinate of the top edge of the sprite, increasing as the sprite moves down |
| Z | Integers with higher numbers layered on top. How the sprite should be layered relative to other sprites, with higher-numbered layers in front of lower-numbered layers |
| Speed \(pixels / interval\) | In pixels per interval. The speed at which the sprite moves in pixels per interval |
| Interval \(milliseconds\) | The interval in milliseconds at which the sprite's position is updated. For example, if the interval is 50 and the speed is 10, then the sprite will move 10 pixels every 50 milliseconds |
| Enabled | If checked, sprite will move when its speed is non-zero  |



