# Date Input

## Date Input Overview

* [Getting Started](date-input.md#getting-started)
* [Set the Date Format](date-input.md#set-the-date-format)
* [Save the Date](date-input.md#save-the-date)
* [Events](date-input.md#events)
* [Functions](date-input.md#functions)
* [Properties](date-input.md#properties)

A Date Input component is helpful when you want the user of your app to easily select a specific date using the native Android or iOS date picker

![Native Android Date Picker on the left and iOS on the right](.gitbook/assets/thunkable-docs-exhibits-37.png)

## Getting Started 

The Date Input component needs no set-up \(Woohoo!\). Just drag and drop the component into your project. As a bonus, the current date will automatically show up as a label.

When a user of your app taps on the Date Input, it will automatically launch the native Android or iOS date pickers.

## Set the Date Format

You can set the format of the date by choosing an option from the `Style` property. Currently supported styles are:

* YYYY-MM-DD
* MM/DD/YYYY
* M/D/YY
* Month Day, Year
* Mth. Day, Year

![](.gitbook/assets/date_input_style.png)

## Save the Date

The date that a user selects will show up automatically in the Date Input label but if you want to save the date somewhere to be uploaded later, you'll need to add a block like the one below. 

![](.gitbook/assets/get_date.png)

| Event | Output |
| :--- | :--- |
| Get Date | Date in whichever format you specify e.g. `YYYY-MM-DD` |
| Get Year | Year in 4 digit format e.g. `2019` |
| Get Month | Numerical month from `1-12` |
| Get Day | Day of the month from `1-31` \(depending on the month\) |

## Events

### Date Picked

![](.gitbook/assets/dp1-8%20%281%29.png)

## Functions

### Get Date 

![](.gitbook/assets/f_get_date.png)

### Get Day 

![](.gitbook/assets/f_get_day.png)

### Get Month 

![](.gitbook/assets/f_get_month.png)

### Get Year 

![](.gitbook/assets/f_get_year.png)

### Launch Picker

![](.gitbook/assets/f_launch_picker.png)

##  Properties

### Background Color 

![](.gitbook/assets/bg_color%20%283%29.png)

### Color 

![](.gitbook/assets/color%20%281%29.png)

### Computed Height and Width 

![](.gitbook/assets/comp_height.png)

### Font Size 

![](.gitbook/assets/font_size%20%282%29.png)

### Font Style 

![](.gitbook/assets/font_style%20%281%29.png)

### Font Weight 

![](.gitbook/assets/font_weight%20%282%29.png)

### Style 

![](.gitbook/assets/dp1-2.png)

### Text Align 

![](.gitbook/assets/text_align%20%282%29.png)

### Visible

![](.gitbook/assets/visible%20%287%29.png)

