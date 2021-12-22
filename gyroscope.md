# Gyroscope

## Description

The gyroscope is capable of measuring how quickly the phone is being turned. It measures the rate of rotation of the phone and returns values in radians per second about the x axis, the y axis and the z axis. This rate of rotation is also known as the _Angular Velocity, _so the gyroscope can tell us the speed of rotation of the phone. By extension, if the speed of rotation is any number greater than 0, we can infer that the phone is being turned.

![The x, y and z axes of a standard smartphone](.gitbook/assets/screenshot-2019-05-18-at-15.27.06.png)



## Blocks

### Events

#### when Gyroscope Changes

Whenever the phone is turned, or rotated, the `Changes` event will fire.&#x20;

![](.gitbook/assets/gyro\_changes.png)

### Properties

By default the gyroscope sensor is turned on, but the `enabled`property can be used to read and write new values to the gyroscope, thus allowing you to turn it on or off.

![](.gitbook/assets/gyros\_enabled.png)

| Property      | Type | Default |
| ------------- | ---- | ------- |
| `set Enabled` | Bool | true    |
| `get Enabled` | Bool |         |

![](<.gitbook/assets/image (25).png>)

![](.gitbook/assets/gyro1.png)

| Property | Type   | Description               |
| -------- | ------ | ------------------------- |
| `Alpha`  | Number | Rotation about the y-axis |
| `Beta`   | Number | Rotation about the x-axis |
| `Gamma`  | Number | Rotation about the z-axis |

![](.gitbook/assets/gyro2.png)

| Property | Type   | Description                       |
| -------- | ------ | --------------------------------- |
| `X`      | Number | Angular velocity about the X axis |
| `Y`      | Number | Angular velocity about the Y axis |
| `Z`      | Number | Angular velocity about the Z axis |
