---
description: Create interactive gaming apps with sprites.
---

# Sprites

## Sprite Overview

Sprites are images that can be placed on the Stage in the Canvas. \
They can react to being touched or dragged across the screen, or colliding with other sprites or the edge of the screen.

## Sprites vs Sprite Types

A **Sprite Type** is a **category** of Sprites that you can add to your app. For example, in a video game you might have a Main Character Sprite Type and Obstacle Sprite Types.&#x20;

A **Sprite** is a **single instance** of a Sprite Type. In the video game example, you could have a single Obstacle Sprite Type, but multiple Obstacle Sprites in your app. They would be multiple Sprites of the same Sprite Type.

### Example: Different Types of Sprites

Groups of sprites that have the same behavior should belong to the same sprite type. In the example below, WallType is a Sprite Type, and there are multiple Sprites of this type in the app (ie. the walls).&#x20;

Whenever the ball touches any of the WallType Sprites, the ball goes back to its starting location.

![](.gitbook/assets/screen-shot-2019-09-09-at-7.47.21-am.png)

## Sprite Types

### Adding Sprites Types to your app

To add a Sprite Type to your app, click on the Stage of your Canvas.&#x20;

This will automatically bring you to the Canvas tab.&#x20;

Underneath your component tree, where you would see a component menu in the Design tab, you will see your Sprite Type menu.

![](<.gitbook/assets/canvas tab  component UI .png>)

You can click on 'Add Sprite Type' to add a new Sprite Type to your app.

### Sprite Type Properties

| Name           | Description                                                                                                                                                                                                                                                                                        | Data Type   |
| -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- |
| Picture List   | Images that can be shown with the given Sprite Type                                                                                                                                                                                                                                                | Image files |
| Height         | Height of the sprite picture.                                                                                                                                                                                                                                                                      | Number      |
| Width          | Width of the sprite picture.                                                                                                                                                                                                                                                                       | Number      |
| Angle          | Change the angle of the sprite. The angle is measured in a clockwise direction and is measured in degrees, eg. setting the angle to 30 will rotate your sprite 30 degrees clockwise                                                                                                                | Number      |
| Z              | Control the sprite's depth on the screen and the overlap of sprites. Sprites with a higher value for Z will overlap the sprites with a lower Z value.                                                                                                                                              | Number      |
| Opacity        | Change the opacity of the Sprite, where 100% is max opacity and 0 is max transparency                                                                                                                                                                                                              | Number      |
| Bounce         | When a sprite hits a surface or another sprite, this is the percentage of the speed that sprite with bounce back with. A bounce of 100 means that the sprite will bounce back at the same speed it had in its collision. A bounce of 200 will cause the sprite to bounce off with twice its speed. | Number      |
| Is Draggable   | Toggle whether the player can drag the Sprite Type                                                                                                                                                                                                                                                 | True/False  |
| Passes Through | Toggle whether Sprite Type passes through other Sprites                                                                                                                                                                                                                                            | True/False  |
| Is Static      | Toggle whether Sprite Type's location is fixed                                                                                                                                                                                                                                                     | True/False  |
| Ignore Gravity | Toggle whether of not the sprite is affected by the Stage's gravity                                                                                                                                                                                                                                | True/False  |
| Fixed Rotation | Toggle whether Sprite Type's Angle can be changed                                                                                                                                                                                                                                                  | True/False  |
| Drawing        | Toggle whether Sprite Type draws a line as it moves                                                                                                                                                                                                                                                | True/False  |
| Drawing Color  | Toggle color of line drawn when Drawing is true                                                                                                                                                                                                                                                    | Color       |
| Drawing Width  | Width of line drawn when Drawing is true                                                                                                                                                                                                                                                           | Width       |

### See Also

You can read more about the Stage's gravity properties [here](canvas.md#gravity).

## Sprites

### Adding Sprites to your app

Click on the Canvas to see the menu of Canvas components you can add to your project.

You will see this menu under the component tree, where the Component menu is usually shown in the Designer.

