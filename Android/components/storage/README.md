#### **Thunkable for Android **❤

# Storage

---

Data is the content that powers most apps and storage is an essential elements of almost every single app that you use. Deciding on which storage option can be complex but the key things to consider are i\) the file types you want to store and retrieve, ii\) the amount of data and iii\) the amount of security you want to have on that data. Since most data for your app should be secured, there is often some set up required to use these components.

At Thunkable, we particularly love data storage options like Firebase that require little set-up to get started but provide the option of security once you have your app working.

---

#### Data Storage

|  | ![](/assets/tiny-db-icon.png) | ![](/assets/file-icon.png) | ![](/assets/firebase-icon.png) | ![](/assets/spreadsheets-icon.png) | ![](/assets/fusion-tables-icon.png) | ![](/assets/web-icon.png) |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
|  | [Tiny DB](/Android/components/storage/tiny-db.md) | [File](/Android/components/storage/file.md) | [Firebase DB](/Android/components/storage/firebase-db.md) | [Spreadsheets](/Android/components/storage/spreadsheets.md) | [Fusion Tables](/Android/components/storage/fusion-tables.md) | [Web](/Android/components/storage/web.md) |
| Description | Store and retrieve one row of data stored locally on the device; ideal for saving data from a previous app session | Store and retrieve files \(e.g. PDFs\) stored locally on the device | Store and retrieve one row of data stored in the cloud that can be set to private | Store and retrieve multiple rows of data stored in a Google or Microsoft spreadsheet | Store, query and delete more than a thousand rows of data secured by Google Service authentication | Query data from a web service \(e.g. Weather information\) |
| Local / cloud | Works offline | Works offline | Can work offline in limited ways | Reliable data connection | Reliable data connection | Reliable data connection |
| Sample app types | All | PDF viewers | Messaging | Apps with lists, simple mapping | Complex mapping | Stock quotes, weather info |

**Important note**: Since the introduction of Firebase, we only recommend the [Tiny Web DB](/Android/components/storage/tiny-web-db.md) component for specific cases where you want to own and manage your own database infrastructure

---

#### Special Cases

For image files, we love the [Cloudinary DB](/Android/components/image/cloudinary-db.md)  ![](/assets/cloudinary-icon.png) component

