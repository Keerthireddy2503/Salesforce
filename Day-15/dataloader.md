## Introduction to Salesforce Data Loader

[YouTube Tutorial – Introduction to Data Loader in Salesforce](https://www.youtube.com/watch?v=2KRGa86nbOg&utm_source=chatgpt.com)

### What is Data Loader?

Salesforce Data Loader is a tool used to import, export, update, and delete large amounts of data in Salesforce using CSV files.

---

## Installing Data Loader

1. Login to Salesforce.
2. Go to Setup.
3. Search for **Data Loader**.
4. Download and install it.
5. Open the application and login with Salesforce credentials.

---

## Importing Data

1. Open Data Loader.
2. Select **Insert**, **Update**, or **Upsert**.
3. Choose a Salesforce object.
4. Upload CSV file.
5. Map fields.
6. Click **Finish**.

---

## Export and Export All

* **Export** → Downloads existing records.
* **Export All** → Downloads existing and deleted records.

Steps:

1. Select Export/Export All.
2. Choose object.
3. Write SOQL query.
4. Save CSV file.

---

## Beginner Workflow

CSV File → Data Loader → Salesforce Object

### Beginner Tips

* Use clean CSV data.
* Test with small records first.
* Check success and error logs.

| Operation | Purpose          |
| --------- | ---------------- |
| Insert    | Add records      |
| Update    | Modify records   |
| Export    | Download records |

---

## Key Points

* Best for bulk data handling.
* Uses CSV files.
* Supports import and export operations.
* Commonly used by Salesforce admins and developers.
