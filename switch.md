# Switch

## Switch Overview​ <a href="#switch-overview" id="switch-overview"></a>

A switch is a component that has two settings, true and false. You can get your app to do specific tasks based on the value of the switch.

<div align="left">

<figure><img src=".gitbook/assets/switch (web preview - cropped).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

## Properties <a href="#getting-started" id="getting-started"></a>

### Switch

| Property         | Description                                        | Data Type  |
| ---------------- | -------------------------------------------------- | ---------- |
| Value            | Initial value of Switch                            | True/False |
| Tint Color       | Color of background when Switch is **false**       | Color      |
| On Tint Color    | Color of background when Switch is **true**        | Color      |
| Thumb Tint Color | Color of the Switch's slider                       | Color      |
| Disabled         | Toggle whether value Switch can be changed by user | True/False |

### Layout

| Property    | Description                                                                      | Data Type                                    |
| ----------- | -------------------------------------------------------------------------------- | -------------------------------------------- |
| X           | Location of top left corner of Switch on X-axis, where the left hand side is X=0 | Number                                       |
| Y           | Location of top left corner of Switch on Y-axis, where the top side is Y=0       | Number                                       |
| Height      | Height of Switch in pixels                                                       | Number                                       |
| Width       | Width of Switch in pixels                                                        | Number                                       |
| Resize Mode | Define dimensions of the Switch's component/container                            | Select from list `[Stretch, Float in Place]` |

## Blocks <a href="#events" id="events"></a>

### Events&#x20;

#### On Value Change

![](.gitbook/assets/screen-shot-2021-08-23-at-12.51.10-pm.png)

This event fires every time the switch is clicked.

Returns `newValue` output block, which returns the new value of the Switch (`true` or `false`).

### Properties

Use these blocks to set and get the named [properties](switch.md#getting-started) of the Switch.

#### Value&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZGFgk\_NS1U31Z65lg%2Fvalue.png?alt=media\&token=1e299ebf-80b0-4eca-9de1-bffa49bf40da)

#### Tint Color&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZGEHN\_gpbrhgSKHxM%2Ftint\_color.png?alt=media\&token=39b92335-6977-4768-9a67-d874838f9425)

#### On Tint Color&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZG6DZJ4tRxXoh61Dy%2Fon\_tint\_color.png?alt=media\&token=c980b50b-8eeb-4732-a802-1eb3d60fd05f)

#### Thumb Tint Color&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZG7d5VsHWrnTT99VE%2Fthumb\_tint\_color.png?alt=media\&token=223e8e93-175c-489f-bc04-2df46398601a)

#### Disabled&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZG3NqO-Qepj7sp5hj%2Fdisabled.png?alt=media\&token=ef01971d-5acc-4fa7-99a8-80d9e73c2b19)

#### X&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZGJHPWiFk0A6jxttz%2Fx.png?alt=media\&token=970de731-7f9d-4377-a161-a47889826d95)

#### Y

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZGKPvI15ZDZMgD4dU%2Fy.png?alt=media\&token=5f8c09a0-48a7-46a9-884d-742f1f984b3a)

#### Height&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZG4gitjHowTsf\_j\_L%2Fheight.png?alt=media\&token=8d69e6cd-4c36-45cc-a9ba-5c0d85afb8b2)

#### Width&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZGI49tqFn8CnxjOQa%2Fwidth.png?alt=media\&token=9e21c30e-8e20-4b01-830d-1c4f720cd4da)

####

#### Visible&#x20;

![](https://gblobscdn.gitbook.com/assets%2F-LAn5scXl2uqUJUOqkJo%2F-MWZ9fsYSsJxH4WcN4Jj%2F-MWZGGpog3cyq9npq5Qo%2Fvisible.png?alt=media\&token=e0f07925-562e-41ac-8476-cf92eda91461)
