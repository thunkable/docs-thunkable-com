---
description: Create interactive gaming apps with sprites.
---

# Sprites

Sprites are images that can be placed on the canvas, where they can react to being touched or dragged across the screen, or collided with other sprites or the edge of the screen.

## Adding Sprites

To add a sprite to the canvas, drag and drop a "Sprite Type" onto the app builder. Click and drag to move sprites around the canvas to determine their location.

## Sprite Properties

**PictureList/Picture Selection:** To change the picture of your sprite, in the Sprite Type, add images to the Picture List. The in the individual sprites, you can select a picture from the list.

**Height:** Changes the height of the sprite

**Width:** Changes the width of the sprite

**Angle:** Change the angle of the sprite. We assume that 0º is to the right \(where the beaver is facing\).

**Bounce:** When a sprite hits a surface or another sprite, this is the percentage of the speed that sprite with bounce back with. So a bounce of 100 means that the sprite will bounce back at the same speed it had in its collision. A bounce of 200 will cause the sprite to bounce off with twice its speed.

**isDraggable:** When true, the player can drag the sprite

**PassesThrough:** When true, all sprites will pass under or above the sprite. When false, the sprites will collide using the physics engine. 

**IsStatic:** When a sprite is static, it acts like a wall. No forces can move it.

**FixedRotation:** When fixed rotation is false, the sprite can rotate in any direction. When fixed rotation is true, the sprite will remain at its current angle.

## Adding Different Types of Sprites

Groups of sprites that have the same behavior should belong to the same sprite type. In the example below, whenever the ball touches any of the wall sprites, the ball goes back to its starting location.

![](.gitbook/assets/screen-shot-2019-09-09-at-7.47.21-am.png)



