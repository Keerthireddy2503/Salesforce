## Salesforce Data Loader Tutorial

### What is Data Loader?

Salesforce Data Loader is a tool used to manage large amounts of data in Salesforce. It helps users insert, update, delete, and export records using CSV files. ([Developer][1])

---

## Insert, Update, and Delete Records

### Insert Records

Used to add new records into Salesforce.

Steps:

1. Open Data Loader.
2. Select **Insert**.
3. Choose object.
4. Upload CSV file.
5. Map fields.
6. Click **Finish**.

### Update Records

Used to modify existing records.

Requirements:

* Record ID
* Updated field values

### Delete Records

Used to remove records from Salesforce in bulk.

Important:

* Use correct record IDs.
* Deleted records move to Recycle Bin unless hard deleted. ([Salesforce Tutorial][2])

---

## Bulk Operations

Data Loader supports bulk processing of thousands or even millions of records. It is commonly used for:

* Mass insert
* Bulk update
* Bulk delete
* Data migration

Salesforce recommends using Bulk API mode for very large datasets. ([Salesforce][3])

---

## Enterprise Data Handling

In enterprise environments, Data Loader helps with:

* Migrating data from other systems
* Cleaning large datasets
* Exporting backup data
* Managing standard and custom objects

It supports:

* CSV files
* Bulk API
* Error and success logs
* Large file handling up to millions of records ([Developer][1])

| Operation | Purpose         |
| --------- | --------------- |
| Insert    | Add new records |
| Update    | Modify records  |
| Delete    | Remove records  |

---

## Key Points

* Data Loader is best for bulk data management.
* CSV files are required.
* Field mapping is important.
* Always check success and error logs after operations.

[1]: https://developer.salesforce.com/tools/data-loader/?utm_source=chatgpt.com "Salesforce Data Loader | Developer"
[2]: https://www.salesforcetutorial.com/delete-and-export-operations-using-apex-data-loader/?utm_source=chatgpt.com "Delete and Export operations using Apex Data Loader"
[3]: https://help.salesforce.com/s/articleView?id=000382601&language=en_US&type=1&utm_source=chatgpt.com "Use Data Loader with the Bulk API"
