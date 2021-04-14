# Switch

Think of a Light Switch. It has two settings, On and Off. That is exactly what the switch component is like.

## Switch Overview <a id="switch-overview"></a>

* ​[Getting Started](https://docs.thunkable.com/switch#getting-started)​
* ​[Style the Switch](https://docs.thunkable.com/switch#style-the-switch)​
* ​[Events](https://docs.thunkable.com/switch#events)​
* ​[Properties](https://docs.thunkable.com/switch#properties)​

A switch is a component that has two settings, true and false. You can get your app to do specific tasks only if the switch is set to true.![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-LAn5wecEraNWaG7Ig2g%2F-LAn68KdTsbXiRGsjXH9%2Fswitch-%E2%9C%95-fig-1.gif?alt=media)

## Getting Started <a id="getting-started"></a>

Each time the switch is clicked the value will change. The value returned will only ever be `true` or `false`. To test this for yourself you can use the following blocks.![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWiVqCOptR2gSHR9wYp%2F-MWiX9j8t3LVznuX3mHm%2Fsw_basic.png?alt=media&token=ff6f7776-fc89-466b-a551-761e415db136)

In the following example, the user can only advance to `Screen2` if the acknowledge they have accepted the terms and conditions by clicking on the switch.![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWiVqCOptR2gSHR9wYp%2F-MWiXQwteEJ16aJq86ov%2Fsw_adv.png?alt=media&token=f2a000dc-01fe-4365-a064-934e92e3c4b5)

| Event | Description |
| :--- | :--- |
| On Value Change | By default, the switch `newValue` will be set to `false`. If turned on, the `newValue` will be set to `true` |
| Value | If on, value is set to `true`; if off, `false` |
| Disabled | If set to `true`, switch will be disabled |

## Style the Switch <a id="style-the-switch"></a>

You can customize the switch with the following properties:

* **Tint Color:** Color of the switch track when switch is set to off
* **On Tint Color:** Color of the switch track when switch set to on
* **Thumb Tint Color:** Color of the switch thumb

## Events  <a id="events"></a>

### On Value Change <a id="on-value-change"></a>

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWiVqCOptR2gSHR9wYp%2F-MWiXu-th3Ep7LerkKjl%2Fon_value_changed.png?alt=media&token=709a3260-811b-4d43-a6ba-3e6521a2ec6f)

This event fires every time the switch is clicked.

## Properties <a id="properties"></a>

### Disabled  <a id="disabled"></a>

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZG3NqO-Qepj7sp5hj%2Fdisabled.png?alt=media&token=ef01971d-5acc-4fa7-99a8-80d9e73c2b19)

The disabled property is used to set whether or not the button is "clickable". Expected values for this property are:

* True
* False

### Height  <a id="height"></a>

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZG4gitjHowTsf_j_L%2Fheight.png?alt=media&token=8d69e6cd-4c36-45cc-a9ba-5c0d85afb8b2)

The set and get height blocks work with the Height property of the switch component.

### On Tint Color  <a id="on-tint-color"></a>

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZG6DZJ4tRxXoh61Dy%2Fon_tint_color.png?alt=media&token=c980b50b-8eeb-4732-a802-1eb3d60fd05f)

Change the "active" color of the switch.

### Thumb Tint Color  <a id="thumb-tint-color"></a>

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZG7d5VsHWrnTT99VE%2Fthumb_tint_color.png?alt=media&token=223e8e93-175c-489f-bc04-2df46398601a)

Change the color of the switch

### Tint Color  <a id="tint-color"></a>

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZGEHN_gpbrhgSKHxM%2Ftint_color.png?alt=media&token=39b92335-6977-4768-9a67-d874838f9425)

Change the "inactive" color of the switch

### Value  <a id="value"></a>

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZGFgk_NS1U31Z65lg%2Fvalue.png?alt=media&token=1e299ebf-80b0-4eca-9de1-bffa49bf40da)

Change the state \(on or off\) of the switch

### Visible  <a id="visible"></a>

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZGGpog3cyq9npq5Qo%2Fvisible.png?alt=media&token=e0f07925-562e-41ac-8476-cf92eda91461)

Show or hide the switch on the screen.

### Width  <a id="width"></a>

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZGI49tqFn8CnxjOQa%2Fwidth.png?alt=media&token=9e21c30e-8e20-4b01-830d-1c4f720cd4da)

The set and get height blocks work with the Width property of the switch component.

### X  <a id="x"></a>

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZGJHPWiFk0A6jxttz%2Fx.png?alt=media&token=970de731-7f9d-4377-a161-a47889826d95)

### Y <a id="y"></a>

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZGKPvI15ZDZMgD4dU%2Fy.png?alt=media&token=5f8c09a0-48a7-46a9-884d-742f1f984b3a)