Select a Sprite Type and drag it onto your Canvas to create an instance of a Sprite Type. This is a single **Sprite**.

In the below GIF, there is a canvas with a Sprite, called Sprite1. There is also a Sprite Type in the Sprite Type menu called Sprite\_Type1. When a Sprite is dragged from Sprite\_Type1 and dropped onto the Canvas, we see a new Sprite, called Sprite\_2.

![](.gitbook/assets/newsprite.gif)

### Sprite Properties

| Name              | Description                                                                                                                                                                                                                                                                                        | Data Type        |
| ----------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- |
| Picture Selection | Select an image from the Picture List defined in the Sprite Type to display on the SpriteImage files                                                                                                                                                                                               | Select from menu |
| X                 | Location of the top-left pixel of the Sprite on the X-axis of the stage, where the left-hand side is 0                                                                                                                                                                                             | Number           |
| Y                 | Location of the top-left pixel of the Sprite on the Y-axis of the stage, where the top is 0                                                                                                                                                                                                        | Number           |
| Z                 | Where the Sprite is in the depth of the Canvas. A Sprite with a higher Z-value will appear in front of a Sprite with a lower Z-value.                                                                                                                                                              | Number           |
| Height            | Height of the sprite picture.                                                                                                                                                                                                                                                                      | Number           |
| Width             | Width of the sprite picture.                                                                                                                                                                                                                                                                       | Number           |
| Angle             | Change the angle of the sprite. The angle is measured in a clockwise direction and is measured in degrees, eg. setting angle to 30 will rotate your sprite 30 degrees clockwise                                                                                                                    | Number           |
| Opacity           | Change the opacity of the Sprite, where 100% is max opacity and 0 is max transparency                                                                                                                                                                                                              | Number           |
| Bounce            | When a sprite hits a surface or another sprite, this is the percentage of the speed that sprite with bounce back with. A bounce of 100 means that the sprite will bounce back at the same speed it had in its collision. A bounce of 200 will cause the sprite to bounce off with twice its speed. | Number           |
| Stage Selection   | The stage the sprite is part of.                                                                                                                                                                                                                                                                   | Select from list |
| Is Draggable      | Toggle whether the player can drag the Sprite Type                                                                                                                                                                                                                                                 | True/False       |
| Passes Through    | Toggle whether Sprite Type passes through other Sprites                                                                                                                                                                                                                                            | True/False       |
| Is Static         | Toggle whether Sprite Type's location is fixed                                                                                                                                                                                                                                                     | True/False       |
| Ignore Gravity    | Toggle whether of not the sprite is affected by the Stage's gravity                                                                                                                                                                                                                                | True/False       |
| Fixed Rotation    | Toggle whether Sprite Type's Angle can be changed                                                                                                                                                                                                                                                  | True/False       |
| Drawing           | Toggle whether Sprite Type draws a line as it moves                                                                                                                                                                                                                                                | True/False       |
| Drawing Color     | Toggle color of line drawn when Drawing is true                                                                                                                                                                                                                                                    | Color            |
| Drawing Width     | Width of line drawn when Drawing is true                                                                                                                                                                                                                                                           | Number           |

## Demo

### Demo

In the GIF below, we see that when one Sprite (the Thunkable Beaver) collides with another Sprite (the tree trunk), the appearance of the Tree Sprite changes.

This demonstrates the following:

Picture List: we see the image displayed by the Tree sprite changing

Bounce: We see the Beaver sprite bounce off of the Tree sprite. As it bounces, it has a speed of 50% of its original speed

Passes Through: the Beaver Sprite does not pass through the Tree sprite until it has collided with the Tree sprite 3 times

Z: The Beaver sprite has a higher Z-value than the Tree sprite, so the beaver passes in front of the tree



![The Picture List of Sprite\_Type2](.gitbook/assets/spritetype2.png)

![Demonstration of cycling through Image List](.gitbook/assets/imagelist.gif)

## Blocks

Check out the [Gaming Blocks](gaming-blocks.md) to see the blocks available to use with Sprites in your project.
