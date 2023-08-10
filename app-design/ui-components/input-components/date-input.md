# Date Input Component

## Date Input Overview

A Date Input component is helpful when you want the user of your app to easily select a specific date using the native Android or iOS date picker

![Native Android Date Picker on the left and iOS on the right](../../../.gitbook/assets/thunkable-docs-exhibits-37.png)

## Properties

### Date Input

| Property    | Description                                 | Data Type                                                                            |
| ----------- | ------------------------------------------- | ------------------------------------------------------------------------------------ |
| Style       | Format to use when displaying selected date | Select from menu `[YYYY-MM-DD, MM/DD/YYYY, M/D/YY, Month Day, Year, Mth. Day, Year]` |
| Font Size   | Size of font when displaying date           | Number                                                                               |
| Font Style  | Make the date's text italicized             | True/False                                                                           |
| Font Weight | Make the date's text bold                   | True/False                                                                           |
| Color       | Color of font when displaying date          | Color                                                                                |

### Layout

| Property    | Description                                                                          | Data Type                                    |
| ----------- | ------------------------------------------------------------------------------------ | -------------------------------------------- |
| X           | Location of top left corner of Date Input on X-axis, where the left hand side is X=0 | Number                                       |
| Y           | Location of top left corner of Date Input on Y-axis, where the top side is Y=0       | Number                                       |
| Height      | Height of Date Input in pixels                                                       | Number                                       |
| Width       | Width of Date Input in pixels                                                        | Number                                       |
| Resize Mode | Define dimensions of the date input component/container                              | Select from list `[Stretch, Float in Place]` |

### **Style**

| Property       | Description                                                                             | Data Type                                  |
| -------------- | --------------------------------------------------------------------------------------- | ------------------------------------------ |
| Visible        | Toggle whether your end users can see the Date Input                                    | True/False                                 |
| Border Style   | Set whether border style is solid, dotted or dashed  (only visible if border width > 0) | Select from list `[solid, dotted, dashed]` |
| Border Color   | Color of border (only visible if border width > 0)                                      | Color                                      |
| Border Width   | Width of border around Date Input in pixels                                             | Number                                     |
| Border Radius  | Radius of corners of border on Date Input in degrees                                    | Number                                     |
| Shadow Color   | Color of date input's shadow                                                            | Color                                      |
| Shadow Opacity | Opacity of date input's  shadow                                                         | Number between 0 and 100                   |
| Shadow Radius  | Radius of corners of date input's shadow in pixels                                      | Number                                     |
| Shadow Offset  | How far date input's  shadow should be offset, in Height and Width, in pixels           | Number                                     |

## Blocks

### Events

You can trigger actions to happen when an event occurs.

#### Date Picked

This event fires when the user has selected a date using the Date Picker.

![](<../../../.gitbook/assets/dp1-8 (1).png>)

### Functions

#### Get Date&#x20;

Returns full date from Date Picker in format Mon., DD, YYYY.

![](../../../.gitbook/assets/f\_get\_date.png)

#### Get Day&#x20;

Returns date from Date Picker in numeric form.

Eg. If February 17, 2021 has been selected in Date Picker, this block will return 17. \
If 5 March 2021 is selected in Date Picker, this block will return 5.

![](../../../.gitbook/assets/f\_get\_day.png)

#### Get Month&#x20;

Returns date from Date Picker in numeric form.

Eg. If February 17, 2021 has been selected in Date Picker, this block will return 2. \
If 7 November 2021 is selected in Date Picker, this block will return 11.

![](../../../.gitbook/assets/f\_get\_month.png)

#### Get Year&#x20;

Returns date from Date Picker in YYYY form.

![](../../../.gitbook/assets/f\_get\_year.png)

#### Launch Picker

Opens Picker of the Date Input to prompt the user to enter a date.

![](../../../.gitbook/assets/f\_launch\_picker.png)

### &#x20;Properties

Set and get [properties](date-input.md#properties) of the Date Picker.

#### Background Color&#x20;

![](<../../../.gitbook/assets/bg\_color (3).png>)

#### Color&#x20;

![](<../../../.gitbook/assets/color (1).png>)

#### Computed Height and Width&#x20;

![](../../../.gitbook/assets/comp\_height.png)

Returns the height/width of the Date Input on the device screen in pixels.

#### Font Size&#x20;

![](<../../../.gitbook/assets/font\_size (2).png>)

#### Font Style&#x20;

![](<../../../.gitbook/assets/font\_style (1).png>)

#### Font Weight&#x20;

![](<../../../.gitbook/assets/font\_weight (2).png>)

#### Style&#x20;

![](../../../.gitbook/assets/dp1-2.png)

#### Text Align&#x20;

![](<../../../.gitbook/assets/text\_align (2).png>)

Set the Text Alignment of the Date Input to `Auto`, `Left`, `Right`, `Center` or `Justify`.

#### Visible

![](<../../../.gitbook/assets/visible (7).png>)
