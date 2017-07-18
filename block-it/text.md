#### **Thunkable for Android **❤

# Text

---

Text blocks are essential for any app functions that uses, retrieves, stores and transforming text into usable formats for your app

* [Basic text](#basic-text)

* [Reformat text](#reformat-text)

* [Conditionals with text](#conditionals-with-text)

* [Text calculators](#text-calculators)

---

#### Basic text

![](/assets/text-block-1.png)

`Contains a text string.`

`This string can contain any characters (letters, numbers, or other special characters). On Thunkable it will be considered a Text object`

---

#### Reformat text

![](/assets/text-block-2.png)

\(a\) ![](/assets/text-block-3.png)\(b\) ![](/assets/text-block-7.png)\(c\) ![](/assets/text-block-9.png)\(d\)![](/assets/text-block-8.png)\(e\)![](/assets/text-block-11.png)   
\(f\) ![](/assets/text-block-12.png)\(g\) ![](/assets/text-block-13.png)\(h\) ![](/assets/text-block-14.png)

\(a\) **Join **`Appends all of the inputs to make a single string. If no inputs, returns an empty string`

\(b\) **Trim **`Removes any spaces leading or trailing the input string and returns the result`

\(c\) **Split **`Divides text into pieces using at as the dividing points and produces a list of the results. Splitting one, two, three, four at, (comma) returns the list one two three four. Splitting one-potato, two-potato, three-potato, four at-potato, returns the list one two three four`

\(d\) **Split at first **`Divides the given text into two pieces using the location of the first occurrence of at as the dividing point, and returns a two-item list consisting of the piece before the dividing point and the piece after the dividing point. Splitting apple, banana, cherry, dogfood with a comma as the splitting point returns a list of two items: the first is the text apple and the second is the text banana, cherry, dogfood. Notice that the comma after apple doesn't appear in the result, because that is the dividing point`

\(e\) **Split at any / first to a list **`Divides the given text into a two-item list, using the first location of any item in the list at as the dividing point. Splitting i love apples bananas apples grapes by the list [ba,ap] would result in a list of two items the first being i love and the second ples bananas apples grapes`

\(f\) **Split at spaces **`Divides the given text at any occurrence of a space, producing a list of the pieces`

\(g\) **Segment **`Extracts part of the text starting at start position and continuing for length characters`

\(h\) **Replace** `Returns a new text string obtained by replacing all occurrences of the substring with the replacement. Replace all with She loves eating. She loves writing. She loves coding as the text,She as the segment, and Hannah as the replacement would result in Hannah loves eating. Hannah loves writing. Hannah loves coding.`

---

#### Conditionals with text

\(a\) ![](/assets/text-block-5.png)\(b\) ![](/assets/text-block-6.png)

\(a\) Less than, equal or greater than 

---

#### Text calculators

\(a\) ![](/assets/text-block-4.png)\(b\)

