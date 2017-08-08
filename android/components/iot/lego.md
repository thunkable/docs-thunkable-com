#### **Thunkable for Android **❤

# Lego Mindstorms

---

![](/assets/lego-mindstorm-fig-1.png)

Lego was the inspiration for the blocks that are a core part of the Thunkable app building experience.

Lego Mindstorms are series of kits contain software and hardware to create customizable, programmable robots. They include an intelligent brick computer that controls the system, a set of modular sensors and motors, and [Lego](https://en.wikipedia.org/wiki/Lego) parts from the [Technic](https://en.wikipedia.org/wiki/Lego_Technic) line to create the mechanical systems. EV3 is the current version of Lego Minstorms and NXT has now been retired.

With Thunkable, you can build an app that controls your Lego Mindstorm robot.

LEGO and MINDSTORMS are registered trademarks of the LEGO Group.

---

#### Add a Bluetooth Client component to set up your Lego Mindstorm component\(s\)

All of these components have a Bluetooth Client property that tells which Bluetooth Client component to use for communication with the robot. You will need to explicitly add a Bluetooth Client component to your project.

If you have one robot, you should have one BluetoothClient component. If you are lucky enough to have two robots and you want to control both of them simultaneously from one application, you'll need two BluetoothClient components in your project.

| Property | Description |
| :--- | :--- |
| Bluetooth Client | The BluetoothClient component that should be used for communication |

---

#### Programming your robot

| EV3 | NXT | Description |
| :--- | :--- | :--- |
| [Motors](#ev3-motors) | Drive | Controls the motors / move or turns the robot |
| [UI](#ev3-ui) |  | Draws graphs on the EV3 screen |
| [Gyro Sensor](#ev3-gyro-sensor) |  | Controls the gyro sensor |
| [Color Sensor](#ev3-color-sensor) | Color Sensor | Controls the color sensor |
| [Touch Sensor](#ev3-touch-sensor) | Touch Sensor | Controls the touch sensor |
| [Ultrasonic Sensor](#ev3-ultrasonic-sensor) | Ultrasonic Sensor | Controls the ultrasonic sensor |
| [Sound Sensor](#ev3-sound-sensor) | Sound Sensor | Controls the sound sensor |
| [Commands](#ev3-commands) | Direct Commands | Sends system or direct commands |

---

#### EV3 Motors

| Property | Description |
| :--- | :--- |
| Motor Ports | The motor ports that the motors are connected to. The ports are specified by a sequence of port letters |
| Wheel Diameter \(cm\) | The diameter of the wheels attached on the motors in centimeters |
| Reverse Direction | It specifies if the direction of the motors is reversed |
| Enable Speed Regulation | The robot adjusts the power to maintain the speed if speed regulation is enabled |
| Stop Before Disconnect | Whether to stop the motor before disconnecting |
| Tacho Count Changed Event Enabled | Whether the TachoCountChanged event should fire when the angle is changed |

| Events | Description |
| :--- | :--- |
| Rotate Indefinitely \(power\) | Start to rotate the motors |
| Rotate In Tacho Counts \(power, tachoCounts, useBrake\) | Rotate the motors in a number of tacho counts |
| Rotate In Duration \(power, milliseconds, useBrake\) | Rotate the motors in a period of time |
| Rotate In Distance \(power, distance, useBrake\) | Rotate the motors in a distance |
| Rotate Sync Indefinitely \(power, turnRatio\) | Start to rotate the motors at the same speed |
| Rotate Sync In Distance \(power, distance, turnRatio, useBrake\) | Rotate the motors at the same speed for a distance in cm |
| Rotate Sync In Duration \(power, milliseconds, turnRatio, useBrake\) | Rotate the motors at the same speed in a period of time |
| Rotate Sync In Tacho Counts \(power, tachoCounts, turnRatio, useBrake\) | Rotate the motors at the same speed in a number of tacho counts |
| Stop \(useBrake\) | Stop the motors of the robot |
| Toggle Direction | Toggle the direction of motors |
| Reset Tacho Count | Set the current tacho count to zero |
| Get Tacho Count | Get the current tacho count |

---

#### EV3 UI

| Event | Description |
| :--- | :--- |
| Draw Point \(color, x, y\) | Draw a point on the screen |
| Draw Icon \(color, x, y, type, no\) | Draw a built-in icon on screen |
| Draw Line \(color, x1, y1, x2, y2\) | Draw a line on the screen |
| Draw Rect \(color, x, y, width, height, fill\) | Draw a rectangle on the screen |
| Draw Circle \(color, x, y, radius, fill\) | Draw a circle on the screen |
| Fill Screen \(color\) | Fill the screen with a color |

---

#### EV3 Gyro Sensor

| Property | Description |
| :--- | :--- |
| Sensor Port | The sensor port that the sensor is connected to |
| Mode | The sensor mode can be a text constant of either 'rate' or 'angle', which correspond to Set Angle Mode or Set Rate Mode respectively |
| Sensor Value Changed Event Enabled | Whether the SensorValueChanged event should fire when the sensor value changed |

| Event | Description |
| :--- | :--- |
| Get Sensor Value | Returns the current angle or rotation speed based on current mode, or -1 if the value cannot be read from sensor |
| Set Angle Mode | Measures the orientation of the sensor |
| Set Rate Mode | Measures the angular velocity of the sensor |

---

#### EV3 Color Sensor

| Property | Description |
| :--- | :--- |
| Sensor Port | The sensor port that the sensor is connected to |
| Bottom Of Range | The bottom of the range used for the Below Range, Within Range, and Above Range events |
| Top Of Range | The top of the range used for the Below Range, Within Range, and Above Range events |
| Below Range Event Enabled | Whether the Below Range event should fire when the light level goes below the Bottom Of Range |
| Within Range Event Enabled | Whether the Within Range event should fire when the light level goes between the Bottom Of Range and the Top Of Range |
| Above Range Event Enabled | Whether the Above Range event should fire when the light level goes above the Top Of Range |
| Color Changed Event Enabled | Whether the Color Changed event should fire when the Mode property is set to "color" and the detected color changes |
| Mode | Get the current sensor mode |

| Events | Description |
| :--- | :--- |
| Get Light Level | It returns the light level in percentage, or -1 when the light level cannot be read |
| Get Color Code | It returns the color code from 0 to 7 corresponding to no color, black, blue, green, yellow, red, white and brown |
| Get Color Name | Return the color name in one of "No Color", "Black", "Blue", "Green", "Yellow", "Red", "White", "Brown" |
| Set Color Mode | Enter the color detection mode |
| Set Reflected Mode | Make the sensor read the light level with reflected light |
| Set Ambient Mode | Make the sensor read the light level without reflected light |

---

#### EV3 Touch Sensor

| Property / Event | Description |
| :--- | :--- |
| Sensor Port | The sensor port that the sensor is connected to |
| Pressed Event Enabled | Whether the Released event should fire when the touch sensor is pressed |
| Released Event Enabled | Whether the Released event should fire when the touch sensor is released |
| Is Pressed | Returns true if the touch sensor is pressed |

---

#### EV3 Ultrasonic Sensor

| Property | Description |
| :--- | :--- |
| Sensor Port | The sensor port that the sensor is connected to |
| Bottom Of Range | The bottom of the range used for the Below Range, Within Range, and Above Range events |
| Top Of Range | The top of the range used for the Below Range, Within Range, and Above Range events |
| Below Range Event Enabled | Whether the Below Range event should fire when the light level goes below the Bottom Of Range |
| Within Range Event Enabled | Whether the Within Range event should fire when the light level goes between the Bottom Of Range and the Top Of Range |
| Above Range Event Enabled | Whether the Above Range event should fire when the light level goes above the Top Of Range |
| Color Changed Event Enabled | Whether the Color Changed event should fire when the Mode property is set to "color" and the detected color changes |
| Unit | The distance unit, which can be either "cm" or "inch" |

| Event | Description |
| :--- | :--- |
| Get Distance | Returns the current distance in centimeters as a value between 0 and 254, or -1 if the distance can not be read |
| Set Cm Unit | Measure the distance in centimeters |
| Set Inch Unit | Measure the distance in inches |

---

#### EV3 Sound Sensor

| Event | Description |
| :--- | :--- |
| PlayTone \(volume, frequency, milliseconds\) | Make the robot play a tone |
| Stop Sound | Stop any sound on the robot |

---

#### EV3 Commands

| Event | Description |
| :--- | :--- |
| Keep Alive \(minutes\) | Keep the EV3 brick from shutdown for a period of time |
| Get Battery Voltage | Get the battery voltage |
| Get Battery Current | Get the battery current |
| Get OS Version | Get the OS version on EV3 |
| Get OS Build | Get the OS build on EV3 |
| Get Firmware Version | Get the firmware version on EV3 |
| Get Firmware Build | Get the firmware build on EV3 |
| Get Hardware Version | Get the hardware version of EV3 |



