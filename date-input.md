# Date Input

{% hint style="info" %}
This component has not yet been released but will be available soon
{% endhint %}

Date Input components are helpful when you want the user of your app to easily select a specific date using the native Android or iOS date picker

![Native Android Date Picker on the left and iOS on the right](.gitbook/assets/thunkable-docs-exhibits-37.png)

## Set up 

The Date Input component is only surfaced after you have triggered it from another event so you'll need to select the event using an event block like the one below.

After the user has selected a date, you will get the following outputs which you can format however you choose

| Property | Output |
| :--- | :--- |
| Year | Year in 4 digit format e.g. `2019` |
| Month | Numerical month from `1-12` |
| Day | Day of the month from `1-31` \(depending on the month |

![](.gitbook/assets/screen-shot-2019-08-28-at-3.58.25-pm.png)



