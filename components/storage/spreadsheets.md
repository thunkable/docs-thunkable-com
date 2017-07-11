#### **Thunkable for Android **❤

# Spreadsheets ![](/assets/spreadsheets-icon.png) by Cloudstitch

---

Spreadsheets is an easy to use component for managing the data that powers your app. Set up is much easier than Fusion Tables and Spreadsheets can store more rows of data than Firebase or TinyDB, which are both limited to one row of data. The data is also easily visible and manipulated in a Google or Microsoft 360 spreadsheet, which makes like a lot easier.

Spreadsheets is powered by Cloudstitch, a service that makes it easy to connect your Google or Microsoft 360 spreadsheets  to your app. Our friends at Cloudstitch have also provided free auto-syncing of data exclusively for Thunkers.

---

#### Set up

1. First [follow these instructions](https://www.youtube.com/watch?v=OfZE4zSd4h8) to create an account an a Spreadsheet API with Cloudstitch
2. After you create a Spreadsheet, you should get a screen that looks like the one below. Select 'Edit in Google'![](/assets/spreadsheets-fig-1.png)
3. Add your data to the Spreadsheet with columnNames in the first row. Please do not include spaces in your columnNames or in your Sheet Name
   ![](/assets/spreadsheets-fig-2.png)
4. Make sure to hit 'Sync to Template' every time you refresh your data. Your app is likely to crash if you do not follow this step![](/assets/spreadsheets-fig-3.png)
5. Go to Thunkable and add the API Endpoint that you see in Cloudstitch BUT remember to exclude `/datasources/sheet` and include `dev?=true` to the end of the given url. For example, if the Cloudstitch API endpoint is `https://api.cloudstitch.com/alberthunkable/sf-trees/datasources/sheet`, the API endpoint you want to enter into Thunkable is `https://api.cloudstitch.com/alberthunkable/sf-trees/dev?=true `![](/assets/spreadsheets-fig-4.png)
6. Add the Sheet Name.  You're all set!

| Property | Description |
| :--- | :--- |
| API Endpoint | Unique url for each spreadsheet created in Cloudstitch. The url is called the API endpoint on Cloudstitch but excludes the '/datasources/sheet' at the end of the endpoint. If you plan to upload data to your spreadsheet, enable auto-sync by adding 'dev?=true' to the end of your API endpoint |
| Sheet Name | Name of the sheet in the Spreadsheet |





