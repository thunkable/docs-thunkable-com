# Slider

## Slider Overview

The Slider is a great UI element to enable users easily select a value from a fixed range of values.

![](.gitbook/assets/slider-fig-2.png)

##

## Getting Started

To set up a slider, you'll have to first define the `minimum` and `maximum` values, the initial `value` and the incremental `steps` of the slider

We recommend using a Label with the Slider so that users can get immediate feedback on the value being set.

![](.gitbook/assets/slider\_change.png)

| Property      | Description                                               |
| ------------- | --------------------------------------------------------- |
| Minimum Value | Default (`0`); Minimum and leftmost value of the Slider   |
| Maximum Value | Default (`100`); Maximum and rightmost value of the Slide |
| Value         | Default (`0`); Initial value of the Slider                |
| Step          | Default (`0`); Increments of the Slider                   |

## Style the Slider

* **Minimum Track Tint Color: **Color of the slider track to the left of the thumb
* **Maximum Track Tint Color: **Color of the slider track to the right of the thumb
* **Thumb Tint Color (Android only): **Color of the thumb
* **Border: **
  * **Width: **Enter how wide you want the border outline of the Slider to be
  * **Color: **Pick a color for the border of the Slider
  * **Style: **Select if you want the border to be a dotted, dashed or solid line
  * **Radius: **Enter how round you want the edges of the border for the Slider to be

| Property                        | Description                                                                                                                |
| ------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| Minimum Track Tint Color        | Default (`none`); Color of the slider track to the left of the thumb                                                       |
| Maximum Track Tint Color        | Default (`none`); Color of the slider track to the right of the thumb                                                      |
| Thumb Tint Color (Android only) | Default (`none`); Color of the thumb                                                                                       |
| Border                          | Default (`none`); You can add a border with customized `width`, `color`, `style (solid, dotted, dashed)`and `borderRadius` |

### Edit the Slider size

You can set how tall the Slider is using the height property and set how wide it is using the width property.

**Height**

* **Fill container - **The Slider fills the entire screen vertically
* **Fit contents - **The Slider’s height changes to fit the contents it contains
* **Relative size - **The Slider fills the specified percentage of the screen
* **Absolute size - **Sizes the Slider to a specified number of pixels

**Width**

* **Fill container - **The Slider fills the entire screen horizontally
* **Fit contents - **The Slider’s width changes to fit the contents it contains
* **Relative size - **The Slider fills the specified percentage of the screen
* **Absolute - **Sizes the Slider to a specified number of pixels

## Add spacing

You change the spacing and positioning of the Slider with the Margin and Padding properties.

**Margin**

* You can specify how much space you want between the border and the contents of Slider using either pixel or percent values.

**Padding**

* You can specify how much space you want between the edges of the Slider and the screen using either pixel or percent values.

## Events&#x20;

### On Sliding Complete

![](.gitbook/assets/on\_sliding\_complete.png)

When the user takes their finger off the slider. The event returns the value that the slider has settled on.

Please note that the `on Sliding Complete ` event does not work in web preview

### On Value Change

![](.gitbook/assets/on\_value\_change.png)

This event fires each time the slider moves to a new position. Each time a new values is selected this event will return an updated value.

## Properties

### Disabled&#x20;

![](<.gitbook/assets/disabled (2).png>)

### Height&#x20;

![](<.gitbook/assets/height (7).png>)

The set and get height blocks work with the Height property of the slider component. Acceptable input values are.&#x20;

* Number of Pixels
* Percentage Height
* "Fit Contents"
* "Fill Container"

The `Computed Height`block returns the on-screen dimensions of the slider, after it has been rendered on-screen. The value returned is an integer, representing the size of the slider in pixels.

### Maximum Track Tint Color

### &#x20;

![](.gitbook/assets/max\_track\_tint\_color.png)

Set or get the color of the right side of the slider.

### Maximum Value

![](.gitbook/assets/max\_value.png)

Set or get the biggest value of the slider

### Minimum Track Tint Color&#x20;

![](.gitbook/assets/min\_track\_tint\_color.png)

Set or get the color of the left side of the slider

### Minimum Value

![](.gitbook/assets/min\_value.png)

Set or get the smallest value of the slider

### Step&#x20;

![](.gitbook/assets/step.png)

Set or get the step-size, also known as the increment, of the slider.

### Thumb Tint Color&#x20;

![](<.gitbook/assets/thumb\_tint\_color (2).png>)

Change the color of the slider itself.

### Value&#x20;

![](<.gitbook/assets/value (1).png>)

The set and get value blocks are user to work with the position of the slider.

### Visible&#x20;

![](<.gitbook/assets/visible (11).png>)



The set and get visible blocks are used to show or hide the entire Slider component. Acceptable values are:

* True
* False

### Width

![](<.gitbook/assets/width (7).png>)

The set and get width blocks work with the Width property of the Slider component. Acceptable input values are.&#x20;

* Number of Pixels
* Percentage Height
* "Fit Contents"
* "Fill Container"

The `Computed Width`block returns the on-screen dimensions of the slider, after it has been rendered on-screen. The value returned is an integer, representing the size of the slider in pixels.
