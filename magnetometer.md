# Magnetometer

## Description

The magnetometer is used to measure magnetic flux density. This is the total magnetic field passing through a given area, per metre squared, $$\frac{T \cdot m^2}{m^2}$$ . The sensor will returns values with units of microtesla $$\mu T$$ for each of the three coordinate axes; x, y and, z. The magnetic flux density is quite similar to magnetic field strength.

![](.gitbook/assets/screenshot-2019-05-18-at-15.27.06.png)

## Events

When the magnetometer detects a change in the ambient magnetic field the `Changes` event will fire. The event returns 4 parameters that we can work with. 

![](.gitbook/assets/screenshot-2019-05-18-at-14.15.20.png)

| Parameter | Type | Returns |
| :--- | :--- | :--- |
| `xFluxDensity` | Number | Flux density, in the x direction, expressed in $$\mu T$$  |
| `yFluxDensity` | Number | Flux density, in the y direction, expressed in $$\mu T$$  |
| `zFluxDensity` | Number | Flux density, in the z direction, expressed in $$\mu T$$  |
| `error` | String | Error message from the Sensor |

## Properties

The magnetometer is, by default, turned on, but the `enabled` property can be used to turn in on and off by setting it to `true` or `false` respectively.

![](.gitbook/assets/screenshot-2019-05-18-at-14.15.29.png)

| Property | Type | Default |
| :--- | :--- | :--- |
| `set Enabled` | Bool | true |
| `get Enabled` | Bool | true |

