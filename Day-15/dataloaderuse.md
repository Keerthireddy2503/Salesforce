## How to Use Salesforce Data Loader
### What is Data Loader?

Data Loader is a tool used to upload, update, export, and delete large amounts of Salesforce data using CSV files. It supports bulk operations and field mapping. ([Salesforce][1])

---

## Uploading CSV Data

1. Open Data Loader.
2. Login with Salesforce credentials.
3. Select an operation like **Insert** or **Update**.
4. Choose the Salesforce object.
5. Upload the CSV file.
6. Click **Next**.

CSV files are required for importing data into Salesforce. ([Salesforce][1])

---

## Field Mapping

Field mapping connects CSV columns with Salesforce fields.

Example:

* CSV Name → Salesforce Name
* CSV Email → Salesforce Email

Steps:

1. Click **Create or Edit a Map**.
2. Use **Auto-Match Fields** if names are similar.
3. Verify mappings carefully.
4. Save the mapping and continue.

Incorrect mapping may cause import errors. ([SalesForce FAQs][2])

---

## Bulk Operation

Bulk operations help users process thousands of records at once.

Common bulk operations:

* Insert
* Update
* Upsert
* Delete
* Export

Data Loader supports large data volumes and creates success/error log files after processing. ([Developer][3])

| Operation | Purpose          |
| --------- | ---------------- |
| Insert    | Add records      |
| Update    | Modify records   |
| Export    | Download records |

---

## Beginner Workflow

CSV File → Data Loader → Salesforce Object

### Tips

* Use clean CSV data.
* Test with small records first.
* Check success and error logs after upload. ([Salesforce][4])

[1]: https://help.salesforce.com/s/articleView?id=sf.data_loader.htm&language=en_US&utm_source=chatgpt.com "Data Loader"
[2]: https://salesforcefaqs.com/insert-operation-in-salesforce-data-loader/?utm_source=chatgpt.com "Insert Operation in Salesforce Data Loader [Detailed Guide]"
[3]: https://developer.salesforce.com/tools/data-loader/?utm_source=chatgpt.com "Salesforce Data Loader | Developer"
[4]: https://help.salesforce.com/s/articleView?id=000381876&language=en_US&type=1&utm_source=chatgpt.com "Prepare a CSV File for an Import or Update in Salesforce"
