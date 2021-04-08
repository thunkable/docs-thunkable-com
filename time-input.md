# Time Input

## Time Input Overview

* [Getting Started](time-input.md#getting-started)
* [Set the Time Format](time-input.md#set-the-time-format)
* [Save the Time](time-input.md#save-the-time)
* [Events](time-input.md#events)
* [Functions](time-input.md#functions)
* [Properties](time-input.md#properties)

A Time Input component is helpful when you want the user of your app to easily select a specific time using the native Android or iOS date picker

![Native Android Time Picker on the left and iOS on the right](.gitbook/assets/thunkable-docs-exhibits-38%20%281%29.png)

## Getting Started 

The Time Input component needs no set-up \(Woohoo!\). Just drag and drop the component into your project. As a bonus, the current time will automatically show up as a label.

When a user of your app taps on the Date Input, it will automatically launch the native Android or iOS date pickers.

## Set the time format

You can set the format of the time by simply choosing your desired format from the `Style` property

![](.gitbook/assets/screen-shot-2021-04-08-at-4.58.31-pm.png)

## Save the time

The time that a user selects will show up automatically in the Time Input label but if you want to save the date somewhere to be uploaded later, you'll need to add a block like the one below. 

![](.gitbook/assets/screen-shot-2019-09-04-at-4.43.02-pm.png)

| Event Property | Output |
| :--- | :--- |
| Get Time | Date in whichever format you specify  |
| Get Hours | Hour of the Day from `1-24` |
| Get Minutes | Minutes from `1-60` |

## Events

### Time Picked

![](.gitbook/assets/e_time_picked.png)

## Functions

### Get Hour 

![](.gitbook/assets/f_get_hour.png)

### Get Minute 

![](.gitbook/assets/f_get_min.png)

### Get Time 

![](.gitbook/assets/f_get_time.png)

### Launch Picker

![](.gitbook/assets/f_launch.png)

## Properties

### Background Color 

![](.gitbook/assets/bg_color%20%284%29.png)

### Color 

![](.gitbook/assets/color%20%283%29.png)

### Computed Height and Width 

![](.gitbook/assets/comp.png)

### Font Size 

![](.gitbook/assets/font_size%20%284%29.png)

### Font Style 

![](.gitbook/assets/font_style%20%282%29.png)

### Font Weight 

![](.gitbook/assets/font_weight%20%281%29.png)

### Style

###  

![](.gitbook/assets/style.png)

### Text Align 

![](.gitbook/assets/text_align%20%281%29.png)

### Visible

![](.gitbook/assets/visible%20%286%29.png)





