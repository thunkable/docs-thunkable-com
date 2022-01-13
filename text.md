# Text

## Text Value

### String

The most basic but most often used text block is below. You can type into this text block, or leave it empty.

![](.gitbook/assets/text-str.png)

### Join

Often, you'll want to join text values together with the `join` block:

![](.gitbook/assets/text-join.png)

### Newline

You can use the `newline` block to add a line break in a piece of text.

![](.gitbook/assets/textblocks-newline.png)

## Reformat Text

Use these blocks to change the content or formatting of your text. These blocks will return the reformatted text.

### Set case

Set a piece of text to the selected case:

![](.gitbook/assets/text-case.png)

### Trim Spaces

Trim blank spaces from the left side, the right side, or both sides of a string of text:

![](.gitbook/assets/text-trim.png)

### Replace all

Find and replace all occurrences of a substring within a string.

![](.gitbook/assets/textblocks-replace.png)

## Analyze Text

### Is Empty

The block below tests whether the text value is empty. Returns `true` or `false`

![](.gitbook/assets/text-empty.png)

### Get letter

Returns the character at the specified position, where 1 is the first letter of the string.\
Returns the empty string if the length of text given is less than the position specified.

![](.gitbook/assets/text-get;etter.png)

### Get substring

Returns the substring at the specified start and end position, where 1 is the first letter of the string.\
Returns the empty string if the length of text given is less than the starting position specified.

![](.gitbook/assets/text-substr1.png)

![](.gitbook/assets/text-substr2.png)

### Find first/last occurrence

Returns the starting position of a substring within a string, where 1 is the first letter of the string.\
Returns 0 if the string does not contain the substring.

![](.gitbook/assets/text-first.png)

### Does string contain

Checks if a string contains a substring. Returns `true` or `false`.&#x20;

![](.gitbook/assets/textblocks-does-contain.png)

### Get length of string

Returns length of a given string as a number

![](.gitbook/assets/text-length.png)
