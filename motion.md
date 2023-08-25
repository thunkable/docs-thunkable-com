---
description: Program a sprite's speed and location
---

# Motion

## Speed&#x20;

### Set Speed To&#x20;

![](.gitbook/assets/mov\_set\_speed\_to.png)

Set the X or Y value for the sprite's speed to a particular value.

### Change Speed By&#x20;

![](.gitbook/assets/mov\_set\_speed\_to2.png)

Change the X or Y value for the sprite's speed by a specific amount.

### Get Speed&#x20;

![](.gitbook/assets/mov\_get\_speed.png)

Get the X or Y value for the sprite's speed.

###

### Set Velocity

![](.gitbook/assets/mov\_set\_speed.png)

Set or change the sprite's velocity, by a given amount, in the pointing or moving direction.

## Position&#x20;

### Move Sprite To

![](.gitbook/assets/mov\_move\_to.png)

Move the sprite to the x and y location specified in the block

### Set Sprite Position

![](.gitbook/assets/mov\_set\_coord.png)

Set the sprite's X, Y, Z or Angle value to a specific position.

Change the sprites X, Y, Z or Angle value by a given amount.

**Note**: Sprite angle is measured in degrees, so should be a value between 0 and 360.&#x20;

### Get Sprite Position

![](.gitbook/assets/mov\_get\_coord.png)

Get the sprite's current X, Y, Z or Angle value.

**Note**: Sprite angle is measured in degrees, so should be a value between 0 and 360

## Pointer

### Get Pointer Value

![](.gitbook/assets/mov\_pointer.png)

![](.gitbook/assets/mov\_pointer2.png)

Get the X, Y, or Angle of the where the user tapped on the canvas

## Behavior

On the canvas, it's possible to make a sprite either draggable or to have it fixed in position.

Similarly, it's possible for other sprites to pass through a sprite, or it can be made impassable.&#x20;

Finally, if a sprite is moving, it's possible to programatically cause it to stop moving.&#x20;

### Set Draggable or Passable&#x20;

![](.gitbook/assets/mov\_set\_draggable.png)

Set the draggability or passability of the sprit

### Get Draggable or Passable

![](.gitbook/assets/mov\_get\_draggable.png)

Get draggability of the sprite

### Stop All Sprites

![](.gitbook/assets/mov\_stop\_sprites.png)

Stop all sprites that are moving.

## Examples

### Move Sprite to Pointer

When the user clicks on the canvas these blocks will move the `Sprite1` to the location that was touched.&#x20;

![](.gitbook/assets/move\_sprite\_to.png)
