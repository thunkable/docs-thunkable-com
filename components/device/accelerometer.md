#### **Thunkable for Android **❤

# Accelerometer ![](/assets/accelerometer-icon.png)

---

The Accelerometer is a phone sensor that detects shaking and measures acceleration in 3 dimensions:

* xAccel: 0 when the phone is at rest on a flat surface, positive when the phone is tilted to the right \(i.e., its left side is raised\), and negative when the phone is tilted to the left \(i.e., its right size is raised\)
* yAccel: 0 when the phone is at rest on a flat surface, positive when its bottom is raised, and negative when its top is raised.
* zAccel: Equal to -9.8 \(earth's gravity in meters per second per second when the device is at rest parallel to the ground with the display facing up, 0 when perpindicular to the ground, and +9.8 when facing down. The value can also be affected by accelerating it with or against gravity

---

#### Trigger an event by shaking your phone

|  |  |
| :--- | :--- |
|  |  |
|  |  |
|  |  |



Enabled

MinimumInterval

The minimum interval, in milliseconds, between phone shakes

Sensitivity

A number that encodes how sensitive the accelerometer is. The choices are: 1 = weak, 2 = moderate, 3 = strong.

XAccel

YAccel

ZAccel

AccelerationChanged\(number xAccel, number yAccel, number zAccel\)

Indicates the acceleration changed in the X, Y, and/or Z dimensions.

Shaking\(\)

Indicates the device started being shaken or continues to be shaken.

