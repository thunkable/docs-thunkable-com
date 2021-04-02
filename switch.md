---
description: >-
  Think of a Light Switch. It has two settings, On and Off. That is exactly what
  the switch component is like.
---

# Switch

A switch is a component that has two settings, true and false. You can get your app to do specific tasks only if the switch is set to true. 

* [Getting Started](switch.md#getting-started)
* [Style the Switch](switch.md#style-the-switch)
* [Events](switch.md#events)
* [Properties](switch.md#properties)

![](.gitbook/assets/switch-fig-1.gif)

## Getting Started

Each time the switch is clicked the value will change. The value returned will only ever be `true` or `false`. To test this for yourself you can use the following blocks.

![](.gitbook/assets/sw_basic.png)

In the following example, the user can only advance to `Screen2` if the acknowledge they have accepted the terms and conditions by clicking on the switch.

![](.gitbook/assets/sw_adv.png)

| Event | Description |
| :--- | :--- |
| On Value Change | By default, the switch `newValue` will be set to `false`. If turned on, the `newValue` will be set to `true` |
| Value | If on, value is set to `true`; if off, `false` |
| Disabled | If set to `true`, switch will be disabled |

## Style the Switch

You can customize the switch with the following properties:

* **Tint Color:** Color of the switch track when switch is set to off
* **On Tint Color:** Color of the switch track when switch set to on 
* **Thumb Tint Color:** Color of the switch thumb

## Events 

### On Value Change

![](.gitbook/assets/on_value_changed%20%281%29.png)

This event fires every time the switch is clicked.

## Properties

### Disabled 

![](.gitbook/assets/disabled%20%281%29.png)

The disabled property is used to set whether or not the button is "clickable". Expected values for this property are:

* True
* False

### Height 

![](.gitbook/assets/height%20%285%29.png)

The set and get height blocks work with the Height property of the switch component.

### On Tint Color 

![](.gitbook/assets/on_tint_color.png)

Change the "active" color of the switch.

### Thumb Tint Color 

![](.gitbook/assets/thumb_tint_color%20%281%29.png)

Change the color of the switch

### Tint Color 

![](.gitbook/assets/tint_color.png)

Change the "inactive" color of the switch

### Value 

![](.gitbook/assets/value.png)

Change the state \(on or off\) of the switch

### Visible 

![](.gitbook/assets/visible%20%284%29.png)

Show or hide the switch on the screen.

### Width 

![](.gitbook/assets/width%20%286%29.png)

The set and get height blocks work with the Width property of the switch component.

### X 

![](.gitbook/assets/x.png)

### Y

![](.gitbook/assets/y.png)

