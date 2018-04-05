#### **Thunkable for iOS **

# Spreadsheet ![](/assets/iOSviewIconSpreadsheet.png) powered by Airtable

---

The backbone to many apps is data and managing your app data in a Spreadsheet can be very user friendly. The Spreadsheet component is powered by Airtable, a service that looks like a spreadsheet but actually acts like a database so it can do database-like things like store attachments i.e. images in your spreadsheets \(and not just text\) and link records between spreadsheets. 

We like Airtable because set-up is relatively a breeze for a spreadsheet.

* [Set up](#set-up)
* [Getting, uploading, updating and deleting data in a spreadsheet](#getting-uploading-updating-and-deleting-data-in-a-spreadsheet)

---

### Set up

#### Step ① / Create your [free Airtable](https://airtable.com/) spreadsheet and account![](/assets/spreadsheet-airtable-✕-fig-1.png)![](/assets/spreadsheet-airtable-✕-fig-2.png)

#### Step ② / Connect your Airtable spreadsheet with Thunkable

There are four properties that you need to retrieve from Airtable to connect it with Thunkable: `API key`, `Base ID`, `Table Name` and `View Name`

![](/assets/spreadsheet-airtable-✕-fig-3.png)

`API key`

To retrieve the API key, you'll have to navigate to the Account page and generate an API Key

![](/assets/spreadsheet-airtable-✕-fig-4.png)![](/assets/spreadsheet-airtable-✕-fig-5.png)![](/assets/spreadsheet-airtable-✕-fig-6.png)

`Base ID`

To retrieve the Base ID, you'll actually have go to the [Airtable API documentation](https://airtable.com/api) page and select your spreadsheet. You'll then have to select the Node.js tab of the code editor and find the Base ID in the code as shown below

![](/assets/spreadsheet-airtable-✕-fig-7.png)![](/assets/spreadsheet-airtable-✕-fig-8.png)

`Table Name` and `View Name`

The Table Name and View Name can be retrieved by grabbing the fields from your spreadsheet as shown below

![](/assets/spreadsheet-airtable-✕-fig-9.png)

---

### Getting, uploading, updating and deleting data in a spreadsheet

#### Setting items for a ListView from an Airtable column

![](/assets/spreadsheet-airtable-✕-fig-10.png)

#### ![](/assets/spreadsheet-airtable-✕-fig-11.png)![](/assets/spreadsheet-airtable-✕-fig-12.png)

#### Getting data

| Event | Description |
| :--- | :--- |
| Get Cell \(`rowNum`, `columnName`\) | Returns the `value` of a specific cell |
| Get Column \(`columnName`, `maxNumRows`\) | Returns a `column` as a list |
| Get Row \(`rowNum`\) | Returns a row  `value` as an object |
| Get All Rows | Returns `rows` as an object |
| Get Selected Rows \(`startingRowNumber`, `numRows`\) | Returns `rows` as an object based on a specified `startingRowNumber` and `numRows` |

---

#### Uploading and updating data

![](/assets/spreadsheet-airtable-✕-fig-14.png)![](/assets/spreadsheet-airtable-✕-fig-15.png)

![](/assets/spreadsheet-airtable-✕-fig-13.png)

| Event | Description |
| :--- | :--- |
| Create Row \(`rowObject`\) | Uploads a new row of data based on a `rowObject` |
| Set Cell \(`rowNum`,`columnName`,`value`\) | Updates the `value`of a cell in a particular `rowNum` and `columnName` |
| Update Row \(`rowObject`\) | Updates a row based on a `rowObject` |
| Update Row Num \(`rowNum`, `rowObject`\) | Updates a row based on a `rowObject` and a `rowNum` |
| Replace Row Num \(`rowObject`\) | Replaces a row based on a `rowObject` |
| Replace Row \(`rowNum`, `rowObject`\) | Replaces a row based on a `rowObject` and a `rowNum` |

---

#### Deleting data

| Event | Description |
| :--- | :--- |
| Delete Row Num \(`rowNum`\) | Deletes a row based on `rowNum` |
| Delete Row \(`rowNum`, `rowObject`\) | Deletes a row based on a `rowObject` and a `rowNum` |



