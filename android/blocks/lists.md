#### **Thunkable for Android **❤

# Lists

---

Many apps use lists of data for everything from drop down menus to game scores. List blocks are used for creating and managing lists, selecting from a list, placing conditionals on specified app events and even introducing randomness into your app

* [Create a list](#create-a-list)
* [Manage a list](#manage-a-list)
* [Select from a list](#select-from-a-list)
* [Conditionals with lists](#conditionals-with-lists)
* [List calculations](#list-calculations)
* [Introduce randomness](#introduce-randomness)

---

#### Create a list

\(a\) ![](/assets/list-block-1.png)\(b\)![](/assets/list-block-2.png)

\(a\) **Empty list** Creates an empty list with no elements

\(b\)** Makes a list** Creates a list from the given blocks. If you don't supply any arguments, this creates an empty list, which you can add elements to later

---

#### Manage a list

\(a\) ![](/assets/list-block-3.png)\(b\) ![](/assets/list-block-10.png)\(c\) ![](/assets/list-block-11.png)

\(a\) **Add items to a list **Adds the given `items` to the end of the `list`. The difference between this and append to list is that append to list takes the items to be appended as a single list while add items to list takes the items as individual arguments

\(b\) **Insert into a list** Inserts an `item` into the list at the given position

\(c\) **Replace **Inserts `replacement` into the given `list` at position `index`. The previous item at that position is removed

\(d\) ![](/assets/list-block-12.png)\(e\) ![](/assets/list-block-14.png)\(f\) ![](/assets/list-block-13.png)

\(d\) **Remove** Removes the `item` at the given position

\(e\) **Append** Adds the items in the `second list` to the end of the `first list`

\(f\) **Copy list **Makes a copy of a `list`, including copying all sublists

\(g\) ![](/assets/list-block-17.png)\(h\) ![](/assets/list-block-18.png)\(i\) ![](/assets/list-block-19.png)\(j\) ![](/assets/list-block-20.png)

\(g\) **List to csv row** Interprets the `list` as a row of a table and returns a CSV \(comma-separated value\) text representing the row. Each item in the row list is considered to be a field, and is quoted with double-quotes in the resulting CSV text. Items are separated by commas.For example, converting the list \(a b c d\) to a CSV row produces \("a", "b", "c", "d"\). The returned row text does not have a line separator at the end

\(h\) **List from csv row **Parses a `text `as a CSV \(comma-separated value\) formatted row to produce a list of fields. For example, converting \("a", "b", "c", "d"\) to a list produces \(a b c d\)

\(i\) **List to csv table** Interprets the `list` as a table in row-major format and returns a CSV \(comma-separated value\) text representing the table. Each item in the list should itself be a list representing a row of the CSV table. Each item in the row list is considered to be a field, and is quoted with double-quotes in the resulting CSV text. In the returned text, items in rows are separated by commas and rows are separated by CRLF \(\r\n\)

\(j\) **List from csv table **Parses a `text` as a CSV \(comma-separated value\) formatted table to produce a list of rows, each of which is a list of fields.Rows can be separated by newlines \(\n\) or CRLF \(\r\n\)

---

#### Select from a list

\(a\) ![](/assets/list-block-9.png)\(b\) ![](/assets/list-block-16.png)

\(a\) **Select from list** Selects the item at the given `index` in the given `list`. The first list item is at index 1

\(b\) **Pair lookup \(similar to vlookup\)** Used for looking up information in a dictionary-like structure represented as a list. This operation takes three inputs, a `key`, a list `pairs`, and a `notFound`result, which by default, is set to "not found". Here `pairs`must be a list of pairs, that is, a list where each element is itself a list of two elements. Lookup in pairs finds the first pair in the list whose first element is the key, and returns the second element. For example, if the list is \(\(a apple\) \(d dragon\) \(b boxcar\) \(cat 100\)\) then looking up 'b' will return 'boxcar'. If there is no such pair in the list, then the lookup in pairs will return the `notFound`result. If pairs is not a list of pairs, then the operation will signal an error

---

#### Conditionals with lists

\(a\) ![](/assets/list-block-5.png)\(b\) ![](/assets/list-block-15.png)

\(a\) **Is in list?** If `thing` is one of the elements of the `list`, returns true; otherwise, returns false. Note that if a list contains sublists, the members of the sublists are not themselves members of the list. For example, the members of the list \(1 2 \(3 4\)\) are 1, 2, and the list \(3 4\); 3 and 4 are not themselves members of the list

\(b\) **Is a list?** If `thing` is a list, returns true; otherwise, returns false

---

#### List calculations

\(a\) ![](/assets/list-block-6.png)\(b\) ![](/assets/list-block-8.png)

\(a\) **Length of list **Returns the number of items in the `list`

\(b\) **Index **Returns the position of the `thing` in the `list`. If not in the list, returns 0

---

#### Introduce randomness

\(a\)![](/assets/list-block-7.png)

\(a\) **Random** Picks an item at random from the `list`



