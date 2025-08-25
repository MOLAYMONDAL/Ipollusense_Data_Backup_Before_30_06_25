# MongoDB Backup Data Import Instructions

This repository contains zipped backup files exported from MongoDB Compass. These backups represent nodeValue data exported individually due to storage limitations and GitHub's file size restrictions.

## Backup Data Details

- The backups are exported for different `nodeValue` entries including:
  - 7, 1104, 1192, 1193, 1194, 1195, 1196, 1197, 1198, 1199, 1200, 1201, 1203
- All data was exported before **30/06/2025**.
- Each node's data is saved as a separate JSON file inside zipped archives.

## How to Import the Backup Data

To import the JSON data files into your MongoDB instance via MongoDB Compass, follow these steps:

### Prerequisites

- You need the MongoDB connection URL to connect to your MongoDB instance.
- Example MongoDB URL:

### mongodb+srv://username:password@cluster0.mongodb.net

- Replace `username`, `password`, and `cluster0.mongodb.net` with your own credentials and cluster details.

### Steps to Import

1. **Connect to MongoDB Compass**

- Open MongoDB Compass.
- Enter your MongoDB URL and connect to your cluster.
- Save the connection for future use if desired.

2. **Navigate to the `test` database**

- After connecting, select the `test` database from the left sidebar.
- Within the `test` database, select the `nodes` collection.

3. **Add Data to `nodes` Collection**

- At the top of the `nodes` collection view, find the **Filter** box.
- Click the **Add Data** button located next to the filter.
- From the dropdown, select **Import JSON/CSV file**.

4. **Import JSON File**

- Download and unzip the relevant backup zip file from this repository.
- Select the extracted `.json` file corresponding to the nodeValue you want to import.
- Follow the prompts to complete the import.

5. **Verify Import**

- Once imported, verify that the documents appear in the `nodes` collection.

---

## Notes

- This method assumes you are using MongoDB Compass as your GUI tool.
- The backups are exported per nodeValue to make file sizes manageable.
- If you want to import multiple nodeValues, repeat the import process for each JSON file.

---

If you face any issues or have questions, feel free to open an issue here.

---

## Issues

- If you are unable to connect to mongodb compass ask the IPOLLUSENSE project managing members.
- If the mongodb url is correct but still unable to connect then it is probably due to IP address , contact the mongodb access member and provide the IP address in the network access in mongodb ATLAS.
- For windows use command :

### (Invoke-RestMethod -Uri "https://api.ipify.org?format=text").Trim()

- For linux use command :

### ifconfig

---
# Ipollusense_Data_Backup_Before_30_06_25
