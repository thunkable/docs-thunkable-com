#### **Thunkable for Android **❤

# Storage

---

Data is the content that powers most apps and storage is an essential elements of almost every single app that you use. Deciding on which storage option can be complex but the key things to consider are i\) the file types you want to store and retrieve, ii\) the amount of data and iii\) the amount of security you want to have on that data. Since most data for your app should be secured, there is often some set up required to use these components.

At Thunkable, we particularly love data storage options like Firebase that require little set-up to get started but provide the option of security once you have your app working.

---

#### Data Storage

|  | ![](/assets/tiny-db-icon.png) | ![](/assets/file-icon.png) | ![](/assets/firebase-icon.png) | ![](/assets/spreadsheets-icon.png) | ![](/assets/fusion-tables-icon.png) |
| :--- | :--- | :--- | :--- | :--- | :--- |
|  | [Tiny DB](/components/storage/tiny-db.md) | [File](/components/storage/file.md) | [Firebase DB](/components/storage/firebase-db.md) | [Spreadsheets](/components/storage/spreadsheets.md) | [Fusion Tables](/components/storage/fusion-tables.md) |
| Description | One row of data stored locally on the device; ideal for saving data from a previous app session | Access other file types \(e.g. PDFs\) stored locally on the device | One row of data stored in the cloud that can be set to private | Multiple rows of data stored in a Google or Microsoft spreadsheet | More than a thousand rows of data secured by Google Service authentication |
| Local / cloud | Works offline | Works offline | Limited data connection okay | Reliable data connection | Reliable data connection |
| Sample app types | All | PDF viewers | Messaging | Apps with lists, simple mapping | Complex mapping |

**Important note**: Since the introduction of Firebase, we do not recommend the [Tiny Web DB](/components/storage/tiny-web-db.md) component

---

#### Special Cases

For image files, we love the [Cloudinary DB](/components/image-+-video/cloudinary-db.md)  ![](/assets/cloudinary-icon.png) component

