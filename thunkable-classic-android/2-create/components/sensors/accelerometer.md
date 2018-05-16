---
description: >-
  The Accelerometer is a sensor loaded onto most smartphones that signals which
  way is up, commonly used to automatically switch between Portrait and
  Landscape mode
---

# Accelerometer

### ![](../../../../.gitbook/assets/accelerometer-icon.png)

The Accelerometer component on Thunkable can be used to detect shaking events, indicate if the phone should be in Portrait or Landscape mode, and measure acceleration in 3 dimensions:

![](https://github.com/thunkable/thunkable-docs/tree/4a752596e288fca776105e94dc5e863bb9a3e25a/assets/android/accelerometer-fig-1.png)![](../../../../.gitbook/assets/accelerometer-fig-1.png)

Our amazing community member Domhnall made [this great resource](https://community.thunkable.com/t/how-to-use-the-accelerometer-sensor/1038) to further explain the power of this sensor

### Trigger an event by shaking your phone

| Event / Property | Description |
| :--- | :--- |
| Shaking | Indicates the device started being shaken or continues to be shaken |
| Minimum Interval \(milliseconds\) | The minimum interval, in milliseconds, between phone shakes |
| Sensitivity | A number that encodes how sensitive the accelerometer is. The choices are: 1 = weak, 2 = moderate, 3 = strong. |
| Enabled | If 'true', the accelerometer sensor is enabled |

### Measure changes in acceleration

| Event / Property | Description |
| :--- | :--- |
| Acceleration Changed \(xAccel, yAccel, zAccel\) | Indicates the acceleration changed in the X, Y, and/or Z dimensions |
| xAccel | 0 when the phone is at rest on a flat surface, positive when the phone is tilted to the right \(i.e., its left side is raised\), and negative when the phone is tilted to the left \(i.e., its right size is raised\) |
| yAccel | 0 when the phone is at rest on a flat surface, positive when its bottom is raised, and negative when its top is raised |
| zAccel | Equal to -9.8 \(earth's gravity in meters per second per second when the device is at rest parallel to the ground with the display facing up, 0 when perpindicular to the ground, and +9.8 when facing down. The value can also be affected by accelerating it with or against gravity |

