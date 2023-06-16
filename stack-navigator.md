# Stack Navigator

## Stack Navigator Properties

### Set Your Screen Transitions

To enable a Stack transition, you will have to add a Screen navigation block like the one below. You can find the Screen navigation block in the pre-built Control category:

![](.gitbook/assets/btn\_click\_1.png)

Screens can Stack from left to right or from top to bottom. You can set the transition style with the Stack property below:

| Property | Description                          | Data Type                                                                                                                                   |
| -------- | ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------- |
| Mode     | Define how your screens will stack.  | <p>Select from list:<br><code>card</code> - stacks screens from left to right<br><code>modal</code> - stacks screens from top to bottom</p> |

### Hide Your Header

It is possible to hide the Header bar and maintain the Stacking transition by using the Stack property below. Hiding the Header bar will also hide the back button that makes it easier to transition to your original screen

| Property   | Description                                | Data Type                                                                                                                                                                               |
| ---------- | ------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| HeaderMode | Define how the header appears in your app. | <p>Select from list:<br><code>float</code> - headers fade in with the scren change<br><code>screen</code> - header slides with the screen change<br><code>none</code> - hide header</p> |
