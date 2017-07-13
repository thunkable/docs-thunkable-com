#### **Thunkable for Android **❤

# Gyroscope ![](/assets/gyroscope-icon.png)

---

The Gyroscope is a sensor that utilizes the gravity of the earth to indicate its orientation. It consists of a freely-rotating disk mounted onto the center of larger wheels.

The Gyroscope sensor on a phone has become a central component in virtual and augmented reality apps because of its ability to detect how much the phone is being tilted, mostly to provide a smooth experience to a user turning her head.

The sample app [Thunkable Cardboard VR](#) uses a Gyroscope to create a virtual reality drawing app for Google Cardboard

---

#### Detect Phone's Angular Velocity

| Event / Property | Description |
| :--- | :--- |
| Available | Indicates whether the gyroscope is present on the device. Not all devices have gyroscopes |
| Gyroscope Changed \(xAngularVelocity, yAngularVelocity, zAngularVelocity, timestamp \(nanoseconds\)\) | Indicates that the gyroscope sensor data has changed. The timestamp parameter is the time in nanoseconds at which the event occurred |
| X  Angular Velocity |  The angular velocity around the X axis, in degrees per second |
| Y Angular Velocity |  The angular velocity around the Y axis, in degrees per second |
| Z Angular Velocity | The angular velocity around the Z axis, in degrees per second |
| Enabled | If 'true', the gyroscope sensor is enabled |



