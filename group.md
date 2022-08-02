# Group

A Group is a container component.

You can place [User Interface](ui-components.md) components inside a Group to make changing the appearance of your app easier.

## Add Components to Group

To add components to a Group, simply drag and drop the components inside the Group.

You will see the components you added to the Group are now nestled inside the Group in the component tree.

## Moving Groups in Your Project

When a group that contains UI Component(s) is moved, its content are moved with it as a unit.

This makes it easier to design complex layouts.

## Properties

### Group

| Property      | Description                                                                         | Data Type                                                   |
| ------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------- |
| Position      | Set whether the Group is positioned Relative to the Screen or Relative to Device ¹  | Select from menu: \[Relative to Screen, Relative to Device] |
| Touch Opacity | Set opacity of Group when user clicks on Group                                      | Number between 0-100                                        |

¹ Relative to Screen: Group moves as end user scrolls\
Relative to Device: Group stays in place as end user scrolls

² Stretch: Resize Group in proportion with wider Screen\
Float in Place: Keep same dimensions for Group on larger screens

### Layout

| Property    | Description                                                             | Data Type                                   |
| ----------- | ----------------------------------------------------------------------- | ------------------------------------------- |
| X           | Position of top left corner of Group on X-axis                          | Number                                      |
| Y           | Position of top left corner of Group on Y-axis                          | Number                                      |
| Height      | Height of Group in pixels                                               | Number                                      |
| Width       | Width of Group in pixels                                                | Number                                      |
| Resize Mode | Set how Group is resized on wider screens - Stretch or Float in Place ² | Select from menu: \[Resize, Float in Place] |

### Style

| Property                     | Description                                                                                         | Data Type                                                                                                                                                                                                    |
| ---------------------------- | --------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Visible                      | Set whether Group is shown on screen                                                                | True/False                                                                                                                                                                                                   |
| Background Fill              | Color of Group's background                                                                         | Color                                                                                                                                                                                                        |
| Background Image             | The image file to be shown in the Group's background                                                | <p>PNG, JPG, GIF, SVG, etc.<br>Can also use URL that ends in file extension (eg <a href="https://thunkable.com/static/media/logo.ba96eb83.png">https://thunkable.com/static/media/logo.ba96eb83.png</a>)</p> |
| Background Image Resize Mode | Set how picture is shown if the file and the Image component have different dimensions/aspect ratio | Select from list `[cover, contain, stretch, repeat, center]`                                                                                                                                                 |
| Border Style                 | Style of Group's border                                                                             | Select from list `[solid, dotted, dashed]`                                                                                                                                                                   |
| Border Color                 | Color of Group's border                                                                             | Color                                                                                                                                                                                                        |
| Border Width                 | Width of Group's border in pixels                                                                   | Number                                                                                                                                                                                                       |
| Border Radius                | Radius of corners of Group's border in pixels                                                       | Number                                                                                                                                                                                                       |
| Shadow Color                 | Color of Group's shadow                                                                             | Color                                                                                                                                                                                                        |
| Shadow Opacity               | Opacity of Group's shadow                                                                           | Number between 0 and 100                                                                                                                                                                                     |
| Shadow Radius                | Radius of corners of Group's shadow in pixels                                                       | Number                                                                                                                                                                                                       |
| Shadow Offset                | How far Group's shadow should be offset, in Height and Width, in pixels                             | Number                                                                                                                                                                                                       |

## Blocks

### Events

You can use the following blocks to listen for when a specific event occurs

#### Click

Performs an action when the user taps the Group.

### Properties

Set and get the [properties](group.md#properties) of the Group.

#### Background Color

Set and get the Background Color of the Group.

#### Background Picture

Set and get the Background Picture of the Group.

#### Background Picture Resize Mode

Set and get the Background Picture Resize Mode of the Group.

#### Computed Height

Get the height of the of the Group as it appears in-screen in pixels.

#### Visible

Set and get the Visible property of the Group.

#### Computed Width

Get the width of the of the Group as it appears in-screen in pixels.

