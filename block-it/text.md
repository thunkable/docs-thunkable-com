#### **Thunkable for Android **❤

# Text

---

Text blocks are essential for any app functions that uses, retrieves, stores and transforms text into usable formats for your app

* [Basic text](#basic-text)
* [Reformat text](#reformat-text)
* [Conditionals with text](#conditionals-with-text)
* [Text calculations](#text-calculations)

---

#### Basic text

![](/assets/text-block-1.png)

Contains a text string.

This string can contain any characters \(letters, numbers, or other special characters\). On Thunkable it will be considered a Text object

---

#### Reformat text

![](/assets/text-block-2.png)

\(a\) ![](/assets/text-block-3.png)\(b\) ![](/assets/text-block-7.png)\(c\) ![](/assets/text-block-9.png)\(d\)![](/assets/text-block-8.png)\(e\)![](/assets/text-block-11.png)  
\(f\) ![](/assets/text-block-12.png)\(g\) ![](/assets/text-block-13.png)\(h\) ![](/assets/text-block-14.png)\(i\) ![](/assets/text-block-15.png)\(j\) ![](/assets/text-block-16.png)

\(a\) **Join **Appends all of the inputs to make a single string. If no inputs, returns an empty string

\(b\) **Trim **Removes any spaces leading or trailing the input string and returns the result

\(c\) **Split **Divides text into pieces using at as the dividing points and produces a list of the results. Splitting `one, two, three, four` at  `,(comma)` returns the list `one two three four`. Splitting `one-potato, two-potato, three-potato, four` at `-potato`, returns the list `one two three four`

\(d\) **Split at first **Divides the given text into two pieces using the location of the first occurrence of at as the dividing point, and returns a two-item list consisting of the piece before the dividing point and the piece after the dividing point. Splitting `apple, banana, cherry, dogfood` with `a comma` as the splitting point returns a list of two items: the first is the text `apple` and the second is the text `banana, cherry, dogfood`. Notice that the comma after apple doesn't appear in the result, because that is the dividing point

\(e\) **Split at any / first to a list **Divides the given text into a list, using any of the items in at as the dividing point, and returns a list of the results. Splitting `appleberry,banana,cherry,dogfood`_ \_with at as the two-element list whose first item is a comma and whose second item is _`rry` \_returns a list of four items: `applebe, banana, che, dogfood`

\(f\) **Split at spaces **Divides the given text at any occurrence of a `space`, producing a list of the pieces

\(g\) **Segment **Extracts part of the `text` starting at `start` position and continuing for `length` characters

\(h\) **Replace** Returns a new `text` string obtained by replacing all occurrences of the `segment` with the `replacement`.

\(i\) **Uppercase **Returns a copy of its text string argument converted to all upper case

\(j\) **Lowercase **Returns a copy of its text string argument converted to all lower case

---

#### Conditionals with text

\(a\) ![](/assets/text-block-5.png)\(b\) ![](/assets/text-block-6.png)\(c\) ![](/assets/text-block-17.png)

\(a\) **Compare** **texts** Returns whether or not the first string is lexicographically `<, >, or =` the second string depending on which dropdown is selected A string a considered lexicographically greater than another if it is alphabetically greater than the other string. Essentially, it would come after it in the dictionary. All uppercase letters are considered smaller or to occur before lowercase letters. cat would be &gt;Cat

\(b\) **Contains specific text **Returns true if `piece` appears in text; otherwise, returns false

\(c\) **Is empty **Returns whether or not the string contains any characters \(including spaces\). When the string length is 0, returns true otherwise it returns false

---

#### Text calculations

\(a\) ![](/assets/text-block-4.png)\(b\) ![](/assets/text-block-18.png)

\(a\) **Length of text **Returns the number of characters including spaces in the string. This is the length of the given text string

\(b\) **Character position **Returns the character position where the first character of piece first appears in text, or 0 if not present. For example, the location of `ana` in `havana banana` is 4

