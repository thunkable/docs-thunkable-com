#### **Thunkable for iOS **

# Spreadsheets powered by Airtable

---

The backbone to many apps is data and managing your app data in a Spreadsheet can be very user friendly. The Spreadsheet component is powered by Airtable, a radically different and Ashton Kutcher's favorite way of organizing anything from film projects to apartment hunts and customer lists.

Airtable looks like a spreadsheet but actually acts like a database so it can store attachments i.e. images in your spreadsheets \(and not just text\) and easily link records between spreadsheets

* [Set up](#set-up)
* [Retrieving, updating and deleting data in a spreadsheet](#retrieving-updating-and-deleting-data-in-a-spreadsheet)

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

### Retrieving, updating and deleting data in a spreadsheet

#### Setting items for a ListView from an Airtable column

![](/assets/spreadsheet-airtable-✕-fig-10.png)

![](/assets/spreadsheet-airtable-✕-fig-11.png)![](/assets/spreadsheet-airtable-✕-fig-12.png)

| Event | Description |
| :--- | :--- |
| Get Cell \(rowNum, columnName\) |  |



