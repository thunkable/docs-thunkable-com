# Time Input

A Time Input component is helpful when you want the user of your app to easily select a specific time using the native Android or iOS date picker

![Native Android Time Picker on the left and iOS on the right](.gitbook/assets/thunkable-docs-exhibits-38%20%281%29.png)

## Getting Started 

The Time Input component needs no set-up \(Woohoo!\). Just drag and drop the component into your project. As a bonus, the current time will automatically show up as a label.

When a user of your app taps on the Date Input, it will automatically launch the native Android or iOS date pickers.

## Set the time format

You can set the format of the time by simply choosing your desired format from the `Style` property

![](.gitbook/assets/screen-shot-2019-09-04-at-5.15.39-pm.png)

## Save the time

The time that a user selects will show up automatically in the Time Input label but if you want to save the date somewhere to be uploaded later, you'll need to add a block like the one below. 

![](.gitbook/assets/screen-shot-2019-09-04-at-4.43.02-pm.png)

| Event Property | Output |
| :--- | :--- |
| Get Time | Date in whichever format you specify  |
| Get Hours | Hour of the Day from `1-24` |
| Get Minutes | Minutes from `1-60` |

