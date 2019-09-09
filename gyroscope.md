# Gyroscope

## Description

The gyroscope is capable of measuring how quickly the phone is being turned. It measures the rate of rotation of the phone and returns values in radians per second about the x axis, the y axis and the z axis. This rate of rotation is also known as the _Angular Velocity,_ so the gyroscope can tell us the speed of rotation of the phone. By extension, if the speed of rotation is any number greater than 0, we can infer that the phone is being turned.

![The x, y and z axes of a standard smartphone](.gitbook/assets/screenshot-2019-05-18-at-15.27.06.png)



## Events

Whenever the phone is turned, or rotated, the `Changes` event will fire. This event returns 4 parameters for us to work with. 

![](.gitbook/assets/screenshot-2019-05-18-at-14.15.00.png)

| Parameter | Type | Returns |
| :--- | :--- | :--- |
| `xRotationRate` | Number | Angular velocity, about the x axis, in $$rad/s$$  |
| `yRotationRate` | Number | Angular velocity, about the y axis, in $$rad/s$$  |
| `zRotationRate` | Number | Angular velocity, about the z axis, in $$rad/s$$  |
| `error` | String | Error message from the sensor |

## Properties

By default the gyroscope sensor is turned on, but the `enabled`property can be used to read and write new values to the gyroscope, thus allowing you to turn it on or off.

![](.gitbook/assets/screenshot-2019-05-18-at-14.15.07.png)

| Property | Type | Default |
| :--- | :--- | :--- |
| `set Enabled` | Bool | true |
| `get Enabled` | Bool |  |

![](.gitbook/assets/image%20%2823%29.png)

| Property | Type | Description |
| :--- | :--- | :--- |
| `Alpha` | Number | Rotation about the y-axis |
| `Beta` | Number | Rotation about the x-axis |
| `Gamma` | Number | Rotation about the z-axis |

