# Checkbox

## Checkbox Overview​ <a href="#switch-overview" id="switch-overview"></a>

A Checkbox is a component that has two settings, true and false. You can get your app to do specific tasks based on the value of the Checkbox.

![Examples of uncheck and checked Checkboxes](<.gitbook/assets/Screen Shot 2022-05-04 at 10.56.57 AM.png>)

## Properties <a href="#getting-started" id="getting-started"></a>

### Checkbox

| Property Name | Description                                        | Data Type  |
| ------------- | -------------------------------------------------- | ---------- |
| Value         | Initial value of Checkbox                          | True/False |
| Disabled      | Toggle whether value Switch can be changed by user | True/False |
| Color         | Color of background when Checkbox is **checked**   | Color      |

### Layout

| Property | Description                                                                        | Data Type  |
| -------- | ---------------------------------------------------------------------------------- | ---------- |
| X        | Location of top left corner of Checkbox on X-axis, where the left hand side is X=0 | Number     |
| Y        | Location of top left corner of Checkbox on Y-axis, where the top side is Y=0       | Number     |
| Height   | Height of Checkbox in pixels                                                       | Number     |
| Width    | Width of Checkbox in pixels                                                        | Number     |
| Visible  | Toggle whether your end users can see the Checkbox                                 | True/False |

## Blocks <a href="#events" id="events"></a>

### Events&#x20;

#### Value Changes

This event fires every time the value of the Checkbox is changed.

Returns `newValue` output block, which returns the new value of the Checkbox (`true` or `false`).

### Properties

Use these blocks to set and get the named [properties](checkbox.md#getting-started) of the Checkbox.

#### Value&#x20;

Set and get the Value of the Checkbox

#### Color&#x20;

Set and get the Color of the Checkbox

#### Disabled&#x20;

Set and get the Disabled property of the Checkbox

#### Visible&#x20;

Set and get the Visible property of the Checkbox
