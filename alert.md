# Alert

Alerts are useful components for displaying important messages while users are in the app itself

![Demonstration of how an Alert looks on Android, iOS and Web](.gitbook/assets/alertdemo.jpg)

## One Button Alert

A one button alert, also known as a notification, displays a message and one button to confirm user has viewed the message

![](.gitbook/assets/thunkable-docs-exhibits-15.png)

To set up an alert, simply fill in the following `simple` properties. The Cancel Button Text only needs to be filled out for a two-button alert. You can use blocks to start an event when

| Property            | Description               |
| ------------------- | ------------------------- |
| Title               | The title of the alert    |
| Message             | The subtitle of the alert |
| Confirm Button Text | The text of the button    |
| Cancel Button Text  | `LEAVE BLANK`             |

## Two button alert

Two button alerts have two buttons, one that dismisses the notification and one that can be programmed to start an event

To set one up, simply add the following `simple` properties

![](<.gitbook/assets/thunkable-docs-exhibits-14 (2).png>)

| Property            | Description                                                                                                   |
| ------------------- | ------------------------------------------------------------------------------------------------------------- |
| Title               | The title of the alert                                                                                        |
| Message             | The subtitle of the alert                                                                                     |
| Confirm Button Text | The text of the right confirm button; If the `danger` switch is turned on, the text will be in red (iOS only) |
| Cancel Button Text  | The text of the left cancel button                                                                            |

If you want to start an event from a confirm button, you will want to add the blocks below:

![](<.gitbook/assets/image (194).png>)

## Button List: Alert with three or more buttons

It is possible to add buttons to an alert for more sophisticated use cases.\
This can be done using the `set Button List to` block by creating a [list](lists.md) of [objects](objects.md).

You can set the **Text** of the Alert. You can set the **Style** of the Alert to **ok, destructive** or **cancel.**

On iOS, the Alert can show more than 3 Buttons.\
On Android, the Alert can show up to 3 buttons. If more than 3 buttons are specified, the first 3 will be shown. \


![](.gitbook/assets/screen-shot-2021-04-19-at-10.23.10-am.png)

![A three button alert displayed on Android and iOS devices](.gitbook/assets/thunkable-docs-exhibits-16.png)

| Property         | Description                                                                                                                                      |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| Title            | The title of the alert                                                                                                                           |
| Message          | The subtitle of the alert                                                                                                                        |
| Text `Advanced`  | The text of the button                                                                                                                           |
| Style `Advanced` | The style of the button; `ok` is a confirm button, `cancel` is a cancel button and `destructive` is a confirm button with text in red (iOS only) |

The 'showButtonList' block will return an output called 'buttonPressed'.\
This will return the position of the Button in your Button List.\
You can take some action based on which button was pressed.

![](<.gitbook/assets/image (193).png>)

Note: the Buttons may appear in a different order when testing the app on a device. \
The number that ‘buttonPressed’ returns is the order that the Buttons are added in the app project.
