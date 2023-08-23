---
description: >-
  The text input allows the person using your app to type in anything that they
  want such as words, passwords or numbers.
---

# Text Input Component

## Text Input Overview

![](../../../.gitbook/assets/text-input-fig-1.png)

## Properties

### Text Input

| Property                                 | Description                                                                                                              | Data Type                                                       |
| ---------------------------------------- | ------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------- |
| Hint                                     | The prompt text the user sees when the Text Input is empty (eg. `Type Here`)                                             | Text                                                            |
| Text                                     | Text value of the Text Input                                                                                             | Text                                                            |
| Keyboard                                 | Set a keyboard to sppear when your end user clicks the Text Input                                                        | Select from list `[default, email address, numeric, phone pad]` |
| Secure Text Entry                        | Toggle whether text is obscured as your end user types (suitable for entering passwords and other sensitive information) | True/False                                                      |
| Font                                     | Set the font for the Hint and Text properties. Options can be found here: [Google Fonts](https://fonts.google.com/).     | Text                                                            |
| Font Italic (web app only)               | Select whether hint and text are shown in italics_._                                                                     | True/False                                                      |
| Underline (web app only)                 | Select whether the hint and text are underlined.                                                                         | True/False                                                      |
| Strikethrough (web app only)             | Apply strikethrough formatting to the hint and text.                                                                     | True/False                                                      |
| Writing Direction (iOS and web app only) | Set whether text should be written left-to-right or right-to-left.                                                       | Select from icons.                                              |
| Font Size                                | Height of hint and text in pixels.                                                                                       | Number                                                          |
| Letter Spacing                           | Spacing between letters in pixels.                                                                                       | Number                                                          |

### Advanced Properties

| Property                               | Description                                                                   | Data Type                                                         |
| -------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| Editable                               | Toggle whether your end user can edit the text                                | True/False                                                        |
| Multiline                              | Toggle whether your end user can enter multiple lines of text                 | True/False                                                        |
| Auto Focus                             | Toggle whether Text Input is automatically in focus when the Screen opens     | True/False                                                        |
| Max Length (Android and iOS only)      | Set maximum number of lines of text your end user can enter                   | Number                                                            |
| Clear Button Mode (iOS only)           | Toggle when your iOS end users have the option to clear the Text Input's text | Select from list `[never, while-editing, unless-editing, always]` |
| Input Color                            | Color of Text Input's Text                                                    | Color                                                             |
| Background Color                       | Color of Text Input's background                                              | Color                                                             |
| Hint Text Color                        | Color of Text Input's hint                                                    | Color                                                             |
| Selection Color (Android and iOS only) | Set the color to highlight text when your end user selects text               | Color                                                             |

### Layout

| Property    | Description                                                 | Data Type                                    |
| ----------- | ----------------------------------------------------------- | -------------------------------------------- |
| X           | Set the location of your Text Input the X-axis in pixels    | Number                                       |
| Y           | Set the location of your Text Input on the Y-axis in pixels | Number                                       |
| Height      | Set the Height of your Text Input in pixels                 | Number                                       |
| Width       | Set the Width of your Text Input in pixels                  | Number                                       |
| Resize Mode | Define dimensions of the text input component/container     | Select from list `[Stretch, Float in Place]` |

### Style

| Property       | Description                                                                  | Data Type                                  |
| -------------- | ---------------------------------------------------------------------------- | ------------------------------------------ |
| Visible        | Toggle whether your end users can see the Text Input                         | True/False                                 |
| Border Style   | Style of Text Input's border                                                 | Select from list `[solid, dotted, dashed]` |
| Border Color   | Color of Text Input's border                                                 | Color                                      |
| Border Width   | Width of Text Input's border in pixels                                       | Number                                     |
| Border Radius  | Radius of corners of Text Input's border in pixels                           | Number                                     |
| Shadow Color   | Color of Text Input's shadow                                                 | Color                                      |
| Shadow Opacity | Opacity of Text Input's shadow                                               | Number between 0 and 100                   |
| Shadow Radius  | Radius of corners of Text Input's shadow in pixels                           | Number                                     |
| Shadow Offset  | How far Text Input's shadow should be offset, in Height and Width, in pixels | Number                                     |

## Blocks

### Events

#### Click

![](../../../.gitbook/assets/ti\_click.png)

This event fires when the user clicks on the Text Input component.

#### Unfocus&#x20;

![](../../../.gitbook/assets/ti\_unfocus.png)

This event fires when the component looses focus, i.e the user clicks on another component.

#### Submit&#x20;

![](../../../.gitbook/assets/ti\_submit.png)

This event fires when the enter or submit button is pressed on the device keyboard.

#### Changes

![](../../../.gitbook/assets/ti\_changes.png)

This event fires every time a character is added or removed to the Text Input.

### Properties

#### Border Width

![](../../../.gitbook/assets/boder\_width.png)

Set and get the Text Input's [border width.](text-input.md#style)

#### Height&#x20;

![](../../../.gitbook/assets/tih.png)

Returns the height of the Text Input component in pixels after it has been rendered on-screen.

#### Hint&#x20;

![](../../../.gitbook/assets/tihi.png)

Set and get the Text Input's [Hint text](text-input.md#text-input).

#### Keyboard Type&#x20;

![](../../../.gitbook/assets/keyboard.png)

Set and get the Text Input's [keyboard type](text-input.md#text-input).

#### Text&#x20;

![](<../../../.gitbook/assets/text (1).png>)

Set and get the Text Input's [Text](text-input.md#text-input).

#### Visible&#x20;

![](<../../../.gitbook/assets/visible (2).png>)

Set and get the Text Input's [visibility](text-input.md#layout).&#x20;

#### Width

![](../../../.gitbook/assets/tiw.png)



Returns the width of the Text Input component in pixels after it has been rendered on-screen.