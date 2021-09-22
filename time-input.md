# Time Input

## Time Input Overview

A Time Input component is helpful when you want the user of your app to easily select a specific time using the native Android or iOS date picker

![Native Android Time Picker on the left and iOS on the right](.gitbook/assets/thunkable-docs-exhibits-38%20%281%29.png)

## Properties

### Time Input

| Property | Description | Data Type |
| :--- | :--- | :--- |
| Style | Format to use when displaying selected date | Select from menu |
| Font Size | Size of font when displaying date | Number |
| Font Style | Select whether font is normal or italic | Select from menu |
| Font Weight | Set boldness of font | Select from menu |
| Color | Color of font when displaying date | Color |

The following formats are currently available to use as `Style:`

* Hour:Minute AM/PM, eg. `3:30 PM`
* Hour:Minute 24h, eg. `15:30`

### Layout

| Property | Description | Data Type |
| :--- | :--- | :--- |
| X | Location of top left corner of Web Viewer on X-axis, where the left hand side is X=0 | Number |
| Y | Location of top left corner of Web Viewer on Y-axis, where the top side is Y=0 | Number |
| Height | Height of Web Viewer in pixels | Number |
| Width | Width of Web Viewer in pixels | Number |
| Visible | Set whether the Web Viewer is visible | True/False |

### **Style**

| **Property** | Description | Data Type |
| :--- | :--- | :--- |
| Border Width | Width of border around Web Viewer in pixels | Number |
| Border Radius | Radius of corners of border on Web Viewer in degrees | Number |
| Border Color | Color of border \(only visible if border width &gt; 0\) | Color |
| Border Style | Set whether border style is solid, dotted or dashed  \(only visible if border width &gt; 0\) | Select from menu |

## 

## Save the time

The time that a user selects will show up automatically in the Time Input label but if you want to save the date somewhere to be uploaded later, you'll need to add a block like the one below. 

![](.gitbook/assets/screen-shot-2019-09-04-at-4.43.02-pm.png)

| Event Property | Output |
| :--- | :--- |
| Get Time | Date in whichever format you specify  |
| Get Hours | Hour of the Day from `1-24` |
| Get Minutes | Minutes from `1-60` |

## Blocks

### Events

#### Time Picked

Fires when the user has selected a time with the Time Input

![](.gitbook/assets/e_time_picked.png)

### Functions

#### Launch Picker

Launches the Time Input picker for the user to select a time.

![](.gitbook/assets/f_launch.png)

#### Get Hour 

Returns the hour of the currently selected time in 24 hour format.

Example: if the user selects 2:30 PM, this block will return 14.

![](.gitbook/assets/f_get_hour.png)

#### Get Minute 

Returns the minute of the currently selected time.

Example: if the user selects 2:30 PM, this block will return 30.

![](.gitbook/assets/f_get_min.png)

#### Get Time 

Returns the selected time in the same format as the Style [property](time-input.md#time-input) of the Time Input.

Example: if the user selects 2:30 PM, and the Style is set to Hour:Minute AM/PM, this block will return 2:30 PM.

If the user selects 2:30 PM, and the Style is set to Hour:Minute 24h, this block will return 14:30.

![](.gitbook/assets/f_get_time.png)

### Properties

Set and get [properties](time-input.md#properties) of the Time Input

#### Style

![](.gitbook/assets/style.png)

#### Computed Height and Width 

Returns the height/width of the Date Input on the device screen in pixels.

![](.gitbook/assets/comp.png)

#### Visible

![](.gitbook/assets/visible%20%286%29.png)

#### Font Size 

![](.gitbook/assets/font_size%20%284%29.png)

#### Color 

![](.gitbook/assets/color%20%283%29.png)

#### Background Color 

Set the background color of the Time Input as it is displayed in the project.

![](.gitbook/assets/bg_color%20%284%29.png)

#### Font Style 

![](.gitbook/assets/font_style%20%282%29.png)

#### Font Weight 

![](.gitbook/assets/font_weight%20%281%29.png)

#### Text Align 

Set the Text Alignment of the Time Input to `Auto`, `Left`, `Right`, `Center` or `Justify`.

![](.gitbook/assets/text_align%20%281%29.png)



