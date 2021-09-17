# Date Input

## Date Input Overview

A Date Input component is helpful when you want the user of your app to easily select a specific date using the native Android or iOS date picker

![Native Android Date Picker on the left and iOS on the right](.gitbook/assets/thunkable-docs-exhibits-37.png)

## Properties

### Date Input

| Property | Description | Data Type |
| :--- | :--- | :--- |
| Style | Format to use when displaying selected date | Select from menu |
| Font Size | Size of font when displaying date | Number |
| Font Style | Select whether font is normal or italic | Select from menu |
| Font Weight | Set boldness of font | Select from menu |
| Color | Color of font when displaying date | Color |

The following formats are currently available to use as `Style:`

* YYYY-MM-DD
* MM/DD/YYYY
* M/D/YY
* Month Day, Year
* Mth. Day, Year

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

## Blocks

### Events

You can trigger actions to happen when an event occurs.

#### Date Picked

This event fires when the user has selected a date using the Date Picker.

![](.gitbook/assets/dp1-8%20%281%29.png)

### Functions

#### Get Date 

Returns full date from Date Picker in format Mon., DD, YYYY.

![](.gitbook/assets/f_get_date.png)

#### Get Day 

Returns date from Date Picker in numeric form.

Eg. If February 17, 2021 has been selected in Date Picker, this block will return 17.   
If 5 March 2021 is selected in Date Picker, this block will return 5.

![](.gitbook/assets/f_get_day.png)

#### Get Month 

Returns date from Date Picker in numeric form.

Eg. If February 17, 2021 has been selected in Date Picker, this block will return 2.   
If 7 November 2021 is selected in Date Picker, this block will return 11.

![](.gitbook/assets/f_get_month.png)

#### Get Year 

Returns date from Date Picker in YYYY form.

![](.gitbook/assets/f_get_year.png)

#### Launch Picker

Opens Picker of the Date Input to prompt the user to enter a date.

![](.gitbook/assets/f_launch_picker.png)

###  Properties

Set and get [properties](date-input.md#properties) of the Date Picker.

#### Background Color 

![](.gitbook/assets/bg_color%20%283%29.png)

#### Color 

![](.gitbook/assets/color%20%281%29.png)

#### Computed Height and Width 

![](.gitbook/assets/comp_height.png)

Returns the height/width of the Date Input on the device screen in pixels.

#### Font Size 

![](.gitbook/assets/font_size%20%282%29.png)

#### Font Style 

![](.gitbook/assets/font_style%20%281%29.png)

#### Font Weight 

![](.gitbook/assets/font_weight%20%282%29.png)

#### Style 

![](.gitbook/assets/dp1-2.png)

#### Text Align 

![](.gitbook/assets/text_align%20%282%29.png)

Set the Text Alignment of the Date Input to `Auto`, `Left`, `Right`, `Center` or `Justify`.

#### Visible

![](.gitbook/assets/visible%20%287%29.png)

